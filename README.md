# DURD
This is the code repository for paper “Deep Unfolding Residual Decomposition for Infrared Small Target Detection”.

> 当前仓库状态：**代码/模型即将上传**（整理中）。  

## Updates
- 2026-01: Release official split lists for SIRST / NUST-SIRST / NUDT-SIRST. Code coming soon.

## Dataset Splits (How to Use)

- Dataset: [NUDT-SIRST](https://github.com/YeRen123455/Infrared-Small-Target-Detection), [SIRST](https://github.com/YimianDai/sirst), [NUST-SIRST](https://github.com/wanghuanphd/MDvsFA_cGAN).

Each `.txt` file contains **one sample name per line**, e.g. `Misc_238`. Train/Test are nearly 1:1 in our official splits. 

You can use these ids to index your local dataset files (dataset/images/xx.png; dataset/masks/xx.png) according to your dataset naming rule.
