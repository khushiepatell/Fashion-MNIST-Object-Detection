# Fashion-MNIST Object Detection Workspace using YOLOv8

An end-to-end computer vision pipeline that adapts the classic Fashion-MNIST image classification dataset into an object detection task using YOLOv8, built with PyTorch and Ultralytics.

## 🚀 Project Overview
Instead of standard classification, this project implements an image-masking workflow to dynamically generate bounding box targets (`bbox_from_mask`) for clothing items. A YOLOv8 Nano architecture is then trained, fine-tuned, and benchmarked directly on these custom-engineered datasets.

## 📊 Performance Metrics (Final Epoch)
* **Overall Evaluation Accuracy:** 79.12%
* **Mean Average Precision (mAP50):** 0.88
* **mAP50-95:** 0.772

### Class-Wise Precision Breakdowns:
* **Trouser:** 0.98 Precision | 0.94 Recall
* **Bag:** 0.95 Precision | 0.98 Recall
* **Sneaker:** 0.96 Precision | 0.87 Recall
* **Ankle Boot:** 0.96 Precision | 0.92 Recall

## 🛠️ Repository Structure
* `Fashion_MNIST_YOLOv8.ipynb` - Core pipeline notebook (Data processing, training, evaluation)
* `fashion.yaml` - Model dataset routing configurations
* `requirements.txt` - Fixed software library dependencies 

## 📦 Getting Started
1. Clone this repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Run the Jupyter notebook to rebuild the data folders and execute inference.
