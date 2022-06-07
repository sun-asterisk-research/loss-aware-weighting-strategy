
# To run experiment on YOLOR:
```shell
python train.py --batch-size 64 --img 640 640 --data data/coco.yaml --cfg models/yolor-ssss-dwt.yaml --weights '' --device 0 --name yolor-ssss-dwt-loss-aware1 --hyp hyp.scratch.s.yaml --epochs 300
```
# To run experiment on YOLOX:
```shell
export YOLOX_DATADIR=/path/to/dataset

CUDA_VISIBLE_DEVICES=0 python -m yolox.tools.train -n yolox-s -d 1 -b 64 --fp16 -o
```