<div align="center">

<svg width="900" height="180" viewBox="0 0 900 180" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0f0c29"/>
      <stop offset="50%" style="stop-color:#302b63"/>
      <stop offset="100%" style="stop-color:#24243e"/>
    </linearGradient>
    <linearGradient id="textGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#5DCAA5"/>
      <stop offset="50%" style="stop-color:#378ADD"/>
      <stop offset="100%" style="stop-color:#7F77DD"/>
    </linearGradient>
    <linearGradient id="pulse1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#5DCAA5;stop-opacity:0"/>
      <stop offset="50%" style="stop-color:#5DCAA5;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#5DCAA5;stop-opacity:0"/>
      <animateTransform attributeName="gradientTransform" type="translate" from="-1 0" to="1 0" dur="2s" repeatCount="indefinite"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="900" height="180" rx="18" fill="url(#bgGrad)"/>

  <!-- Decorative circles -->
  <circle cx="60" cy="90" r="45" fill="none" stroke="#5DCAA5" stroke-width="1" opacity="0.3">
    <animate attributeName="r" values="45;55;45" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0.6;0.3" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="60" cy="90" r="28" fill="none" stroke="#378ADD" stroke-width="1.5" opacity="0.5">
    <animate attributeName="r" values="28;35;28" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <!-- ECG line left -->
  <polyline points="20,90 35,90 40,60 45,115 50,70 55,105 60,90 90,90" fill="none" stroke="#5DCAA5" stroke-width="2" filter="url(#glow)">
    <animate attributeName="opacity" values="0.4;1;0.4" dur="1.5s" repeatCount="indefinite"/>
  </polyline>

  <circle cx="840" cy="90" r="45" fill="none" stroke="#7F77DD" stroke-width="1" opacity="0.3">
    <animate attributeName="r" values="45;55;45" dur="3.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0.6;0.3" dur="3.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="840" cy="90" r="28" fill="none" stroke="#D85A30" stroke-width="1.5" opacity="0.5">
    <animate attributeName="r" values="28;35;28" dur="2.8s" repeatCount="indefinite"/>
  </circle>
  <polyline points="810,90 825,90 830,60 835,115 840,70 845,105 850,90 880,90" fill="none" stroke="#7F77DD" stroke-width="2" filter="url(#glow)">
    <animate attributeName="opacity" values="0.4;1;0.4" dur="2s" repeatCount="indefinite"/>
  </polyline>

  <!-- Title -->
  <text x="450" y="72" font-family="'Segoe UI', system-ui, sans-serif" font-size="42" font-weight="800" text-anchor="middle" fill="url(#textGrad)" filter="url(#glow)">MedRisk Classifier</text>

  <!-- Subtitle -->
  <text x="450" y="108" font-family="'Segoe UI', system-ui, sans-serif" font-size="16" text-anchor="middle" fill="#a0aec0" letter-spacing="3">GENERALIZABLE ML · CHRONIC DISEASE PREDICTION</text>

  <!-- Animated underline -->
  <rect x="200" y="120" width="0" height="2" rx="1" fill="url(#textGrad)">
    <animate attributeName="width" values="0;500;0" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="x" values="450;200;450" dur="4s" repeatCount="indefinite"/>
  </rect>

  <!-- Stats row -->
  <text x="230" y="155" font-family="'Segoe UI', sans-serif" font-size="13" text-anchor="middle" fill="#5DCAA5" font-weight="600">3 DATASETS</text>
  <text x="350" y="155" font-family="'Segoe UI', sans-serif" font-size="13" text-anchor="middle" fill="#378ADD" font-weight="600">4 MODELS</text>
  <text x="450" y="155" font-family="'Segoe UI', sans-serif" font-size="13" text-anchor="middle" fill="#7F77DD" font-weight="600">AUC UP TO 0.979</text>
  <text x="570" y="155" font-family="'Segoe UI', sans-serif" font-size="13" text-anchor="middle" fill="#D85A30" font-weight="600">OPTUNA TUNED</text>
  <text x="680" y="155" font-family="'Segoe UI', sans-serif" font-size="13" text-anchor="middle" fill="#EF9F27" font-weight="600">GRADIO DEPLOYED</text>
</svg>

<br/>

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-GPU%20Accelerated-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-Tuned-FF6600?style=for-the-badge&logo=xgboost&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-Optimized-0175C2?style=for-the-badge&logo=lightgbm&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-Live%20Demo-F97316?style=for-the-badge&logo=gradio&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-10B981?style=for-the-badge)

</div>

---

<div align="center">

## 🎯 Live Demo

**▶ [Try the App on Kaggle](YOUR_KAGGLE_NOTEBOOK_LINK)**&nbsp;&nbsp;|&nbsp;&nbsp;**📓 [View Notebook](YOUR_NOTEBOOK_LINK)**&nbsp;&nbsp;|&nbsp;&nbsp;**📊 [Datasets](#-datasets)**

</div>

---

## 📖 Overview

> **MedRisk Classifier** is a production-ready, generalizable machine learning pipeline for chronic disease risk prediction. It demonstrates that a single, well-engineered ML workflow can be adapted across multiple clinical datasets with minimal changes — making it a template for real-world medical AI applications.

The project trains, evaluates, tunes, and deploys **four classifiers** across **three independent clinical datasets**, using clinically meaningful evaluation metrics (sensitivity, specificity, ROC-AUC), SMOTE balancing, Optuna hyperparameter tuning, and feature engineering. The final Gradio interface allows anyone to input patient vitals and receive an instant risk assessment — no setup required.

---

## ✨ Key Highlights

<div align="center">

<table>
<tr>
<td align="center" width="200">

<svg width="64" height="64" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
  <circle cx="32" cy="32" r="30" fill="#0f1923" stroke="#5DCAA5" stroke-width="2"/>
  <path d="M16,32 L24,32 L27,20 L30,42 L33,26 L36,36 L39,32 L48,32" fill="none" stroke="#5DCAA5" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
    <animate attributeName="stroke-dasharray" values="0,100;100,0" dur="2s" fill="freeze"/>
  </path>
</svg>

**Clinical Metrics**
Sensitivity · Specificity · ROC-AUC · F1

</td>
<td align="center" width="200">

<svg width="64" height="64" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
  <circle cx="32" cy="32" r="30" fill="#0f1923" stroke="#378ADD" stroke-width="2"/>
  <rect x="18" y="38" width="8" height="12" rx="2" fill="#378ADD" opacity="0.5"/>
  <rect x="28" y="28" width="8" height="22" rx="2" fill="#378ADD" opacity="0.75"/>
  <rect x="38" y="18" width="8" height="32" rx="2" fill="#378ADD">
    <animate attributeName="height" values="10;32;10" dur="2.5s" repeatCount="indefinite"/>
    <animate attributeName="y" values="40;18;40" dur="2.5s" repeatCount="indefinite"/>
  </rect>
</svg>

**Optuna Tuning**
50–100 TPE trials per model

</td>
<td align="center" width="200">

<svg width="64" height="64" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
  <circle cx="32" cy="32" r="30" fill="#0f1923" stroke="#7F77DD" stroke-width="2"/>
  <circle cx="32" cy="32" r="14" fill="none" stroke="#7F77DD" stroke-width="2" stroke-dasharray="4,4">
    <animateTransform attributeName="transform" type="rotate" from="0 32 32" to="360 32 32" dur="6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="32" cy="18" r="4" fill="#7F77DD"/>
  <circle cx="44" cy="40" r="4" fill="#5DCAA5"/>
  <circle cx="20" cy="40" r="4" fill="#D85A30"/>
</svg>

**3 Datasets**
100k · 297 · 768 patients

</td>
<td align="center" width="200">

<svg width="64" height="64" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
  <circle cx="32" cy="32" r="30" fill="#0f1923" stroke="#D85A30" stroke-width="2"/>
  <rect x="20" y="20" width="24" height="28" rx="4" fill="none" stroke="#D85A30" stroke-width="2"/>
  <line x1="26" y1="30" x2="38" y2="30" stroke="#D85A30" stroke-width="2" stroke-linecap="round"/>
  <line x1="26" y1="36" x2="34" y2="36" stroke="#D85A30" stroke-width="2" stroke-linecap="round" opacity="0.6"/>
  <circle cx="44" cy="44" r="8" fill="#1D9E75"/>
  <text x="44" y="48" font-size="10" text-anchor="middle" fill="white" font-weight="bold">✓</text>
</svg>

**Live Gradio App**
3-tab interactive demo

</td>
<td align="center" width="200">

<svg width="64" height="64" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
  <circle cx="32" cy="32" r="30" fill="#0f1923" stroke="#EF9F27" stroke-width="2"/>
  <polygon points="32,14 36,26 48,26 38,34 42,46 32,38 22,46 26,34 16,26 28,26" fill="none" stroke="#EF9F27" stroke-width="2">
    <animate attributeName="opacity" values="0.4;1;0.4" dur="2s" repeatCount="indefinite"/>
  </polygon>
  <polygon points="32,20 34,27 41,27 36,31 38,38 32,34 26,38 28,31 23,27 30,27" fill="#EF9F27" opacity="0.6"/>
</svg>

**Feature Engineering**
16 clinical interaction features

</td>
</tr>
</table>

</div>

---

## 🗂️ Datasets

<div align="center">

<svg width="860" height="200" viewBox="0 0 860 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="card1" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#0d3b2e"/>
      <stop offset="100%" style="stop-color:#0a1a14"/>
    </linearGradient>
    <linearGradient id="card2" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#0d2a3b"/>
      <stop offset="100%" style="stop-color:#0a1520"/>
    </linearGradient>
    <linearGradient id="card3" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#2d1a3b"/>
      <stop offset="100%" style="stop-color:#150a1a"/>
    </linearGradient>
  </defs>

  <!-- Card 1 -->
  <rect x="10" y="10" width="260" height="180" rx="14" fill="url(#card1)" stroke="#5DCAA5" stroke-width="1.5"/>
  <rect x="10" y="10" width="260" height="6" rx="4" fill="#5DCAA5"/>
  <text x="140" y="50" font-family="'Segoe UI',sans-serif" font-size="14" font-weight="700" text-anchor="middle" fill="#5DCAA5">🩸 Diabetes Prediction</text>
  <text x="140" y="72" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#a0aec0">iammustafatz · Kaggle</text>
  <line x1="30" y1="82" x2="250" y2="82" stroke="#5DCAA5" stroke-width="0.5" opacity="0.4"/>
  <text x="30" y="100" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">📦 Rows</text>
  <text x="250" y="100" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#5DCAA5" font-weight="600">100,000</text>
  <text x="30" y="118" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">🔢 Features</text>
  <text x="250" y="118" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#5DCAA5" font-weight="600">8</text>
  <text x="30" y="136" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">⚖️ Positive Rate</text>
  <text x="250" y="136" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#D85A30" font-weight="600">8.5% (imbalanced)</text>
  <text x="30" y="154" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">🏆 Best Model</text>
  <text x="250" y="154" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#EF9F27" font-weight="600">LightGBM</text>
  <text x="30" y="172" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">📈 AUC</text>
  <text x="250" y="172" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#5DCAA5" font-weight="700">0.979</text>

  <!-- Card 2 -->
  <rect x="300" y="10" width="260" height="180" rx="14" fill="url(#card2)" stroke="#378ADD" stroke-width="1.5"/>
  <rect x="300" y="10" width="260" height="6" rx="4" fill="#378ADD"/>
  <text x="430" y="50" font-family="'Segoe UI',sans-serif" font-size="14" font-weight="700" text-anchor="middle" fill="#378ADD">❤️ Heart Disease</text>
  <text x="430" y="72" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#a0aec0">Cleveland UCI · cherngs</text>
  <line x1="320" y1="82" x2="540" y2="82" stroke="#378ADD" stroke-width="0.5" opacity="0.4"/>
  <text x="320" y="100" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">📦 Rows</text>
  <text x="540" y="100" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#378ADD" font-weight="600">297</text>
  <text x="320" y="118" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">🔢 Features</text>
  <text x="540" y="118" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#378ADD" font-weight="600">13</text>
  <text x="320" y="136" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">⚖️ Positive Rate</text>
  <text x="540" y="136" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#5DCAA5" font-weight="600">46.1% (balanced)</text>
  <text x="320" y="154" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">🏆 Best Model</text>
  <text x="540" y="154" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#EF9F27" font-weight="600">Logistic Regression</text>
  <text x="320" y="172" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">📈 AUC</text>
  <text x="540" y="172" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#378ADD" font-weight="700">0.958</text>

  <!-- Card 3 -->
  <rect x="590" y="10" width="260" height="180" rx="14" fill="url(#card3)" stroke="#7F77DD" stroke-width="1.5"/>
  <rect x="590" y="10" width="260" height="6" rx="4" fill="#7F77DD"/>
  <text x="720" y="50" font-family="'Segoe UI',sans-serif" font-size="14" font-weight="700" text-anchor="middle" fill="#7F77DD">🧬 Pima Diabetes</text>
  <text x="720" y="72" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#a0aec0">UCI ML · Pima Indians</text>
  <line x1="610" y1="82" x2="830" y2="82" stroke="#7F77DD" stroke-width="0.5" opacity="0.4"/>
  <text x="610" y="100" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">📦 Rows</text>
  <text x="830" y="100" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#7F77DD" font-weight="600">768</text>
  <text x="610" y="118" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">🔢 Features</text>
  <text x="830" y="118" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#7F77DD" font-weight="600">8 → 16 (engineered)</text>
  <text x="610" y="136" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">⚖️ Positive Rate</text>
  <text x="830" y="136" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#EF9F27" font-weight="600">34.9% (moderate)</text>
  <text x="610" y="154" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">🏆 Best Model</text>
  <text x="830" y="154" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#EF9F27" font-weight="600">XGBoost (tuned)</text>
  <text x="610" y="172" font-family="'Segoe UI',sans-serif" font-size="12" fill="#e2e8f0">📈 AUC</text>
  <text x="830" y="172" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="end" fill="#7F77DD" font-weight="700">0.838</text>
</svg>

</div>

---

## 🔄 Pipeline Architecture

<div align="center">

<svg width="860" height="520" viewBox="0 0 860 520" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="stageBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0a0a1a"/>
      <stop offset="100%" style="stop-color:#0d1117"/>
    </linearGradient>
    <marker id="arrowG" markerWidth="8" markerHeight="8" refX="6" refY="3" orient="auto">
      <path d="M0,0 L0,6 L8,3 z" fill="#5DCAA5"/>
    </marker>
    <marker id="arrowB" markerWidth="8" markerHeight="8" refX="6" refY="3" orient="auto">
      <path d="M0,0 L0,6 L8,3 z" fill="#378ADD"/>
    </marker>
    <marker id="arrowP" markerWidth="8" markerHeight="8" refX="6" refY="3" orient="auto">
      <path d="M0,0 L0,6 L8,3 z" fill="#7F77DD"/>
    </marker>
    <marker id="arrowO" markerWidth="8" markerHeight="8" refX="6" refY="3" orient="auto">
      <path d="M0,0 L0,6 L8,3 z" fill="#EF9F27"/>
    </marker>
    <filter id="softGlow">
      <feGaussianBlur stdDeviation="2" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <rect width="860" height="520" rx="16" fill="url(#stageBg)" stroke="#1e2433" stroke-width="1"/>

  <!-- Title -->
  <text x="430" y="32" font-family="'Segoe UI',sans-serif" font-size="15" font-weight="700" text-anchor="middle" fill="#e2e8f0" letter-spacing="2">END-TO-END PIPELINE</text>
  <line x1="160" y1="42" x2="700" y2="42" stroke="#2d3748" stroke-width="1"/>

  <!-- STAGE 1: DATA INGESTION -->
  <rect x="30" y="58" width="800" height="72" rx="10" fill="#0d1f12" stroke="#5DCAA5" stroke-width="1.5"/>
  <rect x="30" y="58" width="5" height="72" rx="3" fill="#5DCAA5"/>
  <text x="58" y="82" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" fill="#5DCAA5" letter-spacing="1">STAGE 1 · DATA INGESTION</text>
  <!-- 3 dataset pills -->
  <rect x="58" y="92" width="180" height="28" rx="6" fill="#0a2d1a" stroke="#5DCAA5" stroke-width="1"/>
  <text x="148" y="111" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#5DCAA5">🩸 Diabetes-Large (100k)</text>
  <rect x="254" y="92" width="180" height="28" rx="6" fill="#0a2d1a" stroke="#5DCAA5" stroke-width="1"/>
  <text x="344" y="111" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#5DCAA5">❤️ Heart-Cleveland (297)</text>
  <rect x="450" y="92" width="180" height="28" rx="6" fill="#0a2d1a" stroke="#5DCAA5" stroke-width="1"/>
  <text x="540" y="111" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#5DCAA5">🧬 Pima Diabetes (768)</text>
  <text x="680" y="99" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">target → 0/1</text>
  <text x="680" y="115" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">normalized</text>

  <!-- Arrow 1→2 -->
  <line x1="430" y1="130" x2="430" y2="150" stroke="#5DCAA5" stroke-width="2" marker-end="url(#arrowG)"/>

  <!-- STAGE 2: PREPROCESSING -->
  <rect x="30" y="152" width="800" height="72" rx="10" fill="#0d1a2a" stroke="#378ADD" stroke-width="1.5"/>
  <rect x="30" y="152" width="5" height="72" rx="3" fill="#378ADD"/>
  <text x="58" y="176" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" fill="#378ADD" letter-spacing="1">STAGE 2 · PREPROCESSING</text>
  <rect x="58" y="186" width="140" height="28" rx="6" fill="#0a1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="128" y="205" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#378ADD">Zero Imputation</text>
  <rect x="210" y="186" width="140" height="28" rx="6" fill="#0a1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="280" y="205" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#378ADD">Label Encoding</text>
  <rect x="362" y="186" width="140" height="28" rx="6" fill="#0a1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="432" y="205" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#378ADD">StandardScaler</text>
  <rect x="514" y="186" width="140" height="28" rx="6" fill="#0a1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="584" y="205" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#378ADD">SMOTE Balance</text>
  <rect x="666" y="186" width="148" height="28" rx="6" fill="#0a1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="740" y="205" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#378ADD">80/20 Stratified Split</text>

  <!-- Arrow 2→3 -->
  <line x1="430" y1="224" x2="430" y2="244" stroke="#378ADD" stroke-width="2" marker-end="url(#arrowB)"/>

  <!-- STAGE 3: FEATURE ENGINEERING (Pima only) -->
  <rect x="30" y="246" width="800" height="58" rx="10" fill="#1a0d2a" stroke="#7F77DD" stroke-width="1.5"/>
  <rect x="30" y="246" width="5" height="58" rx="3" fill="#7F77DD"/>
  <text x="58" y="268" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" fill="#7F77DD" letter-spacing="1">STAGE 3 · FEATURE ENGINEERING  <tspan fill="#4a5568" font-weight="400">(Pima only · 8 → 16 features)</tspan></text>
  <rect x="58" y="276" width="110" height="20" rx="4" fill="#1a0a2d" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="113" y="290" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#7F77DD">glucose × BMI</text>
  <rect x="178" y="276" width="110" height="20" rx="4" fill="#1a0a2d" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="233" y="290" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#7F77DD">BP × Age</text>
  <rect x="298" y="276" width="110" height="20" rx="4" fill="#1a0a2d" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="353" y="290" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#7F77DD">Insulin Sensitivity</text>
  <rect x="418" y="276" width="110" height="20" rx="4" fill="#1a0a2d" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="473" y="290" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#7F77DD">WHO BMI Bins</text>
  <rect x="538" y="276" width="110" height="20" rx="4" fill="#1a0a2d" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="593" y="290" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#7F77DD">Glucose Bins</text>
  <rect x="658" y="276" width="156" height="20" rx="4" fill="#1a0a2d" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="736" y="290" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#7F77DD">+3 more interactions</text>

  <!-- Arrow 3→4 -->
  <line x1="430" y1="304" x2="430" y2="322" stroke="#7F77DD" stroke-width="2" marker-end="url(#arrowP)"/>

  <!-- STAGE 4: MODEL TRAINING -->
  <rect x="30" y="324" width="800" height="72" rx="10" fill="#1a1a0a" stroke="#EF9F27" stroke-width="1.5"/>
  <rect x="30" y="324" width="5" height="72" rx="3" fill="#EF9F27"/>
  <text x="58" y="348" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" fill="#EF9F27" letter-spacing="1">STAGE 4 · MODEL TRAINING + OPTUNA TUNING</text>
  <rect x="58" y="358" width="162" height="28" rx="6" fill="#1a1400" stroke="#EF9F27" stroke-width="1"/>
  <text x="139" y="377" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#EF9F27">Logistic Regression</text>
  <rect x="232" y="358" width="162" height="28" rx="6" fill="#1a1400" stroke="#EF9F27" stroke-width="1"/>
  <text x="313" y="377" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#EF9F27">Random Forest</text>
  <rect x="406" y="358" width="162" height="28" rx="6" fill="#1a1400" stroke="#EF9F27" stroke-width="1"/>
  <text x="487" y="377" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#EF9F27">XGBoost (GPU)</text>
  <rect x="580" y="358" width="162" height="28" rx="6" fill="#1a1400" stroke="#EF9F27" stroke-width="1"/>
  <text x="661" y="377" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#EF9F27">LightGBM</text>

  <!-- Arrow 4→5 -->
  <line x1="430" y1="396" x2="430" y2="414" stroke="#EF9F27" stroke-width="2" marker-end="url(#arrowO)"/>

  <!-- STAGE 5: DEPLOYMENT -->
  <rect x="30" y="416" width="800" height="58" rx="10" fill="#1a0d12" stroke="#D85A30" stroke-width="1.5"/>
  <rect x="30" y="416" width="5" height="58" rx="3" fill="#D85A30"/>
  <text x="58" y="438" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" fill="#D85A30" letter-spacing="1">STAGE 5 · EVALUATION + GRADIO DEPLOYMENT</text>
  <rect x="58" y="446" width="150" height="20" rx="4" fill="#2d0a0a" stroke="#D85A30" stroke-width="0.8"/>
  <text x="133" y="460" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#D85A30">ROC-AUC · F1 · Sens/Spec</text>
  <rect x="222" y="446" width="150" height="20" rx="4" fill="#2d0a0a" stroke="#D85A30" stroke-width="0.8"/>
  <text x="297" y="460" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#D85A30">Confusion Matrices</text>
  <rect x="386" y="446" width="150" height="20" rx="4" fill="#2d0a0a" stroke="#D85A30" stroke-width="0.8"/>
  <text x="461" y="460" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#D85A30">Feature Importance</text>
  <rect x="550" y="446" width="150" height="20" rx="4" fill="#2d0a0a" stroke="#D85A30" stroke-width="0.8"/>
  <text x="625" y="460" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#D85A30">3-Tab Gradio App</text>
  <rect x="714" y="446" width="106" height="20" rx="4" fill="#2d0a0a" stroke="#D85A30" stroke-width="0.8"/>
  <text x="767" y="460" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#D85A30">Public Live Link</text>

  <!-- Animated flow line -->
  <line x1="35" y1="500" x2="825" y2="500" stroke="#1e2433" stroke-width="1"/>
  <rect x="35" y="497" width="60" height="6" rx="3" fill="#5DCAA5" opacity="0.7">
    <animate attributeName="x" values="35;765;35" dur="4s" repeatCount="indefinite"/>
  </rect>
  <text x="430" y="515" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#4a5568">data flows through pipeline · 5 stages · end-to-end reproducible</text>
</svg>

</div>

---

## 📊 Model Performance

<div align="center">

<svg width="860" height="320" viewBox="0 0 860 320" xmlns="http://www.w3.org/2000/svg">
  <rect width="860" height="320" rx="14" fill="#0a0d14" stroke="#1e2433" stroke-width="1"/>
  <text x="430" y="28" font-family="'Segoe UI',sans-serif" font-size="14" font-weight="700" text-anchor="middle" fill="#e2e8f0" letter-spacing="1">LEADERBOARD · ALL MODELS · ALL DATASETS</text>
  <line x1="40" y1="38" x2="820" y2="38" stroke="#1e2433" stroke-width="1"/>

  <!-- Header row -->
  <rect x="40" y="48" width="780" height="26" rx="4" fill="#111827"/>
  <text x="120" y="66" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" text-anchor="middle" fill="#718096" letter-spacing="1">DATASET</text>
  <text x="270" y="66" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" text-anchor="middle" fill="#718096" letter-spacing="1">MODEL</text>
  <text x="420" y="66" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" text-anchor="middle" fill="#718096" letter-spacing="1">ROC-AUC</text>
  <text x="520" y="66" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" text-anchor="middle" fill="#718096" letter-spacing="1">F1</text>
  <text x="620" y="66" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" text-anchor="middle" fill="#718096" letter-spacing="1">SENSITIVITY</text>
  <text x="740" y="66" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" text-anchor="middle" fill="#718096" letter-spacing="1">SPECIFICITY</text>

  <!-- Row 1 - winner -->
  <rect x="40" y="80" width="780" height="30" rx="4" fill="#0d2a0d" stroke="#5DCAA5" stroke-width="0.5"/>
  <text x="52" y="100" font-family="'Segoe UI',sans-serif" font-size="10" fill="#EF9F27">🏆</text>
  <text x="120" y="100" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#5DCAA5" font-weight="600">Diabetes-Large</text>
  <text x="270" y="100" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#e2e8f0">LightGBM</text>
  <!-- AUC bar -->
  <rect x="370" y="88" width="97.9" height="14" rx="3" fill="#5DCAA5" opacity="0.85"/>
  <text x="478" y="100" font-family="'Segoe UI',sans-serif" font-size="11" fill="#5DCAA5" font-weight="700">0.979</text>
  <rect x="490" y="88" width="80.4" height="14" rx="3" fill="#378ADD" opacity="0.7"/>
  <text x="577" y="100" font-family="'Segoe UI',sans-serif" font-size="11" fill="#378ADD">0.804</text>
  <rect x="588" y="88" width="70.9" height="14" rx="3" fill="#7F77DD" opacity="0.7"/>
  <text x="664" y="100" font-family="'Segoe UI',sans-serif" font-size="11" fill="#7F77DD">0.709</text>
  <rect x="690" y="88" width="99.5" height="14" rx="3" fill="#EF9F27" opacity="0.7"/>
  <text x="795" y="100" font-family="'Segoe UI',sans-serif" font-size="11" fill="#EF9F27">0.995</text>

  <!-- Row 2 -->
  <rect x="40" y="116" width="780" height="30" rx="4" fill="#111827"/>
  <text x="120" y="136" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#5DCAA5">Diabetes-Large</text>
  <text x="270" y="136" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#e2e8f0">XGBoost</text>
  <rect x="370" y="124" width="97.8" height="14" rx="3" fill="#5DCAA5" opacity="0.55"/>
  <text x="478" y="136" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.978</text>
  <rect x="490" y="124" width="78" height="14" rx="3" fill="#378ADD" opacity="0.5"/>
  <text x="577" y="136" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.780</text>
  <rect x="588" y="124" width="76.2" height="14" rx="3" fill="#7F77DD" opacity="0.5"/>
  <text x="664" y="136" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.762</text>
  <rect x="690" y="124" width="98.2" height="14" rx="3" fill="#EF9F27" opacity="0.5"/>
  <text x="795" y="136" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.982</text>

  <!-- Row 3 - winner -->
  <rect x="40" y="152" width="780" height="30" rx="4" fill="#0a1a2d" stroke="#378ADD" stroke-width="0.5"/>
  <text x="52" y="172" font-family="'Segoe UI',sans-serif" font-size="10" fill="#EF9F27">🏆</text>
  <text x="120" y="172" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#378ADD" font-weight="600">Heart-Cleveland</text>
  <text x="270" y="172" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#e2e8f0">Logistic Regression</text>
  <rect x="370" y="160" width="95.4" height="14" rx="3" fill="#378ADD" opacity="0.85"/>
  <text x="478" y="172" font-family="'Segoe UI',sans-serif" font-size="11" fill="#378ADD" font-weight="700">0.954</text>
  <rect x="490" y="160" width="90.2" height="14" rx="3" fill="#378ADD" opacity="0.7"/>
  <text x="577" y="172" font-family="'Segoe UI',sans-serif" font-size="11" fill="#378ADD">0.902</text>
  <rect x="588" y="160" width="82.1" height="14" rx="3" fill="#7F77DD" opacity="0.7"/>
  <text x="664" y="172" font-family="'Segoe UI',sans-serif" font-size="11" fill="#7F77DD">0.821</text>
  <rect x="690" y="160" width="100" height="14" rx="3" fill="#EF9F27" opacity="0.9"/>
  <text x="795" y="172" font-family="'Segoe UI',sans-serif" font-size="11" fill="#EF9F27" font-weight="700">1.000</text>

  <!-- Row 4 -->
  <rect x="40" y="188" width="780" height="30" rx="4" fill="#111827"/>
  <text x="120" y="208" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#378ADD">Heart-Cleveland</text>
  <text x="270" y="208" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#e2e8f0">LightGBM</text>
  <rect x="370" y="196" width="94.9" height="14" rx="3" fill="#378ADD" opacity="0.55"/>
  <text x="478" y="208" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.949</text>
  <rect x="490" y="196" width="85.2" height="14" rx="3" fill="#378ADD" opacity="0.5"/>
  <text x="577" y="208" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.852</text>
  <rect x="588" y="196" width="82.1" height="14" rx="3" fill="#7F77DD" opacity="0.5"/>
  <text x="664" y="208" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.821</text>
  <rect x="690" y="196" width="90.6" height="14" rx="3" fill="#EF9F27" opacity="0.5"/>
  <text x="795" y="208" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.906</text>

  <!-- Row 5 - winner -->
  <rect x="40" y="224" width="780" height="30" rx="4" fill="#1a0d2a" stroke="#7F77DD" stroke-width="0.5"/>
  <text x="52" y="244" font-family="'Segoe UI',sans-serif" font-size="10" fill="#EF9F27">🏆</text>
  <text x="120" y="244" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#7F77DD" font-weight="600">Diabetes-Pima</text>
  <text x="270" y="244" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#e2e8f0">XGBoost (tuned)</text>
  <rect x="370" y="232" width="83.8" height="14" rx="3" fill="#7F77DD" opacity="0.85"/>
  <text x="478" y="244" font-family="'Segoe UI',sans-serif" font-size="11" fill="#7F77DD" font-weight="700">0.838</text>
  <rect x="490" y="232" width="64.9" height="14" rx="3" fill="#7F77DD" opacity="0.7"/>
  <text x="577" y="244" font-family="'Segoe UI',sans-serif" font-size="11" fill="#7F77DD">0.649</text>
  <rect x="588" y="232" width="68.5" height="14" rx="3" fill="#7F77DD" opacity="0.7"/>
  <text x="664" y="244" font-family="'Segoe UI',sans-serif" font-size="11" fill="#7F77DD">0.685</text>
  <rect x="690" y="232" width="77" height="14" rx="3" fill="#EF9F27" opacity="0.7"/>
  <text x="795" y="244" font-family="'Segoe UI',sans-serif" font-size="11" fill="#EF9F27">0.770</text>

  <!-- Row 6 -->
  <rect x="40" y="260" width="780" height="30" rx="4" fill="#111827"/>
  <text x="120" y="280" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#7F77DD">Diabetes-Pima</text>
  <text x="270" y="280" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#e2e8f0">LightGBM</text>
  <rect x="370" y="268" width="81.6" height="14" rx="3" fill="#7F77DD" opacity="0.55"/>
  <text x="478" y="280" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.816</text>
  <rect x="490" y="268" width="63.7" height="14" rx="3" fill="#7F77DD" opacity="0.5"/>
  <text x="577" y="280" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.637</text>
  <rect x="588" y="268" width="66.7" height="14" rx="3" fill="#7F77DD" opacity="0.5"/>
  <text x="664" y="280" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.667</text>
  <rect x="690" y="268" width="77" height="14" rx="3" fill="#EF9F27" opacity="0.5"/>
  <text x="795" y="280" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">0.770</text>

  <!-- Legend -->
  <rect x="370" y="300" width="12" height="10" rx="2" fill="#5DCAA5"/>
  <text x="386" y="310" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">ROC-AUC</text>
  <rect x="460" y="300" width="12" height="10" rx="2" fill="#378ADD"/>
  <text x="476" y="310" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">F1</text>
  <rect x="510" y="300" width="12" height="10" rx="2" fill="#7F77DD"/>
  <text x="526" y="310" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">Sensitivity</text>
  <rect x="610" y="300" width="12" height="10" rx="2" fill="#EF9F27"/>
  <text x="626" y="310" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">Specificity</text>
  <text x="52" y="310" font-family="'Segoe UI',sans-serif" font-size="10" fill="#4a5568">🏆 = best per dataset (by AUC) · bar width proportional to score</text>
</svg>

</div>

---

## ⚙️ Tech Stack

<div align="center">

<svg width="860" height="130" viewBox="0 0 860 130" xmlns="http://www.w3.org/2000/svg">
  <rect width="860" height="130" rx="12" fill="#0a0d14" stroke="#1e2433" stroke-width="1"/>

  <!-- Category: Data -->
  <text x="80" y="24" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096" letter-spacing="1">DATA</text>
  <rect x="20" y="32" width="120" height="28" rx="6" fill="#0d2a1a" stroke="#5DCAA5" stroke-width="1"/>
  <text x="80" y="51" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#5DCAA5">pandas · numpy</text>
  <rect x="20" y="66" width="120" height="28" rx="6" fill="#0d2a1a" stroke="#5DCAA5" stroke-width="1"/>
  <text x="80" y="85" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#5DCAA5">imbalanced-learn</text>
  <rect x="20" y="100" width="120" height="24" rx="6" fill="#0d2a1a" stroke="#5DCAA5" stroke-width="1"/>
  <text x="80" y="117" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#5DCAA5">SMOTE</text>

  <!-- Divider -->
  <line x1="158" y1="20" x2="158" y2="120" stroke="#1e2433" stroke-width="1"/>

  <!-- Category: ML -->
  <text x="290" y="24" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096" letter-spacing="1">MACHINE LEARNING</text>
  <rect x="168" y="32" width="120" height="28" rx="6" fill="#0d1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="228" y="51" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#378ADD">scikit-learn</text>
  <rect x="298" y="32" width="120" height="28" rx="6" fill="#0d1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="358" y="51" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#378ADD">XGBoost (GPU)</text>
  <rect x="168" y="66" width="120" height="28" rx="6" fill="#0d1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="228" y="85" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#378ADD">LightGBM</text>
  <rect x="298" y="66" width="120" height="28" rx="6" fill="#0d1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="358" y="85" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#378ADD">Optuna (TPE)</text>
  <rect x="168" y="100" width="250" height="24" rx="6" fill="#0d1a2d" stroke="#378ADD" stroke-width="1"/>
  <text x="293" y="117" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#378ADD">StackingClassifier · 5-fold CV</text>

  <!-- Divider -->
  <line x1="436" y1="20" x2="436" y2="120" stroke="#1e2433" stroke-width="1"/>

  <!-- Category: Viz -->
  <text x="546" y="24" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096" letter-spacing="1">VISUALIZATION</text>
  <rect x="446" y="32" width="120" height="28" rx="6" fill="#1a0d2a" stroke="#7F77DD" stroke-width="1"/>
  <text x="506" y="51" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#7F77DD">matplotlib</text>
  <rect x="576" y="32" width="120" height="28" rx="6" fill="#1a0d2a" stroke="#7F77DD" stroke-width="1"/>
  <text x="636" y="51" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#7F77DD">seaborn</text>
  <rect x="446" y="66" width="250" height="28" rx="6" fill="#1a0d2a" stroke="#7F77DD" stroke-width="1"/>
  <text x="571" y="85" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#7F77DD">ROC · Confusion · Heatmaps</text>
  <rect x="446" y="100" width="250" height="24" rx="6" fill="#1a0d2a" stroke="#7F77DD" stroke-width="1"/>
  <text x="571" y="117" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#7F77DD">Feature Importance · KDE Dist.</text>

  <!-- Divider -->
  <line x1="714" y1="20" x2="714" y2="120" stroke="#1e2433" stroke-width="1"/>

  <!-- Category: Deploy -->
  <text x="787" y="24" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096" letter-spacing="1">DEPLOYMENT</text>
  <rect x="724" y="32" width="120" height="28" rx="6" fill="#2d0a0a" stroke="#D85A30" stroke-width="1"/>
  <text x="784" y="51" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#D85A30">Gradio</text>
  <rect x="724" y="66" width="120" height="28" rx="6" fill="#2d0a0a" stroke="#D85A30" stroke-width="1"/>
  <text x="784" y="85" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#D85A30">Kaggle GPU P100</text>
  <rect x="724" y="100" width="120" height="24" rx="6" fill="#2d0a0a" stroke="#D85A30" stroke-width="1"/>
  <text x="784" y="117" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#D85A30">Public Share Link</text>
</svg>

</div>

---

## 🗺️ Repository Structure

```
medrisk-classifier/
│
├── 📓 medrisk_classifier.ipynb     ← Main Kaggle notebook (all 5 snippets)
│
├── 📊 outputs/
│   ├── class_balance.png           ← EDA: class distribution across datasets
│   ├── dist_*.png                  ← KDE feature distributions per dataset
│   ├── corr_*.png                  ← Correlation heatmaps
│   ├── smote_balance.png           ← Before/after SMOTE comparison
│   ├── target_correlation.png      ← Pearson r with target per dataset
│   ├── metrics_heatmap.png         ← All models × all metrics
│   ├── roc_curves.png              ← ROC curves overlaid per dataset
│   ├── confusion_matrices.png      ← Best model per dataset
│   ├── feature_importance.png      ← RF + LightGBM importance
│   ├── tuned_vs_baseline.png       ← Optuna improvement
│   ├── optuna_history.png          ← Trial convergence plots
│   ├── pima_progression.png        ← Baseline → Engineered → Stacked
│   └── pima_feature_importance_eng.png
│
└── 📄 README.md
```

---

## 🚀 Reproduce Locally

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/medrisk-classifier.git
cd medrisk-classifier

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn \
            imbalanced-learn xgboost lightgbm optuna gradio

# 3. Add datasets (Kaggle API)
kaggle datasets download iammustafatz/diabetes-prediction-dataset
kaggle datasets download cherngs/heart-disease-cleveland-uci
kaggle datasets download -d uciml/pima-indians-diabetes-database

# 4. Run on Kaggle (recommended — free GPU)
#    Upload the notebook and enable GPU accelerator
#    Run All → Gradio link appears in the last cell output
```

---

## 🧪 Feature Engineering Details

<div align="center">

<svg width="860" height="260" viewBox="0 0 860 260" xmlns="http://www.w3.org/2000/svg">
  <rect width="860" height="260" rx="12" fill="#0a0d14" stroke="#1e2433" stroke-width="1"/>
  <text x="430" y="26" font-family="'Segoe UI',sans-serif" font-size="13" font-weight="700" text-anchor="middle" fill="#7F77DD" letter-spacing="1">PIMA FEATURE ENGINEERING  ·  8 → 16 FEATURES</text>

  <!-- Original features box -->
  <rect x="20" y="40" width="180" height="205" rx="10" fill="#1a0d2a" stroke="#7F77DD" stroke-width="1.5"/>
  <text x="110" y="60" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" text-anchor="middle" fill="#7F77DD">ORIGINAL (8)</text>
  <text x="35" y="80" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">Pregnancies</text>
  <text x="35" y="98" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">Glucose</text>
  <text x="35" y="116" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">BloodPressure</text>
  <text x="35" y="134" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">SkinThickness</text>
  <text x="35" y="152" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">Insulin</text>
  <text x="35" y="170" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">BMI</text>
  <text x="35" y="188" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">DiabetesPedigreeFunc</text>
  <text x="35" y="206" font-family="'Segoe UI',sans-serif" font-size="11" fill="#a0aec0">Age</text>
  <!-- zero fix note -->
  <rect x="30" y="216" width="160" height="20" rx="4" fill="#2d0a0a" stroke="#D85A30" stroke-width="0.8"/>
  <text x="110" y="230" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#D85A30">⚠ zeros → median imputed</text>

  <!-- Arrow -->
  <text x="215" y="142" font-family="'Segoe UI',sans-serif" font-size="22" fill="#7F77DD">→</text>

  <!-- Engineered features box -->
  <rect x="240" y="40" width="600" height="205" rx="10" fill="#0d0a1a" stroke="#7F77DD" stroke-width="1.5"/>
  <text x="540" y="60" font-family="'Segoe UI',sans-serif" font-size="11" font-weight="700" text-anchor="middle" fill="#7F77DD">ENGINEERED (8 new · clinical rationale)</text>

  <!-- 8 new feature cards, 2 columns -->
  <rect x="256" y="70" width="274" height="40" rx="6" fill="#1a0d2a" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="393" y="86" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#e2e8f0" font-weight="600">glucose_bmi</text>
  <text x="393" y="102" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096">Glucose × BMI · insulin resistance proxy</text>

  <rect x="550" y="70" width="274" height="40" rx="6" fill="#1a0d2a" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="687" y="86" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#e2e8f0" font-weight="600">bp_age</text>
  <text x="687" y="102" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096">BloodPressure × Age · cardiovascular stress</text>

  <rect x="256" y="118" width="274" height="40" rx="6" fill="#1a0d2a" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="393" y="134" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#e2e8f0" font-weight="600">glucose_bmi_ratio</text>
  <text x="393" y="150" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096">Glucose / BMI · thin + high glucose risk</text>

  <rect x="550" y="118" width="274" height="40" rx="6" fill="#1a0d2a" stroke="#7F77DD" stroke-width="0.8"/>
  <text x="687" y="134" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#e2e8f0" font-weight="600">insulin_glucose</text>
  <text x="687" y="150" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096">Insulin / Glucose · sensitivity ratio</text>

  <rect x="256" y="166" width="274" height="40" rx="6" fill="#1a0d2a" stroke="#5DCAA5" stroke-width="0.8"/>
  <text x="393" y="182" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#e2e8f0" font-weight="600">bmi_bin</text>
  <text x="393" y="198" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096">WHO categories: under/normal/over/obese</text>

  <rect x="550" y="166" width="274" height="40" rx="6" fill="#1a0d2a" stroke="#5DCAA5" stroke-width="0.8"/>
  <text x="687" y="182" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#e2e8f0" font-weight="600">glucose_bin</text>
  <text x="687" y="198" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096">Clinical: normal / pre-diabetic / diabetic</text>

  <!-- AUC improvement tag -->
  <rect x="350" y="218" width="380" height="20" rx="6" fill="#0d2a0d" stroke="#5DCAA5" stroke-width="0.8"/>
  <text x="540" y="232" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#5DCAA5">📈 AUC improvement: 0.823 (baseline) → 0.838 (engineered) · +1.8%</text>
</svg>

</div>

---

## 🎛️ Gradio App — Interface Preview

<div align="center">

<svg width="860" height="300" viewBox="0 0 860 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="appBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0f0c29"/>
      <stop offset="100%" style="stop-color:#1a1040"/>
    </linearGradient>
  </defs>
  <rect width="860" height="300" rx="14" fill="url(#appBg)" stroke="#302b63" stroke-width="1.5"/>

  <!-- Browser chrome -->
  <rect x="0" y="0" width="860" height="36" rx="14" fill="#1a1535"/>
  <rect x="0" y="24" width="860" height="12" fill="#1a1535"/>
  <circle cx="22" cy="18" r="6" fill="#D85A30" opacity="0.8"/>
  <circle cx="40" cy="18" r="6" fill="#EF9F27" opacity="0.8"/>
  <circle cx="58" cy="18" r="6" fill="#5DCAA5" opacity="0.8"/>
  <rect x="100" y="10" width="480" height="16" rx="8" fill="#0d0a1a"/>
  <text x="340" y="22" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#718096">🔒 kaggle.com/your-notebook · MedRisk Classifier</text>

  <!-- Tab bar -->
  <rect x="20" y="46" width="200" height="28" rx="6" fill="#5DCAA5" opacity="0.15" stroke="#5DCAA5" stroke-width="1"/>
  <text x="120" y="65" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#5DCAA5" font-weight="600">🩸 Diabetes Risk (Large)</text>
  <rect x="230" y="46" width="180" height="28" rx="6" fill="none" stroke="#378ADD" stroke-width="0.5"/>
  <text x="320" y="65" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#718096">❤️ Heart Disease Risk</text>
  <rect x="420" y="46" width="180" height="28" rx="6" fill="none" stroke="#7F77DD" stroke-width="0.5"/>
  <text x="510" y="65" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#718096">🧬 Diabetes Risk (Pima)</text>

  <!-- Model badge -->
  <rect x="640" y="46" width="200" height="28" rx="6" fill="#0d2a0d" stroke="#5DCAA5" stroke-width="0.5"/>
  <text x="740" y="65" font-family="'Segoe UI',sans-serif" font-size="10" text-anchor="middle" fill="#5DCAA5">Model: LightGBM · AUC: 0.979</text>

  <!-- Left panel: inputs -->
  <text x="30" y="100" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">Gender</text>
  <rect x="30" y="106" width="180" height="20" rx="4" fill="#1a1535" stroke="#302b63" stroke-width="1"/>
  <text x="40" y="120" font-family="'Segoe UI',sans-serif" font-size="10" fill="#e2e8f0">Female</text>
  <text x="195" y="120" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">▾</text>

  <text x="30" y="138" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">Age  <tspan fill="#5DCAA5">45</tspan></text>
  <rect x="30" y="144" width="180" height="8" rx="4" fill="#1a1535" stroke="#302b63" stroke-width="1"/>
  <rect x="30" y="144" width="90" height="8" rx="4" fill="#5DCAA5" opacity="0.6"/>
  <circle cx="120" cy="148" r="6" fill="#5DCAA5"/>

  <text x="30" y="168" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">BMI  <tspan fill="#5DCAA5">27.0</tspan></text>
  <rect x="30" y="174" width="180" height="8" rx="4" fill="#1a1535" stroke="#302b63" stroke-width="1"/>
  <rect x="30" y="174" width="70" height="8" rx="4" fill="#5DCAA5" opacity="0.6"/>
  <circle cx="100" cy="178" r="6" fill="#5DCAA5"/>

  <text x="30" y="198" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">HbA1c  <tspan fill="#5DCAA5">5.5%</tspan></text>
  <rect x="30" y="204" width="180" height="8" rx="4" fill="#1a1535" stroke="#302b63" stroke-width="1"/>
  <rect x="30" y="204" width="50" height="8" rx="4" fill="#5DCAA5" opacity="0.6"/>
  <circle cx="80" cy="208" r="6" fill="#5DCAA5"/>

  <text x="30" y="228" font-family="'Segoe UI',sans-serif" font-size="10" fill="#718096">Blood Glucose  <tspan fill="#5DCAA5">100 mg/dL</tspan></text>
  <rect x="30" y="234" width="180" height="8" rx="4" fill="#1a1535" stroke="#302b63" stroke-width="1"/>
  <rect x="30" y="234" width="40" height="8" rx="4" fill="#5DCAA5" opacity="0.6"/>
  <circle cx="70" cy="238" r="6" fill="#5DCAA5"/>

  <!-- Checkbox row -->
  <rect x="30" y="254" width="12" height="12" rx="2" fill="#0d2a0d" stroke="#5DCAA5" stroke-width="1"/>
  <text x="47" y="264" font-family="'Segoe UI',sans-serif" font-size="10" fill="#a0aec0">Hypertension</text>
  <rect x="150" y="254" width="12" height="12" rx="2" fill="#0d2a0d" stroke="#5DCAA5" stroke-width="1"/>
  <text x="167" y="264" font-family="'Segoe UI',sans-serif" font-size="10" fill="#a0aec0">Heart Disease</text>

  <!-- Predict button -->
  <rect x="30" y="272" width="180" height="22" rx="8" fill="#5DCAA5"/>
  <text x="120" y="287" font-family="'Segoe UI',sans-serif" font-size="12" text-anchor="middle" fill="#0a1a14" font-weight="700">🔍 Predict</text>

  <!-- Separator -->
  <line x1="230" y1="80" x2="230" y2="295" stroke="#302b63" stroke-width="1"/>

  <!-- Right panel: output -->
  <rect x="250" y="86" width="590" height="200" rx="12" fill="#0d0a1a" stroke="#302b63" stroke-width="1"/>

  <!-- Risk output card -->
  <rect x="350" y="110" width="390" height="150" rx="12" fill="#0d2a0d" stroke="#5DCAA5" stroke-width="2"/>
  <text x="545" y="148" font-family="'Segoe UI',sans-serif" font-size="18" text-anchor="middle" fill="#5DCAA5" font-weight="800">🟢 Low Risk</text>
  <text x="545" y="190" font-family="'Segoe UI',sans-serif" font-size="36" text-anchor="middle" fill="#5DCAA5" font-weight="800">12.4%</text>
  <text x="545" y="218" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#718096">Estimated disease probability</text>
  <text x="545" y="248" font-family="'Segoe UI',sans-serif" font-size="9" text-anchor="middle" fill="#4a5568">⚠️ For informational purposes only. Consult a medical professional.</text>

  <!-- Risk legend -->
  <circle cx="268" cy="106" r="6" fill="#5DCAA5"/>
  <text x="280" y="110" font-family="'Segoe UI',sans-serif" font-size="10" fill="#a0aec0">Low (&lt;20%)</text>
  <circle cx="268" cy="126" r="6" fill="#EF9F27"/>
  <text x="280" y="130" font-family="'Segoe UI',sans-serif" font-size="10" fill="#a0aec0">Moderate (20–50%)</text>
  <circle cx="268" cy="146" r="6" fill="#D85A30"/>
  <text x="280" y="150" font-family="'Segoe UI',sans-serif" font-size="10" fill="#a0aec0">High (&gt;50%)</text>

  <!-- Animated pulse on output -->
  <circle cx="545" cy="190" r="80" fill="none" stroke="#5DCAA5" stroke-width="1" opacity="0">
    <animate attributeName="r" values="60;90;60" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0;0.3" dur="2s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>

---

## 📈 Results Interpretation

<div align="center">

| Dataset | Key Insight |
|---|---|
| 🩸 **Diabetes-Large** | LightGBM and XGBoost tie at AUC=0.978/0.979. High specificity (0.995) means very few false alarms. HbA1c and blood glucose are dominant features by a large margin. |
| ❤️ **Heart-Cleveland** | Logistic Regression outperforms tree models — evidence that the decision boundary is approximately linear for this dataset. Specificity=1.0 means zero false positives on the test set. Small dataset (237 train rows) favors simpler models. |
| 🧬 **Diabetes-Pima** | Hardest dataset — 1988 data, many imputed zeros, noisy features. Feature engineering lifted AUC from 0.823 → 0.838. Glucose and BMI dominate importance. Insulin has lower importance than expected due to 374 original zero values. |

</div>

---

## 📝 Citation

If you use this project or find it helpful, please cite:

```bibtex
@misc{medrisk2025,
  title   = {MedRisk Classifier: A Generalizable ML Pipeline for Chronic Disease Prediction},
  author  = {YOUR NAME},
  year    = {2025},
  url     = {https://github.com/YOUR_USERNAME/medrisk-classifier},
  note    = {Trained on Kaggle GPU · Gradio deployed}
}
```

---

<div align="center">

<svg width="860" height="60" viewBox="0 0 860 60" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="footerGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#5DCAA5;stop-opacity:0"/>
      <stop offset="30%" style="stop-color:#5DCAA5"/>
      <stop offset="70%" style="stop-color:#7F77DD"/>
      <stop offset="100%" style="stop-color:#7F77DD;stop-opacity:0"/>
    </linearGradient>
  </defs>
  <rect height="1" width="860" y="0" fill="url(#footerGrad)"/>
  <text x="430" y="28" font-family="'Segoe UI',sans-serif" font-size="13" text-anchor="middle" fill="#718096">Built with ❤️ for open-source medical AI · All models trained on free, public datasets</text>
  <text x="430" y="50" font-family="'Segoe UI',sans-serif" font-size="11" text-anchor="middle" fill="#4a5568">MIT License · Contributions welcome · Star ⭐ if this helped you</text>
</svg>

</div>
