# User Guide — repository

How to use this repo for ML Zoomcamp homework in general.  
For homework-specific steps and answers, open that folder’s `USER_GUIDE.md` (e.g. [`HW1/USER_GUIDE.md`](../HW1/USER_GUIDE.md)).

---

## 1. Prerequisites

- Python 3.10+ (3.12/3.13 fine)
- `pip` available in your terminal
- Optional: Jupyter, or Cursor/VS Code with the Python + Jupyter extensions

Install packages inside the homework folder you are working on:

```bash
cd HW1   # or HW2, HW3, …
pip install -r requirements.txt
```

Typical packages: `numpy`, `pandas`, `matplotlib`, `seaborn`, `jupyter`.

---

## 2. Working on any homework

1. Open the homework folder (e.g. `HW1/`).
2. Read that folder’s `README.md` for overview and deadline.
3. Follow that folder’s `USER_GUIDE.md` for run/submit steps.
4. Open `homework.ipynb` and run cells top to bottom.
5. Submit answers on the course site before the deadline.

Use the data file shipped in the homework folder (or re-download from the course repo if missing). Do not invent datasets unless the homework asks for it.

---

## 3. Submitting answers

1. Go to https://courses.datatalks.club/ml-zoomcamp-2026/
2. Open the submit page for that homework (links are in each folder’s README).
3. Enter answers from your notebook.
4. Submit before the deadline.

**Deadline source of truth:** the course site (`data-deadline` in UTC).  
UTC → IST for this course: **23:00 UTC = next calendar day 04:30 AM IST**.

---

## 4. Documentation layout

| Level | Files | Purpose |
|-------|-------|---------|
| Root | `README.md` | Short landing page with links |
| Repo | `readme/README.md`, `readme/USER_GUIDE.md` | Shared overview and workflow |
| Per homework | `HWn/README.md`, `HWn/USER_GUIDE.md` | Module-specific setup, answers, submit URL |

---

## 5. Git workflow (optional)

```bash
git status
git add HWn/
git commit -m "Complete HWn solutions"
git push
```

Remote: https://github.com/asvnphanindra/2026-mlzoomcamp

---

## 6. Troubleshooting (common)

| Problem | Fix |
|---------|-----|
| `ModuleNotFoundError` | `pip install -r requirements.txt` inside the HW folder |
| CSV / data not found | Re-download using the URL in that homework’s USER_GUIDE |
| Notebook kernel wrong | Select the Python env where you installed packages |
| Answers don’t match options | Use the **cohort year** dataset from the course repo for that homework |

---

## 7. Planning / Logseq

Deadlines may also be tracked on your Logseq page `MLZoomCamp`. Always re-check the course site before trusting a deadline.
