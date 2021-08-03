# Faster-RCNN Implementation
First version of Faster-RCNN

## Tutorial Link
Following is the [Tutorial](https://debuggercafe.com/faster-rcnn-object-detection-with-pytorch/)


## Installation

Installation using conda and pip

```

conda create --name pytorch python=3.8 --yes

conda activate pytorch

pip install --upgrade torch 

pip install --upgrade torchvision

pip install opencv-python

mkdir -p outputs

```

## Usage

Usage for detecting objects & persons in images & videos

### For inference on images

```
python detect.py --input input/horses.jpg

python detect.py --input input/people.jpg

python detect.py --input input/people.jpg --min-size 1024

```

### For inference on videos

```
python detect_vid.py --input input/video2.mp4

python detect_vid.py --input input/video2.mp4 --min-size 300

```
