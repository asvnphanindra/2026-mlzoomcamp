# User Guide — HW2

How to run and submit Homework 2 (Regression).

Repo-wide workflow: [`../readme/USER_GUIDE.md`](../readme/USER_GUIDE.md)

---

## 1. Setup

Use the dedicated conda env **`ml-zoomcamp`** (Python 3.12).

```bash
conda activate ml-zoomcamp
```

In Cursor/VS Code, select kernel **Python (ml-zoomcamp)** for `homework.ipynb`.

Interpreter path: `C:\Users\phani\miniconda3\envs\ml-zoomcamp\python.exe`

---

## 2. Run the notebook

1. Open `homework.ipynb`.
2. Run all cells top to bottom.
3. Read the **Answer** markdown cells and the summary table at the end.
4. Enter those values on the submit form.

### Data file

This folder already includes `car_fuel_efficiency_2026.csv`. To re-download:

```powershell
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/DataTalksClub/machine-learning-zoomcamp/main/cohorts/2026/data/car_fuel_efficiency_2026.csv" -OutFile "car_fuel_efficiency_2026.csv"
```

---

## 3. Submit

- Form: https://courses.datatalks.club/ml-zoomcamp-2026/homework/hw02
- Deadline: **Mon 5 Oct 2026, 23:00**
- Always confirm on the [course site](https://courses.datatalks.club/ml-zoomcamp-2026/)

---

## 4. Answer sheet

| Question | What it asks | Answer in this repo |
|----------|--------------|---------------------|
| Q1 | Column with missing values | `horsepower` |
| Q2 | Median of `horsepower` | `254` |
| Q3 | Better fill for NAs (0 vs mean) | With mean |
| Q4 | Best regularization `r` | `0` |
| Q5 | Std of RMSE across seeds 0–9 | `0.029` |
| Q6 | Test RMSE (seed 9, r=0.001) | `2.236` |
