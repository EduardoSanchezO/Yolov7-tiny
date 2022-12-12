To run the code you need to have installed some linux distribution, 
in this case the commands that I will put in this file are from the ubuntu distribution. 

The network trained was a tiny yolov7 with the Coco dataset.
The network classifies 80 classes which are:

'person', 'bicycle', 'car', 'motorcycle', 'airplane', 'bus', 'train', 'truck', 'boat', 'traffic light',
 'fire hydrant', 'stop sign', 'parking meter', 'bench', 'bird', 'cat', 'dog', 'horse', 'sheep', 'cow',
 'elephant', 'bear', 'zebra', 'giraffe', 'backpack', 'umbrella', 'handbag', 'tie', 'suitcase', 'frisbee',
 'skis', 'snowboard', 'sports ball', 'kite', 'baseball bat', 'baseball glove', 'skateboard', 'surfboard',
 'tennis racket', 'bottle', 'wine glass', 'cup', 'fork', 'knife', 'spoon', 'bowl', 'banana', 'apple',
 'sandwich', 'orange', 'broccoli', 'carrot', 'hot dog', 'pizza', 'donut', 'cake', 'chair', 'couch',
 'potted plant', 'bed', 'dining table', 'toilet', 'tv', 'laptop', 'mouse', 'remote', 'keyboard', 'cell phone',
 'microwave', 'oven', 'toaster', 'sink', 'refrigerator', 'book', 'clock', 'vase', 'scissors', 'teddy bear',
 'hair drier', 'toothbrush'

If you want to train your own network or do transfer learning here below is a link where you can do that.
https://github.com/WongKinYiu/yolov7.git

The steps to run the image detector are shown below:

1.OPEN TERMINAL  
click ctrl+alt+t

2.DOWNLOAD FOLDER 
Download and enter the folder:

$  git clone https://github.com/EduardoSanchezO/Yolov7-tiny.git

$ cd Yolov7-tiny/

3.ANACONDA ENVIRONMENT
We have to create an anaconda environment.write the following line code:

$ conda create -n detectobj python=3.6

$ source activate detectobj
 
That´s all!!

3. INSTALL PACKAGES AND DEPENDENCIES
Run the following command:

$ pip install -r requirements.txt 

In this step we have to have pip installed in our ubuntu distribution.

4.EXECUTE
Finally we execute the following line of code.

$ python detect.py --source prueba/i1.jpg

In the source option you can make several choices:
0                               # webcam
img.jpg                         # image
vid.mp4                         # video
screen                          # screenshot
path/                           # directory
list.txt                        # list of images
list.streams                    # list of streams
'path/*.jpg'                    # glob
'https://youtu.be/Zgi9g1ksQHc'  # YouTube
'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream

In the folder prueba/ save some images for testing. 
If you want to use the webcam you only need to set 0.
