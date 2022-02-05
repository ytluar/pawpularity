# PetFinder.my - Pawpularity Contest

https://www.kaggle.com/c/petfinder-pawpularity-score

Predict the popularity of shelter pet photos to help stray cats and dogs finding their homes.

The notebooks here are all trained in Kaggle platform. Therefore, the paths in the notebook will need to be adjusted.

Paths imported:
GPUtil - https://www.kaggle.com/tusonggao/gputil
timm (PyTorch Image Models) - https://www.kaggle.com/kozodoi/timm-pytorch-image-models
Swin Transformer - https://www.kaggle.com/tanlikesmath/swin-transformer
ConvNeXt - https://github.com/facebookresearch/ConvNeXt

Models are trained in Tensorflow/ fastai PyTorch

Special thanks to the fastai starter notebook: https://www.kaggle.com/adityasharma01/fork-of-17-90508-notebook/notebook

Models
| Model  | Local CV (RMSE) |
| ------------- | ------------- |
| swin_224_tiny  | 17.691  |
| swin_224_tiny_custom_head  | 17.657  |
| swin_224_tiny_mixup+cutmix | 17.589 |
| swin_384_base | 17.578 |
| swin_384_large | 17.652 |
| convnext_xlarge | 17.624 |
| Ensembled (Average) | 17.284 |
