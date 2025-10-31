# Impact of Phone Usage Before Sleep on Sleep Duration and Daily Energy

**Course:** DSA 210 – Introduction to Data Science  
**Term:** 2025–2026 Fall  
**Project Type:** Individual Scientific Data Project  
**Author:** Oguz Temelli  
**Date:** October 31, 2024

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

- **H1:** Higher phone usage before bed → shorter sleep
- **H2:** Shorter sleep → higher morning tiredness
- **H3:** Higher total daily screen time → lower daily energy

---

## Data Collection

~30 days of self-recorded data:
- iPhone Screen Time logs
- Manual entries in Google Sheets for sleep and mood
- Last phone use before bed

### Variables

| Variable | Description |
|----------|-------------|
| date | Day |
| sleep_duration_hours | Total sleep |
| bedtime | Time went to bed |
| wake_time | Time woke up |
| last_phone_use_minutes_before_sleep | Minutes between last screen use and sleep |
| total_screen_time_hours | Total daily screen time |
| screen_time_before_sleep_min | Phone usage in last 2 hours before bedtime |
| morning_tiredness_1_5 | (1=not tired, 5=very tired) |
| energy_level_1_5 | Daily energy score |

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

| Date | Task |
|------|------|
| Oct 31 | Submit proposal |
| Nov 1–28 | Collect data + EDA + tests |
| Jan 2 | Models + report |
| Jan 9 | Final submission |

---

## Expected Results

- Plots showing phone behavior vs sleep/energy
- Significance tests for H1–H3
- Behavioral recommendations

---

## Academic Integrity & AI Disclosure

Planning used AI assistance. Data collection, analysis, and interpretation are manual.
