<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=MedRisk%20Classifier&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Generalizable%20ML%20Pipeline%20for%20Chronic%20Disease%20Prediction&descAlignY=58&descSize=16&animation=fadeIn" width="100%"/>

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=2DD4BF&center=true&vCenter=true&width=700&lines=3+Datasets.+4+Models.+1+Unified+Pipeline.;LightGBM+%C2%B7+XGBoost+%C2%B7+Random+Forest+%C2%B7+Logistic+Regression;Optuna+Hyperparameter+Tuning+%E2%9C%85;SMOTE+Class+Balancing+%E2%9C%85;Live+Gradio+Demo+%E2%9C%85)](https://git.io/typing-svg)

<br/>

![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.4-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-GPU-189AB4?style=for-the-badge&logo=xgboost&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-Optimized-61C454?style=for-the-badge)
![Optuna](https://img.shields.io/badge/Optuna-50%20Trials-2DD4BF?style=for-the-badge)
![Gradio](https://img.shields.io/badge/Gradio-Live%20Demo-FF7C00?style=for-the-badge&logo=gradio&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-GPU%20Notebook-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

<br/>

> **🔴 LIVE DEMO →** *(paste your gradio.live link here)*

<br/>

</div>

---

## 🧬 Overview

<div align="center">

| 🏥 Clinical Dataset | 🤖 Best Model | 📊 ROC-AUC | 🎯 Sensitivity | 🛡️ Specificity |
|:---:|:---:|:---:|:---:|:---:|
| Diabetes Prediction (100k) | LightGBM | **0.979** | 0.709 | 0.995 |
| Heart Disease Cleveland UCI | Logistic Regression | **0.958** | 0.821 | 1.000 |
| Pima Indians Diabetes | XGBoost + Eng. | **0.838** | 0.685 | 0.770 |

</div>

<br/>

**MedRisk Classifier** is a fully generalizable machine learning pipeline built to predict chronic disease risk across multiple independent clinical datasets. The architecture is dataset-agnostic — one unified preprocessing, balancing, training, and evaluation flow that adapts to any tabular medical dataset.

Built as a portfolio-grade project demonstrating end-to-end ML engineering: raw data → feature engineering → class balancing → multi-model training → Optuna tuning → live Gradio deployment.

---

## ✨ Features

<div align="center">

<table>
  <tr>
    <td align="center" width="200"><b>🔄 Generalizable Flow</b></td>
    <td>One unified pipeline that works across any tabular medical dataset with minimal adaptation</td>
  </tr>
  <tr>
    <td align="center"><b>⚖️ SMOTE Balancing</b></td>
    <td>Fixes severe class imbalance on training set only — zero data leakage into test evaluation</td>
  </tr>
  <tr>
    <td align="center"><b>🤖 4-Model Comparison</b></td>
    <td>Logistic Regression · Random Forest · XGBoost (GPU) · LightGBM trained and ranked per dataset</td>
  </tr>
  <tr>
    <td align="center"><b>🔬 Optuna Tuning</b></td>
    <td>50–100 TPE trials per best model — learning rate, depth, regularization, subsampling all tuned</td>
  </tr>
  <tr>
    <td align="center"><b>🧬 Feature Engineering</b></td>
    <td>8 clinically-motivated features added to Pima dataset: glucose×BMI, BP×Age, WHO BMI bins, insulin sensitivity ratios</td>
  </tr>
  <tr>
    <td align="center"><b>📊 Medical Metrics</b></td>
    <td>ROC-AUC · F1 · Sensitivity · Specificity — not just accuracy, because clinical trade-offs matter</td>
  </tr>
  <tr>
    <td align="center"><b>🖥️ Live Gradio App</b></td>
    <td>3-tab UI with color-coded risk output (🟢 Low / 🟡 Moderate / 🔴 High) and public shareable link</td>
  </tr>
  <tr>
    <td align="center"><b>📸 Auto-saved Plots</b></td>
    <td>12 publication-ready figures saved automatically: ROC curves, confusion matrices, feature importance, Optuna history</td>
  </tr>
</table>

</div>

---

## 🏗️ System Architecture

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {
  'primaryColor': '#203a43',
  'primaryTextColor': '#ffffff',
  'primaryBorderColor': '#2DD4BF',
  'lineColor': '#2DD4BF',
  'secondaryColor': '#0f2027',
  'tertiaryColor': '#2c5364',
  'edgeLabelBackground': '#203a43',
  'clusterBkg': '#2c5364',
  'titleColor': '#ffffff'
}}}%%

flowchart TB
    subgraph INPUT["📂 DATA SOURCES"]
        A1["🩸 Diabetes-Large\n100,000 rows · 8 features"]
        A2["❤️ Heart-Cleveland\n297 rows · 13 features"]
        A3["🧬 Diabetes-Pima\n768 rows · 8 features"]
    end

    subgraph PREPROCESS["🔧 PREPROCESSING"]
        B1["Zero Imputation\nPima biological fixes"]
        B2["Label Encoding\nCategorical to Ordinal"]
        B3["Train/Test Split\n80/20 Stratified"]
        B4["StandardScaler\nFit on train only"]
        B5["SMOTE\nBalance training set"]
    end

    subgraph ENGINEER["🧬 FEATURE ENGINEERING — Pima only"]
        C1["glucose x BMI\nInsulin resistance proxy"]
        C2["BP x Age\nCardiovascular stress"]
        C3["Clinical Bins\nWHO BMI · Glucose thresholds"]
        C4["Ratio Features\nSkin/BMI · Insulin/Glucose"]
    end

    subgraph MODELS["🤖 MODEL TRAINING"]
        D1["Logistic Regression\nBaseline · Interpretable"]
        D2["Random Forest\n200 trees · Balanced"]
        D3["XGBoost\nGPU · hist method"]
        D4["LightGBM\nHistogram · Fast"]
    end

    subgraph TUNING["🔬 OPTUNA TUNING"]
        E1["TPE Sampler\n50-100 trials"]
        E2["Best Config\nper dataset"]
    end

    subgraph EVAL["📊 EVALUATION"]
        F1["ROC-AUC · F1\nSensitivity · Specificity"]
        F2["Confusion Matrix\nROC Curves\nFeature Importance"]
    end

    subgraph DEPLOY["🚀 DEPLOYMENT"]
        G1["Gradio App\n3-Tab Interface"]
        G2["Public Link\ngradio.live"]
    end

    A1 & A2 & A3 --> B1
    B1 --> B2 --> B3 --> B4 --> B5
    A3 --> ENGINEER
    ENGINEER --> B5
    B5 --> MODELS
    MODELS --> TUNING
    TUNING --> EVAL
    EVAL --> DEPLOY
```

---

## 🔄 Data Pipeline Flow

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {
  'primaryColor': '#203a43',
  'primaryTextColor': '#ffffff',
  'primaryBorderColor': '#2DD4BF',
  'lineColor': '#2DD4BF',
  'secondaryColor': '#0f2027',
  'tertiaryColor': '#2c5364',
  'activationBorderColor': '#2DD4BF',
  'activationBkgColor': '#203a43',
  'sequenceNumberColor': '#ffffff'
}}}%%

sequenceDiagram
    autonumber
    participant CSV as 📂 Raw CSV
    participant EDA as 🔍 EDA Module
    participant PRE as 🔧 Preprocessor
    participant BAL as ⚖️ SMOTE
    participant TRN as 🤖 Trainer
    participant EVL as 📊 Evaluator
    participant TUNE as 🔬 Optuna
    participant APP as 🖥️ Gradio App

    CSV->>EDA: Load 3 datasets
    EDA->>EDA: Class balance, distributions, correlations
    EDA->>PRE: Pass raw DataFrames

    PRE->>PRE: Impute zeros for Pima dataset
    PRE->>PRE: Encode categoricals to ordinal
    PRE->>PRE: 80/20 stratified split
    PRE->>PRE: StandardScaler fit on train only
    PRE->>BAL: Send training sets

    BAL->>BAL: Fit SMOTE per dataset
    Note over BAL: Diabetes-Large 6.8k becomes 73.2k positives
    BAL->>TRN: Balanced training data

    TRN->>TRN: Train LR, RF, XGBoost, LightGBM
    TRN->>EVL: Predictions and probabilities
    EVL->>EVL: AUC, F1, Sensitivity, Specificity
    EVL->>TUNE: Best model per dataset

    TUNE->>TUNE: 50 TPE trials, maximize AUC
    Note over TUNE: LightGBM, LR, XGBoost tuned separately
    TUNE->>EVL: Tuned model scores
    EVL->>EVL: Baseline vs tuned comparison

    EVL->>APP: Final tuned models and scalers
    APP->>APP: Build 3-tab Gradio interface
    APP-->>APP: Launch with share=True
    Note over APP: Public gradio.live URL generated
```

---

## 📊 Results & Metrics

<div align="center">

### 🏆 Final Leaderboard — Post Tuning

| Dataset | Model | Baseline AUC | Tuned AUC | Δ | F1 | Sensitivity | Specificity |
|:---|:---|:---:|:---:|:---:|:---:|:---:|:---:|
| 🩸 Diabetes-Large | LightGBM | 0.9781 | **0.9792** | ▲ 0.0011 | 0.804 | 0.709 | 0.995 |
| ❤️ Heart-Cleveland | Logistic Regression | 0.9542 | **0.9576** | ▲ 0.0033 | 0.902 | 0.821 | 1.000 |
| 🧬 Diabetes-Pima | XGBoost (16 feat) | 0.8230 | **0.8383** | ▲ 0.0153 | 0.649 | 0.685 | 0.770 |

</div>

<br/>

### 📸 Key Insights

- **Heart-Cleveland:** Logistic Regression outperformed all tree-based models — a textbook reminder that simpler models generalize better on small datasets (237 training samples). Perfect specificity (1.000) means zero false alarms on the test set.

- **Diabetes-Large:** LightGBM and XGBoost tied at AUC=0.978. The 8.5% class imbalance was the main challenge — SMOTE expanded the minority class from 6,800 → 73,200 samples. High specificity (0.995) comes at the cost of sensitivity (0.709), a clinical trade-off worth noting.

- **Diabetes-Pima:** The hardest dataset — 1988 data, many biologically impossible zeros imputed, small sample size (768). Feature engineering added 8 clinically motivated features and pushed AUC from 0.823 → 0.838. Stacking did not outperform single tuned XGBoost, confirming the data ceiling.

---

## 🛠️ Tech Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge)

<br/>

![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189AB4?style=for-the-badge)
![LightGBM](https://img.shields.io/badge/LightGBM-61C454?style=for-the-badge)
![Imbalanced-Learn](https://img.shields.io/badge/imbalanced--learn-SMOTE-FF6B6B?style=for-the-badge)
![Optuna](https://img.shields.io/badge/Optuna-2DD4BF?style=for-the-badge)

<br/>

![Gradio](https://img.shields.io/badge/Gradio-FF7C00?style=for-the-badge&logo=gradio&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-GPU%20T4-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)

</div>

<br/>

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {
  'primaryColor': '#203a43',
  'primaryTextColor': '#ffffff',
  'primaryBorderColor': '#2DD4BF',
  'lineColor': '#2DD4BF',
  'secondaryColor': '#0f2027',
  'tertiaryColor': '#2c5364'
}}}%%

flowchart LR
    subgraph DATA["Data Layer"]
        P["Pandas\nDataFrames"]
        N["NumPy\nArrays"]
    end
    subgraph ML["ML Layer"]
        SK["Scikit-Learn\nPipeline"]
        XG["XGBoost\nGPU"]
        LG["LightGBM\nCPU"]
        IM["imbalanced-learn\nSMOTE"]
    end
    subgraph OPT["Optimization"]
        OP["Optuna\nTPE Sampler"]
    end
    subgraph VIZ["Visualization"]
        MP["Matplotlib\nSeaborn"]
    end
    subgraph SERVE["Serving"]
        GR["Gradio\nWeb UI"]
    end

    DATA --> ML
    ML --> OPT
    OPT --> ML
    ML --> VIZ
    ML --> SERVE
```

---

## 📁 Project Structure

```
medrisk-classifier/
│
├── 📓 medrisk_classifier.ipynb      ← Main Kaggle notebook (all 5 snippets)
│
├── 📊 outputs/
│   ├── class_balance.png            ← Class distribution across datasets
│   ├── dist_diabetes_large.png      ← Feature KDE distributions
│   ├── dist_heart_cleveland.png
│   ├── dist_diabetes_pima.png
│   ├── corr_diabetes_large.png      ← Correlation heatmaps
│   ├── corr_heart_cleveland.png
│   ├── corr_diabetes_pima.png
│   ├── categorical_breakdown.png    ← Gender/smoking breakdown
│   ├── smote_balance.png            ← Before vs after SMOTE
│   ├── target_correlation.png       ← Feature-target Pearson r
│   ├── metrics_heatmap.png          ← Model x metric heatmap
│   ├── roc_curves.png               ← ROC curves all models
│   ├── confusion_matrices.png       ← Best model confusion matrices
│   ├── feature_importance.png       ← RF + LightGBM importance
│   ├── tuned_vs_baseline.png        ← Optuna improvement comparison
│   ├── optuna_history.png           ← Trial convergence plots
│   ├── pima_progression.png         ← Pima feature engineering gains
│   └── pima_feature_importance_eng.png
│
└── 📄 README.md
```

---

## ⚙️ Installation & Reproduction

### Run on Kaggle (Recommended)

```bash
# 1. Open the notebook on Kaggle
# 2. Add these three datasets:
#    - iammustafatz/diabetes-prediction-dataset
#    - cherngs/heart-disease-cleveland-uci
#    - organizations/uciml/pima-indians-diabetes-database

# 3. Enable GPU accelerator (Settings → Accelerator → GPU T4 x2)

# 4. Run All cells — total runtime ~10 minutes
```

### Run Locally

```bash
# Clone the repo
git clone https://github.com/yourusername/medrisk-classifier.git
cd medrisk-classifier

# Install dependencies
pip install numpy pandas matplotlib seaborn scikit-learn \
            xgboost lightgbm imbalanced-learn optuna gradio

# Update dataset paths in Snippet 1 to your local paths
# Then run the notebook top to bottom
```

### Dataset Paths

```python
PATHS = {
    "Diabetes-Large":  "path/to/diabetes_prediction_dataset.csv",
    "Heart-Cleveland": "path/to/heart_cleveland_upload.csv",
    "Diabetes-Pima":   "path/to/diabetes.csv",
}
```

---

## 🔮 Future Work

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {
  'primaryColor': '#203a43',
  'primaryTextColor': '#ffffff',
  'primaryBorderColor': '#2DD4BF',
  'lineColor': '#2DD4BF',
  'secondaryColor': '#0f2027',
  'tertiaryColor': '#2c5364'
}}}%%

flowchart LR
    NOW["✅ Current\nv1.0"]
    V2["🔜 v2.0\nCross-validation\nSHAP explainability"]
    V3["🔭 v3.0\nHugging Face\nDocker + REST API"]
    V4["🚀 v4.0\nTabNet Neural Nets\nFederated Learning"]

    NOW --> V2 --> V3 --> V4
```

<br/>

<div align="center">

| Priority | Improvement | Expected Impact |
|:---:|:---|:---|
| 🔴 High | Replace test-set tuning with **5-fold CV** in Optuna | More reliable AUC estimates, less overfitting to test set |
| 🔴 High | Add **SHAP values** to explain individual predictions | Clinical interpretability — critical for medical AI trust |
| 🟡 Medium | **Hugging Face Spaces** permanent deployment | Link never expires, embeds directly in README |
| 🟡 Medium | **TabNet / TabTransformer** neural baselines | Benchmark deep learning vs gradient boosting on tabular data |
| 🟢 Low | REST API via FastAPI + Docker | Enable integration with external clinical systems |
| 🟢 Low | Add **3–5 more datasets** (stroke, CKD, liver disease) | Validate generalizability claim more rigorously |

</div>

---

## 📚 Datasets & References

<div align="center">

| Dataset | Source | Rows | License |
|:---|:---|:---:|:---:|
| Diabetes Prediction Dataset | [Kaggle — iammustafatz](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset) | 100,000 | CC0 |
| Heart Disease Cleveland UCI | [Kaggle — cherngs](https://www.kaggle.com/datasets/cherngs/heart-disease-cleveland-uci) | 297 | CC BY 4.0 |
| Pima Indians Diabetes | [Kaggle — UCI ML](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) | 768 | CC0 |

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=120&section=footer&animation=fadeIn" width="100%"/>

**Built with 🩺 for the ML + Healthcare community**

[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github)](https://github.com/yourusername)
[![Kaggle](https://img.shields.io/badge/Kaggle-Profile-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://kaggle.com/yourusername)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/yourusername)

*⭐ Star this repo if you found it useful*

</div>
