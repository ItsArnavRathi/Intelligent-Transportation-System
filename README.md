#  Intelligent Transportation System

A comprehensive multi-phase traffic management system integrating deep learning, computer vision, and adaptive control algorithms.

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/downloads/)

---

##  Overview

This project implements a complete **Intelligent Transportation System (ITS)** combining:

-  **Traffic Flow Prediction** using LSTM neural networks
-  **Lane Behavior Analysis** using naturalistic driving data (HighD)
-  **Aerial Vehicle Detection** using YOLO + Computer Vision ensemble
-  **Adaptive Signal Control** optimizing green time based on real-time demand

Dashboard Link: https://intelligent-transportation-system.streamlit.app/

### Key Innovation

**Two-Stage Ensemble Vehicle Detection**: Achieves **80-95% recall** on aerial traffic imagery by combining YOLOv8 micro-tiling with classical computer vision.

---

##  Project Structure

```
Intelligent-Transportation-System/
├── notebooks/          # Jupyter notebooks (Phases 2A, 2B, 3, 4)
├── docs/              # Complete documentation
├── data/              # Datasets (not tracked in git)
├── requirements.txt   # Python dependencies
└── README.md
```

---

##  Methodology

### Phase 2A: Lane Behavior Analysis
- **Dataset**: HighD (110,000+ trajectories)
- **Analysis**: Lane changes, speed distribution, driving behavior
- **Output**: CSV files with lane metrics

### Phase 2B: Aerial Vehicle Detection
- **Challenge**: YOLO fails on aerial views
- **Solution**: Two-stage ensemble (YOLO + CV)
- **Result**: 80-95% recall

### Phase 3: Adaptive Signal Control
- **Algorithm**: `GREEN = BASE + α × COUNT × CONGESTION`
- **Performance**: 15-30% efficiency gain

---

##  Key Results

| Phase | Metric | Result |
|---|---|---|
| Lane Analysis | Vehicles Analyzed | 110,000+ |
| Detection | Recall | 80-95% |
| Signal Control | Efficiency Gain | 15-30% |

---

##  Technologies

- **Deep Learning**: PyTorch, YOLOv8
- **Computer Vision**: OpenCV
- **Data**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn

---

##  Citation

```bibtex
@misc{its2026,
  author = {Arnav Rathi},
  title = {Intelligent Transportation System},
  year = {2026},
  url = {https://github.com/ItsArnavRathi/Intelligent-Transportation-System}
}
```

---

##  Contact

**Arnav Rathi**  
GitHub: [@ItsArnavRathi](https://github.com/ItsArnavRathi)

---

**Status**:  Active Development | **Last Updated**: March 2026
