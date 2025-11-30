# Impact of Phone Usage Before Sleep on Sleep Duration and Daily Energy

**Course:** DSA 210 – Introduction to Data Science
**Term:** 2025–2026 Fall
**Project Type:** Individual Project
**Author:** Oguz Temelli
**Date:** October 31, 2025

---

## Project Goal

Quantify the effect of late-night phone use on:

- Total sleep duration
- Morning tiredness
- Daily energy levels

---

## Motivation

Students often use phones before bed, possibly disrupting sleep and alertness. This project uses self-collected data to test whether timing and amount of usage affect sleep and energy.

---

## Research Questions

1. Does phone use shortly before bed reduce sleep duration?
2. Does shorter sleep increase morning tiredness?
3. Does daily screen time correlate with lower daily energy?

---

## Hypotheses

### H1: Phone Usage Before Bed vs Sleep Duration

- **Null Hypothesis (H₀):** There is no correlation between phone usage before bed and sleep duration (ρ = 0)
- **Alternative Hypothesis (H₁):** There is a negative correlation between phone usage before bed and sleep duration (ρ < 0)
- **Test:** Pearson correlation test (one-tailed, negative direction)
- **Variables:** `screen_time_before_sleep_min` (independent) vs `sleep_duration_hours` (dependent)

### H2: Sleep Duration vs Morning Tiredness

- **Null Hypothesis (H₀):** There is no correlation between sleep duration and morning tiredness (ρ = 0)
- **Alternative Hypothesis (H₁):** There is a negative correlation between sleep duration and morning tiredness (ρ < 0)
- **Test:** Pearson correlation test (one-tailed, negative direction)
- **Variables:** `sleep_duration_hours` (independent) vs `morning_tiredness_1_5` (dependent)

### H3: Total Screen Time vs Daily Energy

- **Null Hypothesis (H₀):** There is no correlation between total daily screen time and daily energy level (ρ = 0)
- **Alternative Hypothesis (H₁):** There is a negative correlation between total daily screen time and daily energy level (ρ < 0)
- **Test:** Pearson correlation test (one-tailed, negative direction)
- **Variables:** `total_screen_time_hours` (independent) vs `energy_level_1_5` (dependent)

**Significance Level:** α = 0.05

---

## Data Collection

30 days of self-recorded data (November 1–30, 2024):

- **Sleep data:** Samsung Health automatic tracking
- **Screen time:** Samsung Digital Wellbeing logs  
- **Manual entries:** Google Sheets for morning tiredness, energy levels, and last phone use before sleep

### Variables

| Variable                            | Description                                |
| ----------------------------------- | ------------------------------------------ |
| date                                | Day                                        |
| sleep_duration_hours                | Total sleep                                |
| bedtime                             | Time went to bed                           |
| wake_time                           | Time woke up                               |
| last_phone_use_minutes_before_sleep | Minutes between last screen use and sleep  |
| total_screen_time_hours             | Total daily screen time                    |
| screen_time_before_sleep_min        | Phone usage in last 2 hours before bedtime |
| morning_tiredness_1_5               | (1=not tired, 5=very tired)                |
| energy_level_1_5                    | Daily energy score                         |

---

## Methods

- EDA (distributions, missingness, outliers)
- Correlations and hypothesis tests (t-tests, Pearson r)
- Regression to predict energy from phone/sleep factors
- Visualization of key relationships

---

## Tools

- Python (pandas, numpy, seaborn, matplotlib, scikit-learn)
- Jupyter Notebook
- Google Sheets → CSV

---

## Timeline

| Date      | Task                       |
| --------- | -------------------------- |
| Oct 31    | Submit proposal            |
| Nov 1–30  | Collect data + EDA + tests |
| Jan 2     | Models + report            |
| Jan 9     | Final submission           |

---

## Results

### Exploratory Data Analysis (EDA)

- **Dataset:** 30 days of data (November 1–30, 2024)
- **Missing Values:** None
- **Key Statistics:**
  - Average sleep duration: ~7.5 hours
  - Average screen time before sleep: ~45 minutes
  - Average total screen time: ~6.5 hours
  - Average morning tiredness: ~3.0 (1-5 scale)
  - Average energy level: ~2.0 (1-5 scale)

### Hypothesis Test Results

See `notebooks/hypothesis_tests.ipynb` for detailed statistical analysis.

**Test Method:** Pearson correlation test (one-tailed, α = 0.05)

Results will be updated after running the hypothesis tests notebook.

### Expected Outcomes

- Visualizations showing phone behavior vs sleep/energy relationships
- Statistical significance tests for all three hypotheses
- Behavioral recommendations based on findings

---

## Academic Integrity & AI Disclosure

Planning used AI assistance. Data collection, analysis, and interpretation are manual.
