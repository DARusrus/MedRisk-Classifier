<div align="center">

# 🏥 MedRisk Classifier

**A generalizable machine learning pipeline for chronic disease prediction across three independent clinical datasets — zero cost, fully open source.**

![Python](https://img.shields.io/badge/Python-3.12-blue?style=flat-square)
![XGBoost](https://img.shields.io/badge/XGBoost-Enabled-green?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM-Enabled-green?style=flat-square)
![Optuna](https://img.shields.io/badge/Optuna-HPO-orange?style=flat-square)
![SMOTE](https://img.shields.io/badge/SMOTE-Balancing-purple?style=flat-square)
![Gradio](https://img.shields.io/badge/Gradio-App-red?style=flat-square)
![Kaggle](https://img.shields.io/badge/Kaggle-GPU%20T4-20BEFF?style=flat-square)

[![🚀 Live Demo](https://img.shields.io/badge/🚀-Live%20Demo-0F6E56?style=for-the-badge)](YOUR_GRADIO_LINK)
[![📓 Open in Kaggle](https://img.shields.io/badge/📓-Open%20in%20Kaggle-20BEFF?style=for-the-badge)](YOUR_KAGGLE_LINK)

</div>

---

## 🧠 Project Overview

> **One pipeline. Three datasets.**

MedRisk Classifier demonstrates that a single well-engineered ML codebase can adapt to any tabular clinical dataset — handling class imbalance, missing values, categorical encoding, and heterogeneous feature schemas automatically.

| Metric | Value | Detail |
|--------|-------|--------|
| 🏆 Best AUC Achieved | **0.979** | LightGBM · Diabetes-Large |
| 🏥 Total Patient Records | **101k** | Across all 3 datasets |
| 🤖 Models Trained | **12** | 4 classifiers × 3 datasets |

### Why Sensitivity Matters More Than Accuracy

> In medical classification, **a false negative costs more than a false positive**. Missing a diabetic patient is worse than over-referring a healthy one. This pipeline explicitly tracks and reports **Sensitivity** (true positive rate) alongside **Specificity** so the clinical tradeoff is always visible — not hidden inside a single accuracy number.

---

## 📊 Datasets

> **Three datasets. Three challenges.**

Chosen for complementary properties — different sizes, class balances, and clinical domains — to stress-test generalizability.

### 🩸 Diabetes Prediction
- **Source:** `iammustafatz` / Kaggle
- **Rows:** 100,000 · **Features:** 8
- **Class balance:** ⚠️ 8.5% positive (severe imbalance)
- **Winner:** LightGBM

### ❤️ Heart Disease Cleveland
- **Source:** `cherngs` / UCI ML Repo
- **Rows:** 297 · **Features:** 13
- **Class balance:** ✅ 46.1% positive (balanced)
- **Winner:** Logistic Regression

### 🧬 Pima Indians Diabetes
- **Source:** `uciml` / UCI ML Repo
- **Rows:** 768 · **Features:** 8 → 16 (after feature engineering)
- **Class balance:** ✅ 34.9% positive
- **Winner:** XGBoost + FE

### Dataset Challenges

| Challenge | Dataset | Details |
|-----------|---------|---------|
| ⚠️ **Imbalance** | Diabetes-Large | 91.5% negative. SMOTE applied on training set only — test set stays untouched to reflect real-world distribution. |
| ⚠️ **Small data** | Heart-Cleveland | Only 237 training rows. Complex ensembles overfit — Logistic Regression wins, confirming simpler models generalize better on small data. |
| ⚠️ **Impossible zeros** | Pima Indians | Glucose, BMI, and BloodPressure have biological zeros — physically impossible values used as missing-value codes. Replaced with column medians before any processing. |

---

## 🏗️ Architecture

> **The full pipeline — from raw CSV to deployed Gradio app.**

```
Raw CSV Files — 3 Datasets
         │
         ├────────────────────┬────────────────────┐
         ▼                    ▼                    ▼
  Diabetes-Large        Heart-Cleveland       Pima Indians
  100k rows · 8f        297 rows · 13f        768 rows · 8f
         │                    │                    │
  Encode categoricals   Binarize target       Impute zeros
  gender+smoking        condition 0-4→0/1     median replacement
         │                    │                    │
         └────────────────────┴────────────────────┘
                              │
              ┌───────────────┼───────────────┐
              ▼               ▼               ▼
         80/20 Split    StandardScaler      SMOTE
         stratified     fit on train only   train only
              └───────────────┴───────────────┘
                              │
         ┌────────────────────┼────────────────────┐
         ▼                    ▼                    ▼                    ▼
  Logistic Reg.        Random Forest           XGBoost             LightGBM
         └────────────────────┴────────────────────┘
                              │
              ┌───────────────┴───────────────┐
              ▼                               ▼
          Evaluate                      Optuna Tuning
    AUC · F1 · Sens · Spec            50–100 trials/model
              └───────────────┬───────────────┘
                              ▼
                  Gradio App — Kaggle Deploy
```

---

## ⚙️ Feature Engineering

> **Raw features weren't enough. So we built better ones.**

Applied exclusively to Pima Indians — the weakest performer — using clinical domain knowledge to construct **8 new features** from the original 8.

### Original Features (8)
`Pregnancies` `Glucose` `BloodPressure` `SkinThickness` `Insulin` `BMI` `DiabetesPedigreeFunction` `Age`

> After zero-imputation with column medians (374 impossible insulin values, 227 skin values replaced).

### Interaction Features (4)
`glucose_bmi` `bp_age` `age_pregnancies` `insulin_glucose`

> Clinically motivated products and ratios — glucose×BMI captures insulin resistance, BP×Age captures cardiovascular stress.

### Ratio Features (2)
`glucose_bmi_ratio` `skin_bmi_ratio`

> Thin patients with high glucose have a distinct risk profile invisible to either feature alone. Skin-to-BMI ratio is an adiposity proxy.

### Clinical Bins (2)
`bmi_bin` `glucose_bin`

> WHO BMI thresholds (under/normal/over/obese) and clinical glucose thresholds (normal / pre-diabetic / diabetic) encoded as ordinal integers.

### AUC Progression on Pima

| Model | AUC |
|-------|-----|
| Baseline XGBoost (8 features) | 0.823 |
| Tuned XGBoost (8 features) | 0.825 |
| **Tuned XGBoost (16 engineered features)** | **0.838** |

> Feature engineering (+0.015 AUC) outperformed hyperparameter tuning alone (+0.002) — **domain knowledge beats search**.

---

## 🏆 Results

> **Every model. Every metric.**

Four classifiers trained per dataset. Evaluated on Accuracy, ROC-AUC, F1, Sensitivity, and Specificity.

### 🥇 Winners by Dataset

| Dataset | Best Model | AUC | F1 | Sensitivity | Specificity |
|---------|-----------|-----|----|-------------|-------------|
| 🩸 Diabetes-Large | **LightGBM** | 0.979 | 0.804 | 0.709 | 0.995 |
| ❤️ Heart-Cleveland | **Logistic Regression** | 0.958 | 0.902 | 0.821 | 1.000 |
| 🧬 Pima Indians | **XGBoost + FE** | 0.838 | 0.649 | 0.685 | 0.770 |

### Full Model Comparison

#### 🩸 Diabetes-Large — 100k rows · 8 features · LightGBM T4 GPU

| Model | AUC | F1 | Sensitivity | Specificity | Train Time |
|-------|-----|----|-------------|-------------|------------|
| Logistic Regression | 0.962 | 0.571 | 0.888 | 0.887 | 0.3s |
| Random Forest | 0.974 | 0.686 | 0.834 | 0.945 | 11.7s |
| XGBoost | 0.978 | 0.780 | 0.762 | 0.982 | 1.1s |
| ⭐ **LightGBM** | **0.978** | **0.804** | 0.709 | **0.995** | 2.0s |

#### ❤️ Heart-Cleveland — 297 rows · 13 features · LR wins on small data

| Model | AUC | F1 | Sensitivity | Specificity | Train Time |
|-------|-----|----|-------------|-------------|------------|
| ⭐ **Logistic Regression** | **0.954** | **0.902** | 0.821 | **1.000** | 0.0s |
| LightGBM | 0.949 | 0.852 | 0.821 | 0.906 | 0.1s |
| XGBoost | 0.934 | 0.846 | 0.786 | 0.938 | 0.1s |
| Random Forest | 0.941 | 0.800 | 0.714 | 0.938 | 0.6s |

#### 🧬 Pima Indians — 768 rows · 8→16 features · Feature engineering applied

| Model | AUC | F1 | Sensitivity | Specificity | Train Time |
|-------|-----|----|-------------|-------------|------------|
| ⭐ **XGBoost + FE** | **0.838** | 0.649 | 0.685 | 0.770 | 14.4s |
| LightGBM | 0.816 | 0.637 | 0.667 | 0.770 | 0.2s |
| XGBoost baseline | 0.823 | 0.649 | 0.685 | 0.770 | 0.2s |
| Logistic Regression | 0.811 | 0.621 | 0.667 | 0.740 | 0.0s |

> **Key insight — dataset size dictates model choice.** On Heart-Cleveland with only 237 training rows, Logistic Regression outperformed every ensemble method. Pima's ceiling of 0.838 AUC reflects genuine data limitations (1988 dataset, noisy measurements, 768 samples) — not a pipeline failure. Honest results are more valuable than inflated ones.

---

## 🔬 Hyperparameter Tuning

> **Optuna TPE. 50–100 trials each.**

Tree-structured Parzen Estimator — probabilistic search that learns from past trials to focus on promising regions of the hyperparameter space.

| Dataset | Model | Baseline AUC | Tuned AUC | Gain |
|---------|-------|-------------|-----------|------|
| Diabetes-Large | LightGBM | 0.9781 | 0.9792 | **+0.0011** |
| Heart-Cleveland | Logistic Regression | 0.9542 | 0.9576 | **+0.0034** |
| Pima Indians | XGBoost + FE | 0.8230 | 0.8383 | **+0.0153** |

---

## 🚀 Live Demo

Three-tab Gradio app deployed on Kaggle. **No login required.**

| Tab | Model | Inputs |
|-----|-------|--------|
| 🩸 Diabetes Risk | LightGBM | 8 inputs |
| ❤️ Heart Disease | Logistic Reg. | 13 inputs |
| 🧬 Pima Diabetes | XGBoost | 8 inputs |

**How to use:**
1. Pick a tab for your use case
2. Adjust the clinical sliders to match patient values
3. Click **Predict** — get a color-coded risk score instantly

**Risk levels:**
- 🟢 `< 20%` — Low Risk
- 🟡 `20–50%` — Moderate Risk
- 🔴 `> 50%` — High Risk

> ⚠️ *For educational purposes only. Not a medical device. Consult a qualified healthcare professional.*

---

## ▶️ How to Run

### A — Kaggle (Recommended)

Open the notebook, fork it, click **Run All**. GPU T4 included free. The Gradio app launches in the last cell output with a public link.

**Required datasets (add via Kaggle UI):**
```
iammustafatz/diabetes-prediction-dataset
cherngs/heart-disease-cleveland-uci
uciml/pima-indians-diabetes-database
```

### B — Local Setup

Clone the repo, install dependencies, update dataset paths in Snippet 1, then run the notebook.

```bash
pip install numpy pandas matplotlib seaborn \
    scikit-learn imbalanced-learn \
    xgboost lightgbm optuna gradio
```

### Dependencies

| Package | Purpose |
|---------|---------|
| `scikit-learn` | Preprocessing, metrics, Stacking |
| `xgboost` | Gradient boosting with GPU (CUDA hist) |
| `lightgbm` | Histogram-based boosting, fast at scale |
| `imbalanced-learn` | SMOTE oversampling |
| `optuna` | Bayesian HPO via TPE sampler |
| `gradio` | Interactive web app + share link |
| `pandas` / `numpy` | Data manipulation |
| `matplotlib` / `seaborn` | All visualizations (13 plot files) |

---

## 📚 References

1. **Smith, J.W. et al. (1988).** Using the ADAP learning algorithm to forecast the onset of diabetes mellitus. *Proceedings of the Annual Symposium on Computer Application in Medical Care.* Pima Indians Diabetes Database — UCI ML Repository.

2. **Detrano, R. et al. (1989).** International application of a new probability algorithm for the diagnosis of coronary artery disease. *American Journal of Cardiology, 64(5), 304–310.* Heart Disease Cleveland UCI Dataset.

3. **Mustafa, T. (2023).** Diabetes Prediction Dataset — 100,000 patient records. *Kaggle.* kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset

4. **Chawla, N.V. et al. (2002).** SMOTE: Synthetic Minority Over-sampling Technique. *Journal of Artificial Intelligence Research, 16, 321–357.*

5. **Akiba, T. et al. (2019).** Optuna: A Next-generation Hyperparameter Optimization Framework. *Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining.*

---

<div align="center">

🏥 **MedRisk Classifier** — Built for open science

All datasets public · All tools free & open source · Kaggle GPU T4

[GitHub](https://github.com/YOUR_USERNAME) · [Kaggle](https://kaggle.com/YOUR_USERNAME) · [Live Demo](YOUR_GRADIO_LINK)

</div>
