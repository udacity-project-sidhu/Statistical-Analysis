# Statistical Analysis — UCI Bank Marketing Dataset

Project 2 of the Udacity AI Programming Foundations Nanodegree: a complete statistical analysis using descriptive statistics, visualisations, and one hypothesis test, with a written report aimed at both technical and non-technical readers.

## Contents
- `analysis.ipynb` — Jupyter notebook with the full analysis.
- `Statistical_Analysis_Report.pdf` — written report.
- `data/bank-additional-full.csv` — UCI Bank Marketing dataset.
- `requirements.txt` — pinned Python dependencies.

## Reproduce

```
python -m venv Project2-3.12
# Windows
Project2-3.12\Scripts\activate
# macOS / Linux
source Project2-3.12/bin/activate

pip install -r requirements.txt
jupyter lab analysis.ipynb
```

Then run all cells top to bottom. The dataset is included in `data/`; if missing, the load cell auto-downloads it from the UCI repository.

## Environment notes

This project was developed and tested on **Windows 11 with Python 3.12**. `requirements.txt` was generated via `pip freeze` from that environment. If you are reproducing on macOS or Linux and `pip install -r requirements.txt` complains about `pywinpty` (a Windows-only Jupyter terminal dependency), edit that line to `pywinpty==3.0.3 ; sys_platform == "win32"` or remove it — Jupyter will fall back to `ptyprocess` automatically on Unix.

## Dataset

Moro, S., Cortez, P., & Rita, P. (2014). *A data-driven approach to predict the success of bank telemarketing.* Decision Support Systems, 62, 22–31.  
UCI Machine Learning Repository, ID 222: https://archive.ics.uci.edu/dataset/222/bank+marketing