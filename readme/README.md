# Repository overview

Personal coursework for [ML Zoomcamp 2026](https://courses.datatalks.club/ml-zoomcamp-2026/) (DataTalks.Club).

This folder (`readme/`) holds **repo-level** docs. Each homework folder has its own `README.md` and `USER_GUIDE.md`.

## Repository structure

```
2026_MLZoomCamp/
├── README.md                 # Short landing page (links here)
├── environment.yml           # Conda env: ml-zoomcamp
├── readme/                   # Repo-level documentation
│   ├── README.md             # This file
│   └── USER_GUIDE.md         # How to use the repo in general
├── HW1/                      # Homework 1 — Introduction
├── HW2/                      # Homework 2 — Regression
└── HW3/                      # Homework 3 — Classification
    ├── README.md             # HW overview
    ├── USER_GUIDE.md         # How-to + answers
    ├── homework.ipynb
    ├── course_lead_scoring_2026.csv
    └── requirements.txt
```

Each homework folder follows the same pattern (`README.md`, `USER_GUIDE.md`, notebook, data, `requirements.txt`).

## Quick start

```bash
conda activate ml-zoomcamp
cd HW3
jupyter notebook homework.ipynb
```

Or open `HW3/homework.ipynb` in Cursor/VS Code and select kernel **Python (ml-zoomcamp)**.

Env definition: [`../environment.yml`](../environment.yml)

See also: [USER_GUIDE.md](USER_GUIDE.md) · [HW3 docs](../HW3/README.md)

## Course links

| Resource | URL |
|----------|-----|
| Course platform (deadlines + submit) | https://courses.datatalks.club/ml-zoomcamp-2026/ |
| Course GitHub | https://github.com/DataTalksClub/machine-learning-zoomcamp |
| HW3 homework text | https://github.com/DataTalksClub/machine-learning-zoomcamp/blob/main/cohorts/2026/homework/03-classification/homework.md |
| HW3 submit form | https://courses.datatalks.club/ml-zoomcamp-2026/homework/hw03 |

## Current status

| Homework | Folder | Deadline | Status |
|----------|--------|----------|--------|
| HW1 Introduction | [`HW1/`](../HW1/) | Tue 29 Sep 2026, 4:30 AM IST | Notebook ready |
| HW2 Regression | [`HW2/`](../HW2/) | Mon 5 Oct 2026, 23:00 | Notebook ready |
| HW3 Classification | [`HW3/`](../HW3/) | Mon 12 Oct 2026, 23:00 | Notebook ready — submit on course site |

## License / notes

Course materials belong to DataTalks.Club. This repo is for personal solutions and notes.
