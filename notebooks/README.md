# Faster-RCNN Implementation
Using Detectron for Object Detection in images & videos

## Tutorial Link
Following is the [Tutorial](https://detectron2.readthedocs.io/en/latest/tutorials/getting_started.html)


## Installation

Installation using conda and pip

```

conda create --name det python=3.8 --yes

conda activate det

pip install --upgrade torch 

pip install --upgrade torchvision

pip install opencv-python


```

## Usage

Usage for detecting objects & persons in images & videos

### For inference on images

```

cd /opt/detectron2/demo/

python demo.py --config-file ../configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml --input ~/workspace/med/f-rcnn/input/people.jpg ~/workspace/med/f-rcnn/input/street.jpg --opts MODEL.WEIGHTS detectron2://COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x/137849600/model_final_f10217.pkl


```

### For inference on videos

```

cd /opt/detectron2/demo/

python demo.py --config-file ../configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml --video-input ~/workspace/med/f-rcnn/input/video1.mp4 --opts MODEL.WEIGHTS detectron2://COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x/137849600/model_final_f10217.pkl

```