
# 📝 Cross-Camera Player Re-Identification

## 🎯 Objective

The goal of this project is to identify and map soccer players consistently across two distinct video feeds — a standard `broadcast` view and a top-down `tacticam` view. This task supports tactical analysis and real-time tracking in sports analytics.

---

## 🧠 Methodology

### 1. Detection (YOLOv11)

A custom YOLOv11 model (`best.pt`) was used to detect players in both videos. The model was trained to handle multiple angles and occlusions.

### 2. Feature Extraction

Each player detection was processed to extract:
- **Color histogram** (HSV) for appearance
- **Bounding box center coordinates** for spatial context

### 3. Similarity & Matching

- Features from both views were compared using **cosine similarity**
- Best matches were selected based on thresholds and confidence
- Final ID assignments were stored in `matched_ids.pkl`

---

## 📊 Visualization

Visual output included:
- Bounding boxes labeled with consistent IDs
- Side-by-side display of both views for easy comparison

---

## ⚙️ Tools & Libraries

- Python (Google Colab)
- Ultralytics YOLO
- OpenCV
- scikit-learn
- Matplotlib

---

## 🚧 Challenges

- Different perspectives and lighting conditions
- Occlusions and similar uniforms
- Frame misalignment

---

## ✅ Outcomes

- Matched IDs saved in `matched_ids.pkl`
- Model hosted externally due to GitHub file size limits
- Outputs visualized clearly for both videos

---

## 📁 Files

| File | Description |
|------|-------------|
| `reid_pipeline.ipynb` | Main code |
| `matched_ids.pkl` | Output dictionary of player matches |
| `broadcast.mp4` / `tacticam.mp4` | Input videos |
| `README.md` | Setup instructions |
| `Report.md` | This report |

---

## 👤 Author

Anusha — 2025  
Project | Player Re-Identification
