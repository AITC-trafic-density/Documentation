# Revolutionizing Traffic Management with AI-Powered Machine Vision  
### A Step Toward Smart Cities

This repository contains the official implementation and supplementary materials for the paper:

> **Revolutionizing Traffic Management with AI-Powered Machine Vision: A Step Toward Smart Cities**  
> *The First Biennial National Conference on the Application of Artificial Intelligence in Traffic Control*  
> **25–26 February 2025**, University of Isfahan, Iran

---

## 📌 Overview

Rapid urbanization and increasing vehicle density have created critical challenges for modern traffic management systems.  
This project explores the use of **AI-powered machine vision** and **deep learning-based object detection** to enable **real-time traffic monitoring, vehicle counting, anomaly detection, and congestion-aware driver notification**.

By leveraging advanced YOLO-based architectures and real-world surveillance data, the proposed system contributes toward the realization of **intelligent traffic management systems** aligned with the vision of **smart cities**.

---

## 🚦 Key Contributions

- Real-time vehicle detection and counting using **YOLOv8** and **YOLOv11**
- AI-driven detection of traffic anomalies (e.g., congestion, sudden stops, accidents)
- Threshold-based overcrowding analysis for urban roads
- Backend analytics for dynamic traffic condition assessment
- Driver notification system using highway display monitors
- Real-world dataset collected from multiple locations in Isfahan province

---

## 🧠 Methodology

### 1. Data Collection
- Traffic images collected from **10 high-traffic locations** in Isfahan
- Diverse scenarios including:
  - Different times of day
  - Various weather conditions
  - Multiple traffic density levels
- Total of **300 base images**, augmented to **3000 images**

### 2. Data Labeling
- Manual annotation of:
  - Vehicle types (cars, motorcycles, buses, trucks, etc.)
  - Traffic events and anomalies
  - Bounding boxes for all detected objects

### 3. Preprocessing & Augmentation
- Auto-orientation and resizing to **640×640**
- Data augmentation (10 variations per image)
- Dataset split:
  - Training: 2400 images
  - Validation: 300 images
  - Testing: 300 images

### 4. Model Training
- Models used:
  - **YOLOv8**
  - **YOLOv11**
- Training configuration:
  - Optimizer: AdamW
  - Epochs: 100
  - Mixed Precision (AMP) enabled
  - TensorBoard monitoring
- Partial layer freezing for training stability

---

## 📊 Evaluation Results

| Model   | Precision | Recall | mAP@50 | mAP@50–95 |
|--------|-----------|--------|--------|-----------|
| YOLOv8 | 86.1%     | 73.0%  | 87.4%  | 68.2%     |
| YOLOv11| 89.7%     | 72.3%  | 81.3%  | 62.4%     |

**YOLOv8** demonstrated superior overall performance, particularly in recall, mAP, and real-time anomaly detection, making it more suitable for deployment in real-world traffic systems.

---

## 🖥️ System Architecture

1. Surveillance cameras capture real-time traffic footage  
2. YOLO-based detection models analyze video frames  
3. Backend computes vehicle counts and congestion levels  
4. Overcrowded streets are detected using predefined thresholds  
5. Drivers receive live warnings and alternative route suggestions via roadside displays  

---

## 📚 Citation

If you use this work in your research, please cite:

```
@inproceedings{Hosseini2025TrafficAI,
  title={Revolutionizing Traffic Management with AI-Powered Machine Vision: A Step Toward Smart Cities},
  author={Hosseini DolatAbadi, Seyed Hossein and Hashemi, Sayyed Mohammad Hossein and Hosseini, Mohammad and AliHosseini, Moein-Aldin},
  booktitle={The First Biennial National Conference on the Application of Artificial Intelligence in Traffic Control},
  year={2025},
  organization={University of Isfahan}
}

```
<hr>

## 👥 Authors

- **Seyed Hossein Hosseini DolatAbadi** – University of Isfahan  
  📧 s.h.hosseini@mehr.ui.ac.ir  

- **Sayyed Mohammad Hossein Hashemi** – University of Isfahan  
  📧 mhtrxz@gmail.com  

- **Mohammad Hosseini** – Ilam University  
  📧 40013119812@ilam.ac.ir  

- **Moein-Aldin AliHosseini** – University of Isfahan  
  📧 moeinaldin2022@gmail.com  

---

## 📜 License

This project is intended for **academic and research purposes**.  
For **commercial usage or deployment**, please contact the authors.

---

## 🌍 Toward Smarter Cities

This project represents a step toward integrating **AI-driven machine vision** into intelligent transportation systems, with the goal of improving **traffic efficiency, road safety, and overall urban quality of life**.

