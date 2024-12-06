# WasteSortAI: Automated Waste Sorting

|English|[Русский](README_ru.md)|

## Project Overview
- **Client**: Renue (IT company, Yekaterinburg)
- **Technologies**: Python, Computer Vision, Deep Learning, Object Detection
- **Main Goal**: Automatic classification of waste on a conveyor belt

## Key Technologies
- TensorFlow/PyTorch
- YOLOv11
- OpenCV
- Pandas
- NumPy
- Albumentations
- Tqdm
- PyYAML

## Installation
```bash
git clone https://github.com/V0olkER/WasteSortAI
pip install -r requirements.txt
```

## Project Goal
The goal of the project is to create a model that can recognize different types of waste based on images from the conveyor. This automated system will help optimize the sorting process, increase recycling efficiency, and reduce manual sorting costs.

## Tasks

- Develop and train a computer vision model for object detection in images.
- Evaluate model quality using the mAP (mean Average Precision) metric.

## Key Points

- The dataset includes images taken from cameras installed above the sorting conveyor at the recycling plant.
- The variety of waste types adds complexity, as materials may look different depending on lighting conditions and position on the conveyor.
- The solution should be able not only to detect the presence of waste but also to classify it by type for further sorting.
