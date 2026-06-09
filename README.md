# DURD

This is the code repository for paper **“Deep Unfolding Residual Decomposition for Infrared Small Target Detection”**.

## Environment

- Python 3
- PyTorch + torchvision
- numpy, tqdm
- scikit-image 
- scikit-learn 
- ...

## Data Preparation

Datasets available at: 
- [NUDT-SIRST](https://github.com/YeRen123455/Infrared-Small-Target-Detection)
- [SIRST](https://github.com/YimianDai/sirst)
- [NUST-SIRST](https://github.com/wanghuanphd/MDvsFA_cGAN)

Expected dataset structure:

```
dataset/<DATASET_NAME>/
	images/   *.png
	masks/    *.png
```

### Official split lists

This repo includes split files under:

- `dataset/SIRST/`
- `dataset/NUST-SIRST/`
- `dataset/NUDT-SIRST/`

Each `splite_*.txt` contains **one sample id per line** (e.g. `Misc_238`). The dataset loader uses these ids to locate:

- `dataset/<DATASET_NAME>/images/<id>.png`
- `dataset/<DATASET_NAME>/masks/<id>.png`


## Training
Run:

```bash
python train.py
```

Outputs are saved to:

- `result/<DATASET_NAME>_<timestamp>/Saved_parameters.pt`
- `result/<DATASET_NAME>_<timestamp>/best_IoU.log`

## Testing

Run:

```bash
python test.py
```

## Citation

If you find this work useful, please cite the paper:

```bibtex
@ARTICLE{11523120,
  author={Hao, Fan and Wei, Feng and Zhou, Feng and Wang, Zhipeng and Yao, Shichao and Yang, Xueyan and Ma, Zongfang},
  journal={IEEE Transactions on Geoscience and Remote Sensing}, 
  title={Deep Unfolding Residual Decomposition for Infrared Small Target Detection}, 
  year={2026},
  volume={64},
  number={5006013},
  pages={1-13},
  doi={10.1109/TGRS.2026.3694155}}
```

