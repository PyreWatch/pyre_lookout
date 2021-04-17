# pyre-lookout
> YOLOv5 model trainer which produces models for image-based fire detection

## General info
Pyre-lookout generates models for fire and smoke detection. It is baesd on Yolov5. Training results are saved at /yolov5/runs/train/. Currently there are 5 results. We use the best one, yolov5l_best, for our pyre-watch porject. The training setting used is at /yolov5/models/custom_yolov5l.yaml. The traing and test images we used are in data and test folders. There are about 3000 images.

## Setup
To use it you need to install required packages in yolov5/requirements.txt. Run\
  pip install -r requirements.txt
  
## Inference
To detect smokes in images using trained model, run\
  python detect.py --weights runs/train/yolov5l_best/weights/best.pt --img 640 --conf 0.25 --source 'your images'
 ### Example Result:
 ![example](./ExampleResult.jfif)
 
## Source
This project is based on Yolov5. (https://github.com/ultralytics/yolov5)
