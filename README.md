@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;600&display=swap'); \*{margin:0;padding:0;box-sizing:border-box;} :root{ --bg:#070d14;--bg2:#0d1520;--bg3:#111d2b;--surface:#162030;--surface2:#1a2840; --accent:#00e5a0;--accent2:#0ea5e9;--accent3:#f97316;--accent4:#a855f7; --red:#ef4444;--amber:#f59e0b;--green:#22c55e; --text:#e2eaf5;--muted:#6b8099;--border:rgba(0,229,160,0.12); --border2:rgba(14,165,233,0.15);--glow:0 0 20px rgba(0,229,160,0.15); } body{background:var(--bg);color:var(--text);font-family:'Space Grotesk',sans-serif;overflow-x:hidden;} .mono{font-family:'JetBrains Mono',monospace;} /\* HERO \*/ .hero{position:relative;padding:60px 40px 50px;text-align:center;overflow:hidden;} .hero-grid{position:absolute;inset:0;background-image:linear-gradient(rgba(0,229,160,0.04) 1px,transparent 1px),linear-gradient(90deg,rgba(0,229,160,0.04) 1px,transparent 1px);background-size:40px 40px;pointer-events:none;} .hero-glow{position:absolute;top:-60px;left:50%;transform:translateX(-50%);width:600px;height:300px;background:radial-gradient(ellipse,rgba(0,229,160,0.08) 0%,transparent 70%);pointer-events:none;} .badge-row{display:flex;flex-wrap:wrap;justify-content:center;gap:8px;margin-bottom:28px;} .badge{display:inline-flex;align-items:center;gap:6px;padding:4px 10px;border-radius:20px;font-size:11px;font-weight:600;letter-spacing:.5px;border:1px solid;font-family:'JetBrains Mono',monospace;} .b-blue{background:rgba(14,165,233,.1);border-color:rgba(14,165,233,.3);color:#38bdf8;} .b-green{background:rgba(34,197,94,.1);border-color:rgba(34,197,94,.3);color:#4ade80;} .b-orange{background:rgba(249,115,22,.1);border-color:rgba(249,115,22,.3);color:#fb923c;} .b-purple{background:rgba(168,85,247,.1);border-color:rgba(168,85,247,.3);color:#c084fc;} .b-red{background:rgba(239,68,68,.1);border-color:rgba(239,68,68,.3);color:#f87171;} .b-cyan{background:rgba(0,229,160,.1);border-color:rgba(0,229,160,.3);color:var(--accent);} .hero h1{font-size:52px;font-weight:700;line-height:1.05;margin-bottom:12px;background:linear-gradient(135deg,#fff 30%,var(--accent) 100%);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;} .hero-icon{font-size:48px;display:block;margin-bottom:8px;filter:drop-shadow(0 0 20px rgba(0,229,160,.4));} .tagline{font-size:16px;color:var(--muted);letter-spacing:.5px;font-weight:400;} .hero-stat-row{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:32px;max-width:620px;margin-left:auto;margin-right:auto;} .hero-stat{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:16px;position:relative;overflow:hidden;} .hero-stat::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,transparent,var(--accent),transparent);} .hs-num{font-size:28px;font-weight:700;color:var(--accent);font-family:'JetBrains Mono',monospace;} .hs-label{font-size:11px;color:var(--muted);margin-top:2px;letter-spacing:.3px;} /\* SECTIONS \*/ .section{padding:0 32px 40px;} .sec-header{display:flex;align-items:center;gap:10px;margin-bottom:24px;padding-top:40px;} .sec-icon{width:32px;height:32px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:16px;flex-shrink:0;} .si-green{background:rgba(0,229,160,.15);border:1px solid rgba(0,229,160,.3);} .si-blue{background:rgba(14,165,233,.15);border:1px solid rgba(14,165,233,.3);} .si-purple{background:rgba(168,85,247,.15);border:1px solid rgba(168,85,247,.3);} .si-orange{background:rgba(249,115,22,.15);border:1px solid rgba(249,115,22,.3);} .si-amber{background:rgba(245,158,11,.15);border:1px solid rgba(245,158,11,.3);} .sec-title{font-size:22px;font-weight:700;color:#fff;} .sec-sub{font-size:13px;color:var(--muted);margin-left:auto;font-style:italic;} /\* DATASETS \*/ .ds-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;} .ds-card{background:var(--surface);border:1px solid var(--border2);border-radius:14px;padding:20px;position:relative;overflow:hidden;cursor:pointer;transition:border-color .2s,transform .2s;} .ds-card:hover{border-color:var(--accent2);transform:translateY(-2px);} .ds-card::after{content:'';position:absolute;bottom:0;left:0;right:0;height:3px;border-radius:0 0 14px 14px;} .dsc-diabetes::after{background:linear-gradient(90deg,#ef4444,#f97316);} .dsc-heart::after{background:linear-gradient(90deg,#ec4899,#f43f5e);} .dsc-pima::after{background:linear-gradient(90deg,#8b5cf6,#6366f1);} .ds-emoji{font-size:28px;margin-bottom:10px;display:block;} .ds-name{font-size:15px;font-weight:700;margin-bottom:4px;color:#fff;} .ds-meta{font-size:12px;color:var(--muted);margin-bottom:12px;} .ds-pills{display:flex;flex-wrap:wrap;gap:5px;margin-bottom:14px;} .pill{font-size:10px;padding:2px 8px;border-radius:10px;font-weight:600;font-family:'JetBrains Mono',monospace;} .pill-red{background:rgba(239,68,68,.12);color:#f87171;border:1px solid rgba(239,68,68,.2);} .pill-green{background:rgba(34,197,94,.12);color:#4ade80;border:1px solid rgba(34,197,94,.2);} .pill-purple{background:rgba(168,85,247,.12);color:#c084fc;border:1px solid rgba(168,85,247,.2);} .ds-winner{font-size:11px;color:var(--accent);font-weight:600;display:flex;align-items:center;gap:4px;} .ds-winner::before{content:'★';color:var(--amber);} .ds-challenge{font-size:11px;color:var(--muted);margin-top:8px;line-height:1.5;padding:8px;background:rgba(255,255,255,.03);border-radius:6px;border-left:2px solid var(--accent2);} /\* PIPELINE / ARCHITECTURE \*/ .pipeline-wrap{background:var(--surface);border:1px solid var(--border);border-radius:16px;padding:28px;overflow:hidden;position:relative;} .pipeline-wrap::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse at 50% 0%,rgba(0,229,160,.04) 0%,transparent 60%);pointer-events:none;} .pipeline-svg{width:100%;overflow:visible;} /\* FEATURE ENGINEERING \*/ .fe-grid{display:grid;grid-template-columns:1fr 1fr;gap:14px;} .fe-card{background:var(--surface);border:1px solid var(--border2);border-radius:12px;padding:18px;} .fe-card-title{font-size:12px;font-weight:700;letter-spacing:.8px;color:var(--accent2);margin-bottom:12px;text-transform:uppercase;} .feat-tag{display:inline-block;font-size:11px;font-family:'JetBrains Mono',monospace;padding:3px 9px;border-radius:6px;margin:3px;background:rgba(14,165,233,.1);border:1px solid rgba(14,165,233,.2);color:#93c5fd;} .feat-tag-new{background:rgba(0,229,160,.1);border-color:rgba(0,229,160,.25);color:var(--accent);} .auc-bar-wrap{margin-top:6px;} .auc-row{display:flex;align-items:center;gap:10px;margin-bottom:8px;font-size:12px;} .auc-label{width:200px;color:var(--muted);flex-shrink:0;} .auc-bar-bg{flex:1;height:8px;background:rgba(255,255,255,.05);border-radius:4px;overflow:hidden;} .auc-bar-fill{height:100%;border-radius:4px;transition:width 1.2s ease;} .auc-val{width:40px;text-align:right;font-family:'JetBrains Mono',monospace;font-size:12px;color:var(--accent);} /\* RESULTS \*/ .results-tabs{display:flex;gap:8px;margin-bottom:16px;} .rtab{padding:7px 16px;border-radius:8px;font-size:13px;font-weight:600;cursor:pointer;border:1px solid var(--border);background:transparent;color:var(--muted);transition:all .2s;} .rtab.active{background:var(--accent);color:#000;border-color:var(--accent);} .results-table{width:100%;border-collapse:collapse;font-size:13px;} .results-table th{text-align:left;padding:10px 14px;font-size:11px;font-weight:700;letter-spacing:.8px;color:var(--muted);text-transform:uppercase;border-bottom:1px solid var(--border);} .results-table td{padding:10px 14px;border-bottom:1px solid rgba(255,255,255,.04);} .results-table tr:hover td{background:rgba(255,255,255,.02);} .results-table tr.winner td{background:rgba(0,229,160,.04);} .results-table tr.winner td:first-child{border-left:2px solid var(--accent);padding-left:12px;} .star-row{display:flex;align-items:center;gap:6px;} .star{color:var(--amber);font-size:12px;} .metric-pill{display:inline-block;padding:2px 8px;border-radius:12px;font-size:11px;font-family:'JetBrains Mono',monospace;font-weight:600;} .mp-auc{background:rgba(0,229,160,.15);color:var(--accent);} .mp-f1{background:rgba(14,165,233,.15);color:#38bdf8;} .mp-sens{background:rgba(249,115,22,.15);color:#fb923c;} .mp-spec{background:rgba(168,85,247,.15);color:#c084fc;} .train-time{color:var(--muted);font-size:11px;font-family:'JetBrains Mono',monospace;} .rtable-wrap{background:var(--surface);border:1px solid var(--border);border-radius:14px;overflow:hidden;} /\* TUNING \*/ .tuning-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;} .tune-card{background:var(--surface);border:1px solid var(--border2);border-radius:12px;padding:18px;position:relative;} .tune-model{font-size:11px;color:var(--muted);margin-bottom:4px;font-family:'JetBrains Mono',monospace;} .tune-ds{font-size:15px;font-weight:700;margin-bottom:14px;color:#fff;} .tune-bars{display:flex;align-items:flex-end;gap:10px;height:60px;margin-bottom:10px;} .tune-bar-wrap{flex:1;display:flex;flex-direction:column;align-items:center;gap:4px;} .tune-bar{width:100%;border-radius:4px 4px 0 0;transition:height 1s ease;} .tune-bar-base{background:rgba(255,255,255,.15);} .tune-bar-tuned{background:var(--accent);} .tune-bar-label{font-size:10px;color:var(--muted);font-family:'JetBrains Mono',monospace;} .tune-gain{font-size:13px;color:var(--accent);font-weight:700;} .tune-gain-label{font-size:11px;color:var(--muted);} /\* GRADIO APP \*/ .app-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;} .app-tab{background:var(--surface);border:1px solid var(--border2);border-radius:12px;padding:20px;text-align:center;position:relative;overflow:hidden;cursor:pointer;transition:all .2s;} .app-tab:hover{border-color:var(--accent);transform:translateY(-2px);} .app-tab-icon{font-size:32px;margin-bottom:10px;display:block;} .app-tab-title{font-size:14px;font-weight:700;margin-bottom:4px;color:#fff;} .app-tab-model{font-size:11px;color:var(--muted);font-family:'JetBrains Mono',monospace;margin-bottom:12px;} .risk-row{display:flex;flex-direction:column;gap:5px;} .risk-item{display:flex;align-items:center;gap:8px;font-size:11px;color:var(--muted);} .risk-dot{width:10px;height:10px;border-radius:50%;flex-shrink:0;} .rd-green{background:var(--green);} .rd-amber{background:var(--amber);} .rd-red{background:var(--red);} .risk-val{font-family:'JetBrains Mono',monospace;font-size:10px;} /\* DEPS TABLE \*/ .deps-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:10px;} .dep-row{display:flex;align-items:center;gap:12px;background:var(--surface);border:1px solid var(--border);border-radius:10px;padding:12px 14px;} .dep-name{font-family:'JetBrains Mono',monospace;font-size:12px;font-weight:600;color:var(--accent2);width:130px;flex-shrink:0;} .dep-desc{font-size:12px;color:var(--muted);} /\* REFS \*/ .refs-list{display:flex;flex-direction:column;gap:10px;} .ref-item{display:flex;gap:12px;background:var(--surface);border:1px solid var(--border);border-radius:10px;padding:14px;} .ref-num{font-family:'JetBrains Mono',monospace;font-size:12px;font-weight:700;color:var(--accent);width:20px;flex-shrink:0;padding-top:1px;} .ref-text{font-size:12px;color:var(--muted);line-height:1.6;} .ref-text strong{color:var(--text);} /\* FOOTER \*/ .footer{text-align:center;padding:32px;border-top:1px solid var(--border);margin-top:20px;} .footer-title{font-size:18px;font-weight:700;color:var(--accent);margin-bottom:6px;} .footer-links{display:flex;justify-content:center;gap:20px;margin-top:12px;} .footer-link{font-size:13px;color:var(--accent2);text-decoration:none;} .footer-sub{font-size:12px;color:var(--muted);margin-top:8px;} /\* CALLOUT \*/ .callout{background:rgba(0,229,160,.05);border:1px solid rgba(0,229,160,.2);border-radius:10px;padding:14px 18px;margin-bottom:20px;font-size:13px;color:var(--text);line-height:1.6;} .callout strong{color:var(--accent);} .callout-blue{background:rgba(14,165,233,.05);border-color:rgba(14,165,233,.2);} .callout-blue strong{color:#38bdf8;} /\* ANIMATIONS \*/ @keyframes fadeUp{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:translateY(0)}} @keyframes pulse-glow{0%,100%{box-shadow:0 0 0 0 rgba(0,229,160,0)}50%{box-shadow:0 0 20px 4px rgba(0,229,160,0.2)}} @keyframes flow{from{stroke-dashoffset:60}to{stroke-dashoffset:0}} @keyframes node-in{from{opacity:0;transform:scale(.85)}to{opacity:1;transform:scale(1)}} .hero-stat{animation:fadeUp .5s ease both;} .hero-stat:nth-child(1){animation-delay:.1s} .hero-stat:nth-child(2){animation-delay:.2s} .hero-stat:nth-child(3){animation-delay:.3s} .ds-card{animation:fadeUp .5s ease both;} .ds-card:nth-child(1){animation-delay:.05s} .ds-card:nth-child(2){animation-delay:.15s} .ds-card:nth-child(3){animation-delay:.25s} .hero-stat.pulse{animation:pulse-glow 2s ease-in-out infinite;} .pipe-flow{stroke-dasharray:8 4;animation:flow 1.2s linear infinite;} .pipe-flow-slow{stroke-dasharray:8 4;animation:flow 2s linear infinite;} .pipe-node{animation:node-in .4s ease both;} /\* WHY SENSITIVITY \*/ .sens-card{background:linear-gradient(135deg,rgba(249,115,22,.08),rgba(239,68,68,.08));border:1px solid rgba(249,115,22,.25);border-radius:12px;padding:20px;margin-bottom:24px;} .sens-title{font-size:15px;font-weight:700;color:#fb923c;margin-bottom:8px;display:flex;align-items:center;gap:8px;} .sens-body{font-size:13px;color:var(--text);line-height:1.7;} .confusion-mini{display:flex;gap:10px;margin-top:14px;flex-wrap:wrap;} .cf-item{flex:1;min-width:120px;background:rgba(0,0,0,.2);border-radius:8px;padding:10px;text-align:center;} .cf-label{font-size:10px;color:var(--muted);margin-bottom:4px;text-transform:uppercase;letter-spacing:.5px;} .cf-outcome{font-size:14px;font-weight:700;} .cf-good{color:var(--green);} .cf-bad{color:var(--red);} .cf-cost{font-size:10px;margin-top:3px;color:var(--muted);}

Python 3.12 XGBoost LightGBM Optuna HPO SMOTE Gradio App Kaggle GPU T4

🏥

MedRisk Classifier
==================

One pipeline  ·  Three datasets  ·  Zero cost  ·  Fully open source

0.979

🏆 Best AUC — LightGBM · Diabetes-Large

101k

🏥 Total patient records across all datasets

12

🤖 Models trained (4 classifiers × 3 datasets)

📊

Datasets Three datasets. Three challenges.

🩸

Diabetes Prediction

Source: iammustafatz / Kaggle

100,000 rows 8 features ⚠ 8.5% positive

Winner: LightGBM

91.5% negative. SMOTE applied on training set only — test set stays untouched to reflect real-world distribution.

❤️

Heart Disease Cleveland

Source: cherngs / UCI ML Repo

297 rows 13 features ✅ 46.1% positive

Winner: Logistic Regression

Only 237 training rows. Complex ensembles overfit — Logistic Regression wins, confirming simpler models generalize better on small data.

🧬

Pima Indians Diabetes

Source: uciml / UCI ML Repo

768 rows 8 → 16 features ✅ 34.9% positive

Winner: XGBoost + FE

Glucose, BMI, and BloodPressure have biological zeros — replaced with column medians before any processing.

⚠ Why Sensitivity Matters More Than Accuracy

In medical classification, **a false negative costs more than a false positive**. Missing a diabetic patient is worse than over-referring a healthy one. This pipeline explicitly tracks and reports **Sensitivity** (true positive rate) alongside Specificity so the clinical tradeoff is always visible — not hidden inside a single accuracy number.

True Positive

Correct flag

Patient gets care ✓

False Positive

Over-referral

Minor cost

False Negative

Missed case

High clinical cost ✗

True Negative

Correct clear

All good ✓

🏗️

Architecture From raw CSV to deployed Gradio app

Raw CSV Files — 3 Datasets 🩸 Diabetes-Large 100k rows · 8 features ❤️ Heart-Cleveland 297 rows · 13 features 🧬 Pima Indians 768 rows · 8 features Encode categoricals Binarize target Impute zeros → median 80/20 Split stratified StandardScaler fit on train only SMOTE train only Logistic Reg. Random Forest XGBoost LightGBM Evaluate AUC · F1 · Sens · Spec Optuna Tuning 50–100 trials/model · TPE 🚀 Gradio App — Kaggle Deploy Public URL · No login required · 3-tab interface

⚙️

Feature Engineering Raw features weren't enough — so we built better ones

Applied exclusively to **Pima Indians** — the weakest performer — using clinical domain knowledge to construct **8 new features** from the original 8. After zero-imputation with column medians (374 impossible insulin values, 227 skin values replaced).

Original Features (8)

PregnanciesGlucoseBloodPressureSkinThicknessInsulinBMIDiabetesPedigreeFunctionAge

Interaction Features (4)

glucose\_bmibp\_ageage\_pregnanciesinsulin\_glucose

Glucose×BMI captures insulin resistance. BP×Age captures cardiovascular stress.

Ratio Features (2)

glucose\_bmi\_ratioskin\_bmi\_ratio

Thin patients with high glucose have a distinct risk profile invisible to either feature alone. Skin-to-BMI = adiposity proxy.

Clinical Bins (2) + AUC Progression

bmi\_binglucose\_bin

Baseline XGBoost (8 features)

0.823

Tuned XGBoost (8 features)

0.825

Tuned XGBoost (16 features)

0.838

FE (+0.015) beat HPO alone (+0.002) — domain knowledge beats search.

🏆

Results Every model. Every metric.

🩸

Diabetes-Large

LightGBM

AUC 0.979 F1 0.804 Sens 0.709 Spec 0.995

❤️

Heart-Cleveland

Logistic Regression

AUC 0.958 F1 0.902 Sens 0.821 Spec 1.000

🧬

Pima Indians

XGBoost + FE

AUC 0.838 F1 0.649 Sens 0.685 Spec 0.770

🩸 Diabetes-Large ❤️ Heart-Cleveland 🧬 Pima Indians

100k rows · 8 features · LightGBM with GPU T4

Model

AUC

F1

Sensitivity

Specificity

Train Time

Logistic Regression

0.962

0.571

0.888

0.887

0.3s

Random Forest

0.974

0.686

0.834

0.945

11.7s

XGBoost

0.978

0.780

0.762

0.982

1.1s

★ **LightGBM**

0.979

0.804

0.709

0.995

2.0s

297 rows · 13 features · LR wins on small data

Model

AUC

F1

Sensitivity

Specificity

Train Time

★ **Logistic Regression**

0.958

0.902

0.821

1.000

0.0s

LightGBM

0.949

0.852

0.821

0.906

0.1s

XGBoost

0.934

0.846

0.786

0.938

0.1s

Random Forest

0.941

0.800

0.714

0.938

0.6s

768 rows · 8→16 features · Feature engineering applied

Model

AUC

F1

Sensitivity

Specificity

Train Time

★ **XGBoost + FE**

0.838

0.649

0.685

0.770

14.4s

LightGBM

0.816

0.637

0.667

0.770

0.2s

XGBoost baseline

0.823

0.649

0.685

0.770

0.2s

Logistic Regression

0.811

0.621

0.667

0.740

0.0s

**Key insight:** Dataset size dictates model choice. On Heart-Cleveland (237 training rows), Logistic Regression beat every ensemble method. Pima's ceiling of 0.838 reflects genuine data limitations (1988 dataset, 768 samples) — not a pipeline failure. **Honest results are more valuable than inflated ones.**

🔬

Hyperparameter Tuning Optuna TPE · 50–100 trials each

Tree-structured Parzen Estimator — probabilistic search that learns from past trials to focus on promising regions of the hyperparameter space.

LightGBM

🩸 Diabetes-Large

Baseline

0.9781

Tuned

0.9792

+0.0011 AUC

gain from tuning

Logistic Regression

❤️ Heart-Cleveland

Baseline

0.9542

Tuned

0.9576

+0.0034 AUC

gain from tuning

XGBoost + FE

🧬 Pima Indians

Baseline

0.8230

Tuned

0.8383

+0.0153 AUC

gain from tuning

🚀

Live Demo Three-tab Gradio app deployed on Kaggle. No login required.

🩸

Diabetes Risk

LightGBM · 8 inputs

< 20% Low Risk

20–50% Moderate Risk

\> 50% High Risk

❤️

Heart Disease

Logistic Reg. · 13 inputs

< 20% Low Risk

20–50% Moderate Risk

\> 50% High Risk

🧬

Pima Diabetes

XGBoost · 8 inputs

< 20% Low Risk

20–50% Moderate Risk

\> 50% High Risk

⚠ For educational purposes only. Not a medical device. Consult a qualified healthcare professional.

▶️

How to Run

A — Kaggle (Recommended)

Open the notebook, fork it, click Run All. GPU T4 included free. The Gradio app launches in the last cell output with a public link.

Required datasets (add via Kaggle UI):

iammustafatz/diabetes-prediction-dataset  
cherngs/heart-disease-cleveland-uci  
uciml/pima-indians-diabetes-database

B — Local Setup

Clone the repo, install dependencies, update dataset paths in Snippet 1, then run the notebook.

pip install numpy pandas matplotlib  
seaborn scikit-learn imbalanced-learn  
xgboost lightgbm optuna gradio

scikit-learnPreprocessing, metrics, Stacking

xgboostGradient boosting with GPU (CUDA hist)

lightgbmHistogram-based boosting, fast at scale

imbalanced-learnSMOTE oversampling

optunaBayesian HPO via TPE sampler

gradioInteractive web app + share link

pandas / numpyData manipulation

matplotlib / seabornAll visualizations (13 plot files)

📚

References

1**Smith, J.W. et al. (1988).** Using the ADAP learning algorithm to forecast the onset of diabetes mellitus. _Proceedings of the Annual Symposium on Computer Application in Medical Care._ Pima Indians Diabetes Database — UCI ML Repository.

2**Detrano, R. et al. (1989).** International application of a new probability algorithm for the diagnosis of coronary artery disease. _American Journal of Cardiology, 64(5), 304–310._ Heart Disease Cleveland UCI Dataset.

3**Mustafa, T. (2023).** Diabetes Prediction Dataset — 100,000 patient records. _Kaggle._ kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset

4**Chawla, N.V. et al. (2002).** SMOTE: Synthetic Minority Over-sampling Technique. _Journal of Artificial Intelligence Research, 16, 321–357._

5**Akiba, T. et al. (2019).** Optuna: A Next-generation Hyperparameter Optimization Framework. _Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining._

🏥 MedRisk Classifier

Built for open science · All datasets public · All tools free & open source · Kaggle GPU T4

[GitHub](#) [Kaggle](#) [Live Demo](#)

function showTab(name) { \['diabetes','heart','pima'\].forEach(t => { document.getElementById('tab-'+t).style.display = t===name?'block':'none'; }); document.querySelectorAll('.rtab').forEach((btn,i) => { btn.classList.toggle('active', \['diabetes','heart','pima'\]\[i\]===name); }); }
