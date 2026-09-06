---
language:
- en
- de
- es
- fr
- ja
- ko
- zh
- it
- pt
license: other
license_name: ltx-2.x-community-license-agreement
license_link: https://github.com/Lightricks/LTX-2/blob/main/LICENSE-2_x
pipeline_tag: image-to-video
arxiv: 2601.03233
tags:
- image-to-video
- text-to-video
- video-to-video
- image-text-to-video
- audio-to-video
- text-to-audio
- video-to-audio
- audio-to-audio
- text-to-audio-video
- image-to-audio-video
- image-text-to-audio-video
- ltx-video
- lightricks
- comfyui
- ltx-2.5
- diffusion-single-file
- ltx
pinned: true
demo: https://app.ltx.studio/ltx-2-playground/i2v
extra_gated_description: >-
  By clicking "Agree and Access" you acknowledge the [Privacy
  Policy](https://static.lightricks.com/legal/Privacy%20Policy%20-%20LTX%20Platform.pdf) 
  and consent to receive offers and updates including targeted and personalized
  advertisements. You can unsubscribe at any time.
extra_gated_button_content: Agree and Access
---

<!-- LTX-2.5 model card — license-first redesign. YAML frontmatter above kept intact. -->

<div class="lg:-mr-20 xl:-mr-24 2xl:-mr-36" style="border-radius:14px;overflow:hidden;">
<div style="position:relative;line-height:0;font-size:0;height:300px;">
<img src="https://huggingface.co/Lightricks/LTX-2.5/resolve/main/hf-hero-web.webp" alt="LTX-2.5 — Video, Audio &amp; World Simulation" style="display:block;width:100%;height:100%;object-fit:cover;margin:0;vertical-align:top;" />
<video autoplay muted loop playsinline style="position:absolute;inset:0;width:100%;height:100%;object-fit:cover;">
<source src="https://videos.ltx.io/LTX-2/ltx-research/hf-hero-web.mp4" type="video/mp4" />
<source src="https://videos.ltx.io/LTX-2/ltx-research/hf-hero-web.webm" type="video/webm" />
</video>
</div>
<!-- light hero footer -->
<div class="dark:hidden" style="background-color:#eef1f5;padding:2rem 1.5rem 2.4rem;text-align:center;isolation:isolate;">
<h1 style="color:#0a0a0a;margin:0 0 0.5rem;font-size:2rem;font-weight:700;letter-spacing:-0.01em;border:none;padding:0;">LTX-2.5 — Video, Audio &amp; World Simulation</h1>
<p style="color:#555;margin:0 0 1.25rem;font-size:1.05rem;">Full control and customization — self-host on your infrastructure.</p>
<div style="display:flex;flex-wrap:wrap;justify-content:center;gap:0.5rem;">
<a href="https://ltx.io" class="bg-white hover:bg-gray-200 transition-colors duration-150" style="color:#1c1c1c;border:1px solid #d0d3d8;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Homepage</a>
<a href="https://docs.ltx.io" class="bg-white hover:bg-gray-200 transition-colors duration-150" style="color:#1c1c1c;border:1px solid #d0d3d8;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Docs</a>
<a href="https://github.com/Lightricks/LTX-2" class="bg-white hover:bg-gray-200 transition-colors duration-150" style="color:#1c1c1c;border:1px solid #d0d3d8;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">GitHub</a>
<a href="https://huggingface.co/papers/2601.03233" class="bg-white hover:bg-gray-200 transition-colors duration-150" style="color:#1c1c1c;border:1px solid #d0d3d8;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Research</a>
<a href="https://console.ltx.io/playground/" class="bg-white hover:bg-gray-200 transition-colors duration-150" style="color:#1c1c1c;border:1px solid #d0d3d8;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">API Playground</a>
<a href="https://discord.gg/ltxplatform" class="bg-white hover:bg-gray-200 transition-colors duration-150" style="color:#1c1c1c;border:1px solid #d0d3d8;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Discord</a>
</div>
<div style="margin-top:1.5rem;">
<a href="https://github.com/Lightricks/LTX-2/blob/main/LICENSE.md" class="bg-green-500 hover:brightness-110 transition-all duration-150" style="display:inline-block;color:#fff;border-radius:8px;padding:0.65rem 1.6rem;font-size:0.9rem;font-weight:700;text-decoration:none;">LTX License</a>
</div>
</div>
<!-- dark hero footer -->
<div class="hidden dark:block" style="background-color:#0a0a0a;padding:2rem 1.5rem 2.4rem;text-align:center;isolation:isolate;">
<h1 style="color:#fff;margin:0 0 0.5rem;font-size:2rem;font-weight:700;letter-spacing:-0.01em;border:none;padding:0;">LTX-2.5 — Video, Audio &amp; World Simulation</h1>
<p style="color:#c9c9c9;margin:0 0 1.25rem;font-size:1.05rem;">Full control and customization — self-host on your infrastructure.</p>
<div style="display:flex;flex-wrap:wrap;justify-content:center;gap:0.5rem;">
<a href="https://ltx.io" class="bg-gray-800 hover:bg-gray-700 transition-colors duration-150" style="color:#fff;border:1px solid #2e2e2e;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Homepage</a>
<a href="https://docs.ltx.io" class="bg-gray-800 hover:bg-gray-700 transition-colors duration-150" style="color:#fff;border:1px solid #2e2e2e;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Docs</a>
<a href="https://github.com/Lightricks/LTX-2" class="bg-gray-800 hover:bg-gray-700 transition-colors duration-150" style="color:#fff;border:1px solid #2e2e2e;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">GitHub</a>
<a href="https://huggingface.co/papers/2601.03233" class="bg-gray-800 hover:bg-gray-700 transition-colors duration-150" style="color:#fff;border:1px solid #2e2e2e;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Research</a>
<a href="https://console.ltx.io/playground/" class="bg-gray-800 hover:bg-gray-700 transition-colors duration-150" style="color:#fff;border:1px solid #2e2e2e;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">API Playground</a>
<a href="https://discord.gg/ltxplatform" class="bg-gray-800 hover:bg-gray-700 transition-colors duration-150" style="color:#fff;border:1px solid #2e2e2e;border-radius:8px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Discord</a>
</div>
<div style="margin-top:1.5rem;">
<a href="https://github.com/Lightricks/LTX-2/blob/main/LICENSE.md" class="bg-green-500 hover:brightness-110 transition-all duration-150" style="display:inline-block;color:#fff;border-radius:8px;padding:0.65rem 1.6rem;font-size:0.9rem;font-weight:700;text-decoration:none;">LTX License</a>
</div>
</div>
</div>

<!-- LIGHT tier cards -->
<div class="dark:hidden lg:-mr-20 xl:-mr-24 2xl:-mr-36">
<div style="display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-top:1rem;">
<div style="background:#ecf8f2;border:1px solid #d6e9de;border-radius:6px;padding:1.5rem 1.6rem;">
<div style="width:44px;height:44px;border-radius:6px;background:#dceee4;display:flex;align-items:center;justify-content:center;margin:0 0 0.8rem;color:#1c1c1c;"><svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M16 20V4a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"/><rect width="20" height="14" x="2" y="6" rx="2"/></svg></div>
<div style="font-size:1.3rem;font-weight:700;color:#0a0a0a;margin:0 0 0.6rem;line-height:1.35;">Under $10M annual revenue</div>
<p style="color:#333;font-size:1.05rem;margin:1.1rem 0;">Commercial and production use at no cost under the LTX-2.x Community License. Transfer of fine-tunes may require a paid license, in accordance with the LTX-2.x Community License.</p>
<a href="https://docs.ltx.io/open-source-model/getting-started/overview" class="bg-gray-900 hover:bg-gray-700 transition-colors duration-150" style="display:inline-block;color:#fff;border:1px solid #0a0a0a;border-radius:9999px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Read the Documentation</a>
</div>
<div style="background:#f3eff9;border:1px solid #e0d8f0;border-radius:6px;padding:1.5rem 1.6rem;">
<div style="width:44px;height:44px;border-radius:6px;background:#e6deef;display:flex;align-items:center;justify-content:center;margin:0 0 0.8rem;color:#1c1c1c;"><svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M3 21h18"/><path d="M5 21V5a2 2 0 0 1 2-2h6a2 2 0 0 1 2 2v16"/><path d="M15 21V9a1 1 0 0 1 1-1h3a2 2 0 0 1 2 2v11"/><path d="M9 7h2"/><path d="M9 11h2"/><path d="M9 15h2"/></svg></div>
<div style="font-size:1.3rem;font-weight:700;color:#0a0a0a;margin:0 0 0.6rem;line-height:1.35;">Over $10M annual revenue</div>
<p style="color:#333;font-size:1.05rem;margin:1.1rem 0;">Paid Commercial Use Agreement for LTX-2.x with full weights, engineering support, LoRAs, and flexible deployment options. To learn about all licensing options, talk to an expert.</p>
<a href="https://ltx.io/forms/ltx-contact-sales?kpi=licensing" class="bg-gray-900 hover:bg-gray-700 transition-colors duration-150" style="display:inline-block;color:#fff;border:1px solid #0a0a0a;border-radius:9999px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Talk to a Commercial Licensing Expert</a>
</div>
</div>
</div>

<!-- DARK tier cards -->
<div class="hidden dark:block lg:-mr-20 xl:-mr-24 2xl:-mr-36">
<div style="display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-top:1rem;">
<div style="background:#1a2622;border:1px solid #2a3a32;border-radius:6px;padding:1.5rem 1.6rem;">
<div style="width:44px;height:44px;border-radius:6px;background:#22332c;display:flex;align-items:center;justify-content:center;margin:0 0 0.8rem;color:#fff;"><svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M16 20V4a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"/><rect width="20" height="14" x="2" y="6" rx="2"/></svg></div>
<div style="font-size:1.3rem;font-weight:700;color:#fff;margin:0 0 0.6rem;line-height:1.35;">Under $10M annual revenue</div>
<p style="color:#c9ced6;font-size:1.05rem;margin:1.1rem 0;">Commercial and production use at no cost under the LTX-2.x Community License. Transfer of fine-tunes may require a paid license, in accordance with the LTX-2.x Community License.</p>
<a href="https://docs.ltx.io/open-source-model/getting-started/overview" class="bg-gray-50 hover:bg-gray-300 transition-colors duration-150" style="display:inline-block;color:#1c1c1c;border:1px solid #f8fafc;border-radius:9999px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Read the Documentation</a>
</div>
<div style="background:#221a2e;border:1px solid #322a42;border-radius:6px;padding:1.5rem 1.6rem;">
<div style="width:44px;height:44px;border-radius:6px;background:#2a2238;display:flex;align-items:center;justify-content:center;margin:0 0 0.8rem;color:#fff;"><svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M3 21h18"/><path d="M5 21V5a2 2 0 0 1 2-2h6a2 2 0 0 1 2 2v16"/><path d="M15 21V9a1 1 0 0 1 1-1h3a2 2 0 0 1 2 2v11"/><path d="M9 7h2"/><path d="M9 11h2"/><path d="M9 15h2"/></svg></div>
<div style="font-size:1.3rem;font-weight:700;color:#fff;margin:0 0 0.6rem;line-height:1.35;">Over $10M annual revenue</div>
<p style="color:#c9ced6;font-size:1.05rem;margin:1.1rem 0;">Paid Commercial Use Agreement for LTX-2.x with full weights, engineering support, LoRAs, and flexible deployment options. To learn about all licensing options, talk to an expert.</p>
<a href="https://ltx.io/forms/ltx-contact-sales?kpi=licensing" class="bg-gray-50 hover:bg-gray-300 transition-colors duration-150" style="display:inline-block;color:#1c1c1c;border:1px solid #f8fafc;border-radius:9999px;padding:0.5rem 1.1rem;font-size:0.85rem;font-weight:600;text-decoration:none;">Talk to a Commercial Licensing Expert</a>
</div>
</div>
</div>

---

**LTX-2.5** is an open world model with open weights, built for local execution and fine-tuning. Its established use is generating synchronized, high-fidelity video and audio from text, image, and video inputs; applicability to emerging domains such as robotics and physical AI is developing.

**Full control and customization** — self-host on your own infrastructure. No per-generation billing, no per-seat lock-in, no forced API dependency. Revenue is measured across the whole entity, including subsidiaries and affiliates under common control. The full, binding terms live in [`LICENSE`](https://github.com/Lightricks/LTX-2/blob/main/LICENSE.md).


## What's new in LTX-2.5

- **Native multishot generation** — generate connected scenes in a single pass: multiple shots that hold character identity, environment, lighting, voice, and visual style across cuts (previous versions produced a single continuous shot).
- **Diffusion fidelity rendering** — Instead of locking every scene to one compression rate, our model dynamically allocates compute by scene complexity and budget, rendering flawless detail where it matters, efficient everywhere else.
- **New diffusion video decoder** — replaces the VAE reconstruction stage; sharper faces, textures, and on-screen text, better motion, and fewer artifacts in demanding scenes.
- **Custom Gemma 4 12B text encoder** — holds complex prompts together (multiple characters, camera moves, lighting, actions) instead of dropping details across a longer sequence.
- **Prompt enhancer** — expands a short prompt into richer cinematic instructions at minimal extra compute.
- **Duration predictor (optional)** — an opt-in node predicts a clip's length from the prompt and sets the frame count for you, instead of relying on a fixed-duration parameter.
- **Substantially improved distilled model** — retains much more of the full model's visual quality, prompt adherence, and motion consistency in a smaller, faster checkpoint.

---

# Model family & checkpoints

LTX-2.5 ships as a **split, Comfy-aligned pack** (one `.safetensors` per component) rather than a single monolith. Point each CLI flag / loader at the file below.

## Transformers (DiT)

| File | Notes |
|------|-------|
| [`diffusion_models/ltx-2.5-22b-distilled-transformer-bf16.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/diffusion_models/ltx-2.5-22b-distilled-transformer-bf16.safetensors) | Distilled DiT (bf16). Fixed 8-step schedule, CFG=1. |
| [`diffusion_models/ltx-2.5-22b-dev-transformer-bf16.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/diffusion_models/ltx-2.5-22b-dev-transformer-bf16.safetensors) | Full / trainable DiT (bf16). |
| [`diffusion_models/ltx-2.5-22b-distilled-transformer-comfy-int8-convrot.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/diffusion_models/ltx-2.5-22b-distilled-transformer-comfy-int8-convrot.safetensors) | Distilled DiT (Comfy int8 + convrot). **ComfyUI only** — not for `ltx-pipelines` / PyTorch. |
| [`diffusion_models/ltx-2.5-22b-dev-transformer-comfy-int8-convrot.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/diffusion_models/ltx-2.5-22b-dev-transformer-comfy-int8-convrot.safetensors) | Full DiT (Comfy int8 + convrot). **ComfyUI only** — not for `ltx-pipelines` / PyTorch. |
| [`diffusion_models/ltx-2.5-22b-distilled-transformer-nvfp4.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/diffusion_models/ltx-2.5-22b-distilled-transformer-nvfp4.safetensors) | Distilled DiT (NVFP4). ComfyUI, or `ltx-pipelines` with `--quantization nvfp4-prequant` (Blackwell / `ltx-kernels`). |

## Other components

| File | Notes |
|------|-------|
| [`text_encoders/gemma4-12b-with-proj-ltx-2.5-bf16.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/text_encoders/gemma4-12b-with-proj-ltx-2.5-bf16.safetensors) | Gemma4 TE + projections (bf16) |
| [`text_encoders/gemma4-12b-with-proj-ltx-2.5-comfy-int8-convrot.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/text_encoders/gemma4-12b-with-proj-ltx-2.5-comfy-int8-convrot.safetensors) | Same TE, Comfy int8 — **ComfyUI only** |
| [`vae/ltx-2.5-video-vae-bf16.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/vae/ltx-2.5-video-vae-bf16.safetensors) | DiffVAE — higher quality, heavier |
| [`vae/ltx-2.5-video-vae-conv-bf16.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/vae/ltx-2.5-video-vae-conv-bf16.safetensors) | Conv VAE — faster, lighter |
| [`vae/ltx-2.5-audio-vae-bf16.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/vae/ltx-2.5-audio-vae-bf16.safetensors) | Audio VAE + vocoder |
| [`loras/ltx-2.5-22b-distilled-lora-450-bf16.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/loras/ltx-2.5-22b-distilled-lora-450-bf16.safetensors) | Distilled LoRA (dev-transformer workflows) |
| [`model_patches/ltx-2.5-duration-head-bf16.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/model_patches/ltx-2.5-duration-head-bf16.safetensors) | Auto duration when `--num-frames` omitted |
| [`latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors) | x2 spatial upscaler required for multi-stage pipeline |
| [`latent_upscale_models/ltx-2.5-latent-temporal-upscaler-x2-bf16-1.0.safetensors`](https://huggingface.co/Lightricks/LTX-2.5/blob/main/latent_upscale_models/ltx-2.5-latent-temporal-upscaler-x2-bf16-1.0.safetensors) | x2 temporal upscaler |

---

# Usage

### Online demo

Try LTX-2.5 in the [API Playground](https://console.ltx.video/playground/) without installing anything locally.

### Option A — Python (`ltx-pipelines`)

Weights on this repo are **split** (Comfy-aligned): one safetensors file per component. The [LTX-2](https://github.com/Lightricks/LTX-2) `ltx-pipelines` package loads them via `--transformer-path`, `--text-encoder-path`, etc.

#### Install

```bash
git clone https://github.com/Lightricks/LTX-2.git
cd LTX-2
uv sync
source .venv/bin/activate
```

Python >= 3.12, CUDA >= 12.7, PyTorch ~= 2.7 recommended. See the [repo README](https://github.com/Lightricks/LTX-2) for attention backends and optional extras.

#### Download weights

```bash
hf auth login

# LTX-2.5 distilled split pack
hf download Lightricks/LTX-2.5 \
  diffusion_models/ltx-2.5-22b-distilled-transformer-bf16.safetensors \
  text_encoders/gemma4-12b-with-proj-ltx-2.5-bf16.safetensors \
  vae/ltx-2.5-video-vae-bf16.safetensors \
  vae/ltx-2.5-audio-vae-bf16.safetensors \
  model_patches/ltx-2.5-duration-head-bf16.safetensors \
  latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors \
  --local-dir models/ltx-2.5
```

#### Distilled text-to-video

```bash
uv run python -m ltx_pipelines.distilled \
  --transformer-path     models/ltx-2.5/diffusion_models/ltx-2.5-22b-distilled-transformer-bf16.safetensors \
  --text-encoder-path    models/ltx-2.5/text_encoders/gemma4-12b-with-proj-ltx-2.5-bf16.safetensors \
  --video-vae-path       models/ltx-2.5/vae/ltx-2.5-video-vae-bf16.safetensors \
  --audio-vae-path       models/ltx-2.5/vae/ltx-2.5-audio-vae-bf16.safetensors \
  --duration-head-path   models/ltx-2.5/model_patches/ltx-2.5-duration-head-bf16.safetensors \
  --spatial-upsampler-path models/ltx-2.5/latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors \
  --prompt "A golden retriever running through a sunny meadow, cinematic lighting" \
  --seed 42 \
  --output-path output_distilled.mp4
```

Omit `--num-frames` to let the duration head pick a length from the prompt (LTX-2.5+). Or set e.g. `--num-frames 121` (must satisfy `frames % 8 == 1`). Width/height must be divisible by 32.

#### Image-to-video

Add one or more `--image PATH FRAME_IDX STRENGTH` flags (frame 0 = first frame conditioning):

```bash
uv run python -m ltx_pipelines.distilled \
  --transformer-path     models/ltx-2.5/diffusion_models/ltx-2.5-22b-distilled-transformer-bf16.safetensors \
  --text-encoder-path    models/ltx-2.5/text_encoders/gemma4-12b-with-proj-ltx-2.5-bf16.safetensors \
  --video-vae-path       models/ltx-2.5/vae/ltx-2.5-video-vae-bf16.safetensors \
  --audio-vae-path       models/ltx-2.5/vae/ltx-2.5-audio-vae-bf16.safetensors \
  --duration-head-path   models/ltx-2.5/model_patches/ltx-2.5-duration-head-bf16.safetensors \
  --spatial-upsampler-path models/ltx-2.5/latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors \
  --image path/to/first_frame.jpg 0 1.0 \
  --prompt "The camera slowly dollies out as wind moves through the grass" \
  --seed 42 \
  --output-path output_i2v.mp4
```

#### Low-VRAM tips

```bash
# Downcast bf16 transformer on the fly + CPU offload
  ...existing flags... \
  --quantization fp8-cast \
  --offload cpu
```

Use the **bf16** checkpoints with `ltx-pipelines`. The `*-comfy-int8-convrot.safetensors` files are ComfyUI-only and are not loaded by this PyTorch path.

#### Python API (same split paths)

```python
from ltx_pipelines.distilled import DistilledPipeline
from ltx_pipelines.utils.model_paths import ModelPaths

model_paths = ModelPaths.from_split(
    transformer_path="models/ltx-2.5/diffusion_models/ltx-2.5-22b-distilled-transformer-bf16.safetensors",
    text_encoder_path="models/ltx-2.5/text_encoders/gemma4-12b-with-proj-ltx-2.5-bf16.safetensors",
    video_vae_path="models/ltx-2.5/vae/ltx-2.5-video-vae-bf16.safetensors",
    audio_vae_path="models/ltx-2.5/vae/ltx-2.5-audio-vae-bf16.safetensors",
    duration_head_path="models/ltx-2.5/model_patches/ltx-2.5-duration-head-bf16.safetensors",
)

pipe = DistilledPipeline(
    model_paths=model_paths,
    spatial_upsampler_path="models/ltx-2.5/latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors",
)
# See packages/ltx-pipelines for __call__ args (prompt, seed, num_frames, images, ...).
```

```bash
uv run python -m ltx_pipelines.distilled --help
```

Full docs: [ltx-pipelines installation](https://github.com/Lightricks/LTX-2/blob/main/packages/ltx-pipelines/docs/installation.md).

### Option B — ComfyUI

Official LTX-2.5 workflow templates ship in ComfyUI. Full instructions: [ComfyUI integration](https://docs.ltx.video/open-source-model/integration-tools/comfy-ui).

### Option C — Diffusers

A Diffusers-compatible pack lives at [`Lightricks/LTX-2.5-Diffusers`](https://huggingface.co/Lightricks/LTX-2.5-Diffusers) — same model, Diffusers-friendly packaging.

#### Install

LTX-2.5 support is not in a `diffusers` release yet, so install from main:

```bash
pip install git+https://github.com/huggingface/diffusers
```

#### Image-to-video, two stages

```python
import torch
from diffusers import LTX2ImageToVideoPipeline, LTX2LatentUpsamplePipeline
from diffusers.pipelines.ltx2.latent_upsampler import LTX2LatentUpsamplerModel
from diffusers.pipelines.ltx2.utils import (
    DEFAULT_NEGATIVE_PROMPT,
    DISTILLED_SIGMA_VALUES,
    STAGE_2_DISTILLED_SIGMA_VALUES,
)
from diffusers.utils import encode_video, load_image

MODEL_ID = "Lightricks/LTX-2.5-Diffusers"
# Stage 1 resolution; stage 2 runs at 2x this.
HEIGHT, WIDTH, NUM_FRAMES, FRAME_RATE = 544, 960, 121, 24.0

pipe = LTX2ImageToVideoPipeline.from_pretrained(MODEL_ID, dtype=torch.bfloat16)
pipe.enable_model_cpu_offload()
pipe.vae.enable_tiling()  # stage 2 decodes at 2x

latent_upsampler = LTX2LatentUpsamplerModel.from_pretrained(
    MODEL_ID, subfolder="latent_upsampler", dtype=torch.bfloat16
).to("cuda")
upsample_pipe = LTX2LatentUpsamplePipeline(vae=pipe.vae, latent_upsampler=latent_upsampler)

generator = torch.Generator("cuda").manual_seed(42)
shared = dict(
    image=load_image("path/to/first_frame.jpg"),
    prompt="The camera slowly dollies out as wind moves through the grass",
    negative_prompt=DEFAULT_NEGATIVE_PROMPT,
    frame_rate=FRAME_RATE,
    guidance_scale=1.0,
    audio_guidance_scale=1.0,
    stg_scale=0.0,
    audio_stg_scale=0.0,
    modality_scale=1.0,
    audio_modality_scale=1.0,
    generator=generator,
    return_dict=False,
)

stage_1_latents, audio_latents = pipe(
    height=HEIGHT, width=WIDTH, num_frames=NUM_FRAMES,
    sigmas=DISTILLED_SIGMA_VALUES, output_type="latent", **shared,
)

upsampled_latents = upsample_pipe(
    latents=stage_1_latents, output_type="latent", return_dict=False
)[0]

# Stage 2 takes its size from the upsampled latents, so pass no height/width.
video, audio = pipe(
    num_frames=NUM_FRAMES,
    sigmas=STAGE_2_DISTILLED_SIGMA_VALUES,
    latents=upsampled_latents,
    audio_latents=audio_latents,
    noise_scale=STAGE_2_DISTILLED_SIGMA_VALUES[0],
    output_type="np",
    **shared,
)

encode_video(
    video[0],
    fps=int(FRAME_RATE),
    output_path="output_i2v_two_stage.mp4",
    audio=audio[0].float().cpu(),
    audio_sample_rate=pipe.vocoder.config.output_sampling_rate,
)
```

---

### Constraints

- Frame count: `num_frames % 8 == 1` (1, 9, 17, …, 121, …)
- Width and height divisible by 32

### Prompting

Well-structured, detailed prompts materially improve results. For multishot prompting and a full guide, see [How to prompt LTX-2](https://docs.ltx.video/open-source-model/usage-guides/prompting-guide).

---

# Training & fine-tuning

The **dev** transformer is fully trainable. Reproduce published LoRAs and IC-LoRAs with the [LTX-2 Trainer](https://github.com/Lightricks/LTX-2/blob/main/packages/ltx-trainer/README.md).

Based on our testing, the large majority of LoRAs and IC-LoRAs trained on LTX-2.3 run on LTX-2.5 without changes. A small number of exceptions exist — validate your adapters before production use.

---

# Limitations

- This model is not intended or able to provide factual information.
- As a statistical model, this checkpoint may amplify existing societal biases.
- Prompt following is heavily influenced by prompting style.
- The model may fail to generate videos that match the prompt perfectly.
- The model may generate content that is inappropriate or offensive.

---

## Citation

```bibtex
@article{hacohen2025ltx2,
  title={LTX-2: Efficient Joint Audio-Visual Foundation Model},
  author={HaCohen, Yoav and Brazowski, Benny and Chiprut, Nisan and Bitterman, Yaki and Kvochko, Andrew and Berkowitz, Avishai and Shalem, Daniel and Lifschitz, Daphna and Moshe, Dudu and Porat, Eitan and Richardson, Eitan and Guy Shiran and Itay Chachy and Jonathan Chetboun and Michael Finkelson and Michael Kupchick and Nir Zabari and Nitzan Guetta and Noa Kotler and Ofir Bibi and Ori Gordon and Poriya Panet and Roi Benita and Shahar Armon and Victor Kulikov and Yaron Inger and Yonatan Shiftan and Zeev Melumian and Zeev Farbman},
  journal={arXiv preprint arXiv:2601.03233},
  year={2026}
}
```