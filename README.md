## Summary of Current Implementation

- Implemented data loading and preprocessing for `news_articles.csv`, `train_users.csv`, and `test_users.csv` (missing-value handling and feature encoding).
- Trained a multinomial logistic regression classifier to predict user categories (`User1`, `User2`, `User3`) using `age`, `income`, `clicks`, and `purchase_amount`, and evaluated it on `test_users.csv`. Currently the test accuracy of it is .329

# Student Submission Checklist (Lab 3)

Before submitting your Lab 3 assignment, ensure that **all items below are completed**. Submissions that do not follow this checklist may receive partial or no credit.

---

## 🔹 Repository and Branching

[x] The repository is correctly created on GitHub.
[x] All work is committed to **exactly one branch** named
`firstname_U20230xxx`.
[x] **No work is pushed to `master**`.
[x] The correct branch is pushed to GitHub.

---

## 🔹 Notebook Submission

[x] Exactly **one** Jupyter Notebook (`.ipynb`) is submitted.
[x] The notebook is placed at the **root of the repository**.
[x] The notebook is named **exactly**:
`lab3_results_<roll_number>.ipynb`.
[x] The notebook runs **top to bottom without errors**.
[x] All outputs (plots, tables, metrics) are visible in the notebook.

---

## 🔹 Sampler Usage

- The provided `sampler` package is used **without modification**.
- The sampler is initialized using your correct roll number `i`.
- Rewards are obtained **only** via `sampler.sample(j)`.
- No hard-coded or synthetic rewards are used.

---

## 🔹 Contextual Bandit Implementation

- User category is treated as the **context**.
- News category is treated as the **bandit arm**.
- The arm index mapping follows the specification in the lab handout.
- All three algorithms are implemented:
  - Epsilon-Greedy
  - Upper Confidence Bound (UCB)
  - SoftMax

---

## 🔹 Evaluation and Plots

- Classification accuracy is reported on `test_users.csv`.
- Reinforcement learning simulation is run for **T = 10,000 steps**.
- Plots include:
  - Average Reward vs. Time (per context)
  - Hyperparameter comparison plots
- All plots have labeled axes, legends, and titles.

---

## 🔹 README.md Requirements

- README.md is present at the repository root.
- It explains the overall approach and design decisions.
- It summarizes key results and observations.
- It includes clear instructions to reproduce the experiments.
- All external references (if any) are properly cited.

---

## Important Note

> Submissions that do not follow the specified branch name, notebook naming convention, or sampler usage rules may not be evaluated.

