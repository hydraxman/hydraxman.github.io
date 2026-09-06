---
license: mit
library_name: transformers
pipeline_tag: image-text-to-text
---

# DeepSeek-V4-Flash-Vision-Exp

<!-- markdownlint-disable first-line-h1 -->
<!-- markdownlint-disable html -->
<!-- markdownlint-disable no-duplicate-header -->

<div align="center">
  <img src="https://github.com/deepseek-ai/DeepSeek-V2/blob/main/figures/logo.svg?raw=true" width="60%" alt="DeepSeek-V4" />
</div>
<hr>
<div align="center" style="line-height: 1;">
  <a href="https://www.deepseek.com/" target="_blank" style="margin: 2px;">
    <img alt="Homepage" src="https://github.com/deepseek-ai/DeepSeek-V2/blob/main/figures/badge.svg?raw=true" style="display: inline-block; vertical-align: middle;"/>
  </a>
  <a href="https://chat.deepseek.com/" target="_blank" style="margin: 2px;">
    <img alt="Chat" src="https://img.shields.io/badge/🤖%20Chat-DeepSeek%20V4-536af5?color=536af5&logoColor=white" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>
<div align="center" style="line-height: 1;">
  <a href="https://huggingface.co/deepseek-ai" target="_blank" style="margin: 2px;">
    <img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-DeepSeek%20AI-ffc107?color=ffc107&logoColor=white" style="display: inline-block; vertical-align: middle;"/>
  </a>
  <a href="https://twitter.com/deepseek_ai" target="_blank" style="margin: 2px;">
    <img alt="Twitter Follow" src="https://img.shields.io/badge/Twitter-deepseek_ai-white?logo=x&logoColor=white" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>
<div align="center" style="line-height: 1;">
  <a href="LICENSE" style="margin: 2px;">
    <img alt="License" src="https://img.shields.io/badge/License-MIT-f5de53?&color=f5de53" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>

## Introduction

We are excited to introduce **DeepSeek-V4-Flash-Vision-Exp**, our first experimental multimodal model in the DeepSeek-V4 family. It builds on the DeepSeek-V4-Flash architecture by incorporating visual modules and undergoing continued training to unlock visual understanding capabilities.

Compared to DeepSeek-V4-Flash-0731, DeepSeek-V4-Flash-Vision-Exp achieves substantial improvements on its multimodal agent capabilities, while maintaining comparable performance on text-only agent tasks.

<div align="center">

| Benchmark | DeepSeek-V4-Flash-Vision-Exp | DeepSeek-V4-Flash-0731 | Opus-4.8 |
| :--- | :---: | :---: | :---: |
| **Text Agent Capabilities** | | | |
| Terminal Bench 2.1 | 83.9 | 82.7 | 85.0 |
| NL2Repo | 57.7 | 54.2 | 69.7 |
| Cybergym | 75.3 | 76.7 | 78.3 |
| DeepSWE | 59.3 | 54.4 | 58.0 |
| Toolathlon-Verified | 75.9 | 70.3 | 76.2 |
| DSBench-Hard | 63.6 | 59.6 | 71.7 |
| AutomationBench (Public) | 25.7 | 25.1 | 27.2 |
| **Multimodal Agent Capabilities** | | | |
| ApexBench (Pass@1) | 36.5 | 26.2† | 39.4 |
| Agents' Last Exam | 27.3 | 25.2† | 25.7 |
| Chartography | 64.3 | - | 65.0 |
| ZeroBench (Pass@5) | 35.0 | - | 34.0 |

</div>

Notes:

1. For the text agent benchmarks above, DeepSeek models are evaluated with the minimal mode of DeepSeek Harness as the agent framework, using the `max` reasoning effort level with `temperature = 1.0, top_p = 0.95`.
2. † For ApexBench and Agents' Last Exam, DeepSeek-V4-Flash-0731 ignores the multimodal elements in the input.


## Repository layout

This repository contains the tokenizer, prompt encoding reference, and a
minimal PyTorch inference implementation for DeepSeek-V4 Flash Vision. The
reference inference covers the vision encoder and aligner, DFlash attention,
MoE, Hyper-Connections, and the DSpark forward path.

```text
.
├── encoding/                  # OpenAI-style messages -> model prompt
├── inference/                 # weight conversion and minimal inference
│   └── examples/              # equivalent TXT and JSON vision prompts
├── config.json                # Hugging Face model metadata
├── generation_config.json
├── model.safetensors.index.json
├── tokenizer.json
└── tokenizer_config.json
```

`encoding/` and `inference/` deliberately remain separate: prompt formatting
does not depend on PyTorch, while inference imports the sibling encoding module
with an explicit Python path. No symlinks are required.

The tokenizer files are regular files so that the repository can be uploaded
to Hugging Face without relying on local filesystem symlinks. The large model
shards are described by `model.safetensors.index.json` and are not duplicated
inside the source checkout used to assemble this repository.

## Prompt encoding

See [`encoding/README.md`](encoding/README.md). Both OpenAI-style JSON content
blocks and the compact `<image>path</image>` TXT notation are supported. The two
examples under `inference/examples/` encode to identical prompts and token IDs.

## Minimal inference

See [`inference/README.md`](inference/README.md) for dependency installation,
checkpoint conversion, and TXT/JSON inference commands.

## How to Run with vLLM

For example, the command below serves the model with vLLM on a single 4×GB300 node. 
See the [vLLM recipe](https://recipes.vllm.ai/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp) for detailed instructions and other hardware configurations.

```bash
docker run --gpus all \
  vllm/vllm-openai:deepseekv4-flash-vision deepseek-ai/DeepSeek-V4-Flash-Vision-Exp \
  --kv-cache-dtype fp8 \
  --block-size 256 \
  --tensor-parallel-size 4 \
  --tool-call-parser deepseek_v4 \
  --enable-auto-tool-choice \
  --reasoning-parser deepseek_v4 \
  --reasoning-config '{"reasoning_parser":"deepseek_v4","reasoning_start_str":"","reasoning_end_str":""}' \
  --speculative-config '{"method":"dspark","model":"deepseek-ai/DeepSeek-V4-Flash-Vision-Exp","num_speculative_tokens":3,"draft_sample_method":"probabilistic","enable_adaptive_verification":true}'
```

## How to Run with SGLang
Enable DSpark with --speculative-algorithm DSPARK and do not set a separate --speculative-draft-model-path as the target and draft weights therefore come from the same checkpoint. See the [SGLang cookbook](https://docs.sglang.io/cookbook/autoregressive/DeepSeek/DeepSeek-V4#hw=b200&variant=flash-vision&quant=fp4&strategy=low-latency&nodes=single) for detailed instructions, benchmarks and other hardwares configurations.

```
sglang serve \
  --model-path deepseek-ai/DeepSeek-V4-Flash-Vision-Exp \
  --tp 4 \
  --speculative-algorithm DSPARK \
  --mem-fraction-static 0.85 \
  --host 0.0.0.0 \
  --port 30000
```

## License

This repository is licensed under the [MIT License](LICENSE).