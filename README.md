---

## Key Findings

- ~80% of traffic in the dataset is anomalous (heavily imbalanced)
- DoS attacks dominate — SYN flood and smurf are the most frequent
- TCP protocol is strongly associated with attack traffic vs UDP for normal
- `src_bytes`, `serror_rate` and `count` are the most discriminative features
- Isolation Forest achieves competitive F1-score on unsupervised detection

---

## Notebooks Overview

| Notebook | Content |
|---|---|
| `01_exploration` | Shape, dtypes, label distribution, null check |
| `02_cleaning` | Encoding, feature selection, normalization |
| `03_visualization` | 5+ charts — distributions, correlations, protocol analysis |
| `04_anomaly_detection` | Isolation Forest · StandardScaler · classification report · confusion matrix |

---

## How to Run

```bash
# 1. Clone the repo
git clone https://github.com/roua-24/network-intrusion-eda.git
cd network-intrusion-eda

# 2. Create virtual environment
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # Linux / Mac

# 3. Install dependencies
pip install -r requirements.txt

# 4. Download dataset and place in data/raw/
# https://www.kaggle.com/datasets/galaxyh/kdd-cup-1999-data

# 5. Launch Jupyter
jupyter notebook
```

---

## Related Project

This project is part of a portfolio focused on network supervision and AI-based anomaly detection.  
See also : [NOC-Edge FTTH — Embedded AI for Proactive GPON Detection](https://github.com/roua-24/NOC-Edge-FTTH-with-Embedded-Ai-for-Proactive-Detection)

---

## Author

**Roua Jendoubi**  
Graduate in Information & Communication Technologies — Universite Tunis El Manar  
Specialization : Networks · Embedded AI · Cybersecurity  
[github.com/roua-24](https://github.com/roua-24)