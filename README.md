# Machine-Learning-for-Robotics---YoloV8-Training-Model---Test-tube-Detection-Based-on-the-Lid
Hi, my name is Nathanael. This repository contains the source code for my project, with a focus on the training and visualization components.

**Group Members:**
Abram Sparkle -  2702354395
Nathanael Frederick Kristandi - 2702276563 
Berton Kennard - 2702354376 
Roby Wisargi - 2702272073

**Lecture:**
D7040 - RICKY REYNARDO SISWANTO, S.T., M.Kom.

**Note:**
The model provided in this repository has already been trained. If you want to retrain the model, you need to train it by yourself.


I trained the model using the following command, executed directly in the terminal from the project’s main directory (with the correct path already set):
yolo detect train model=yolov8s.pt data="C:/Users/Nathanael F/Documents/Semester5/CK/my_dataset/data.yaml" epochs=100 imgsz=640 batch=16 device=0 workers=0 cache=True

**Explanation:**

This command is run in the terminal, where:
- model=yolov8s.pt is the base YOLOv8 model
- data=.../data.yaml is the dataset configuration path
- epochs=100 sets the number of training epochs
- imgsz=640 defines the input image size
- batch=16 sets the batch size
- device=0 uses the GPU
- workers=0 avoids multiprocessing issues on Windows
- cache=True speeds up training by caching the dataset
