Car Colour Detection Model with GUI & People Counter

This project is developed as part of the internship task for detecting car colors at traffic signals. The model detects cars, classifies their colors, counts people present, and displays visual output with colored rectangles and a user interface.

Features

- Car color classification using VCoR dataset
- People and object detection using YOLOv5
- Red rectangles for **blue cars**, blue rectangles for **other cars**
- Counts and displays number of people present in the image
- Simple GUI preview using Python (Tkinter + OpenCV)
- Evaluation with accuracy, precision, recall, and confusion matrix



---

Datasets Used

1. VCoR Dataset (Vehicle Color Recognition)
- Local Path: `D:/archive (13)`
- Classes: blue, white, black, silver, red, etc.

2. Microsoft COCO (Zhao et al. 2017)
- Local Path: `D:/archive (12)`
- Used for people detection using YOLOv5

> Datasets are not uploaded due to size. Please place them locally at the above paths.

---

Training

- Model: `ResNet18` (PyTorch) for color classification
- Object Detection: YOLOv5 for cars and people
- Jupyter Notebook: Located in `2_Training/train_color_classifier.ipynb`
- Achieved Accuracy: Above 70%

---

GUI Instructions

- Run `car_color_gui.py` in `4_GUI/`
- Select an input image
- It will:
  - Detect and classify car color
  - Show red boxes for blue cars, blue boxes for others
  - Count and show number of people present

---

Evaluation Metrics

Stored in `5_Evaluation/metrics.txt`:

- Accuracy: 72.4%
- Precision: 71.8%
- Recall: 73.2%
- Confusion Matrix: included in metrics file

---

📦Installation

Install all required packages using:
```bash
pip install -r requirements.txt
