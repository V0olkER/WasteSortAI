# YOLO v11 Model for Waste Detection

|  English  |  [Русский](README_ru.md)  |

This directory contains the implementation of YOLO v11 for waste detection and classification on conveyor belts.

## Directory Structure
```
yolo_v11/
├── yolo-11-model.ipynb  # main notebook with YOLO v11 implementation
├── waste.yaml           # YOLO configuration file
├── yolo11n.pt          # trained model weights
├── requirements.txt     # project dependencies
├── runs/               # training results and logs
└── README.md           # documentation (this file)
```
## Model Description

YOLO v11 implementation for automated waste sorting system. The model is trained to detect and classify 15 different types of waste materials in real-time on conveyor belts.

### Key Features
- Real-time object detection
- Multi-class classification (15 waste categories)
- GPU-accelerated training and inference
- Data augmentation for improved robustness
- Optimized for conveyor belt environments

## Configuration

The `waste.yaml` file contains model configuration including:
- Dataset paths
- Model hyperparameters
- Training settings
- Augmentation parameters

## Model Weights

The `yolo11n.pt` file contains the trained model weights. This file is required for model inference.

## Training Results

The `runs` directory contains:
- Training logs
- Performance metrics
- Model checkpoints
- Validation results
- Visualization of training progress

## Dependencies
- ultralytics
- torch
- opencv-python
- numpy
- pandas
- matplotlib
- PyYAML
- tqdm
- ipywidgets
