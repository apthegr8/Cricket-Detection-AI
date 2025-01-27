# 🦗 YOLOv5s Cricket Detection Model for Raspberry Pi 4

## 🚀 Overview
This guide will help you set up the YOLOv5s model for cricket detection on a Raspberry Pi 4. The model runs locally using the Raspberry Pi camera module.

---

## 📋 Requirements

### Hardware
- **Raspberry Pi 4 (8GB)**
- **Camera Module** for Raspberry Pi

### Software
- **Python 3.9.21** (installable using `pyenv`)
- **PyTorch** (for YOLOv5s model)
  
### Model Architecture
- **YOLOv5s** (Small variant of YOLOv5)
- Pretrained model: **yolo.zip** (download from the provided link)

---

## ⚙️ Environment Setup


### 1. Create Python Environment
Navigate to your project directory:

```bash
cd /in/to/yolo
```

Create a Python virtual environment:

```bash
python3 -m venv yolo
```

cd into the directory of your environment and activate your environment
```bash
cd /path/to/your/yolo && source bin/activate
```

Create a directory anywhere and cd into it

cd back into desktop or anywhere you would like and 

Type in console:
```bash
mkdir yolo_model
```
then:
```bash
cd yolo_model
```

## 🐍 Install python version 3.9.21

python environment setup for raspberry pi using the following guide    
[![Pyenv on Ubuntu](https://img.youtube.com/vi/1Zgo8M9yUtM/0.jpg)](https://www.youtube.com/watch?v=1Zgo8M9yUtM&t=58s)


Run the following to list all installable versions of python

```bash
pyenv install --list
```
then run the following (inside your environment):
```bash
pyenv install 3.9.21
```
set the python version in your folder (yolo_model)
```bash
pyenv local 3.9.21
```
use the following command to check the version your folder is in
```bash
python --version
```


🔥 Pretrained Model
Download the pretrained model from here

cd into project

📦 Install Dependencies
Inside the yolov5 directory, install required dependencies:
```bash
cd into \yolo\yolov5
```
then:
```bash
pip install -r requirements.txt
```
▶️ Running the Model
Once dependencies are installed, navigate back to the yolov5 directory and run the detection script:

```bash
python detect.py --weights /path/to/your/yolo/yolov5/best.pt --img 640 --source 0 --conf-thres 0.5 --iou-thres 0.4 --name cricket_inference
```

This part will need to be replaced with your own path
```bash
/path/to/your/yolo/yolov5/best.pt
```


## 🎬 Demonstration



https://github.com/user-attachments/assets/aebb7323-25f9-47e3-949b-659997b453e5




https://github.com/user-attachments/assets/8a3beec0-3b2a-43af-9d23-759cef3b0445


