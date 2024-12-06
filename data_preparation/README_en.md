# Data Preparation Notebook Documentation

|  English  |  [Русский](README_ru.md)  |

This document describes the structure and functionality of the data preparation notebook for the waste detection project.

## Project Overview

This notebook is part of the waste detection project aimed at developing an automated waste sorting system. It focuses on preparing and preprocessing the dataset for training machine learning models.

### Main Functions

1. **Library Installation and Import**
   - Installation of required packages (opencv-python, pyyaml, albumentations)
   - Import of all necessary libraries for data processing

2. **Data Loading and Analysis**
   - Creation of directory structure for data organization
   - Loading training (train.csv) and test (test.csv) datasets
   - Analysis of class distribution in the data
   - Visualization of class distribution

3. **Data Processing Functions**
   - Implementation of functions for oversampling imbalanced classes
   - Image augmentation functions (brightness, contrast, blur adjustments)

4. **Data Preparation and Saving**
   - Application of oversampling for class balancing
   - Image augmentation to increase data diversity
   - Saving processed images and annotations

5. **Data Archiving**
   - Creating archive with prepared dataset
   - Saving archive for further use

### Used Libraries

- pandas - for data manipulation and analysis
- matplotlib - for data visualization
- opencv-python - for image processing
- sklearn - for data preprocessing utilities
- albumentations - for image augmentation
- numpy - for numerical operations
- shutil - for file operations
- pathlib - for path handling
- zipfile - for archive operations

### Directory Structure

data_preparation/
├── load-data.ipynb      # main data processing notebook
└── README.md            # documentation (this file)

*Note: The original dataset and processed data are not included in the repository.*

### Usage Instructions

1. Make sure all required libraries are installed
2. Run the notebook cells sequentially
3. Monitor the output for any processing errors
4. Check the final archive in the specified directory

### Notes

- The notebook handles class imbalance through oversampling
- Various augmentation techniques are applied to increase dataset diversity
- All processed data is automatically archived for convenience
- Progress bars show processing status for long operations
