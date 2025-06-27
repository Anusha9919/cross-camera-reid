
# ⚽ Cross-Camera Player Re-Identification

This project identifies and maps soccer players across two camera views — `broadcast.mp4` and `tacticam.mp4`.

---

## 📦 Model File – `best.pt`

Due to GitHub's 100MB file size limit, the YOLO model is not included in the repository.

👉 **Download the trained YOLO model from Google Drive:**

[🔗 Download best.pt](https://drive.google.com/file/d/1BDOJiRgQz_UK9touoFsN36zyEesevoy5/view?usp=sharing)

---

## 🧪 How to Run (Colab)

1. Upload the following to your Colab environment:
   - `best.pt`
   - `broadcast.mp4`
   - `tacticam.mp4`

2. Run `reid_pipeline.ipynb`.

3. Output: `matched_ids.pkl` and visual side-by-side player matches.

---

## 🗂 Files

| File | Description |
|------|-------------|
| `reid_pipeline.ipynb` | Main pipeline notebook |
| `broadcast.mp4`, `tacticam.mp4` | Input videos |
| `matched_ids.pkl` | Output player mapping |
| `Report.md` | Project summary |
| `README.md` | Setup instructions (this file) |

---

## 👤 Author

Anusha — 2025
