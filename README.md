# Artificial Intelligence Foundations — MSc In-Course Assessment
**Module:** CIS4049-N | Artificial Intelligence Foundations  
**Institution:** Teesside University  
**Author:** Siri Chandana Dhurjati  

---

## Project Overview

This repository contains the implementation, report, and supporting materials for the AI Foundations in-course assessment (CIS4049-N). The project applies supervised machine learning techniques to a real-world case study, following the CRISP-DM methodology, and critically evaluates the selection, implementation, and experimental validation of the AI solution.

The case study focuses on **Customer Behaviour Classification and Prediction** using structured tabular data, demonstrating the full machine learning lifecycle — from exploratory data analysis through feature engineering, model training, evaluation, and reflection on commercial implications.

---

## Repository Structure

```
msc-ai-foundations/
├── docs/
│   ├── REPORT-B[StudentID]_Dhurjati_Siri.pdf        ← Written report (4,000 words)
│   ├── PRESENTATION-B[StudentID]_Dhurjati_Siri.pptx ← Presentation slides
│   └── ARTEFACT-B[StudentID]_Dhurjati_Siri/         ← Supporting artefacts
├── src/
│   ├── ai_solution.py                                ← Main Python implementation
│   ├── eda.ipynb                                     ← Exploratory Data Analysis notebook
│   └── model_evaluation.ipynb                        ← Model comparison and results
├── data/
│   └── README.md                                     ← Data description (raw data not included)
├── walkthrough/
│   └── walkthrough_video_link.md                     ← Link to walkthrough video
└── README.md
```

---

## AI Techniques Applied

| Technique | Purpose |
|---|---|
| Exploratory Data Analysis (EDA) | Understanding feature distributions, correlations, and data quality |
| Feature Engineering | Log transformation, label encoding, feature selection |
| Linear Regression | Baseline model for continuous target prediction |
| Decision Tree Regressor | Interpretable non-linear model |
| Random Forest Regressor | Ensemble method — variance reduction via bagging |
| AdaBoost Regressor | Boosting ensemble — sequential error correction |
| XGBoost Regressor | Gradient boosting — best performing model |

---

## Key Results

The project applied CRISP-DM methodology to an insurance dataset of **98,415 records** to build and compare five regression models for customer lifetime value (CLTV) prediction.

| Model | R² | RMSE | MAE |
|---|---|---|---|
| Linear Regression | baseline | — | — |
| Decision Tree | — | — | — |
| Random Forest | — | — | — |
| AdaBoost | — | — | — |
| **XGBoost** | **0.99** | **3,059** | **670** |

XGBoost achieved the best performance across all evaluation metrics, outperforming all baseline models. Full results and discussion are in the written report.

---

## Technologies Used

- **Python** — scikit-learn, XGBoost, pandas, NumPy, Matplotlib, Seaborn
- **Jupyter Notebook** — EDA, experimentation, and model evaluation
- **CRISP-DM** — Cross-Industry Standard Process for Data Mining methodology

---

## Learning Outcomes Addressed

- **PTS1** — Communicating and evaluating complex AI theory
- **PTS2/PTS3** — Critical reflection on implementation decisions and outcomes
- **RKC1/RKC2/RKC3** — Analysis of scientific literature; application of AI techniques; critical appraisal of recent AI research
- **PS1/PS2** — Commercial risk evaluation; autonomous improvement of AI solution performance

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/SiriChandanaDhurjati/msc-ai-foundations.git
cd msc-ai-foundations

# Install dependencies
pip install -r requirements.txt

# Run EDA notebook
jupyter notebook src/eda.ipynb

# Run model training and evaluation
jupyter notebook src/model_evaluation.ipynb
```

---

## Documentation

Full written report, presentation slides, and artefacts are available in the `docs/` folder.  
Please refer to the ICA specification (CIS4049-N-2023-2024) for full assessment context.

---

## Academic Integrity

This work was completed independently in accordance with Teesside University's academic integrity policy. All external sources are cited within the written report.
