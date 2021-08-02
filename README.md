# f-rcnn
First version of Faster-RCNN

##
Tutorial Link: 
https://debuggercafe.com/faster-rcnn-object-detection-with-pytorch/

## 
Installation
``

conda create --name pytorch python=3.6 --yes

conda activate pytorch

pip install torch==1.9.0+cu111 torchvision==0.10.0+cu111 torchaudio==0.9.0 -f https://download.pytorch.org/whl/torch_stable.html


pip install opencv-python

``

##
Usage

###
For inference on images

``
python detect.py --input input/horses.jpg

python detect.py --input input/people.jpg

python detect.py --input input/people.jpg --min-size 1024

``

###
For inference on videos

``
python detect_vid.py --input input/video2.mp4

python detect_vid.py --input input/video2.mp4 --min-size 300

``
