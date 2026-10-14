# 📈 Progression Analysis Of Parkinson's Disease

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![Status](https://img.shields.io/badge/status-completed-brightgreen)

## 📌 Overview

A clinical data analysis project studying how Parkinson's disease (PD) progresses over time across motor, cognitive, functional and quality of life measures, and which factors influence that progression.

The project combines three parts:
1. **Statistical and progression analysis** of a 70-patient clinical dataset
2. **Drug analysis** comparing PD medications by UPDRS III improvement
3. **A clinical case study** following one patient from symptom onset through diagnosis and treatment

This work was carried out under the guidance of **Dr. Shrivarthan**, `[Neurologist]`, Vihaa Hospital, in collaboration with a movement disorders neurologist.

## 🗂️ Dataset

- **Source:** Collected through clinical evaluations in collaboration with a movement disorders neurologist
- **Size:** 70 patients × 24 variables
- **Data is not included** in this repository to protect patient privacy

**Variables collected**

| Category | Variables |
|----------|-----------|
| Demographics | Age, Sex, Family History |
| Disease timeline | Date of Diagnosis, Disease Duration |
| Motor and severity | UPDRS Parts I to IV, Hoehn & Yahr Stage, Finger Tapping Speed |
| Mobility and balance | Timed Up and Go (TUG), 10-Meter Walk Test, Berg Balance Scale |
| Cognition and mood | MMSE, Geriatric Depression Scale (GDS) |
| Function and quality of life | ADL Score, PDQ-39 |
| Treatment | Levodopa, Dopamine Agonist and MAO-B Inhibitor dosages |
| Other | Comorbidities, Genetic Testing Results (SNCA, LRRK2, PARK2) |

## 🧪 Methodology

### 1. Baseline Assessment
- Descriptive statistics across demographic, clinical and treatment variables
- Distribution comparison of clinical variables across Hoehn & Yahr stages
- Correlation heatmap to explore relationships and multicollinearity
- Histograms and KDE plots to study data spread and outliers

### 2. Progression Analysis
- Rate of change of each clinical feature over disease duration
- Time series and longitudinal analysis of UPDRS Part III scores per patient
- Linear regression of UPDRS Part III against disease duration
- ANOVA and chi-square tests
- Change-point detection (dynamic programming) to find shifts in UPDRS Part III trajectories

### 3. Segmentation Analysis
- By medication: Levodopa, Dopamine Agonist and MAO-B Inhibitor dosage groups
- By disease severity: Hoehn & Yahr stage
- By demographics: age and sex
- Across all clinical measures over disease duration

### 4. Factors Influencing Progression
- Literature review of age at onset, sex, family history, medication, comorbidities, genetics, environment, lifestyle and psychosocial support
- Feature importance analysis to rank the variables most associated with progression

### 5. Drug Analysis
- Comparison of mean UPDRS III improvement for Levodopa-Carbidopa, Ropinirole, Pramipexole, Rasagiline, Selegiline, Bromocriptine and placebo

### 6. Clinical Case Study
- A 53-year-old patient followed from early symptoms to diagnosis and treatment
- Structured patient interviews, movement and posture observation, handwriting samples, MRI review and prescription history

## 📊 Key Findings

- **Cohort:** 51.4% female, 60% with a family history of PD, 62.9% at Hoehn & Yahr Stage 2, 57.1% negative on genetic testing
- **Motor progression:** UPDRS Part III showed a small positive association with disease duration (slope 0.0273 per year)
- **Heterogeneity:** Patients followed very different trajectories, with some stable, some fluctuating and some steadily worsening
- **Feature importance:** Motor and mobility measures ranked highest, with UPDRS Part III as the top feature, followed by finger tapping speed, genetic testing results and the 10-meter walk test
- **Medications:** In the drug comparison, Levodopa-Carbidopa and Bromocriptine showed the highest mean UPDRS III improvement
- **Case study:** Non-motor and subtle motor signs (knee pain, balance issues, micrographia, sleep talking, fatigue) appeared years before diagnosis; MRI ruled out other structural causes

> These are exploratory findings from a small cohort and are not intended as clinical recommendations.

## 🛠️ Tech Stack

| Area | Tools |
|------|-------|
| Language | Python |
| Data analysis | Pandas, NumPy, SciPy |
| Statistics and ML | scikit-learn, statsmodels |
| Change-point detection | ruptures |
| Visualization | Matplotlib, Seaborn |

## 🔒 Ethics And Privacy

Patient data was collected with clinical supervision. All data in this repository is anonymized, and no identifiable patient information is shared.

## 🙏 Acknowledgements

Carried out under the guidance of **Dr. Shrivarthan**, Vihaa Hospital. Thanks to the movement disorders neurologist who supported data collection, and to the patient who shared her journey for the case study.

## 👤 Author

**Sushmitha K**
