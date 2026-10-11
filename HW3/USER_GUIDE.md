# User Guide — HW3

How to run and submit Homework 3 (Classification).

Repo-wide workflow: [`../readme/USER_GUIDE.md`](../readme/USER_GUIDE.md)

---

## 1. Setup

Use the dedicated conda env **`ml-zoomcamp`** (Python 3.12).

```bash
conda activate ml-zoomcamp
```

If `scikit-learn` is missing:

```bash
pip install -r requirements.txt
# or recreate: conda env update -f ../environment.yml
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

This folder already includes `course_lead_scoring_2026.csv`. To re-download:

```powershell
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/DataTalksClub/machine-learning-zoomcamp/main/cohorts/2026/data/course_lead_scoring_2026.csv" -OutFile "course_lead_scoring_2026.csv"
```

### Data prep reminders

- Missing categorical values → `'NA'`
- Missing numerical values → `0.0`
- Target column: `converted`
- Use the exact `train_test_split` calls from the official homework (`random_state=42`)

---

## 3. Submit

- Form: https://courses.datatalks.club/ml-zoomcamp-2026/homework/hw03
- Deadline: **Mon 12 Oct 2026, 23:00**
- Always confirm on the [course site](https://courses.datatalks.club/ml-zoomcamp-2026/)

---

## 4. Answer sheet

| Question | What it asks | Answer in this repo |
|----------|--------------|---------------------|
| Q1 | Mode of `industry` | `technology` |
| Q2 | Biggest correlation (numerical pair) | `interaction_count` and `lead_score` |
| Q3 | Biggest mutual information (categorical) | `lead_source` |
| Q4 | Logistic regression val accuracy (2 decimals) | `0.65` |
| Q5 | Feature with smallest accuracy difference | `number_of_courses_viewed` |
| Q6 | Best regularization `C` (3-decimal accuracy) | `0.001` |

---

## 5. Troubleshooting

| Problem | Fix |
|---------|-----|
| `ModuleNotFoundError: sklearn` | `pip install scikit-learn` (or `pip install -r requirements.txt`) |
| CSV not found | Re-download (section 2) |
| Wrong kernel | Pick **Python (ml-zoomcamp)** |
| Answers don’t match options | Use the **2026** lead-scoring CSV from this folder / course repo |
| Q3 / Q4 off | Confirm you filled NAs, used training set for MI, and exact split seeds |
