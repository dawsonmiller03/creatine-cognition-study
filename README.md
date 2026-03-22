# WIP; Will be completed in May, 2026
# The Impact of Creatine Supplementation on Multiple Object Tracking
A within-subjects experimental study investigating the effects of acute creatine monohydrate supplementation on visual-spatial attention and cognitive performance at Gordon College.

---

## 👥 Research Team

| Role | Name | Email |
|---|---|---|
| Principal Investigator | Dawson Miller | dawsonrmiller03@gmail.com |

**Institution:** Gordon College  
**Project Dates:** April 1, 2026 – April 20, 2026

---

## 📄 Abstract

This study investigates the effects of creatine monohydrate on high-demand cognitive tasks, specifically visual-spatial attention, using a within-subjects double-blind crossover design. While creatine is a well-established supplement, recent research suggests its role in rapid adenosine triphosphate (ATP) resynthesis may significantly benefit the brain's efficiency during intensive cognitive load.

**Hypothesis:** An acute dose (10g) of creatine monohydrate will significantly improve performance on a Multiple Object Tracking (MOT) task compared to performance under placebo conditions.

---

## 🧪 Methods

### Participants

- **Target sample:** N = 24 healthy adults (ages 18–25), recruited from the Gordon College student body
- **Power analysis:** A priori power analysis (G*Power) for matched pairs: effect size d = 0.5, α = 0.05, power = 0.80 → required N = 34; critical t = 2.03
- **Pilot sample:** 22–26 participants (aiming for even male/female distribution)
- **Inclusion criteria:** Normal or corrected-to-normal vision
- **Exclusion criteria:** History of kidney dysfunction, pregnancy, or current creatine use
- **Recruitment:** Word-of-mouth and interpersonal outreach within Gordon College

### Design

Double-blind, within-subjects crossover design. Each participant completes two sessions separated by a minimum of 48 hours — one creatine session and one placebo session.

### Supplementation Protocol

| Condition | Substance | Dose | Delivery |
|---|---|---|---|
| Treatment | Creapure Creatine Monohydrate | 10g | Dissolved in 8oz water |
| Placebo | Cornstarch | 10g | Dissolved in 8oz water |

### Multiple Object Tracking (MOT) Task

The MOT task is administered via computer (Psychtoolbox) and focuses on target identification under dynamic visual conditions:

1. Eight spheres (4 pairs) appear on screen — all initially red
2. Two "target" spheres briefly turn green, then return to red
3. All eight spheres move dynamically in circular motion within each pair
4. After movement stops, either the two original targets or two different spheres turn green
5. Participant presses **Y** (targets match) or **N** (targets do not match)

**Dependent variables:** Response accuracy (% correct) and response time (ms), automatically captured and exported as CSV.

### Participant ID & Anonymization

To maintain anonymity and support the double-blind design, participants are assigned unique codes:

**Format:** `[Sex][Participant Number]_[Condition]`  
**Example:** `m2_t` = Male participant #2, Treatment session | `m2_p` = Male participant #2, Placebo session

- No names or PII are attached to data files
- A master key linking names to codes is stored separately and destroyed upon study completion

---

## 📁 Repository Structure

```
creatine-cognition-study/
│
├── data/
│   ├── raw/                  # Original exported CSV files from MOT task (coded only)
│   ├── processed/            # Cleaned and analysis-ready datasets
│   └── codebook.md           # Variable definitions and ID coding scheme
│
├── analysis/
│   ├── scripts/              # R scripts for statistical analysis (numbered in order)
│   ├── notebooks/            # R Markdown (.Rmd) exploratory notebooks
│   └── output/               # Generated figures, tables, model results
│
├── literature/
│   ├── papers/               # Key reference PDFs
│   └── notes.md              # Literature review notes and summaries
│
├── protocol/
│   ├── study_design.md       # Full study design and hypotheses
│   ├── procedures.md         # Session procedures and MOT task instructions
│   └── IRB/                  # Ethics approval documents
│
├── results/
│   ├── figures/              # Final publication-ready figures
│   └── summary.md            # Key findings and interpretation
│
├── .gitignore
└── README.md
```

---

## 🛠️ Tools & Dependencies

- **R** — statistical analysis and visualization
- **Excel / CSV** — raw data storage and initial export from MOT software
- **Psychtoolbox** — MOT task administration
- **G*Power** — a priori power analysis

Key R packages: `tidyverse`, `ggplot2`, `lme4`, `rmarkdown` *(update as needed)*

---

## 🚀 Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/YOUR_USERNAME/creatine-cognition-study.git
   ```
2. Open in RStudio. Raw data lives in `data/raw/` — **do not modify these files directly.**
3. Run analysis scripts from `analysis/scripts/` in numbered order.

---

## 📄 License

Internal research project — Gordon College, 2026. Not for public distribution without permission.
