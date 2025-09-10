# CPGNet

Official Pytorch Code base for "Detecting semantic changes from VHR remote sensing images by integrating semantic correlations and change priors" [Paper](Under Review)

## Introduction

We propose a change prior-guided network, namely CPGNet, which employs a multi-branch paradigm that integrates supplemental changed information to accurately identify diverse types of land cover changes in very high-resolution (VHR) remote sensing image.

## Using the code:

The code is stable while using Python 3.11.0, CUDA >=12.0

- Clone this repository:
```bash
git clone https://github.com/long123524/CPGNet
cd CPGNet
```

To install all the dependencies using conda or pip:

```
PyTorch
OpenCV
tqdm
skimage
timm
...
```

## Data Format

Make sure to put the files as the following structure:

```
inputs
└── <train>
    ├── image1
    |   ├── 001.tif
    │   ├── 002.tif
    │   ├── 003.tif
    │   ├── ...
    |
    └── image2
    |   ├── 001.tif
    |   ├── 002.tif
    |   ├── 003.tif
    |   ├── ...
    └── label1
    |   ├── 001.tif
    |   ├── 002.tif
    |   ├── 003.tif
    |   ├── ...
    └── label2
    |   ├── 001.tif
    |   ├── 002.tif
    |   ├── 003.tif
    |   ├── ...
    
```

For testing and validation datasets, the same structure as the above.

## Datasets

JL-1 dataset: https://www.jl1mall.com/store/ResourceCenter.

SECOND dataset: https://drive.google.com/file/d/1mN8jzCKKK27p3ODGoDgepjiRYGQpB34u/view.

A preprocessed dataset of cropland non-agriculturalization in Xiamen is available at https://drive.google.com/file/d/1beZ8aPzQk-MuSoRbI64upvjMfNAYjP0-/view?usp=sharing.

## Training and testing

Code will be available after our paper is accepted.

## A pretrained weight
A pretrained weight of PVT-V2 on the ImageNet dataset is provided: https://drive.google.com/file/d/1uzeVfA4gEQ772vzLntnkqvWePSw84F6y/view?usp=sharing

### Acknowledgements:

This code-base uses certain code-blocks and helper functions from [HGINet](https://github.com/long123524/HGINet-torch).

### Citation:
If you find this work useful or interesting, please consider citing the following references.
```
@article{long2024,
  title={Semantic change detection using a hierarchical semantic graph interaction network from high-resolution remote sensing images},
  author={Long, Jiang and Li, Mengmeng and Wang, Xiaoqin and Stein, Alfred},
  journal={ISPRS Journal of Photogrammetry and Remote Sensing},
  volume={211},
  pages={318--335},
  year={2024},
  publisher={Elsevier}
}

...
```
