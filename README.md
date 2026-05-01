<div align="center">

<!-- ANIMATED HEADER BANNER -->
<img src="https://capsule-render.vercel.app/api?type=venom&height=280&color=gradient&customColorList=0,2,2,5,30&text=MedRisk%20Classifier&fontSize=54&fontColor=ffffff&fontAlignY=55&desc=Generalizable%20ML%20Pipeline%20for%20Chronic%20Disease%20Prediction&descSize=16&descAlignY=75&animation=fadeIn&stroke=ffffff&strokeWidth=1" width="100%" alt="MedRisk Classifier"/>

<br/>

<!-- BADGES ROW 1 -->
<a href="#"><img src="https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white"/></a>
<a href="#"><img src="https://img.shields.io/badge/Kaggle-GPU%20Accelerated-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white"/></a>
<a href="#"><img src="https://img.shields.io/badge/Gradio-Live%20Demo-FF7C00?style=for-the-badge&logo=gradio&logoColor=white"/></a>
<a href="#"><img src="https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge"/></a>

<br/><br/>

<!-- BADGES ROW 2 -->
<img src="https://img.shields.io/badge/XGBoost-✓-EC4899?style=flat-square"/>
<img src="https://img.shields.io/badge/LightGBM-✓-A855F7?style=flat-square"/>
<img src="https://img.shields.io/badge/Optuna-Tuned-06B6D4?style=flat-square"/>
<img src="https://img.shields.io/badge/SMOTE-Balanced-F59E0B?style=flat-square"/>
<img src="https://img.shields.io/badge/Sklearn-Stacking-10B981?style=flat-square&logo=scikit-learn&logoColor=white"/>
<img src="https://img.shields.io/badge/Feature%20Engineering-16%20Features-EF4444?style=flat-square"/>

<br/><br/>

<!-- TYPING ANIMATION -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&duration=3000&pause=800&color=1D9E75&center=true&vCenter=true&multiline=true&width=700&height=80&lines=Three+datasets.+Four+models.+One+unified+pipeline.;Diabetes+%E2%80%A2+Heart+Disease+%E2%80%A2+Pima+Indians;AUC+up+to+0.979+%E2%80%94+deployed+live+on+Gradio." alt="Typing SVG"/>
</a>

</div>

---

<!-- LIVE DEMO BANNER -->
<div align="center">

### 🚀 Try the Live Demo

<a href="#">
  <img src="https://img.shields.io/badge/%F0%9F%8E%AF%20%20LIVE%20DEMO%20%E2%80%94%20Click%20to%20Predict%20Your%20Risk-FF7C00?style=for-the-badge&logoColor=white" height="45"/>
</a>

*Enter your clinical values → get instant ML-powered risk assessment across 3 disease models*

</div>

---

## 📖 Table of Contents

<div align="center">

| | Section | | Section |
|:---:|:---|:---:|:---|
| 🎯 | [Project Overview](#-project-overview) | 📊 | [Dataset Summary](#-dataset-summary) |
| 🏗️ | [Pipeline Architecture](#️-pipeline-architecture) | ⚙️ | [Feature Engineering](#️-feature-engineering-pima) |
| 🤖 | [Models & Results](#-models--results) | 🔬 | [Hyperparameter Tuning](#-hyperparameter-tuning) |
| 📈 | [Performance Visuals](#-performance-visuals) | 🖥️ | [App Interface](#️-app-interface) |
| 🚀 | [Quick Start](#-quick-start) | 🗂️ | [Project Structure](#️-project-structure) |

</div>

---

## 🎯 Project Overview

<div align="center">

> **MedRisk Classifier** is a production-grade, generalizable machine learning pipeline designed to predict chronic disease risk across multiple independent clinical datasets — with a single unified codebase.

</div>

Instead of building one model for one dataset, this project demonstrates that a **well-engineered ML pipeline generalizes across disease domains**. The same preprocessing, balancing, training, and evaluation framework is applied identically to three structurally different datasets, proving the pipeline's robustness.

**Key design decisions:**

- 🧬 **SMOTE oversampling** applied only to training folds — zero leakage into test sets
- ⚖️ **`class_weight="balanced"`** on all models as a secondary defense against imbalance
- 🔬 **Optuna TPE search** with 50–100 trials per model for principled hyperparameter tuning
- 🧪 **Feature engineering** on the hardest dataset (Pima) — 8 → 16 clinically motivated features
- 🏆 **Stacking ensemble** combining LightGBM + XGBoost + Random Forest via Logistic Regression meta-learner

---

## 📊 Dataset Summary

<div align="center">

<svg viewBox="0 0 860 220" xmlns="http://www.w3.org/2000/svg" width="860" height="220">
  <defs>
    <linearGradient id="g1" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#1D9E75;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#0F6E56;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="g2" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#D85A30;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#993C1D;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="g3" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#7F77DD;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#534AB7;stop-opacity:1"/>
    </linearGradient>
    <filter id="shadow"><feDropShadow dx="0" dy="4" stdDeviation="6" flood-opacity="0.18"/></filter>
  </defs>
  <rect x="10" y="10" width="260" height="200" rx="16" fill="url(#g1)" filter="url(#shadow)"/>
  <text x="135" y="48" text-anchor="middle" fill="white" font-size="22" font-weight="bold" font-family="sans-serif">🩸 Diabetes</text>
  <text x="135" y="70" text-anchor="middle" fill="rgba(255,255,255,0.8)" font-size="11" font-family="sans-serif">iammustafatz · Kaggle</text>
  <rect x="30" y="85" width="220" height="1" fill="rgba(255,255,255,0.3)"/>
  <text x="30" y="110" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">📦 100,000 rows</text>
  <text x="30" y="130" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">🔢 8 features</text>
  <text x="30" y="150" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">⚠️ 8.5% positive</text>
  <text x="30" y="170" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">🤖 LightGBM</text>
  <rect x="30" y="182" width="200" height="18" rx="9" fill="rgba(255,255,255,0.25)"/>
  <text x="130" y="195" text-anchor="middle" fill="white" font-size="11" font-family="sans-serif" font-weight="bold">AUC 0.979 ⭐</text>
  <rect x="300" y="10" width="260" height="200" rx="16" fill="url(#g2)" filter="url(#shadow)"/>
  <text x="430" y="48" text-anchor="middle" fill="white" font-size="22" font-weight="bold" font-family="sans-serif">❤️ Heart Disease</text>
  <text x="430" y="70" text-anchor="middle" fill="rgba(255,255,255,0.8)" font-size="11" font-family="sans-serif">Cleveland UCI · Kaggle</text>
  <rect x="320" y="85" width="220" height="1" fill="rgba(255,255,255,0.3)"/>
  <text x="320" y="110" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">📦 297 rows</text>
  <text x="320" y="130" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">🔢 13 features</text>
  <text x="320" y="150" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">⚠️ 46.1% positive</text>
  <text x="320" y="170" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">🤖 Logistic Regression</text>
  <rect x="320" y="182" width="200" height="18" rx="9" fill="rgba(255,255,255,0.25)"/>
  <text x="420" y="195" text-anchor="middle" fill="white" font-size="11" font-family="sans-serif" font-weight="bold">AUC 0.958 ⭐</text>
  <rect x="590" y="10" width="260" height="200" rx="16" fill="url(#g3)" filter="url(#shadow)"/>
  <text x="720" y="48" text-anchor="middle" fill="white" font-size="22" font-weight="bold" font-family="sans-serif">🧬 Pima Diabetes</text>
  <text x="720" y="70" text-anchor="middle" fill="rgba(255,255,255,0.8)" font-size="11" font-family="sans-serif">UCI ML Repository · Kaggle</text>
  <rect x="610" y="85" width="220" height="1" fill="rgba(255,255,255,0.3)"/>
  <text x="610" y="110" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">📦 768 rows</text>
  <text x="610" y="130" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">🔢 8 → 16 features (eng.)</text>
  <text x="610" y="150" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">⚠️ 34.9% positive</text>
  <text x="610" y="170" fill="white" font-size="12" font-family="sans-serif" font-weight="bold">🤖 XGBoost + Stack</text>
  <rect x="610" y="182" width="200" height="18" rx="9" fill="rgba(255,255,255,0.25)"/>
  <text x="710" y="195" text-anchor="middle" fill="white" font-size="11" font-family="sans-serif" font-weight="bold">AUC 0.838 ⭐</text>
</svg>

</div>

---

## 🏗️ Pipeline Architecture

<div align="center">

<svg viewBox="0 0 860 540" xmlns="http://www.w3.org/2000/svg" width="860" height="540">
  <defs>
    <linearGradient id="hdr" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#0F6E56"/><stop offset="100%" style="stop-color:#1D9E75"/>
    </linearGradient>
    <linearGradient id="ingest" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#E1F5EE"/><stop offset="100%" style="stop-color:#9FE1CB"/>
    </linearGradient>
    <linearGradient id="prep" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#FFF3E0"/><stop offset="100%" style="stop-color:#FAC775"/>
    </linearGradient>
    <linearGradient id="train" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#EDE9FE"/><stop offset="100%" style="stop-color:#AFA9EC"/>
    </linearGradient>
    <linearGradient id="eval" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#FAECE7"/><stop offset="100%" style="stop-color:#F0997B"/>
    </linearGradient>
    <linearGradient id="deploy" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#E6F1FB"/><stop offset="100%" style="stop-color:#85B7EB"/>
    </linearGradient>
    <marker id="arr" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#888"/>
    </marker>
    <filter id="sh2"><feDropShadow dx="0" dy="3" stdDeviation="4" flood-opacity="0.12"/></filter>
  </defs>
  <rect x="0" y="0" width="860" height="44" fill="url(#hdr)"/>
  <text x="430" y="28" text-anchor="middle" fill="white" font-size="16" font-weight="bold" font-family="sans-serif">MedRisk Classifier — End-to-End ML Pipeline</text>
  <text x="14" y="110" fill="#0F6E56" font-size="10" font-weight="bold" font-family="sans-serif">INGEST</text>
  <text x="14" y="210" fill="#BA7517" font-size="10" font-weight="bold" font-family="sans-serif">PREPROCESS</text>
  <text x="14" y="320" fill="#534AB7" font-size="10" font-weight="bold" font-family="sans-serif">TRAIN</text>
  <text x="14" y="420" fill="#993C1D" font-size="10" font-weight="bold" font-family="sans-serif">EVALUATE</text>
  <text x="14" y="510" fill="#185FA5" font-size="10" font-weight="bold" font-family="sans-serif">DEPLOY</text>
  <line x1="80" y1="140" x2="845" y2="140" stroke="#e5e7eb" stroke-width="1" stroke-dasharray="4"/>
  <line x1="80" y1="250" x2="845" y2="250" stroke="#e5e7eb" stroke-width="1" stroke-dasharray="4"/>
  <line x1="80" y1="360" x2="845" y2="360" stroke="#e5e7eb" stroke-width="1" stroke-dasharray="4"/>
  <line x1="80" y1="455" x2="845" y2="455" stroke="#e5e7eb" stroke-width="1" stroke-dasharray="4"/>
  <rect x="90" y="60" width="170" height="64" rx="10" fill="url(#ingest)" filter="url(#sh2)" stroke="#1D9E75" stroke-width="1.5"/>
  <text x="175" y="84" text-anchor="middle" fill="#0F6E56" font-size="13" font-weight="bold" font-family="sans-serif">🩸 Diabetes-Large</text>
  <text x="175" y="102" text-anchor="middle" fill="#0F6E56" font-size="10" font-family="sans-serif">100k rows · 8 features</text>
  <text x="175" y="116" text-anchor="middle" fill="#0F6E56" font-size="10" font-family="sans-serif">8.5% positive class</text>
  <rect x="340" y="60" width="170" height="64" rx="10" fill="url(#ingest)" filter="url(#sh2)" stroke="#1D9E75" stroke-width="1.5"/>
  <text x="425" y="84" text-anchor="middle" fill="#0F6E56" font-size="13" font-weight="bold" font-family="sans-serif">❤️ Heart-Cleveland</text>
  <text x="425" y="102" text-anchor="middle" fill="#0F6E56" font-size="10" font-family="sans-serif">297 rows · 13 features</text>
  <text x="425" y="116" text-anchor="middle" fill="#0F6E56" font-size="10" font-family="sans-serif">46.1% positive class</text>
  <rect x="590" y="60" width="170" height="64" rx="10" fill="url(#ingest)" filter="url(#sh2)" stroke="#1D9E75" stroke-width="1.5"/>
  <text x="675" y="84" text-anchor="middle" fill="#0F6E56" font-size="13" font-weight="bold" font-family="sans-serif">🧬 Diabetes-Pima</text>
  <text x="675" y="102" text-anchor="middle" fill="#0F6E56" font-size="10" font-family="sans-serif">768 rows · 8 features</text>
  <text x="675" y="116" text-anchor="middle" fill="#0F6E56" font-size="10" font-family="sans-serif">34.9% positive class</text>
  <line x1="175" y1="124" x2="175" y2="158" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <line x1="425" y1="124" x2="425" y2="158" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <line x1="675" y1="124" x2="675" y2="158" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <rect x="90" y="158" width="170" height="76" rx="10" fill="url(#prep)" filter="url(#sh2)" stroke="#BA7517" stroke-width="1.5"/>
  <text x="175" y="180" text-anchor="middle" fill="#633806" font-size="11" font-weight="bold" font-family="sans-serif">🏷️ Label Encoding</text>
  <text x="175" y="196" text-anchor="middle" fill="#633806" font-size="10" font-family="sans-serif">gender · smoking_history</text>
  <text x="175" y="212" text-anchor="middle" fill="#633806" font-size="11" font-weight="bold" font-family="sans-serif">⚖️ SMOTE</text>
  <text x="175" y="226" text-anchor="middle" fill="#633806" font-size="10" font-family="sans-serif">80k → 146k balanced</text>
  <rect x="340" y="158" width="170" height="76" rx="10" fill="url(#prep)" filter="url(#sh2)" stroke="#BA7517" stroke-width="1.5"/>
  <text x="425" y="180" text-anchor="middle" fill="#633806" font-size="11" font-weight="bold" font-family="sans-serif">📐 StandardScaler</text>
  <text x="425" y="196" text-anchor="middle" fill="#633806" font-size="10" font-family="sans-serif">fit on train only</text>
  <text x="425" y="212" text-anchor="middle" fill="#633806" font-size="11" font-weight="bold" font-family="sans-serif">⚖️ SMOTE</text>
  <text x="425" y="226" text-anchor="middle" fill="#633806" font-size="10" font-family="sans-serif">237 → 256 balanced</text>
  <rect x="590" y="158" width="170" height="76" rx="10" fill="url(#prep)" filter="url(#sh2)" stroke="#BA7517" stroke-width="1.5"/>
  <text x="675" y="180" text-anchor="middle" fill="#633806" font-size="11" font-weight="bold" font-family="sans-serif">🩹 Zero Imputation</text>
  <text x="675" y="196" text-anchor="middle" fill="#633806" font-size="10" font-family="sans-serif">median fill · 5 cols</text>
  <text x="675" y="212" text-anchor="middle" fill="#633806" font-size="11" font-weight="bold" font-family="sans-serif">🧪 Feature Eng.</text>
  <text x="675" y="226" text-anchor="middle" fill="#633806" font-size="10" font-family="sans-serif">8 → 16 features</text>
  <line x1="175" y1="234" x2="175" y2="268" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <line x1="425" y1="234" x2="425" y2="268" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <line x1="675" y1="234" x2="675" y2="268" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <rect x="90" y="268" width="170" height="76" rx="10" fill="url(#train)" filter="url(#sh2)" stroke="#7F77DD" stroke-width="1.5"/>
  <text x="175" y="290" text-anchor="middle" fill="#26215C" font-size="11" font-weight="bold" font-family="sans-serif">4 Models Trained</text>
  <text x="175" y="306" text-anchor="middle" fill="#26215C" font-size="10" font-family="sans-serif">LR · RF · XGB · LGBM</text>
  <text x="175" y="322" text-anchor="middle" fill="#26215C" font-size="11" font-weight="bold" font-family="sans-serif">🏆 Best: LightGBM</text>
  <text x="175" y="336" text-anchor="middle" fill="#26215C" font-size="10" font-family="sans-serif">50 Optuna trials</text>
  <rect x="340" y="268" width="170" height="76" rx="10" fill="url(#train)" filter="url(#sh2)" stroke="#7F77DD" stroke-width="1.5"/>
  <text x="425" y="290" text-anchor="middle" fill="#26215C" font-size="11" font-weight="bold" font-family="sans-serif">4 Models Trained</text>
  <text x="425" y="306" text-anchor="middle" fill="#26215C" font-size="10" font-family="sans-serif">LR · RF · XGB · LGBM</text>
  <text x="425" y="322" text-anchor="middle" fill="#26215C" font-size="11" font-weight="bold" font-family="sans-serif">🏆 Best: Log. Reg.</text>
  <text x="425" y="336" text-anchor="middle" fill="#26215C" font-size="10" font-family="sans-serif">50 Optuna trials</text>
  <rect x="590" y="268" width="170" height="76" rx="10" fill="url(#train)" filter="url(#sh2)" stroke="#7F77DD" stroke-width="1.5"/>
  <text x="675" y="290" text-anchor="middle" fill="#26215C" font-size="11" font-weight="bold" font-family="sans-serif">4 Models + Stack</text>
  <text x="675" y="306" text-anchor="middle" fill="#26215C" font-size="10" font-family="sans-serif">LR · RF · XGB · LGBM</text>
  <text x="675" y="322" text-anchor="middle" fill="#26215C" font-size="11" font-weight="bold" font-family="sans-serif">🏆 Best: XGBoost</text>
  <text x="675" y="336" text-anchor="middle" fill="#26215C" font-size="10" font-family="sans-serif">100 Optuna trials</text>
  <line x1="175" y1="344" x2="175" y2="370" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <line x1="425" y1="344" x2="425" y2="370" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <line x1="675" y1="344" x2="675" y2="370" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <rect x="90" y="370" width="170" height="72" rx="10" fill="url(#eval)" filter="url(#sh2)" stroke="#D85A30" stroke-width="1.5"/>
  <text x="175" y="392" text-anchor="middle" fill="#4A1B0C" font-size="11" font-weight="bold" font-family="sans-serif">📊 AUC · F1 · Sens · Spec</text>
  <text x="175" y="408" text-anchor="middle" fill="#4A1B0C" font-size="10" font-family="sans-serif">ROC Curves · Conf. Matrix</text>
  <text x="175" y="424" text-anchor="middle" fill="#4A1B0C" font-size="12" font-weight="bold" font-family="sans-serif">AUC = 0.979 🎯</text>
  <text x="175" y="436" text-anchor="middle" fill="#4A1B0C" font-size="10" font-family="sans-serif">+0.0011 vs baseline</text>
  <rect x="340" y="370" width="170" height="72" rx="10" fill="url(#eval)" filter="url(#sh2)" stroke="#D85A30" stroke-width="1.5"/>
  <text x="425" y="392" text-anchor="middle" fill="#4A1B0C" font-size="11" font-weight="bold" font-family="sans-serif">📊 AUC · F1 · Sens · Spec</text>
  <text x="425" y="408" text-anchor="middle" fill="#4A1B0C" font-size="10" font-family="sans-serif">ROC Curves · Conf. Matrix</text>
  <text x="425" y="424" text-anchor="middle" fill="#4A1B0C" font-size="12" font-weight="bold" font-family="sans-serif">AUC = 0.958 🎯</text>
  <text x="425" y="436" text-anchor="middle" fill="#4A1B0C" font-size="10" font-family="sans-serif">+0.0033 vs baseline</text>
  <rect x="590" y="370" width="170" height="72" rx="10" fill="url(#eval)" filter="url(#sh2)" stroke="#D85A30" stroke-width="1.5"/>
  <text x="675" y="392" text-anchor="middle" fill="#4A1B0C" font-size="11" font-weight="bold" font-family="sans-serif">📊 AUC · F1 · Sens · Spec</text>
  <text x="675" y="408" text-anchor="middle" fill="#4A1B0C" font-size="10" font-family="sans-serif">ROC Curves · Conf. Matrix</text>
  <text x="675" y="424" text-anchor="middle" fill="#4A1B0C" font-size="12" font-weight="bold" font-family="sans-serif">AUC = 0.838 🎯</text>
  <text x="675" y="436" text-anchor="middle" fill="#4A1B0C" font-size="10" font-family="sans-serif">+0.0153 vs baseline</text>
  <line x1="175" y1="442" x2="175" y2="470" stroke="#888" stroke-width="1.5"/>
  <line x1="425" y1="442" x2="425" y2="470" stroke="#888" stroke-width="1.5"/>
  <line x1="675" y1="442" x2="675" y2="470" stroke="#888" stroke-width="1.5"/>
  <line x1="175" y1="470" x2="675" y2="470" stroke="#888" stroke-width="1.5"/>
  <line x1="425" y1="470" x2="425" y2="488" stroke="#888" stroke-width="1.5" marker-end="url(#arr)"/>
  <rect x="270" y="488" width="320" height="40" rx="12" fill="url(#deploy)" filter="url(#sh2)" stroke="#378ADD" stroke-width="2"/>
  <text x="430" y="513" text-anchor="middle" fill="#042C53" font-size="14" font-weight="bold" font-family="sans-serif">🚀 Gradio App — Live on Kaggle</text>
</svg>

</div>

---

## ⚙️ Feature Engineering (Pima)

<div align="center">

*The Pima dataset is the hardest — 768 rows, noisy 1988 data, biological impossibilities in raw values. We added 8 clinically motivated features to push AUC from 0.823 → 0.838.*

<svg viewBox="0 0 860 300" xmlns="http://www.w3.org/2000/svg" width="860" height="300">
  <defs>
    <linearGradient id="rawg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#534AB7"/><stop offset="100%" style="stop-color:#7F77DD"/>
    </linearGradient>
    <linearGradient id="engg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#0F6E56"/><stop offset="100%" style="stop-color:#1D9E75"/>
    </linearGradient>
    <marker id="arr2" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#7F77DD"/>
    </marker>
  </defs>
  <rect x="10" y="20" width="220" height="260" rx="14" fill="#EEEDFE" stroke="#7F77DD" stroke-width="2"/>
  <rect x="10" y="20" width="220" height="40" rx="14" fill="url(#rawg)"/>
  <rect x="10" y="45" width="220" height="15" fill="url(#rawg)"/>
  <text x="120" y="46" text-anchor="middle" fill="white" font-size="13" font-weight="bold" font-family="sans-serif">🔢 8 Raw Features</text>
  <text x="30" y="82" fill="#26215C" font-size="11" font-family="sans-serif">• Pregnancies</text>
  <text x="30" y="102" fill="#26215C" font-size="11" font-family="sans-serif">• Glucose (mg/dL)</text>
  <text x="30" y="122" fill="#26215C" font-size="11" font-family="sans-serif">• Blood Pressure (mmHg)</text>
  <text x="30" y="142" fill="#26215C" font-size="11" font-family="sans-serif">• Skin Thickness (mm)</text>
  <text x="30" y="162" fill="#26215C" font-size="11" font-family="sans-serif">• Insulin (μU/mL)</text>
  <text x="30" y="182" fill="#26215C" font-size="11" font-family="sans-serif">• BMI</text>
  <text x="30" y="202" fill="#26215C" font-size="11" font-family="sans-serif">• Diabetes Pedigree Fn.</text>
  <text x="30" y="222" fill="#26215C" font-size="11" font-family="sans-serif">• Age</text>
  <line x1="230" y1="150" x2="295" y2="150" stroke="#7F77DD" stroke-width="2.5" marker-end="url(#arr2)"/>
  <rect x="233" y="130" width="58" height="38" rx="8" fill="#EEEDFE" stroke="#7F77DD" stroke-width="1"/>
  <text x="262" y="148" text-anchor="middle" fill="#534AB7" font-size="9" font-weight="bold" font-family="sans-serif">Clinical</text>
  <text x="262" y="160" text-anchor="middle" fill="#534AB7" font-size="9" font-weight="bold" font-family="sans-serif">Logic</text>
  <rect x="300" y="20" width="240" height="260" rx="14" fill="#FFF8EE" stroke="#BA7517" stroke-width="2"/>
  <rect x="300" y="20" width="240" height="40" rx="14" fill="#EF9F27"/>
  <rect x="300" y="45" width="240" height="15" fill="#EF9F27"/>
  <text x="420" y="46" text-anchor="middle" fill="white" font-size="13" font-weight="bold" font-family="sans-serif">⚗️ 8 New Features</text>
  <text x="320" y="78" fill="#412402" font-size="10" font-family="sans-serif" font-weight="bold">glucose_bmi</text>
  <text x="320" y="92" fill="#633806" font-size="9" font-family="sans-serif">Glucose × BMI → insulin resistance</text>
  <text x="320" y="112" fill="#412402" font-size="10" font-family="sans-serif" font-weight="bold">bp_age</text>
  <text x="320" y="126" fill="#633806" font-size="9" font-family="sans-serif">BloodPressure × Age → CV stress</text>
  <text x="320" y="146" fill="#412402" font-size="10" font-family="sans-serif" font-weight="bold">glucose_bmi_ratio</text>
  <text x="320" y="160" fill="#633806" font-size="9" font-family="sans-serif">Glucose ÷ BMI → thin+hyperglycemia</text>
  <text x="320" y="180" fill="#412402" font-size="10" font-family="sans-serif" font-weight="bold">skin_bmi_ratio</text>
  <text x="320" y="194" fill="#633806" font-size="9" font-family="sans-serif">SkinThickness ÷ BMI → adiposity</text>
  <text x="320" y="214" fill="#412402" font-size="10" font-family="sans-serif" font-weight="bold">insulin_glucose</text>
  <text x="320" y="228" fill="#633806" font-size="9" font-family="sans-serif">Insulin ÷ Glucose → sensitivity</text>
  <text x="320" y="248" fill="#412402" font-size="10" font-family="sans-serif" font-weight="bold">bmi_bin + glucose_bin</text>
  <text x="320" y="262" fill="#633806" font-size="9" font-family="sans-serif">WHO + clinical thresholds</text>
  <line x1="540" y1="150" x2="600" y2="150" stroke="#1D9E75" stroke-width="2.5" marker-end="url(#arr2)"/>
  <rect x="543" y="130" width="53" height="38" rx="8" fill="#E1F5EE" stroke="#1D9E75" stroke-width="1"/>
  <text x="569" y="148" text-anchor="middle" fill="#0F6E56" font-size="9" font-weight="bold" font-family="sans-serif">SMOTE +</text>
  <text x="569" y="160" text-anchor="middle" fill="#0F6E56" font-size="9" font-weight="bold" font-family="sans-serif">Scale</text>
  <rect x="606" y="20" width="244" height="260" rx="14" fill="#E1F5EE" stroke="#1D9E75" stroke-width="2"/>
  <rect x="606" y="20" width="244" height="40" rx="14" fill="url(#engg)"/>
  <rect x="606" y="45" width="244" height="15" fill="url(#engg)"/>
  <text x="728" y="46" text-anchor="middle" fill="white" font-size="13" font-weight="bold" font-family="sans-serif">🏆 16-Feature XGBoost</text>
  <text x="626" y="82" fill="#04342C" font-size="11" font-family="sans-serif" font-weight="bold">Baseline AUC (8 feat)</text>
  <rect x="626" y="90" width="80" height="14" rx="4" fill="#B4B2A9"/>
  <rect x="626" y="90" width="66" height="14" rx="4" fill="#888780"/>
  <text x="718" y="102" fill="#085041" font-size="11" font-family="sans-serif">0.823</text>
  <text x="626" y="122" fill="#04342C" font-size="11" font-family="sans-serif" font-weight="bold">Tuned AUC (8 feat)</text>
  <rect x="626" y="130" width="80" height="14" rx="4" fill="#9FE1CB"/>
  <rect x="626" y="130" width="67" height="14" rx="4" fill="#5DCAA5"/>
  <text x="718" y="142" fill="#085041" font-size="11" font-family="sans-serif">0.825</text>
  <text x="626" y="162" fill="#04342C" font-size="11" font-family="sans-serif" font-weight="bold">Eng. XGB (16 feat)</text>
  <rect x="626" y="170" width="80" height="14" rx="4" fill="#9FE1CB"/>
  <rect x="626" y="170" width="69" height="14" rx="4" fill="#1D9E75"/>
  <text x="718" y="182" fill="#085041" font-size="11" font-family="sans-serif">0.838</text>
  <text x="626" y="205" fill="#04342C" font-size="11" font-family="sans-serif" font-weight="bold">Top feature impact:</text>
  <text x="626" y="222" fill="#085041" font-size="10" font-family="sans-serif">1. glucose_bmi (insulin resist.)</text>
  <text x="626" y="238" fill="#085041" font-size="10" font-family="sans-serif">2. Glucose (raw)</text>
  <text x="626" y="254" fill="#085041" font-size="10" font-family="sans-serif">3. BMI (raw)</text>
  <text x="626" y="270" fill="#085041" font-size="10" font-family="sans-serif">4. glucose_bmi_ratio</text>
</svg>

</div>

---

## 🤖 Models & Results

<div align="center">

### 🏆 Final Leaderboard

| Dataset | Best Model | AUC | F1 | Sensitivity | Specificity |
|:--------|:-----------|:---:|:--:|:-----------:|:-----------:|
| 🩸 Diabetes-Large | **LightGBM** | `0.979` | `0.804` | `0.709` | `0.995` |
| ❤️ Heart-Cleveland | **Logistic Regression** | `0.958` | `0.902` | `0.821` | `1.000` |
| 🧬 Diabetes-Pima | **XGBoost (eng.)** | `0.838` | `0.649` | `0.685` | `0.770` |

</div>

### 📐 Why These Metrics?

In clinical ML, **accuracy alone is insufficient**. We report:

| Metric | Formula | Why It Matters |
|:-------|:--------|:---------------|
| **ROC-AUC** | Area under ROC curve | Model discrimination regardless of threshold |
| **Sensitivity** | TP / (TP + FN) | Catching real positives — missing a sick patient is costly |
| **Specificity** | TN / (TN + FP) | Avoiding false alarms — unnecessary treatment has costs too |
| **F1 Score** | 2·P·R / (P+R) | Harmonic mean — important under class imbalance |

### 🧠 Model Selection Rationale

<div align="center">

<svg viewBox="0 0 860 180" xmlns="http://www.w3.org/2000/svg" width="860" height="180">
  <defs>
    <linearGradient id="teal2" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#1D9E75"/><stop offset="100%" style="stop-color:#0F6E56"/>
    </linearGradient>
    <linearGradient id="coral2" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#D85A30"/><stop offset="100%" style="stop-color:#993C1D"/>
    </linearGradient>
    <linearGradient id="purple2" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#7F77DD"/><stop offset="100%" style="stop-color:#534AB7"/>
    </linearGradient>
    <filter id="sh3"><feDropShadow dx="0" dy="3" stdDeviation="4" flood-opacity="0.12"/></filter>
  </defs>
  <rect x="10" y="10" width="260" height="160" rx="14" fill="white" stroke="#1D9E75" stroke-width="2" filter="url(#sh3)"/>
  <rect x="10" y="10" width="260" height="44" rx="14" fill="url(#teal2)"/>
  <rect x="10" y="38" width="260" height="16" fill="url(#teal2)"/>
  <text x="140" y="38" text-anchor="middle" fill="white" font-size="13" font-weight="bold" font-family="sans-serif">LightGBM — Diabetes-Large</text>
  <text x="25" y="72" fill="#085041" font-size="10" font-family="sans-serif">✦ 146k training rows — boosting thrives</text>
  <text x="25" y="90" fill="#085041" font-size="10" font-family="sans-serif">✦ Histogram-based → GPU-compatible</text>
  <text x="25" y="108" fill="#085041" font-size="10" font-family="sans-serif">✦ Handles heavy class imbalance well</text>
  <text x="25" y="126" fill="#085041" font-size="10" font-family="sans-serif">✦ Leaf-wise growth catches subtle patterns</text>
  <text x="25" y="144" fill="#085041" font-size="10" font-family="sans-serif">✦ 50 Optuna trials → +0.0011 AUC gain</text>
  <text x="140" y="162" text-anchor="middle" fill="#1D9E75" font-size="11" font-weight="bold" font-family="sans-serif">AUC 0.979</text>
  <rect x="300" y="10" width="260" height="160" rx="14" fill="white" stroke="#D85A30" stroke-width="2" filter="url(#sh3)"/>
  <rect x="300" y="10" width="260" height="44" rx="14" fill="url(#coral2)"/>
  <rect x="300" y="38" width="260" height="16" fill="url(#coral2)"/>
  <text x="430" y="38" text-anchor="middle" fill="white" font-size="13" font-weight="bold" font-family="sans-serif">LogReg — Heart-Cleveland</text>
  <text x="315" y="72" fill="#4A1B0C" font-size="10" font-family="sans-serif">✦ Only 237 train rows — simpler = better</text>
  <text x="315" y="90" fill="#4A1B0C" font-size="10" font-family="sans-serif">✦ Linear decision boundary sufficient</text>
  <text x="315" y="108" fill="#4A1B0C" font-size="10" font-family="sans-serif">✦ L1 penalty (Optuna) → feature selection</text>
  <text x="315" y="126" fill="#4A1B0C" font-size="10" font-family="sans-serif">✦ SAGA solver handles l1 penalty cleanly</text>
  <text x="315" y="144" fill="#4A1B0C" font-size="10" font-family="sans-serif">✦ Spec = 1.0 → zero false positives</text>
  <text x="430" y="162" text-anchor="middle" fill="#D85A30" font-size="11" font-weight="bold" font-family="sans-serif">AUC 0.958</text>
  <rect x="590" y="10" width="260" height="160" rx="14" fill="white" stroke="#7F77DD" stroke-width="2" filter="url(#sh3)"/>
  <rect x="590" y="10" width="260" height="44" rx="14" fill="url(#purple2)"/>
  <rect x="590" y="38" width="260" height="16" fill="url(#purple2)"/>
  <text x="720" y="38" text-anchor="middle" fill="white" font-size="13" font-weight="bold" font-family="sans-serif">XGBoost — Diabetes-Pima</text>
  <text x="605" y="72" fill="#26215C" font-size="10" font-family="sans-serif">✦ 16 engineered features → richer signal</text>
  <text x="605" y="90" fill="#26215C" font-size="10" font-family="sans-serif">✦ Regularization (α, λ, γ) fights overfitting</text>
  <text x="605" y="108" fill="#26215C" font-size="10" font-family="sans-serif">✦ 100 Optuna trials → best search budget</text>
  <text x="605" y="126" fill="#26215C" font-size="10" font-family="sans-serif">✦ CUDA hist mode → fast on Kaggle GPU</text>
  <text x="605" y="144" fill="#26215C" font-size="10" font-family="sans-serif">✦ Stacking ensemble also evaluated</text>
  <text x="720" y="162" text-anchor="middle" fill="#7F77DD" font-size="11" font-weight="bold" font-family="sans-serif">AUC 0.838</text>
</svg>

</div>

---

## 🔬 Hyperparameter Tuning

<div align="center">

*Optuna TPE (Tree-structured Parzen Estimator) — smarter than grid search, faster than random search.*

<svg viewBox="0 0 860 230" xmlns="http://www.w3.org/2000/svg" width="860" height="230">
  <defs>
    <linearGradient id="tabh" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#185FA5"/><stop offset="100%" style="stop-color:#378ADD"/>
    </linearGradient>
  </defs>
  <rect x="10" y="10" width="840" height="34" rx="8" fill="url(#tabh)"/>
  <text x="130" y="33" text-anchor="middle" fill="white" font-size="12" font-weight="bold" font-family="sans-serif">Parameter</text>
  <text x="360" y="33" text-anchor="middle" fill="white" font-size="12" font-weight="bold" font-family="sans-serif">Search Range</text>
  <text x="570" y="33" text-anchor="middle" fill="white" font-size="12" font-weight="bold" font-family="sans-serif">Best Value Found</text>
  <text x="760" y="33" text-anchor="middle" fill="white" font-size="12" font-weight="bold" font-family="sans-serif">Model</text>
  <rect x="10" y="44" width="840" height="26" fill="#F0FFF8"/>
  <text x="130" y="62" text-anchor="middle" fill="#222" font-size="11" font-family="sans-serif">n_estimators</text>
  <text x="360" y="62" text-anchor="middle" fill="#555" font-size="11" font-family="sans-serif">100 – 500 (int)</text>
  <text x="570" y="62" text-anchor="middle" fill="#0F6E56" font-size="11" font-weight="bold" font-family="sans-serif">365</text>
  <text x="760" y="62" text-anchor="middle" fill="#1D9E75" font-size="11" font-family="sans-serif">LightGBM</text>
  <rect x="10" y="70" width="840" height="26" fill="#FAFAFA"/>
  <text x="130" y="88" text-anchor="middle" fill="#222" font-size="11" font-family="sans-serif">learning_rate</text>
  <text x="360" y="88" text-anchor="middle" fill="#555" font-size="11" font-family="sans-serif">0.01 – 0.2 (log scale)</text>
  <text x="570" y="88" text-anchor="middle" fill="#0F6E56" font-size="11" font-weight="bold" font-family="sans-serif">0.1022</text>
  <text x="760" y="88" text-anchor="middle" fill="#1D9E75" font-size="11" font-family="sans-serif">LightGBM</text>
  <rect x="10" y="96" width="840" height="26" fill="#F0FFF8"/>
  <text x="130" y="114" text-anchor="middle" fill="#222" font-size="11" font-family="sans-serif">num_leaves</text>
  <text x="360" y="114" text-anchor="middle" fill="#555" font-size="11" font-family="sans-serif">20 – 150 (int)</text>
  <text x="570" y="114" text-anchor="middle" fill="#0F6E56" font-size="11" font-weight="bold" font-family="sans-serif">100</text>
  <text x="760" y="114" text-anchor="middle" fill="#1D9E75" font-size="11" font-family="sans-serif">LightGBM</text>
  <rect x="10" y="122" width="840" height="26" fill="#FAFAFA"/>
  <text x="130" y="140" text-anchor="middle" fill="#222" font-size="11" font-family="sans-serif">C (regularization)</text>
  <text x="360" y="140" text-anchor="middle" fill="#555" font-size="11" font-family="sans-serif">0.001 – 100 (log scale)</text>
  <text x="570" y="140" text-anchor="middle" fill="#993C1D" font-size="11" font-weight="bold" font-family="sans-serif">70.72</text>
  <text x="760" y="140" text-anchor="middle" fill="#D85A30" font-size="11" font-family="sans-serif">Logistic Reg.</text>
  <rect x="10" y="148" width="840" height="26" fill="#F0FFF8"/>
  <text x="130" y="166" text-anchor="middle" fill="#222" font-size="11" font-family="sans-serif">penalty</text>
  <text x="360" y="166" text-anchor="middle" fill="#555" font-size="11" font-family="sans-serif">l1, l2 (categorical)</text>
  <text x="570" y="166" text-anchor="middle" fill="#993C1D" font-size="11" font-weight="bold" font-family="sans-serif">l1</text>
  <text x="760" y="166" text-anchor="middle" fill="#D85A30" font-size="11" font-family="sans-serif">Logistic Reg.</text>
  <rect x="10" y="174" width="840" height="26" fill="#FAFAFA"/>
  <text x="130" y="192" text-anchor="middle" fill="#222" font-size="11" font-family="sans-serif">max_depth</text>
  <text x="360" y="192" text-anchor="middle" fill="#555" font-size="11" font-family="sans-serif">3 – 10 (int)</text>
  <text x="570" y="192" text-anchor="middle" fill="#534AB7" font-size="11" font-weight="bold" font-family="sans-serif">8</text>
  <text x="760" y="192" text-anchor="middle" fill="#7F77DD" font-size="11" font-family="sans-serif">XGBoost</text>
  <rect x="10" y="200" width="840" height="26" fill="#F0FFF8"/>
  <text x="130" y="218" text-anchor="middle" fill="#222" font-size="11" font-family="sans-serif">gamma / reg_alpha / reg_lambda</text>
  <text x="360" y="218" text-anchor="middle" fill="#555" font-size="11" font-family="sans-serif">0.0–2.0 / 1e-4–10 / 1e-4–10</text>
  <text x="570" y="218" text-anchor="middle" fill="#534AB7" font-size="11" font-weight="bold" font-family="sans-serif">1.10 / 0.104 / 0.005</text>
  <text x="760" y="218" text-anchor="middle" fill="#7F77DD" font-size="11" font-family="sans-serif">XGBoost</text>
</svg>

</div>

---

## 📈 Performance Visuals

<div align="center">

| Plot | Description |
|:----:|:------------|
| `class_balance.png` | Before/after SMOTE class distribution across all 3 datasets |
| `roc_curves.png` | ROC curves — all 4 models overlaid per dataset |
| `metrics_heatmap.png` | Color-coded AUC / F1 / Sensitivity / Specificity grid |
| `confusion_matrices.png` | Confusion matrices for best model per dataset |
| `feature_importance.png` | Normalized RF + LightGBM feature importances |
| `tuned_vs_baseline.png` | Grouped bars — before vs after Optuna tuning |
| `optuna_history.png` | Trial-by-trial convergence scatter + best-so-far line |
| `pima_progression.png` | Baseline → Feature Eng. → Stacking progression |
| `pima_feature_importance_eng.png` | XGBoost importance on 16 engineered features |

</div>

---

## 🖥️ App Interface

<div align="center">

*Three independent prediction tabs — one per disease — each with clinically labeled inputs and a color-coded risk output.*

<svg viewBox="0 0 860 320" xmlns="http://www.w3.org/2000/svg" width="860" height="320">
  <defs>
    <linearGradient id="appbg" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#f8fafc"/><stop offset="100%" style="stop-color:#e2e8f0"/>
    </linearGradient>
    <linearGradient id="greenbtn" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#1D9E75"/><stop offset="100%" style="stop-color:#0F6E56"/>
    </linearGradient>
    <linearGradient id="redrisk" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#FFF5F5"/><stop offset="100%" style="stop-color:#FED7D7"/>
    </linearGradient>
    <filter id="sh4"><feDropShadow dx="0" dy="6" stdDeviation="8" flood-opacity="0.15"/></filter>
  </defs>
  <rect x="10" y="10" width="840" height="300" rx="14" fill="url(#appbg)" filter="url(#sh4)" stroke="#CBD5E0" stroke-width="1"/>
  <rect x="10" y="10" width="840" height="36" rx="14" fill="#2D3748"/>
  <rect x="10" y="32" width="840" height="14" fill="#2D3748"/>
  <circle cx="36" cy="28" r="6" fill="#FC8181"/>
  <circle cx="56" cy="28" r="6" fill="#F6AD55"/>
  <circle cx="76" cy="28" r="6" fill="#68D391"/>
  <rect x="200" y="18" width="460" height="20" rx="10" fill="#4A5568"/>
  <text x="430" y="32" text-anchor="middle" fill="#A0AEC0" font-size="10" font-family="sans-serif">🔒  medrisk-classifier.gradio.live</text>
  <text x="430" y="72" text-anchor="middle" fill="#1A202C" font-size="16" font-weight="bold" font-family="sans-serif">🏥 MedRisk Classifier</text>
  <text x="430" y="90" text-anchor="middle" fill="#718096" font-size="11" font-family="sans-serif">Generalizable ML-based Chronic Disease Risk Predictor</text>
  <rect x="30" y="100" width="180" height="28" rx="8" fill="#1D9E75"/>
  <text x="120" y="119" text-anchor="middle" fill="white" font-size="11" font-weight="bold" font-family="sans-serif">🩸 Diabetes Risk (Large)</text>
  <rect x="220" y="100" width="180" height="28" rx="8" fill="#E2E8F0"/>
  <text x="310" y="119" text-anchor="middle" fill="#4A5568" font-size="11" font-family="sans-serif">❤️ Heart Disease Risk</text>
  <rect x="410" y="100" width="180" height="28" rx="8" fill="#E2E8F0"/>
  <text x="500" y="119" text-anchor="middle" fill="#4A5568" font-size="11" font-family="sans-serif">🧬 Diabetes Risk (Pima)</text>
  <rect x="30" y="136" width="460" height="160" rx="10" fill="white" stroke="#E2E8F0" stroke-width="1"/>
  <text x="50" y="158" fill="#4A5568" font-size="10" font-family="sans-serif">Gender</text>
  <rect x="130" y="145" width="200" height="20" rx="4" fill="#F7FAFC" stroke="#CBD5E0" stroke-width="1"/>
  <text x="140" y="159" fill="#2D3748" font-size="10" font-family="sans-serif">Female ▾</text>
  <text x="50" y="182" fill="#4A5568" font-size="10" font-family="sans-serif">Age</text>
  <rect x="130" y="169" width="200" height="8" rx="4" fill="#E2E8F0"/>
  <rect x="130" y="169" width="120" height="8" rx="4" fill="#1D9E75"/>
  <circle cx="250" cy="173" r="6" fill="white" stroke="#1D9E75" stroke-width="2"/>
  <text x="340" y="178" fill="#2D3748" font-size="10" font-family="sans-serif">45</text>
  <text x="50" y="206" fill="#4A5568" font-size="10" font-family="sans-serif">BMI</text>
  <rect x="130" y="193" width="200" height="8" rx="4" fill="#E2E8F0"/>
  <rect x="130" y="193" width="90" height="8" rx="4" fill="#1D9E75"/>
  <circle cx="220" cy="197" r="6" fill="white" stroke="#1D9E75" stroke-width="2"/>
  <text x="340" y="202" fill="#2D3748" font-size="10" font-family="sans-serif">27.0</text>
  <text x="50" y="230" fill="#4A5568" font-size="10" font-family="sans-serif">HbA1c</text>
  <rect x="130" y="217" width="200" height="8" rx="4" fill="#E2E8F0"/>
  <rect x="130" y="217" width="70" height="8" rx="4" fill="#1D9E75"/>
  <circle cx="200" cy="221" r="6" fill="white" stroke="#1D9E75" stroke-width="2"/>
  <text x="340" y="226" fill="#2D3748" font-size="10" font-family="sans-serif">5.5%</text>
  <text x="50" y="254" fill="#4A5568" font-size="10" font-family="sans-serif">Blood Glucose</text>
  <rect x="130" y="241" width="200" height="8" rx="4" fill="#E2E8F0"/>
  <rect x="130" y="241" width="60" height="8" rx="4" fill="#1D9E75"/>
  <circle cx="190" cy="245" r="6" fill="white" stroke="#1D9E75" stroke-width="2"/>
  <text x="340" y="250" fill="#2D3748" font-size="10" font-family="sans-serif">100 mg/dL</text>
  <rect x="130" y="268" width="150" height="22" rx="8" fill="url(#greenbtn)"/>
  <text x="205" y="283" text-anchor="middle" fill="white" font-size="11" font-weight="bold" font-family="sans-serif">🔍 Predict</text>
  <rect x="510" y="136" width="340" height="160" rx="10" fill="url(#redrisk)" stroke="#FC8181" stroke-width="2"/>
  <text x="680" y="172" text-anchor="middle" fill="#742A2A" font-size="13" font-weight="bold" font-family="sans-serif">🔴 High Risk</text>
  <text x="680" y="210" text-anchor="middle" fill="#742A2A" font-size="36" font-weight="bold" font-family="sans-serif">72.4%</text>
  <text x="680" y="238" text-anchor="middle" fill="#9B2C2C" font-size="11" font-family="sans-serif">Estimated disease probability</text>
  <rect x="540" y="252" width="280" height="1" fill="#FC8181"/>
  <text x="680" y="272" text-anchor="middle" fill="#C53030" font-size="10" font-family="sans-serif">⚠️ For informational purposes only.</text>
  <text x="680" y="286" text-anchor="middle" fill="#C53030" font-size="10" font-family="sans-serif">Consult a medical professional.</text>
</svg>

</div>

---

## 🚀 Quick Start

### Run on Kaggle (Recommended)

```bash
# 1. Fork the notebook on Kaggle
# 2. Add the 3 datasets (paths already configured in code)
# 3. Enable GPU accelerator in Settings
# 4. Run All → Gradio app launches at the bottom
# 5. Copy the public gradio.live link from the output
```

### Local Setup

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/medrisk-classifier.git
cd medrisk-classifier

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook MedRisk_Classifier.ipynb
```

### Requirements

```text
numpy>=1.24
pandas>=2.0
scikit-learn>=1.3
xgboost>=2.0
lightgbm>=4.0
optuna>=3.4
imbalanced-learn>=0.11
gradio>=4.0
matplotlib>=3.7
seaborn>=0.13
```

---

## 🗂️ Project Structure

```
medrisk-classifier/
│
├── 📓 MedRisk_Classifier.ipynb        ← Main Kaggle notebook (all 5 snippets)
│
├── 📊 outputs/
│   ├── class_balance.png
│   ├── smote_balance.png
│   ├── target_correlation.png
│   ├── dist_*.png                     ← Per-dataset KDE distributions
│   ├── corr_*.png                     ← Per-dataset correlation heatmaps
│   ├── categorical_breakdown.png
│   ├── metrics_heatmap.png
│   ├── roc_curves.png
│   ├── confusion_matrices.png
│   ├── feature_importance.png
│   ├── tuned_vs_baseline.png
│   ├── optuna_history.png
│   ├── pima_progression.png
│   └── pima_feature_importance_eng.png
│
├── 📋 requirements.txt
└── 📖 README.md
```

---

## 🔭 What's Next

<div align="center">

<svg viewBox="0 0 860 140" xmlns="http://www.w3.org/2000/svg" width="860" height="140">
  <defs>
    <linearGradient id="nb1" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#E6F1FB"/><stop offset="100%" style="stop-color:#B5D4F4"/>
    </linearGradient>
    <linearGradient id="nb2" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#EAF3DE"/><stop offset="100%" style="stop-color:#C0DD97"/>
    </linearGradient>
    <linearGradient id="nb3" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#FAEEDA"/><stop offset="100%" style="stop-color:#FAC775"/>
    </linearGradient>
    <linearGradient id="nb4" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#FAECE7"/><stop offset="100%" style="stop-color:#F0997B"/>
    </linearGradient>
    <filter id="sh5"><feDropShadow dx="0" dy="3" stdDeviation="4" flood-opacity="0.1"/></filter>
  </defs>
  <rect x="10" y="20" width="190" height="100" rx="12" fill="url(#nb1)" stroke="#378ADD" stroke-width="1.5" filter="url(#sh5)"/>
  <text x="105" y="52" text-anchor="middle" font-size="22" font-family="sans-serif">🧠</text>
  <text x="105" y="74" text-anchor="middle" fill="#042C53" font-size="11" font-weight="bold" font-family="sans-serif">Deep Learning</text>
  <text x="105" y="90" text-anchor="middle" fill="#185FA5" font-size="10" font-family="sans-serif">TabNet / MLP on</text>
  <text x="105" y="106" text-anchor="middle" fill="#185FA5" font-size="10" font-family="sans-serif">Diabetes-Large</text>
  <rect x="220" y="20" width="190" height="100" rx="12" fill="url(#nb2)" stroke="#639922" stroke-width="1.5" filter="url(#sh5)"/>
  <text x="315" y="52" text-anchor="middle" font-size="22" font-family="sans-serif">🔄</text>
  <text x="315" y="74" text-anchor="middle" fill="#173404" font-size="11" font-weight="bold" font-family="sans-serif">Cross-Dataset</text>
  <text x="315" y="90" text-anchor="middle" fill="#3B6D11" font-size="10" font-family="sans-serif">Transfer learning &amp;</text>
  <text x="315" y="106" text-anchor="middle" fill="#3B6D11" font-size="10" font-family="sans-serif">domain adaptation</text>
  <rect x="430" y="20" width="190" height="100" rx="12" fill="url(#nb3)" stroke="#BA7517" stroke-width="1.5" filter="url(#sh5)"/>
  <text x="525" y="52" text-anchor="middle" font-size="22" font-family="sans-serif">📡</text>
  <text x="525" y="74" text-anchor="middle" fill="#412402" font-size="11" font-weight="bold" font-family="sans-serif">HuggingFace Deploy</text>
  <text x="525" y="90" text-anchor="middle" fill="#633806" font-size="10" font-family="sans-serif">Persistent Space with</text>
  <text x="525" y="106" text-anchor="middle" fill="#633806" font-size="10" font-family="sans-serif">model artifacts cached</text>
  <rect x="640" y="20" width="210" height="100" rx="12" fill="url(#nb4)" stroke="#D85A30" stroke-width="1.5" filter="url(#sh5)"/>
  <text x="745" y="52" text-anchor="middle" font-size="22" font-family="sans-serif">🩺</text>
  <text x="745" y="74" text-anchor="middle" fill="#4A1B0C" font-size="11" font-weight="bold" font-family="sans-serif">SHAP Explainability</text>
  <text x="745" y="90" text-anchor="middle" fill="#712B13" font-size="10" font-family="sans-serif">Per-patient feature</text>
  <text x="745" y="106" text-anchor="middle" fill="#712B13" font-size="10" font-family="sans-serif">attribution waterfall</text>
</svg>

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=wave&color=gradient&customColorList=0,2,2,5,30&height=100&section=footer&reversal=false" width="100%" alt="footer"/>

<br/>

**Built with 🩺 for learning · Deployed on Kaggle · Open Source**

<br/>

<img src="https://img.shields.io/badge/Made%20with-Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
<img src="https://img.shields.io/badge/Powered%20by-Kaggle%20GPU-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white"/>
<img src="https://img.shields.io/badge/Models-Production%20Ready-22C55E?style=for-the-badge"/>

<br/><br/>

*⚠️ This project is for educational and portfolio purposes. It is not intended as medical advice.*

</div>
