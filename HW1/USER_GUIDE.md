# User Guide — HW1

How to run and submit Homework 1 (Introduction).

Repo-wide workflow: [`../readme/USER_GUIDE.md`](../readme/USER_GUIDE.md)

---

## 1. Setup

```bash
cd HW1
pip install -r requirements.txt
```

Needs: Python 3.10+, NumPy, Pandas, Matplotlib, Seaborn, Jupyter (or Cursor/VS Code Jupyter).

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

- Form: https://courses.datatalks.club/ml-zoomcamp-2026/homework/hw01  
- Deadline: **Tue 29 Sep 2026, 4:30 AM IST**  
- Always confirm on the [course site](https://courses.datatalks.club/ml-zoomcamp-2026/)

---

## 4. Answer sheet

| Question | What it asks | Answer in this repo |
|----------|--------------|---------------------|
| Q1 | Pandas version | Your `pd.__version__` (here: `3.0.5`) |
| Q2 | Number of records | `10000` |
| Q3 | Number of fuel types | `3` |
| Q4 | Columns with missing values | `2` |
| Q5 | Max fuel efficiency (Asia) | `41.2` |
| Q6 | Median horsepower after fillna(mode) | Yes, it decreased |
| Q7 | Sum of weights `w` | `0.369` |

Q1 depends on your machine — submit whatever `pd.__version__` prints.

---

## 5. Learn in public

Module 1 also asks for a social post (LinkedIn and/or X):

- Tag Alexey Grigorev  
- Use `#mlzoomcamp`  
- Templates: in the [official homework](https://github.com/DataTalksClub/machine-learning-zoomcamp/blob/main/cohorts/2026/homework/01-intro/homework.md)

Separate from the numeric submit form.

---

## 6. Troubleshooting

| Problem | Fix |
|---------|-----|
| `ModuleNotFoundError: pandas` | `pip install -r requirements.txt` in `HW1/` |
| CSV not found | Re-download (section 2) |
| Wrong kernel | Pick the env where packages were installed |
| Answers don’t match options | Use the **2026** CSV from this folder / course repo |
