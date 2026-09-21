# Breast Cancer Detection using YOLO

## Dataset Structure

dataset/
│
├── images/
│   ├── train/
│   ├── val/
│   └── test/
│
├── labels/
│   ├── train/
│   ├── val/
│   └── test/
│
└── data.yaml

--------------------------------------------------

## Dataset Path

Main Dataset Folder:

/content/dataset

Training Images:

/content/dataset/images/train

Validation Images:

/content/dataset/images/val

Test Images:

/content/dataset/images/test

Training Labels:

/content/dataset/labels/train

Validation Labels:

/content/dataset/labels/val

Test Labels:

/content/dataset/labels/test

--------------------------------------------------

## data.yaml

path: /content/dataset

train: images/train
val: images/val
test: images/test

names:
  0: benign
  1: malignant
  2: normal

--------------------------------------------------

## YOLO Training

Train Command:

yolo detect train \
model=yolov8n.pt \
data=/content/dataset/data.yaml \
epochs=80\
imgsz=640

--------------------------------------------------

## Output Path

Training Results:

runs/detect/train/

Best Model:

runs/detect/train/weights/best.pt

Last Model:

runs/detect/train/weights/last.pt

--------------------------------------------------

## Inference

yolo detect predict \
model=runs/detect/train/weights/best.pt \
source=test_image.png

--------------------------------------------------

## Classes

0 -> Benign

1 -> Malignant

2 -> Normal