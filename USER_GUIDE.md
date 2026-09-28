# User Guide — 2026 ML ZoomCamp

How to use this repository for ML Zoomcamp homework.

---

## 1. Prerequisites

- Python 3.10+ (3.12/3.13 fine)
- `pip` available in your terminal
- Optional: Jupyter, or Cursor/VS Code with the Python + Jupyter extensions

Install packages for a homework folder (example: HW1):

```bash
cd HW1
pip install -r requirements.txt
```

Typical packages: `numpy`, `pandas`, `matplotlib`, `seaborn`, `jupyter`.

---

## 2. Working on a homework

1. Open the homework folder (e.g. `HW1/`).
2. Open `homework.ipynb`.
3. Run cells top to bottom (Run All).
4. Compare your printed outputs with the **Answer** cells / summary table.
5. Copy those answers into the official submit form on the course site.

Do **not** invent new data files unless the homework asks for it. Use the CSV that ships in the homework folder (or re-download from the course repo if missing).

### Re-download HW1 data (if needed)

```bash
cd HW1
# PowerShell
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/DataTalksClub/machine-learning-zoomcamp/main/cohorts/2026/data/car_fuel_efficiency_2026.csv" -OutFile "car_fuel_efficiency_2026.csv"
```

Or with `wget` / browser Save As from the same URL.

---

## 3. Submitting answers

1. Go to the course platform: https://courses.datatalks.club/ml-zoomcamp-2026/
2. Open the homework submit page (HW1: https://courses.datatalks.club/ml-zoomcamp-2026/homework/hw01).
3. Enter the multiple-choice / numeric answers from your notebook.
4. Submit before the deadline.

**Deadline source of truth:** the course site (`data-deadline` in UTC).  
This course uses UTC → IST as: **23:00 UTC = next calendar day 04:30 AM IST**.

HW1 deadline: **Tue 29 Sep 2026, 4:30 AM IST**.

---

## 4. HW1 answer cheat-sheet

| Question | What it asks | Answer used in this repo |
|----------|--------------|--------------------------|
| Q1 | Pandas version | Your `pd.__version__` (here: `3.0.5`) |
| Q2 | Number of records | `10000` |
| Q3 | Number of fuel types | `3` |
| Q4 | Columns with missing values | `2` |
| Q5 | Max fuel efficiency (Asia) | `41.2` |
| Q6 | Median horsepower after fillna(mode) | Yes, it decreased |
| Q7 | Sum of linear-regression weights `w` | `0.369` |

Q1 may differ on another machine — submit whatever `pd.__version__` prints for you.

---

## 5. Learn in public (course requirement)

Module 1 asks you to post about what you learned (LinkedIn and/or X/Twitter):

- Tag Alexey Grigorev
- Use `#mlzoomcamp`
- Templates are in the official homework markdown

This is separate from the numeric submit form.

---

## 6. Git workflow (optional)

```bash
git status
git add HW1/
git commit -m "Complete HW1 solutions"
git push
```

Remote: https://github.com/asvnphanindra/2026-mlzoomcamp

---

## 7. Troubleshooting

| Problem | Fix |
|---------|-----|
| `ModuleNotFoundError: pandas` | `pip install -r requirements.txt` inside the HW folder |
| CSV not found | Re-download into the HW folder (section 2) |
| Notebook kernel wrong | Select the Python env where you installed packages |
| Answers don’t match options | Confirm you used the **2026** CSV from the course repo, not an older dataset |

---

## 8. Official materials

- Module 1 materials: https://github.com/DataTalksClub/machine-learning-zoomcamp/tree/main/01-intro  
- HW1 text: https://github.com/DataTalksClub/machine-learning-zoomcamp/blob/main/cohorts/2026/homework/01-intro/homework.md  
- Slack (questions): linked from the course platform  

For planning / deadlines tracked in Logseq, see page `MLZoomCamp` in your personal Logseq graph — always re-check the course site before trusting a deadline.
