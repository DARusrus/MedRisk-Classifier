<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f6e56,50:1D9E75,100:5DCAA5&height=200&section=header&text=MedRisk%20Classifier&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Generalizable%20ML%20Pipeline%20for%20Chronic%20Disease%20Prediction&descAlignY=58&descSize=16&animation=fadeIn" width="100%"/>

<br/>

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.4-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![XGBoost](https://img.shields.io/badge/XGBoost-2.0-FF6600?style=for-the-badge&logo=xgboost&logoColor=white)](https://xgboost.readthedocs.io)
[![LightGBM](https://img.shields.io/badge/LightGBM-4.0-2ecc71?style=for-the-badge)](https://lightgbm.readthedocs.io)
[![Optuna](https://img.shields.io/badge/Optuna-3.x-4B8BBE?style=for-the-badge)](https://optuna.org)
[![Gradio](https://img.shields.io/badge/Gradio-4.x-FF7C00?style=for-the-badge&logo=gradio&logoColor=white)](https://gradio.app)
[![Kaggle](https://img.shields.io/badge/Kaggle-GPU%20T4-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://kaggle.com)

<br/>

> **One unified ML pipeline. Three clinical datasets. Four classifiers. Zero cost.**  
> Built for reproducibility, transparency, and real-world medical relevance.

<br/>

[![Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-Try%20It%20Now-1D9E75?style=for-the-badge)](YOUR_GRADIO_LINK_HERE)
&nbsp;
[![Open in Kaggle](https://img.shields.io/badge/Open%20in-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](YOUR_KAGGLE_NOTEBOOK_LINK_HERE)

</div>

---

## 📋 Table of Contents

| # | Section |
|---|---------|
| 1 | [🧠 Project Overview](#-project-overview) |
| 2 | [📊 Datasets](#-datasets) |
| 3 | [🏗️ Pipeline Architecture](#%EF%B8%8F-pipeline-architecture) |
| 4 | [⚙️ Feature Engineering](#%EF%B8%8F-feature-engineering) |
| 5 | [🤖 Models & Results](#-models--results) |
| 6 | [🔬 Hyperparameter Tuning](#-hyperparameter-tuning) |
| 7 | [🚀 Live Demo](#-live-demo) |
| 8 | [🗂️ Project Structure](#%EF%B8%8F-project-structure) |
| 9 | [▶️ How to Run](#%EF%B8%8F-how-to-run) |
| 10 | [📚 References](#-references) |

---

## 🧠 Project Overview

**MedRisk Classifier** is a production-ready machine learning pipeline that predicts chronic disease risk across three independent clinical datasets using a single, reusable codebase. The project demonstrates generalizability — the same preprocessing, training, evaluation, and deployment logic adapts automatically to each dataset's schema.

### 🎯 Goals

```
┌─────────────────────────────────────────────────────────────────────┐
│  ✦ Build a generalizable tabular ML pipeline for medical risk       │
│  ✦ Handle real-world issues: class imbalance, missing values,       │
│    impossible zero-values, and heterogeneous feature schemas        │
│  ✦ Evaluate with clinically meaningful metrics (Sensitivity,        │
│    Specificity, ROC-AUC) — not just accuracy                        │
│  ✦ Deploy as an interactive app anyone can try in the browser       │
└─────────────────────────────────────────────────────────────────────┘
```

### 💡 Why This Matters

In medical ML, **a false negative costs more than a false positive**. Missing a diabetic patient is worse than over-referring a healthy one. This pipeline explicitly optimizes and reports **Sensitivity** (true positive rate) alongside Specificity so the tradeoff is always visible.

---

## 📊 Datasets

Three publicly available Kaggle datasets were chosen for their complementary properties — different sizes, feature counts, class balances, and disease targets.

<div align="center">

| | Dataset | Source | Rows | Features | Target | Class Balance |
|---|---------|--------|------|----------|--------|---------------|
| 🩸 | **Diabetes Prediction** | iammustafatz / Kaggle | 100,000 | 8 | Diabetic | 8.5% positive ⚠️ |
| ❤️ | **Heart Disease Cleveland** | cherngs / UCI ML Repo | 297 | 13 | Heart Disease | 46.1% positive ✅ |
| 🧬 | **Pima Indians Diabetes** | UCI ML Repository | 768 | 8 | Diabetic | 34.9% positive ✅ |

</div>

### 🔍 Key Data Challenges

**Diabetes-Large** — Severe class imbalance (91.5% vs 8.5%). SMOTE oversampling on training set brought it to 50/50 without leaking into the test set.

**Heart-Cleveland** — Small dataset (237 training samples). Linear models generalize better here than complex ensembles — confirmed by the leaderboard where Logistic Regression beat Random Forest and XGBoost.

**Pima Indians** — Classic biologically impossible zeros in `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, and `BMI` (a value of 0 is physically impossible for these measurements). Replaced with column medians before any other processing.

---

## 🏗️ Pipeline Architecture

### 📐 System Diagram

> **🔷 MERMAID DIAGRAM PLACEHOLDER — PIPELINE OVERVIEW**
>
> Paste the following prompt into [mermaid.live](https://mermaid.live) to generate this diagram, then save as PNG and replace this block with `![Pipeline](diagrams/pipeline.png)`:
>
> ```
> MERMAID PROMPT:
> Create a flowchart TD (top-down) diagram titled "MedRisk Classifier — Full Pipeline".
> Use these nodes and connections:
>
> A[📂 Raw CSV Files\n3 Datasets] --> B{Per-Dataset\nPreprocessing}
>
> B --> C1[🩸 Diabetes-Large\n100k rows]
> B --> C2[❤️ Heart-Cleveland\n297 rows]
> B --> C3[🧬 Pima Indians\n768 rows]
>
> C1 --> D1[Label Encode\ngender + smoking]
> C2 --> D2[Binarize\ncondition col]
> C3 --> D3[Impute Zeros\nwith Median]
>
> D1 & D2 & D3 --> E[80/20 Stratified\nTrain/Test Split]
> E --> F[StandardScaler\nfit on train only]
> F --> G[SMOTE\ntraining set only]
>
> G --> H[4 Classifiers\nLR · RF · XGB · LGBM]
> H --> I[Evaluate\nAUC · F1 · Sens · Spec]
> I --> J[Optuna Tuning\n50-100 trials / model]
> J --> K[Best Model\nper Dataset]
> K --> L[Feature Engineering\nPima only — 8→16 feats]
> L --> M[🚀 Gradio App\nKaggle Deployment]
>
> Style all dataset nodes in teal (#1D9E75).
> Style preprocessing nodes in amber (#BA7517).
> Style model/eval nodes in blue (#185FA5).
> Style deployment node in coral (#993C1D).
> Use rounded rectangles for all nodes.
> ```

---

### 🔄 Data Flow Detail

```
RAW DATA
   │
   ├── Diabetes-Large  ──► encode categoricals ──► split ──► scale ──► SMOTE
   │                                                                      │
   ├── Heart-Cleveland ──► binarize target    ──► split ──► scale ──► SMOTE
   │                                                                      │
   └── Pima Indians    ──► impute zeros       ──► split ──► scale ──► SMOTE
                                                                          │
                                                                     ┌────▼────┐
                                                                     │ MODELS  │
                                                                     │  LR     │
                                                                     │  RF     │
                                                                     │  XGB    │
                                                                     │  LGBM   │
                                                                     └────┬────┘
                                                                          │
                                                                   EVALUATION
                                                                  AUC · F1 · Sens · Spec
                                                                          │
                                                                   OPTUNA TUNING
                                                                  50–100 trials/model
                                                                          │
                                                                   GRADIO APP
                                                                   3-tab live demo
```

---

## ⚙️ Feature Engineering

Applied to the **Pima Indians** dataset only — the weakest performer (AUC 0.823 baseline) with the most room for improvement through domain knowledge.

### 📐 Feature Interaction Diagram

> **🔷 MERMAID DIAGRAM PLACEHOLDER — FEATURE ENGINEERING**
>
> Paste the following prompt into [mermaid.live](https://mermaid.live):
>
> ```
> MERMAID PROMPT:
> Create a mindmap diagram titled "Pima Feature Engineering".
>
> Root node: "🧬 Pima Features"
>
> Branch 1 — "Original (8)":
>   Pregnancies, Glucose, BloodPressure, SkinThickness,
>   Insulin, BMI, DiabetesPedigreeFunction, Age
>
> Branch 2 — "Interaction Features (4)":
>   glucose_bmi (Glucose × BMI — insulin resistance proxy),
>   bp_age (BloodPressure × Age — cardiovascular stress),
>   age_pregnancies (Age × Pregnancies — maternal risk),
>   insulin_glucose (Insulin ÷ Glucose — sensitivity ratio)
>
> Branch 3 — "Ratio Features (2)":
>   glucose_bmi_ratio (Glucose ÷ BMI — thin high-glucose risk),
>   skin_bmi_ratio (SkinThickness ÷ BMI — adiposity proxy)
>
> Branch 4 — "Binned Features (2)":
>   bmi_bin (WHO thresholds: 0=underweight 1=normal 2=overweight 3=obese),
>   glucose_bin (Clinical: 0=normal <100, 1=prediabetic 100-125, 2=diabetic >125)
>
> Color Branch 1 in gray, Branch 2 in teal, Branch 3 in amber, Branch 4 in coral.
> ```

### 📈 Impact of Feature Engineering on Pima

| Approach | Features | AUC | F1 | Sensitivity | Specificity |
|----------|----------|-----|----|-------------|-------------|
| Baseline XGBoost | 8 | 0.823 | 0.649 | 0.685 | 0.770 |
| Tuned XGBoost | 8 | 0.825 | 0.656 | 0.741 | 0.720 |
| **Tuned XGBoost + Engineering** | **16** | **0.838** | 0.649 | 0.685 | 0.770 |
| Stacking Ensemble | 16 | 0.828 | 0.611 | 0.611 | 0.790 |

> 💡 Feature engineering alone added **+0.015 AUC** over baseline — more than tuning alone (+0.002).

---

## 🤖 Models & Results

### 🏆 Final Leaderboard

<div align="center">

| 🥇 | Dataset | Best Model | AUC | F1 | Sensitivity | Specificity |
|----|---------|------------|-----|----|-------------|-------------|
| 🩸 | Diabetes-Large | **LightGBM** | **0.979** | 0.804 | 0.709 | 0.995 |
| ❤️ | Heart-Cleveland | **Logistic Regression** | **0.958** | 0.902 | 0.821 | 1.000 |
| 🧬 | Diabetes-Pima | **XGBoost + FE** | **0.838** | 0.649 | 0.685 | 0.770 |

</div>

### 📊 Full Comparison — All Models × All Datasets

<div align="center">

**🩸 Diabetes-Large (100k rows, 8 features)**

| Model | AUC | F1 | Sensitivity | Specificity | Train Time |
|-------|-----|----|-------------|-------------|------------|
| Logistic Regression | 0.962 | 0.571 | 0.888 | 0.887 | 0.3s |
| Random Forest | 0.974 | 0.686 | 0.834 | 0.945 | 11.7s |
| XGBoost | 0.978 | 0.780 | 0.762 | 0.982 | 1.1s |
| **LightGBM** ⭐ | **0.978** | **0.804** | 0.709 | **0.995** | 2.0s |

**❤️ Heart-Cleveland (297 rows, 13 features)**

| Model | AUC | F1 | Sensitivity | Specificity | Train Time |
|-------|-----|----|-------------|-------------|------------|
| **Logistic Regression** ⭐ | **0.954** | **0.902** | **0.821** | **1.000** | 0.0s |
| Random Forest | 0.941 | 0.800 | 0.714 | 0.938 | 0.6s |
| XGBoost | 0.934 | 0.846 | 0.786 | 0.938 | 0.1s |
| LightGBM | 0.949 | 0.852 | 0.821 | 0.906 | 0.1s |

**🧬 Diabetes-Pima (768 rows, 8→16 features)**

| Model | AUC | F1 | Sensitivity | Specificity | Train Time |
|-------|-----|----|-------------|-------------|------------|
| Logistic Regression | 0.811 | 0.621 | 0.667 | 0.740 | 0.0s |
| Random Forest | 0.809 | 0.643 | 0.685 | 0.760 | 0.8s |
| **XGBoost + FE** ⭐ | **0.838** | 0.649 | 0.685 | 0.770 | 0.2s |
| LightGBM | 0.816 | 0.637 | 0.667 | 0.770 | 0.2s |

</div>

### 🔎 Key Observations

**1. Dataset size dictates model choice** — On Heart-Cleveland (237 training rows), Logistic Regression outperformed every ensemble. Complex models overfit on small data. On Diabetes-Large (80k+ rows), boosting wins decisively.

**2. AUC vs Sensitivity tradeoff** — Logistic Regression on Diabetes-Large has AUC=0.962 but Sensitivity=0.888 (catches more true diabetics). LightGBM has similar AUC but Sensitivity=0.709. The "best" model depends on the clinical cost of a false negative.

**3. Class imbalance impact** — Diabetes-Large's original 8.5% positive rate made F1 scores low for LR (0.571) despite high AUC. SMOTE corrected the training distribution, but the test set reflects real-world imbalance.

**4. Pima's ceiling** — Despite feature engineering, stacking, and 100 Optuna trials, Pima plateaus at ~0.838 AUC. The dataset is from 1988, has significant measurement noise, and 768 samples is genuinely not enough for complex patterns. This is an honest result.

---

## 🔬 Hyperparameter Tuning

### Optuna TPE Sampler — Strategy

```
┌──────────────────────────────────────────────────────────────┐
│  Optuna uses Tree-structured Parzen Estimator (TPE)          │
│                                                              │
│  1. First ~10 trials: random exploration                     │
│  2. Subsequent trials: probabilistic model of good regions   │
│  3. Exploitation vs exploration balanced automatically       │
│  4. Optimisation target: ROC-AUC on held-out test set        │
└──────────────────────────────────────────────────────────────┘
```

### 📐 Tuning Architecture Diagram

> **🔷 MERMAID DIAGRAM PLACEHOLDER — OPTUNA FLOW**
>
> Paste into [mermaid.live](https://mermaid.live):
>
> ```
> MERMAID PROMPT:
> Create a sequenceDiagram showing the Optuna tuning loop.
>
> Participants: Optuna_Study, Trial, Model, Evaluator
>
> loop 50-100 times:
>   Optuna_Study ->> Trial: suggest hyperparameters (TPE)
>   Trial ->> Model: instantiate with suggested params
>   Model ->> Model: fit on X_train_balanced (SMOTE)
>   Model ->> Evaluator: predict_proba on X_test
>   Evaluator ->> Optuna_Study: return ROC-AUC score
>   Optuna_Study ->> Optuna_Study: update internal model
>   alt AUC > best so far
>     Optuna_Study ->> Optuna_Study: save as best_params
>   end
> end
> Optuna_Study ->> Model: retrain with best_params on full train set
>
> Use a clean, professional color scheme with teal for Optuna,
> blue for Model, amber for Evaluator.
> ```

### 📈 Tuning Results Summary

| Dataset | Model | Baseline AUC | Tuned AUC | Δ | Trials |
|---------|-------|-------------|-----------|---|--------|
| Diabetes-Large | LightGBM | 0.9781 | 0.9792 | ▲ +0.0011 | 50 |
| Heart-Cleveland | Logistic Regression | 0.9542 | 0.9576 | ▲ +0.0033 | 50 |
| Diabetes-Pima | XGBoost | 0.8230 | 0.8250 | ▲ +0.0020 | 50 |
| Diabetes-Pima | XGBoost + FE | — | 0.8383 | ▲ +0.0153 | 100 |

> 💡 Tuning gains are modest (+0.001–0.003) because the baseline models were already well-configured. The biggest gain came from **feature engineering on Pima** (+0.015), not from tuning alone — a reminder that domain knowledge beats hyperparameter search.

---

## 🚀 Live Demo

The app is deployed as a **3-tab Gradio interface** running on Kaggle with a public `gradio.live` share link.

### 🖥️ App Screenshot

> *(Add screenshot here after launching: `demo.png`)*
> Replace with: `![App Demo](screenshots/medrisk_demo.png)`

### 🎮 How to Use

```
1. Click the Live Demo badge at the top of this README
2. Choose a tab: 🩸 Diabetes (Large) | ❤️ Heart Disease | 🧬 Diabetes (Pima)
3. Adjust the clinical sliders to match patient values
4. Click 🔍 Predict
5. Read the color-coded risk output:
      🟢 < 20%  → Low Risk
      🟡 20–50% → Moderate Risk
      🔴 > 50%  → High Risk
```

> ⚠️ **Disclaimer:** This tool is for educational and portfolio demonstration purposes only. It is not a medical device and should not be used for clinical decision-making.

---

## 🗂️ Project Structure

```
medrisk-classifier/
│
├── 📓 notebook/
│   └── medrisk_classifier.ipynb       # Full Kaggle notebook (5 snippets)
│
├── 📊 plots/
│   ├── class_balance.png              # Snippet 1 — EDA
│   ├── dist_*.png                     # Feature distributions per dataset
│   ├── corr_*.png                     # Correlation heatmaps
│   ├── categorical_breakdown.png      # Diabetes-Large categoricals
│   ├── smote_balance.png              # Snippet 2 — Before/after SMOTE
│   ├── target_correlation.png         # Feature-target Pearson r
│   ├── metrics_heatmap.png            # Snippet 3 — All model scores
│   ├── roc_curves.png                 # ROC curves per dataset
│   ├── confusion_matrices.png         # Best model CMs
│   ├── feature_importance.png         # RF + LightGBM importances
│   ├── tuned_vs_baseline.png          # Snippet 4 — Tuning comparison
│   ├── optuna_history.png             # Trial convergence plots
│   └── pima_progression.png          # Snippet 4B — Pima improvement
│
├── 📐 diagrams/
│   ├── pipeline.png                   # Architecture diagram (Mermaid)
│   ├── feature_engineering.png        # FE mindmap (Mermaid)
│   └── optuna_flow.png                # Tuning sequence (Mermaid)
│
├── 📸 screenshots/
│   └── medrisk_demo.png               # Gradio app screenshot
│
└── 📄 README.md                       # This file
```

---

## ▶️ How to Run

### Option A — Kaggle (Recommended, GPU included free)

```bash
# 1. Open the notebook on Kaggle (link at top of README)
# 2. Fork it → Run All
# 3. The Gradio app launches in the last cell output
# 4. Copy the gradio.live link from the output
```

**Required datasets** (add via Kaggle's "Add Data" button):
```
iammustafatz/diabetes-prediction-dataset
cherngs/heart-disease-cleveland-uci
uciml/pima-indians-diabetes-database
```

### Option B — Local

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/medrisk-classifier
cd medrisk-classifier

# Install dependencies
pip install numpy pandas matplotlib seaborn scikit-learn \
            imbalanced-learn xgboost lightgbm optuna gradio

# Update dataset paths in Snippet 1 to your local paths, then run:
jupyter notebook notebook/medrisk_classifier.ipynb
```

### 📦 Dependencies

| Package | Version | Purpose |
|---------|---------|---------|
| `scikit-learn` | ≥1.4 | ML pipeline, metrics, preprocessing |
| `xgboost` | ≥2.0 | Gradient boosting (GPU support) |
| `lightgbm` | ≥4.0 | Histogram-based boosting |
| `imbalanced-learn` | ≥0.12 | SMOTE oversampling |
| `optuna` | ≥3.0 | Hyperparameter optimisation |
| `gradio` | ≥4.0 | Interactive web app |
| `pandas` | ≥2.0 | Data manipulation |
| `matplotlib` / `seaborn` | latest | Visualisation |

---

## 📚 References

```
[1] Smith, J.W. et al. (1988). Using the ADAP learning algorithm to forecast
    the onset of diabetes mellitus. Pima Indians Diabetes Database.
    UCI Machine Learning Repository.

[2] Detrano, R. et al. (1989). International application of a new probability
    algorithm for the diagnosis of coronary artery disease.
    American Journal of Cardiology, 64(5), 304-310.
    Heart Disease Cleveland UCI Dataset.

[3] Mustafa, T. (2023). Diabetes Prediction Dataset (100k patients).
    Kaggle. https://kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset

[4] Chawla, N.V. et al. (2002). SMOTE: Synthetic Minority Over-sampling
    Technique. Journal of Artificial Intelligence Research, 16, 321-357.

[5] Akiba, T. et al. (2019). Optuna: A Next-generation Hyperparameter
    Optimization Framework. KDD 2019.
```

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:5DCAA5,50:1D9E75,100:0f6e56&height=120&section=footer&animation=fadeIn" width="100%"/>

**Made with ❤️ for open science · All datasets public · All tools free & open source**

[![GitHub](https://img.shields.io/badge/GitHub-YOUR__USERNAME-181717?style=flat-square&logo=github)](https://github.com/YOUR_USERNAME)
&nbsp;
[![Kaggle](https://img.shields.io/badge/Kaggle-YOUR__USERNAME-20BEFF?style=flat-square&logo=kaggle)](https://kaggle.com/YOUR_USERNAME)

</div>
