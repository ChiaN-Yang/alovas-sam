# Segment Anything for ALOVAS
[[`Github`](https://github.com/facebookresearch/segment-anything)] [[`Paper`](https://arxiv.org/abs/2304.02643)]

## Installation
```
conda env create -f environment.yml
```

## Model Checkpoints
```
mkdir weights
cd weights
wget -q https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth
```

## Inference
```
python amg.py --checkpoint ./weights/sam_vit_h_4b8939.pth --model-type vit_h --input /work/u4307600/nlac_playground/lymphocyte/109-P08_HF2_L+I.svs --points 20000 19000 --level 3 --output out --convert-to-rle
```
