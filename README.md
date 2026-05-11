# Depression Pattern Analysis — CNN Classifier

> **Research Internship Project** — Cotton University, Guwahati, Assam (Jul 2024)  
> Identifying behavioural patterns associated with depression using exploratory data analysis and a CNN-based classifier built in TensorFlow.

---

## Overview

Depression is one of the most underdiagnosed mental health conditions globally, partly because its indicators are distributed across lifestyle, behavioural, and demographic factors rather than a single clinical marker. This project applies machine learning to a structured behavioural dataset to identify which combinations of features are most predictive of depression, and trains a CNN classifier to automate that pattern recognition.

The work was completed as part of a research internship at **Cotton University, Guwahati, Assam**, focusing on data-driven approaches to mental health analytics.

---

## Key Result

| Model | Accuracy | Task |
|---|---|---|
| CNN Classifier (TensorFlow) | **71%** | Binary depression pattern classification |

> The model identified statistically significant correlations between lifestyle factors (sleep, exercise, social behaviour) and depression indicators, providing a data-driven basis for pattern recognition in mental health datasets.

---

## Repository Structure

```
depression-Analysis/
│
├── Depression_analysis.ipynb        # Main notebook: EDA, feature engineering, CNN training
├── depression_analysis_dataset.xlsx # Behavioural dataset used for analysis
└── README.md
```

---

## Dataset

A primary dataset collected via **Google Form survey** as part of the research internship at Cotton University. Respondents self-reported across the following attributes:

- **Age & Gender** — demographic features
- **Symptoms** — self-reported depression-related symptoms
- **Treatment Status** — whether the individual has received therapy or counselling
- **Severity** — self-assessed depression severity rating
- **Family History** — presence of mental health history in the family
- **Lifestyle Factors** — sleep patterns, exercise habits, diet, social activity

Being a self-collected primary dataset (rather than a pre-existing benchmark), the work involved designing the survey instrument, collecting responses, and handling the full data pipeline from raw form responses to model-ready features.

---

## Methodology

### 1. Exploratory Data Analysis (EDA)
- Distribution analysis of age, gender, and severity across the dataset
- Correlation heatmaps to identify features most associated with depression indicators
- Statistical validation using hypothesis testing to confirm feature significance

### 2. Feature Engineering
- Handled missing values and outliers
- Encoded categorical variables (gender, treatment status, family history)
- Normalised continuous features (age, lifestyle scores) for model input

### 3. CNN Classifier
- Built a 1D CNN in TensorFlow/Keras to learn patterns from structured tabular features
- Applied class weighting to handle label imbalance
- Evaluated using accuracy, precision, recall, and F1-score

---

## Requirements

```bash
pip install tensorflow pandas numpy matplotlib seaborn scikit-learn openpyxl
```

**Python version**: 3.8+

---

## How to Run

1. Clone the repository:
```bash
git clone https://github.com/Komal-phogat/depression-Analysis.git
cd depression-Analysis
```

2. Install dependencies (see above)

3. Open the notebook:
```bash
jupyter notebook Depression_analysis.ipynb
```

4. Run cells sequentially — EDA → preprocessing → feature engineering → CNN training → evaluation

---

## Context & Motivation

Mental health analytics is an emerging application area for machine learning, where structured behavioural data can surface patterns that are difficult to detect through clinical observation alone. This project explores whether a CNN — typically used for image data — can effectively learn from structured tabular features when treated as sequential input, and what accuracy is achievable on a real-world behavioural dataset without large-scale data.

---

## Author

**Komal Phogat**  
MSc Data Science, Amity University (2023–2025), GPA: 8.27/10  
Research Intern — Cotton University, Guwahati, Assam  
📧 komalphogat02@gmail.com  
🔗 [github.com/Komal-phogat](https://github.com/Komal-phogat)

---

## Tags

`mental-health` `depression-analysis` `cnn-classifier` `tensorflow` `eda` `behavioural-data` `healthcare-ml` `python` `pandas` `scikit-learn`
