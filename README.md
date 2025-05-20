# 🧠 Brain Tumor Object Detection using YOLOv8 & YOLOv9 (Google Colab)

This project implements object detection of brain tumors in MRI images using YOLOv8 and YOLOv9 models on Google Colab. The aim is to detect and localize tumors in real-time with high accuracy, supporting early diagnosis and research in medical imaging.

---

## 📌 Features

- ✅ Google Colab-based, no local installation required
- 🧠 Detects and localizes brain tumors from MRI scans
- 📊 Performance comparison between YOLOv8 and YOLOv9
- 🔁 Trained using custom medical dataset (Roboflow)
- 📦 Exports annotated results with bounding boxes
- 🚀 Real-time inference via Colab

---

## 🧠 Models Used

| Model   | Version | Framework  | Accuracy (mAP@0.5) |
|---------|---------|------------|--------------------|
| YOLOv8s | v8.1    | Ultralytics | ~89%               |
| YOLOv9s | v9.0    | Ultralytics | ~91.7%             |

---

## 🩻 Dataset

- **Source**: Roboflow medical dataset (MRI brain tumor scans)
- **Annotations**: YOLO format, with bounding boxes
- **Classes**: Tumor / No Tumor

---

## ⚙️ Google Colab Setup


## 🚀 Usage in Colab

### ✅ Training YOLOv8

```python
!yolo task=detect mode=train model=yolov8s.pt data=data.yaml epochs=100 imgsz=640
