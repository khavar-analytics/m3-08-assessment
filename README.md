![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Assessment | Statistical Inference in Practice

## Overview

Statistical inference is the bridge between a sample and the broader population it represents. In this assessment you will move beyond descriptive summaries and use hypothesis testing and confidence intervals to draw conclusions that hold up under uncertainty.

You will work with a provided dataset that contains multiple variables suitable for different types of tests. Part of the challenge is deciding which test fits each question — a skill that separates analysts who follow recipes from those who truly understand the methodology.

The assessment closes with an executive summary, because the value of any analysis is only realized when its results are communicated clearly and accurately to decision-makers.

## Learning Goals

- Perform exploratory checks for data quality and assumption violations before testing
- Select the appropriate statistical test for a given research question and data structure
- Execute t-tests, chi-square tests, and related non-parametric alternatives correctly
- Construct and interpret confidence intervals at specified significance levels
- Conduct a basic power analysis to evaluate test reliability
- Write a concise executive summary translating statistical results into actionable insights

## Prerequisites

- Python 3.9+
- Libraries: pandas, numpy, scipy, statsmodels, matplotlib, seaborn

```bash
pip install pandas numpy scipy statsmodels matplotlib seaborn
```

## Requirements

1. **Fork** the assessment repository to your GitHub account.
2. **Clone** your fork locally.
3. Work inside the Jupyter notebook named **`m3-08-assessment.ipynb`**.
4. Commit and push your work regularly.

## Tasks

### Task 1 — Data Exploration and Assumption Checks

1. Load the dataset and perform a quick EDA (shape, types, missing values, distributions).
2. For each numeric variable you plan to test, check normality (Shapiro-Wilk or Q-Q plot) and equal-variance assumptions (Levene's test).
3. Identify and document any assumption violations and state how they influence your test selection.

### Task 2 — Hypothesis Test Selection and Execution

1. Formulate at least three research questions that can be answered with the dataset (e.g., comparing group means, testing independence of categorical variables).
2. For each question:
   a. State the null and alternative hypotheses.
   b. Justify your choice of test (e.g., independent t-test, paired t-test, Mann-Whitney U, chi-square test of independence).
   c. Run the test and report the test statistic, p-value, and effect size.
   d. State your conclusion in plain language.

### Task 3 — Confidence Intervals

1. Compute 95% confidence intervals for at least two population parameters (e.g., a mean difference, a proportion).
2. Visualize the confidence intervals using error-bar or forest plots.
3. Interpret each interval: What does it tell you about the parameter? How does it relate to the hypothesis test result?

### Task 4 — Power Analysis

1. For one of your hypothesis tests, perform a post-hoc power analysis.
2. Determine the minimum sample size needed to detect the observed effect at 80% power and α = 0.05.
3. Discuss whether the dataset provides sufficient power and what this means for the reliability of your conclusions.

### Task 5 — Executive Summary

1. Write an executive summary (400–600 words) aimed at a non-technical stakeholder.
2. Cover: the business question, key findings, confidence levels, limitations, and recommended actions.
3. Avoid raw statistical jargon — translate p-values and confidence intervals into practical language.

## Submission

### What to submit

- A completed Jupyter notebook (`m3-08-assessment.ipynb`) with all code, outputs, and markdown explanations.
- The executive summary can be included as a final markdown section in the notebook.

### Definition of done

- [ ] EDA and assumption checks are documented with visualizations
- [ ] At least three hypothesis tests are correctly selected, executed, and interpreted
- [ ] Confidence intervals are computed, visualized, and interpreted
- [ ] Power analysis is performed for at least one test
- [ ] Executive summary is 400–600 words and accessible to non-technical readers
- [ ] All hypotheses include null/alternative statements and effect sizes
- [ ] Notebook runs top-to-bottom without errors

### How to submit

1. Stage and commit your changes:
   ```bash
   git add .
   git commit -m "Complete m3-08 assessment"
   ```
2. Push to your fork:
   ```bash
   git push origin main
   ```
3. Open a **Pull Request** from your fork to the original repository.
4. Paste the Pull Request URL into the Student Portal.

## Evaluation Criteria

| Criterion | Weight | Description |
|---|---|---|
| Assumption Checks | 15% | Thorough verification of test assumptions with clear documentation |
| Test Selection & Execution | 25% | Correct test choice, proper execution, and accurate reporting |
| Confidence Intervals | 20% | Correct computation, clear visualization, and meaningful interpretation |
| Power Analysis | 10% | Correct implementation and thoughtful discussion of implications |
| Executive Summary | 20% | Well-structured, clear, and actionable for non-technical readers |
| Code Quality | 10% | Clean, well-organized notebook that runs without errors |
