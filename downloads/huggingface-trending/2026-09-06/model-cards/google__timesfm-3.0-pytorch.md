---
license: other
license_name: timesfm-non-commercial-license-v1.0
license_link: LICENSE
tags:
- time-series
- forecasting
- pretrained
- pytorch
- google
pipeline_tag: time-series-forecasting
---

# TimesFM 3.0 (PyTorch)

TimesFM (Time Series Foundation Model) is a pretrained time-series foundation model developed by Google Research for time-series forecasting.

This repository contains the official PyTorch weights and configurations for **TimesFM 3.0**.

## License

This model is released under the **[TimesFM Non-Commercial License v1.0](https://huggingface.co/google/timesfm-3.0-pytorch/blob/main/LICENSE)**.

## Model Details
- **Architecture**: Stacked Mixing Transformer with Variate Attention and CPM Iterative RevIN.
- **Context Patch Length**: 32
- **Forecast Horizon Patch Length**: 64
- **Layers**: 20 transformer layers (model dim: 1280, heads: 16)
- **Quantiles**:  (median at index 4)

## Data
timesfm-3.0 is pretrained using

- GiftEvalPretrain excluding the datasets that overlap with fev-bench
- Wikipedia Pageviews, cutoff Nov 2023 (see paper for details).
- Google Trends top queries, cutoff EoY 2022 (see paper for details).
- Synthetic and augmented data.



## Citation

@article{das2023decoder,
  title={A decoder-only foundation model for time-series forecasting},
  author={Das, Abhimanyu and Kong, Weihao and Sen, Rajat and Zhou, Yichen},
  journal={arXiv preprint arXiv:2310.10688},
  year={2023}
}


