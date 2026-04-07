# 🎾 ATP Tennis GOAT Debate — What Does the Data Actually Say?

**Dataset:** ATP Tennis 2000–2023 | **Source:** Kaggle | **Tools:** Python, pandas, matplotlib, seaborn

---

## Background

The Federer–Nadal–Djokovic GOAT debate is one of the loudest arguments in sports. Djokovic now holds the most Grand Slam titles, but a common counter-argument goes something like this:

> *"Djokovic only racked up those titles because Federer and Nadal were already past their prime. The competition wasn't the same."*

It's a reasonable thing to wonder. It's also the kind of claim that tends to get repeated without anyone actually checking the numbers. So I did.

---

## What I'm Trying to Answer

Three questions, roughly in order of complexity:

**1. When were each of the Big 3 actually at their peak?**
Before we can argue about whether someone faced "weakened" competition, we need to establish when each player was prime — and whether those windows overlapped.

**2. How did they perform head-to-head, and when?**
If Djokovic consistently beat Federer and Nadal even during their peak years, the "they were already declining" argument gets a lot harder to make.

**3. How hard were those wins, really?**
Win totals don't tell the whole story. Who did they beat to get there? Were those matches close? Did they win as favorites or as underdogs?

---

## The Dataset

| | |
|---|---|
| **Source** | [Kaggle — ATP Tennis 2000–2023](https://www.kaggle.com/datasets/dissfya/atp-tennis-2000-2023daily-pull) |
| **Coverage** | ATP tour matches from 2000 to 2023 |
| **Rows** | Match-level data (one row per match) |
| **Key columns** | `Player_1`, `Player_2`, `Winner`, `Rank_1`, `Rank_2`, `Tournament`, `Series`, `Surface`, `Round`, `Score`, `Date`, `Odd_1`, `Odd_2` |

The dataset for this project is included in the `Dataset` folder. The data is based on the version 1053 that is downloaded in 29 March 2026. A more updated data should not make a significant changes on the result of this analysis as Novak Djokovic is the only remain active player among the others 2 (Nadal and Federer).

---

## Notebook Structure

The notebook follows a single narrative thread — from raw data to a factual answer, section by section.

**Section 0 — Setup & Data Loading**
Libraries, loading the CSV, first look at the data.

**Section 1 — Cleaning & Feature Engineering**
Deriving what we need: match year, age at match time, Grand Slam flag, and match difficulty (straight sets vs. extended matches).

**Section 2 — The Prime Era**
When was each player actually at their peak? ATP ranking trends and Grand Slam title timelines, overlaid on the same chart so the picture is clear.

**Section 3 — Head-to-Head**
Direct matchup records between the Big 3 — overall, per year, per surface, and filtered to Grand Slams only.

**Section 4 — Quality of Wins**
Who did each player actually beat to win their Grand Slams? Average opponent ranking, frequency of Top 10 wins, and performance in the final rounds.

**Section 5 — Match Difficulty**
Straight sets vs. five-setters. Underdog wins using betting odds as a proxy for pre-match expectations.

**Section 6 — Conclusions & Caveats**
What the data shows, what it doesn't, and where reasonable people can still disagree.

---

## Tools

| Tool | Purpose |
|------|---------|
| `Python` | Core language |
| `pandas` | Data manipulation |
| `matplotlib` | Visualizations |
| `seaborn` | Chart styling |
| `numpy` | Calculations |

---

## A Note on What This Analysis Can and Can't Do

Data can tell you what happened. It can't fully settle a debate that's partly about aesthetics, era differences, and things that never got measured — like how Federer might have performed on a fully healthy knee, or how Nadal's clay dominance would look on a different surface calendar.

What this notebook tries to do is separate the factual claims from the opinions. Some parts of the GOAT argument hold up under scrutiny. Others don't survive contact with the actual numbers.

---

*Dataset credit: [dissfya on Kaggle](https://www.kaggle.com/datasets/dissfya/atp-tennis-2000-2023daily-pull)*
