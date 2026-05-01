<div align="center">

<!-- BADGES -->
<p>
  <img src="https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/XGBoost-FF6600?style=flat-square&logo=xgboost&logoColor=white"/>
  <img src="https://img.shields.io/badge/LightGBM-00D09C?style=flat-square"/>
  <img src="https://img.shields.io/badge/Optuna_HPO-6A0DAD?style=flat-square"/>
  <img src="https://img.shields.io/badge/SMOTE-8B5CF6?style=flat-square"/>
  <img src="https://img.shields.io/badge/Gradio_App-EF4444?style=flat-square&logo=gradio&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kaggle_GPU_T4-20BEFF?style=flat-square&logo=kaggle&logoColor=white"/>
</p>

<br/>

# 🏥 MedRisk Classifier

### One pipeline &nbsp;·&nbsp; Three datasets &nbsp;·&nbsp; Zero cost &nbsp;·&nbsp; Fully open source

<br/>

<table>
  <tr>
    <td align="center"><b>🏆 Best AUC</b><br/><code>0.979</code><br/><sub>LightGBM · Diabetes-Large</sub></td>
    <td align="center"><b>🏥 Patient Records</b><br/><code>101k</code><br/><sub>Total across all datasets</sub></td>
    <td align="center"><b>🤖 Models Trained</b><br/><code>12</code><br/><sub>4 classifiers × 3 datasets</sub></td>
  </tr>
</table>

</div>

---

## 📊 Datasets &nbsp;·&nbsp; Three datasets. Three challenges.

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>🩸 Diabetes Prediction</h3>
      <b>Source:</b> iammustafatz / Kaggle<br/><br/>
      <img src="https://img.shields.io/badge/100%2C000_rows-22C55E?style=flat-square"/>
      <img src="https://img.shields.io/badge/8_features-22C55E?style=flat-square"/>
      <img src="https://img.shields.io/badge/⚠_8.5%25_positive-EF4444?style=flat-square"/>
      <br/><br/>
      ★ <b>Winner: LightGBM</b><br/><br/>
      <sub>91.5% negative. SMOTE applied on training set only — test set stays untouched to reflect real-world distribution.</sub>
    </td>
    <td width="33%" valign="top">
      <h3>❤️ Heart Disease Cleveland</h3>
      <b>Source:</b> cherngs / UCI ML Repo<br/><br/>
      <img src="https://img.shields.io/badge/297_rows-22C55E?style=flat-square"/>
      <img src="https://img.shields.io/badge/13_features-22C55E?style=flat-square"/>
      <img src="https://img.shields.io/badge/✅_46.1%25_positive-22C55E?style=flat-square"/>
      <br/><br/>
      ★ <b>Winner: Logistic Regression</b><br/><br/>
      <sub>Only 237 training rows. Complex ensembles overfit — Logistic Regression wins, confirming simpler models generalize better on small data.</sub>
    </td>
    <td width="33%" valign="top">
      <h3>🧬 Pima Indians Diabetes</h3>
      <b>Source:</b> uciml / UCI ML Repo<br/><br/>
      <img src="https://img.shields.io/badge/768_rows-22C55E?style=flat-square"/>
      <img src="https://img.shields.io/badge/8_→_16_features-A855F7?style=flat-square"/>
      <img src="https://img.shields.io/badge/✅_34.9%25_positive-22C55E?style=flat-square"/>
      <br/><br/>
      ★ <b>Winner: XGBoost + FE</b><br/><br/>
      <sub>Glucose, BMI, and BloodPressure have biological zeros — replaced with column medians before any processing.</sub>
    </td>
  </tr>
</table>

---

## ⚠ Why Sensitivity Matters More Than Accuracy

> In medical classification, **a false negative costs more than a false positive**. Missing a diabetic patient is worse than over-referring a healthy one. This pipeline explicitly tracks and reports **Sensitivity** (true positive rate) alongside Specificity so the clinical tradeoff is always visible — not hidden inside a single accuracy number.

<table>
  <tr>
    <th align="center">True Positive</th>
    <th align="center">False Positive</th>
    <th align="center">False Negative</th>
    <th align="center">True Negative</th>
  </tr>
  <tr>
    <td align="center">✅ Correct flag<br/><sub>Patient gets care ✓</sub></td>
    <td align="center">⚠️ Over-referral<br/><sub>Minor cost</sub></td>
    <td align="center">❌ Missed case<br/><sub>High clinical cost ✗</sub></td>
    <td align="center">✅ Correct clear<br/><sub>All good ✓</sub></td>
  </tr>
</table>

---

## 🏗️ Architecture &nbsp;·&nbsp; From raw CSV to deployed Gradio app

```
┌─────────────────────────────────────────────────────────────────┐
│                  Raw CSV Files — 3 Datasets                     │
└────────────┬───────────────────┬────────────────────────────────┘
             │                   │                        │
             ▼                   ▼                        ▼
  ┌──────────────────┐ ┌──────────────────┐  ┌──────────────────────┐
  │ 🩸 Diabetes-Large│ │ ❤️ Heart-Cleveland│  │   🧬 Pima Indians    │
  │ 100k rows · 8 ft │ │ 297 rows · 13 ft │  │  768 rows · 8 ft     │
  │ Encode categorics│ │ Binarize target  │  │ Impute zeros→median  │
  └────────┬─────────┘ └────────┬─────────┘  └──────────┬───────────┘
           └─────────────────────┴────────────────────────┘
                                 │
              ┌──────────────────┼──────────────────┐
              ▼                  ▼                  ▼
        ┌──────────┐      ┌─────────────┐    ┌──────────┐
        │ 80/20    │ ───▶ │StandardScaler│──▶ │  SMOTE   │
        │  Split   │      │ fit on train │    │train only│
        │stratified│      └─────────────┘    └──────────┘
        └──────────┘
                                 │
              ┌──────────────────┼──────────────────┐
              ▼                  ▼                  ▼          ▼
    ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐
    │ Logistic Reg.│  │Random Forest │  │   XGBoost    │  │   LightGBM   │
    └──────┬───────┘  └──────┬───────┘  └──────┬───────┘  └──────┬───────┘
           └─────────────────┴──────────────────┴─────────────────┘
                                       │
                   ┌───────────────────┴──────────────────────┐
                   ▼                                          ▼
         ┌──────────────────┐                    ┌──────────────────────┐
         │     Evaluate     │ ◀────────────────▶ │    Optuna Tuning     │
         │ AUC·F1·Sens·Spec │                    │ 50–100 trials · TPE  │
         └──────────────────┘                    └──────────────────────┘
                                       │
                                       ▼
              ┌────────────────────────────────────────────┐
              │        🚀 Gradio App — Kaggle Deploy        │
              │  Public URL · No login required · 3-tab UI  │
              └────────────────────────────────────────────┘
```

---

## ⚙️ Feature Engineering &nbsp;·&nbsp; Raw features weren't enough — so we built better ones

> Applied exclusively to **Pima Indians** — the weakest performer — using clinical domain knowledge to construct **8 new features** from the original 8. After zero-imputation with column medians (374 impossible insulin values, 227 skin values replaced).

<table>
  <tr>
    <td width="50%" valign="top">
      <b>Original Features (8)</b><br/><br/>
      <code>Pregnancies</code> <code>Glucose</code> <code>BloodPressure</code> <code>SkinThickness</code> <code>Insulin</code> <code>BMI</code> <code>DiabetesPedigreeFunction</code> <code>Age</code>
    </td>
    <td width="50%" valign="top">
      <b>Interaction Features (4) ✨</b><br/><br/>
      <code>glucose_bmi</code> <code>bp_age</code> <code>age_pregnancies</code> <code>insulin_glucose</code><br/><br/>
      <sub>Glucose×BMI captures insulin resistance. BP×Age captures cardiovascular stress.</sub>
    </td>
  </tr>
  <tr>
    <td valign="top">
      <b>Ratio Features (2) ✨</b><br/><br/>
      <code>glucose_bmi_ratio</code> <code>skin_bmi_ratio</code><br/><br/>
      <sub>Thin patients with high glucose have a distinct risk profile invisible to either feature alone. Skin-to-BMI = adiposity proxy.</sub>
    </td>
    <td valign="top">
      <b>Clinical Bins (2) ✨ + AUC Progression</b><br/><br/>
      <code>bmi_bin</code> <code>glucose_bin</code><br/><br/>

| Model | AUC |
|---|---|
| Baseline XGBoost (8 features) | 0.823 |
| Tuned XGBoost (8 features) | 0.825 |
| **Tuned XGBoost (16 features)** | **0.838** |

<sub>✅ FE (+0.015) beat HPO alone (+0.002) — domain knowledge beats search.</sub>
    </td>
  </tr>
</table>

---

## 🏆 Results &nbsp;·&nbsp; Every model. Every metric.

### Dataset Winners

<table>
  <tr>
    <td align="center" width="33%">
      <h3>🩸 Diabetes-Large</h3>
      <b>LightGBM</b><br/><br/>
      <img src="https://img.shields.io/badge/AUC-0.979-00E5A0?style=flat-square"/>
      <img src="https://img.shields.io/badge/F1-0.804-0EA5E9?style=flat-square"/>
      <img src="https://img.shields.io/badge/Sens-0.709-F97316?style=flat-square"/>
      <img src="https://img.shields.io/badge/Spec-0.995-A855F7?style=flat-square"/>
    </td>
    <td align="center" width="33%">
      <h3>❤️ Heart-Cleveland</h3>
      <b>Logistic Regression</b><br/><br/>
      <img src="https://img.shields.io/badge/AUC-0.958-00E5A0?style=flat-square"/>
      <img src="https://img.shields.io/badge/F1-0.902-0EA5E9?style=flat-square"/>
      <img src="https://img.shields.io/badge/Sens-0.821-F97316?style=flat-square"/>
      <img src="https://img.shields.io/badge/Spec-1.000-A855F7?style=flat-square"/>
    </td>
    <td align="center" width="33%">
      <h3>🧬 Pima Indians</h3>
      <b>XGBoost + FE</b><br/><br/>
      <img src="https://img.shields.io/badge/AUC-0.838-00E5A0?style=flat-square"/>
      <img src="https://img.shields.io/badge/F1-0.649-0EA5E9?style=flat-square"/>
      <img src="https://img.shields.io/badge/Sens-0.685-F97316?style=flat-square"/>
      <img src="https://img.shields.io/badge/Spec-0.770-A855F7?style=flat-square"/>
    </td>
  </tr>
</table>

### 🩸 Diabetes-Large — 100k rows · 8 features · LightGBM with GPU T4

| Model | AUC | F1 | Sensitivity | Specificity | Train Time |
|---|---|---|---|---|---|
| Logistic Regression | 0.962 | 0.571 | 0.888 | 0.887 | 0.3s |
| Random Forest | 0.974 | 0.686 | 0.834 | 0.945 | 11.7s |
| XGBoost | 0.978 | 0.780 | 0.762 | 0.982 | 1.1s |
| ⭐ **LightGBM** | **0.979** | **0.804** | 0.709 | **0.995** | 2.0s |

### ❤️ Heart-Cleveland — 297 rows · 13 features · LR wins on small data

| Model | AUC | F1 | Sensitivity | Specificity | Train Time |
|---|---|---|---|---|---|
| ⭐ **Logistic Regression** | **0.958** | **0.902** | 0.821 | **1.000** | 0.0s |
| LightGBM | 0.949 | 0.852 | 0.821 | 0.906 | 0.1s |
| XGBoost | 0.934 | 0.846 | 0.786 | 0.938 | 0.1s |
| Random Forest | 0.941 | 0.800 | 0.714 | 0.938 | 0.6s |

### 🧬 Pima Indians — 768 rows · 8→16 features · Feature engineering applied

| Model | AUC | F1 | Sensitivity | Specificity | Train Time |
|---|---|---|---|---|---|
| ⭐ **XGBoost + FE** | **0.838** | **0.649** | 0.685 | 0.770 | 14.4s |
| LightGBM | 0.816 | 0.637 | 0.667 | 0.770 | 0.2s |
| XGBoost baseline | 0.823 | 0.649 | 0.685 | 0.770 | 0.2s |
| Logistic Regression | 0.811 | 0.621 | 0.667 | 0.740 | 0.0s |

> 💡 **Key insight:** Dataset size dictates model choice. On Heart-Cleveland (237 training rows), Logistic Regression beat every ensemble method. Pima's ceiling of 0.838 reflects genuine data limitations (1988 dataset, 768 samples) — not a pipeline failure. **Honest results are more valuable than inflated ones.**

---

## 🔬 Hyperparameter Tuning &nbsp;·&nbsp; Optuna TPE · 50–100 trials each

> Tree-structured Parzen Estimator — probabilistic search that learns from past trials to focus on promising regions of the hyperparameter space.

| Dataset | Model | Baseline AUC | Tuned AUC | Gain |
|---|---|---|---|---|
| 🩸 Diabetes-Large | LightGBM | 0.9781 | 0.9792 | **+0.0011** |
| ❤️ Heart-Cleveland | Logistic Regression | 0.9542 | 0.9576 | **+0.0034** |
| 🧬 Pima Indians | XGBoost + FE | 0.8230 | 0.8383 | **+0.0153** |

---

## 🚀 Live Demo &nbsp;·&nbsp; Three-tab Gradio app deployed on Kaggle. No login required.

<table>
  <tr>
    <td align="center" width="33%">
      <h3>🩸 Diabetes Risk</h3>
      <code>LightGBM · 8 inputs</code><br/><br/>
      🟢 &lt; 20% — Low Risk<br/>
      🟡 20–50% — Moderate Risk<br/>
      🔴 &gt; 50% — High Risk
    </td>
    <td align="center" width="33%">
      <h3>❤️ Heart Disease</h3>
      <code>Logistic Reg. · 13 inputs</code><br/><br/>
      🟢 &lt; 20% — Low Risk<br/>
      🟡 20–50% — Moderate Risk<br/>
      🔴 &gt; 50% — High Risk
    </td>
    <td align="center" width="33%">
      <h3>🧬 Pima Diabetes</h3>
      <code>XGBoost · 8 inputs</code><br/><br/>
      🟢 &lt; 20% — Low Risk<br/>
      🟡 20–50% — Moderate Risk<br/>
      🔴 &gt; 50% — High Risk
    </td>
  </tr>
</table>

> ⚠️ **For educational purposes only. Not a medical device. Consult a qualified healthcare professional.**

---

## ▶️ How to Run

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>A — Kaggle (Recommended)</h3>
      Open the notebook, fork it, click Run All. GPU T4 included free. The Gradio app launches in the last cell output with a public link.<br/><br/>
      <b>Required datasets (add via Kaggle UI):</b>
      
```
iammustafatz/diabetes-prediction-dataset
cherngs/heart-disease-cleveland-uci
uciml/pima-indians-diabetes-database
```
    </td>
    <td width="50%" valign="top">
      <h3>B — Local Setup</h3>
      Clone the repo, install dependencies, update dataset paths in Snippet 1, then run the notebook.<br/><br/>

```bash
pip install numpy pandas matplotlib \
  seaborn scikit-learn imbalanced-learn \
  xgboost lightgbm optuna gradio
```
    </td>
  </tr>
</table>

### Dependencies

| Package | Purpose |
|---|---|
| `scikit-learn` | Preprocessing, metrics, Stacking |
| `xgboost` | Gradient boosting with GPU (CUDA hist) |
| `lightgbm` | Histogram-based boosting, fast at scale |
| `imbalanced-learn` | SMOTE oversampling |
| `optuna` | Bayesian HPO via TPE sampler |
| `gradio` | Interactive web app + share link |
| `pandas / numpy` | Data manipulation |
| `matplotlib / seaborn` | All visualizations (13 plot files) |

---

## 📚 References

1. **Smith, J.W. et al. (1988).** Using the ADAP learning algorithm to forecast the onset of diabetes mellitus. *Proceedings of the Annual Symposium on Computer Application in Medical Care.* Pima Indians Diabetes Database — UCI ML Repository.

2. **Detrano, R. et al. (1989).** International application of a new probability algorithm for the diagnosis of coronary artery disease. *American Journal of Cardiology, 64(5), 304–310.* Heart Disease Cleveland UCI Dataset.

3. **Mustafa, T. (2023).** Diabetes Prediction Dataset — 100,000 patient records. *Kaggle.* kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset

4. **Chawla, N.V. et al. (2002).** SMOTE: Synthetic Minority Over-sampling Technique. *Journal of Artificial Intelligence Research, 16, 321–357.*

5. **Akiba, T. et al. (2019).** Optuna: A Next-generation Hyperparameter Optimization Framework. *Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining.*

---

<div align="center">

### 🏥 MedRisk Classifier

Built for open science · All datasets public · All tools free & open source · Kaggle GPU T4

[GitHub](#) &nbsp;·&nbsp; [Kaggle](#) &nbsp;·&nbsp; [Live Demo](#)

</div>
