 # YOLO v11 Testing for Waste Detection

 |  English  |  [Русский](README.md)  |

This notebook contains code for testing and making predictions using the trained YOLO v11 model for waste classification on conveyor belts.

## Main Components

1. Files used from the `yolo_v11` directory:
   - `waste.yaml` - configuration file with class descriptions
   - `yolo11n.pt` - trained model weights file

2. Notebook functionality:
   - Loading the pre-trained model
   - Making predictions on new images
   - Visualizing detection results

## Waste Classes

The model distinguishes 15 types of waste:
1. PET (transparent) (green)
2. PET (transparent) (brown)
3. PET (transparent) (blue)
4. PET (transparent)
5. PET (transparent) (dark blue)
6. PET (black)
7. PET (white)
8. PET (with sticker)
9. PET (flacon)
10. PET (household chemicals)
11. PND (household chemicals)
12. PND packet
13. Other plastic
14. Other plastic (transparent)
15. Not plastic

## Dependencies

Main libraries:
- ultralytics
- torch
- opencv-python
- numpy
- pandas
- matplotlib
- PyYAML
- tqdm
- ipywidgets

## Project Structure

```
waste-detection/
├── yolo_v11/
│   ├── waste.yaml    # model configuration
│   └── yolo11n.pt   # model weights
└── yolo_test/
    ├── test_images/  # folder for test images
    └── results/      # prediction results
```
