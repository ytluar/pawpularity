# PetFinder.my - Pawpularity Contest

Competition link: https://www.kaggle.com/c/petfinder-pawpularity-score <br />
Kaggle competition to predict the popularity of shelter pet photos to help stray cats and dogs finding their homes.

The models here are all trained on Kaggle except for the training of ConvNeXt model which is on Google Colab. Therefore, the paths in the notebook will need to be adjusted.

Paths imported: <br />
GPUtil - https://www.kaggle.com/tusonggao/gputil <br />
timm (PyTorch Image Models) - https://www.kaggle.com/kozodoi/timm-pytorch-image-models <br />
Swin Transformer - https://www.kaggle.com/tanlikesmath/swin-transformer <br />
ConvNeXt - https://github.com/facebookresearch/ConvNeXt <br />

Models are trained in Tensorflow/ fastai PyTorch. Model weights are not added into the repository.

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

The ensemble of the models achieved Top 3% on the private leaderboard. 

Things that wanted to try but did not manage to do due to time constraint: <br />
* Try different models such as ViT, BEiT, EfficientNetV2.
* Use different ensemble methods such as stacking, weighted average etc.
* Adding SVR heads. Details can be found here https://www.kaggle.com/c/petfinder-pawpularity-score/discussion/276724
