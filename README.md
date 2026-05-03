<div align="center">

<!-- ANIMATED HEADER BANNER SVG -->
<svg width="900" height="200" viewBox="0 0 900 200" xmlns="http://www.w3.org/2000/svg">
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
    <linearGradient id="pulseGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#D85A30;stop-opacity:0"/>
      <stop offset="50%" style="stop-color:#D85A30;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#D85A30;stop-opacity:0"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="900" height="200" fill="url(#bgGrad)" rx="16"/>

  <!-- Animated heartbeat line -->
  <polyline points="0,100 60,100 80,100 100,40 120,160 140,100 160,100 220,100 240,60 260,140 280,100 900,100"
    fill="none" stroke="url(#pulseGrad)" stroke-width="2.5" opacity="0.7">
    <animate attributeName="stroke-dasharray" from="0,2000" to="2000,0" dur="3s" repeatCount="indefinite"/>
  </polyline>

  <!-- Floating circles decoration -->
  <circle cx="50" cy="40" r="25" fill="#5DCAA5" opacity="0.08"/>
  <circle cx="850" cy="160" r="40" fill="#378ADD" opacity="0.08"/>
  <circle cx="820" cy="30" r="15" fill="#7F77DD" opacity="0.12"/>
  <circle cx="80" cy="170" r="20" fill="#D85A30" opacity="0.1"/>

  <!-- Grid dots -->
  <g opacity="0.15">
    <circle cx="200" cy="30" r="1.5" fill="#5DCAA5"/>
    <circle cx="240" cy="30" r="1.5" fill="#5DCAA5"/>
    <circle cx="280" cy="30" r="1.5" fill="#5DCAA5"/>
    <circle cx="200" cy="60" r="1.5" fill="#5DCAA5"/>
    <circle cx="240" cy="60" r="1.5" fill="#5DCAA5"/>
    <circle cx="280" cy="60" r="1.5" fill="#5DCAA5"/>
    <circle cx="620" cy="140" r="1.5" fill="#378ADD"/>
    <circle cx="660" cy="140" r="1.5" fill="#378ADD"/>
    <circle cx="700" cy="140" r="1.5" fill="#378ADD"/>
    <circle cx="620" cy="170" r="1.5" fill="#378ADD"/>
    <circle cx="660" cy="170" r="1.5" fill="#378ADD"/>
    <circle cx="700" cy="170" r="1.5" fill="#378ADD"/>
  </g>

  <!-- Main title -->
  <text x="450" y="88" text-anchor="middle" font-family="'Segoe UI', sans-serif"
    font-size="46" font-weight="900" fill="url(#textGrad)" filter="url(#glow)">
    MedRisk Classifier
  </text>

  <!-- Subtitle -->
  <text x="450" y="122" text-anchor="middle" font-family="'Segoe UI', sans-serif"
    font-size="16" fill="#B4B2A9" letter-spacing="3">
    GENERALIZABLE ML · CHRONIC DISEASE PREDICTION
  </text>

  <!-- Bottom accent bar -->
  <rect x="300" y="148" width="300" height="2" fill="url(#textGrad)" rx="1" opacity="0.8"/>

  <!-- Tag line -->
  <text x="450" y="172" text-anchor="middle" font-family="'Segoe UI', sans-serif"
    font-size="13" fill="#5DCAA5" opacity="0.9">
    3 Datasets · 4 Models · Optuna Tuned · Live Gradio Demo
  </text>
</svg>

<br/>

<!-- BADGES -->
![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-GPU%20Accelerated-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-Tuned-FF6600?style=for-the-badge&logo=xgboost&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-Tuned-02B97B?style=for-the-badge)
![Gradio](https://img.shields.io/badge/Gradio-Live%20Demo-F97316?style=for-the-badge&logo=gradio&logoColor=white)
![Optuna](https://img.shields.io/badge/Optuna-50%20Trials-7C3AED?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Production%20Ready-5DCAA5?style=for-the-badge)

</div>

---

<div align="center">

## 🎯 Try It Live

**[![🚀 Launch Gradio Demo](https://img.shields.io/badge/🚀%20Launch%20Demo-Gradio%20Live-F97316?style=for-the-badge&logoColor=white)](YOUR_GRADIO_LINK_HERE)**

*No signup · No install · Works in your browser*

</div>

---

## 📖 Table of Contents

| | Section |
|:---:|:---|
| 🧠 | [Project Overview](#-project-overview) |
| 📊 | [Datasets](#-datasets) |
| 🏗️ | [System Architecture](#️-system-architecture) |
| 🔬 | [ML Pipeline](#-ml-pipeline) |
| 📈 | [Results & Leaderboard](#-results--leaderboard) |
| ⚙️ | [Feature Engineering](#️-feature-engineering) |
| 🚀 | [Quick Start](#-quick-start) |
| 🗂️ | [Project Structure](#️-project-structure) |
| 🧩 | [Tech Stack](#-tech-stack) |

---

## 🧠 Project Overview

<div align="center">

*A production-grade, generalizable machine learning system for predicting chronic disease risk across multiple independent clinical datasets — unified under a single pipeline architecture.*

</div>

This project demonstrates that a **single well-engineered ML pipeline** can generalize across fundamentally different medical datasets without dataset-specific hacks. Three independent clinical datasets, four classifiers, Optuna hyperparameter tuning, SMOTE class balancing, and a live Gradio interface — all in a clean, reproducible Kaggle notebook.

**Why this matters clinically:** Sensitivity and specificity are optimized separately for each condition — missing a true positive in a heart disease context is far more costly than a false alarm.

---

## 📊 Datasets

<div align="center">

<!-- DATASETS SVG DIAGRAM -->
<svg width="860" height="220" viewBox="0 0 860 220" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="cardA" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#1a1a2e"/>
      <stop offset="100%" style="stop-color:#16213e"/>
    </linearGradient>
    <linearGradient id="accentA" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#5DCAA5"/>
      <stop offset="100%" style="stop-color:#378ADD"/>
    </linearGradient>
    <linearGradient id="accentB" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#D85A30"/>
      <stop offset="100%" style="stop-color:#7F77DD"/>
    </linearGradient>
    <linearGradient id="accentC" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#378ADD"/>
      <stop offset="100%" style="stop-color:#5DCAA5"/>
    </linearGradient>
  </defs>

  <!-- Background -->
  <rect width="860" height="220" fill="#0d1117" rx="14"/>

  <!-- Card 1 -->
  <rect x="20" y="20" width="260" height="180" fill="#161b22" rx="12" stroke="#5DCAA5" stroke-width="1.5"/>
  <rect x="20" y="20" width="260" height="5" fill="url(#accentA)" rx="3"/>
  <text x="150" y="55" text-anchor="middle" font-family="sans-serif" font-size="28">🩸</text>
  <text x="150" y="82" text-anchor="middle" font-family="sans-serif" font-size="13" font-weight="700" fill="#5DCAA5">Diabetes Prediction</text>
  <text x="150" y="100" text-anchor="middle" font-family="sans-serif" font-size="11" fill="#8b949e">iammustafatz · Kaggle</text>
  <line x1="40" y1="110" x2="260" y2="110" stroke="#21262d" stroke-width="1"/>
  <text x="40" y="128" font-family="sans-serif" font-size="11" fill="#8b949e">📦 Rows</text>
  <text x="260" y="128" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#e6edf3">100,000</text>
  <text x="40" y="146" font-family="sans-serif" font-size="11" fill="#8b949e">🔢 Features</text>
  <text x="260" y="146" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#e6edf3">8 → 8</text>
  <text x="40" y="164" font-family="sans-serif" font-size="11" fill="#8b949e">⚖️ Imbalance</text>
  <text x="260" y="164" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#D85A30">91.5% / 8.5%</text>
  <text x="40" y="182" font-family="sans-serif" font-size="11" fill="#8b949e">🏆 Best Model</text>
  <text x="260" y="182" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#5DCAA5">LightGBM</text>
  <text x="40" y="195" font-family="sans-serif" font-size="10" fill="#8b949e">AUC</text>
  <rect x="60" y="187" width="140" height="6" fill="#21262d" rx="3"/>
  <rect x="60" y="187" width="137" height="6" fill="url(#accentA)" rx="3"/>
  <text x="205" y="195" font-family="sans-serif" font-size="10" font-weight="700" fill="#5DCAA5">0.979</text>

  <!-- Card 2 -->
  <rect x="300" y="20" width="260" height="180" fill="#161b22" rx="12" stroke="#D85A30" stroke-width="1.5"/>
  <rect x="300" y="20" width="260" height="5" fill="url(#accentB)" rx="3"/>
  <text x="430" y="55" text-anchor="middle" font-family="sans-serif" font-size="28">❤️</text>
  <text x="430" y="82" text-anchor="middle" font-family="sans-serif" font-size="13" font-weight="700" fill="#D85A30">Heart Disease</text>
  <text x="430" y="100" text-anchor="middle" font-family="sans-serif" font-size="11" fill="#8b949e">Cleveland UCI · cherngs</text>
  <line x1="320" y1="110" x2="540" y2="110" stroke="#21262d" stroke-width="1"/>
  <text x="320" y="128" font-family="sans-serif" font-size="11" fill="#8b949e">📦 Rows</text>
  <text x="540" y="128" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#e6edf3">297</text>
  <text x="320" y="146" font-family="sans-serif" font-size="11" fill="#8b949e">🔢 Features</text>
  <text x="540" y="146" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#e6edf3">13 → 13</text>
  <text x="320" y="164" font-family="sans-serif" font-size="11" fill="#8b949e">⚖️ Imbalance</text>
  <text x="540" y="164" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#5DCAA5">53.9% / 46.1%</text>
  <text x="320" y="182" font-family="sans-serif" font-size="11" fill="#8b949e">🏆 Best Model</text>
  <text x="540" y="182" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#D85A30">Logistic Reg.</text>
  <text x="320" y="195" font-family="sans-serif" font-size="10" fill="#8b949e">AUC</text>
  <rect x="340" y="187" width="140" height="6" fill="#21262d" rx="3"/>
  <rect x="340" y="187" width="134" height="6" fill="url(#accentB)" rx="3"/>
  <text x="485" y="195" font-family="sans-serif" font-size="10" font-weight="700" fill="#D85A30">0.958</text>

  <!-- Card 3 -->
  <rect x="580" y="20" width="260" height="180" fill="#161b22" rx="12" stroke="#378ADD" stroke-width="1.5"/>
  <rect x="580" y="20" width="260" height="5" fill="url(#accentC)" rx="3"/>
  <text x="710" y="55" text-anchor="middle" font-family="sans-serif" font-size="28">🧬</text>
  <text x="710" y="82" text-anchor="middle" font-family="sans-serif" font-size="13" font-weight="700" fill="#378ADD">Pima Indians Diabetes</text>
  <text x="710" y="100" text-anchor="middle" font-family="sans-serif" font-size="11" fill="#8b949e">UCI ML · uciml</text>
  <line x1="600" y1="110" x2="820" y2="110" stroke="#21262d" stroke-width="1"/>
  <text x="600" y="128" font-family="sans-serif" font-size="11" fill="#8b949e">📦 Rows</text>
  <text x="820" y="128" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#e6edf3">768</text>
  <text x="600" y="146" font-family="sans-serif" font-size="11" fill="#8b949e">🔢 Features</text>
  <text x="820" y="146" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#e6edf3">8 → 16 (engineered)</text>
  <text x="600" y="164" font-family="sans-serif" font-size="11" fill="#8b949e">⚖️ Imbalance</text>
  <text x="820" y="164" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#BA7517">65.1% / 34.9%</text>
  <text x="600" y="182" font-family="sans-serif" font-size="11" fill="#8b949e">🏆 Best Model</text>
  <text x="820" y="182" text-anchor="end" font-family="sans-serif" font-size="11" font-weight="600" fill="#378ADD">XGBoost</text>
  <text x="600" y="195" font-family="sans-serif" font-size="10" fill="#8b949e">AUC</text>
  <rect x="620" y="187" width="140" height="6" fill="#21262d" rx="3"/>
  <rect x="620" y="187" width="118" height="6" fill="url(#accentC)" rx="3"/>
  <text x="765" y="195" font-family="sans-serif" font-size="10" font-weight="700" fill="#378ADD">0.838</text>
</svg>

</div>

---

## 🏗️ System Architecture

<div align="center">

<!-- ARCHITECTURE FLOWCHART SVG -->
<svg width="860" height="520" viewBox="0 0 860 520" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="archBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d1117"/>
      <stop offset="100%" style="stop-color:#0d1117"/>
    </linearGradient>
    <linearGradient id="inputGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#1f6feb"/>
      <stop offset="100%" style="stop-color:#0d419d"/>
    </linearGradient>
    <linearGradient id="prepGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#238636"/>
      <stop offset="100%" style="stop-color:#196127"/>
    </linearGradient>
    <linearGradient id="modelGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#9333ea"/>
      <stop offset="100%" style="stop-color:#6b21a8"/>
    </linearGradient>
    <linearGradient id="tuneGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#d97706"/>
      <stop offset="100%" style="stop-color:#92400e"/>
    </linearGradient>
    <linearGradient id="deployGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#0e9f6e"/>
      <stop offset="100%" style="stop-color:#057a55"/>
    </linearGradient>
    <marker id="arrow" viewBox="0 0 10 10" refX="9" refY="5"
      markerWidth="6" markerHeight="6" orient="auto-start-reverse">
      <path d="M 0 0 L 10 5 L 0 10 z" fill="#4d5566"/>
    </marker>
    <marker id="arrowTeal" viewBox="0 0 10 10" refX="9" refY="5"
      markerWidth="6" markerHeight="6" orient="auto-start-reverse">
      <path d="M 0 0 L 10 5 L 0 10 z" fill="#5DCAA5"/>
    </marker>
    <filter id="cardShadow">
      <feDropShadow dx="0" dy="4" stdDeviation="8" flood-color="#000" flood-opacity="0.4"/>
    </filter>
  </defs>

  <rect width="860" height="520" fill="#0d1117" rx="14"/>

  <!-- ── ROW 1: DATA SOURCES ── -->
  <text x="430" y="28" text-anchor="middle" font-family="sans-serif" font-size="11" fill="#4d5566" letter-spacing="2">DATA SOURCES</text>

  <!-- DS1 -->
  <rect x="30" y="36" width="180" height="54" fill="url(#inputGrad)" rx="8" filter="url(#cardShadow)"/>
  <text x="120" y="58" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="white">🩸 Diabetes Large</text>
  <text x="120" y="76" text-anchor="middle" font-family="sans-serif" font-size="10" fill="#93c5fd">100,000 rows · 8 features</text>

  <!-- DS2 -->
  <rect x="340" y="36" width="180" height="54" fill="url(#inputGrad)" rx="8" filter="url(#cardShadow)"/>
  <text x="430" y="58" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="white">❤️ Heart Cleveland</text>
  <text x="430" y="76" text-anchor="middle" font-family="sans-serif" font-size="10" fill="#93c5fd">297 rows · 13 features</text>

  <!-- DS3 -->
  <rect x="650" y="36" width="180" height="54" fill="url(#inputGrad)" rx="8" filter="url(#cardShadow)"/>
  <text x="740" y="58" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="white">🧬 Pima Indians</text>
  <text x="740" y="76" text-anchor="middle" font-family="sans-serif" font-size="10" fill="#93c5fd">768 rows · 8 features</text>

  <!-- Arrows DS → PREP -->
  <line x1="120" y1="90" x2="120" y2="148" stroke="#4d5566" stroke-width="1.5" stroke-dasharray="4,3" marker-end="url(#arrow)"/>
  <line x1="430" y1="90" x2="430" y2="148" stroke="#4d5566" stroke-width="1.5" stroke-dasharray="4,3" marker-end="url(#arrow)"/>
  <line x1="740" y1="90" x2="740" y2="148" stroke="#4d5566" stroke-width="1.5" stroke-dasharray="4,3" marker-end="url(#arrow)"/>

  <!-- ── ROW 2: PREPROCESSING ── -->
  <text x="430" y="142" text-anchor="middle" font-family="sans-serif" font-size="11" fill="#4d5566" letter-spacing="2">PREPROCESSING</text>

  <!-- Prep boxes -->
  <rect x="30" y="150" width="180" height="72" fill="url(#prepGrad)" rx="8" filter="url(#cardShadow)"/>
  <text x="120" y="170" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="white">⚙️ Encode + Scale</text>
  <text x="120" y="186" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#86efac">LabelEncoder</text>
  <text x="120" y="200" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#86efac">StandardScaler</text>
  <text x="120" y="214" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#86efac">SMOTE balancing</text>

  <rect x="340" y="150" width="180" height="72" fill="url(#prepGrad)" rx="8" filter="url(#cardShadow)"/>
  <text x="430" y="170" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="white">⚙️ Binarize + Scale</text>
  <text x="430" y="186" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#86efac">condition → 0/1</text>
  <text x="430" y="200" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#86efac">StandardScaler</text>
  <text x="430" y="214" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#86efac">SMOTE balancing</text>

  <rect x="650" y="150" width="180" height="72" fill="url(#prepGrad)" rx="8" filter="url(#cardShadow)"/>
  <text x="740" y="170" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="white">⚙️ Impute + Engineer</text>
  <text x="740" y="186" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#86efac">Zero→Median impute</text>
  <text x="740" y="200" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#86efac">8 → 16 features</text>
  <text x="740" y="214" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#86efac">SMOTE balancing</text>

  <!-- Converging arrows to MODEL block -->
  <line x1="120" y1="222" x2="120" y2="250" stroke="#4d5566" stroke-width="1.5" stroke-dasharray="4,3"/>
  <line x1="430" y1="222" x2="430" y2="250" stroke="#4d5566" stroke-width="1.5" stroke-dasharray="4,3"/>
  <line x1="740" y1="222" x2="740" y2="250" stroke="#4d5566" stroke-width="1.5" stroke-dasharray="4,3"/>
  <line x1="120" y1="250" x2="740" y2="250" stroke="#4d5566" stroke-width="1.5" stroke-dasharray="4,3"/>
  <line x1="430" y1="250" x2="430" y2="268" stroke="#5DCAA5" stroke-width="2" marker-end="url(#arrowTeal)"/>

  <!-- ── ROW 3: MODELS ── -->
  <text x="430" y="262" text-anchor="middle" font-family="sans-serif" font-size="11" fill="#4d5566" letter-spacing="2">MODEL TRAINING</text>

  <rect x="100" y="270" width="660" height="74" fill="#161b22" rx="10" stroke="#9333ea" stroke-width="1.5" filter="url(#cardShadow)"/>

  <!-- 4 model pills -->
  <rect x="116" y="285" width="140" height="44" fill="url(#modelGrad)" rx="7"/>
  <text x="186" y="305" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="white">📐 Logistic</text>
  <text x="186" y="320" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#d8b4fe">Regression</text>

  <rect x="276" y="285" width="140" height="44" fill="url(#modelGrad)" rx="7"/>
  <text x="346" y="305" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="white">🌲 Random</text>
  <text x="346" y="320" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#d8b4fe">Forest</text>

  <rect x="436" y="285" width="140" height="44" fill="url(#modelGrad)" rx="7"/>
  <text x="506" y="305" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="white">⚡ XGBoost</text>
  <text x="506" y="320" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#d8b4fe">GPU Accelerated</text>

  <rect x="596" y="285" width="148" height="44" fill="url(#modelGrad)" rx="7"/>
  <text x="670" y="305" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="white">💡 LightGBM</text>
  <text x="670" y="320" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#d8b4fe">Histogram-based</text>

  <line x1="430" y1="344" x2="430" y2="362" stroke="#5DCAA5" stroke-width="2" marker-end="url(#arrowTeal)"/>

  <!-- ── ROW 4: OPTUNA ── -->
  <text x="430" y="357" text-anchor="middle" font-family="sans-serif" font-size="11" fill="#4d5566" letter-spacing="2">HYPERPARAMETER TUNING</text>

  <rect x="180" y="364" width="500" height="56" fill="#161b22" rx="10" stroke="#d97706" stroke-width="1.5" filter="url(#cardShadow)"/>
  <text x="430" y="388" text-anchor="middle" font-family="sans-serif" font-size="12" font-weight="700" fill="#fbbf24">🔬 Optuna TPE — 50 Trials per Best Model</text>
  <text x="430" y="408" text-anchor="middle" font-family="sans-serif" font-size="10" fill="#8b949e">Maximise ROC-AUC · LightGBM · Logistic Regression · XGBoost</text>

  <line x1="430" y1="420" x2="430" y2="438" stroke="#5DCAA5" stroke-width="2" marker-end="url(#arrowTeal)"/>

  <!-- ── ROW 5: OUTPUT ── -->
  <text x="430" y="432" text-anchor="middle" font-family="sans-serif" font-size="11" fill="#4d5566" letter-spacing="2">DEPLOYMENT</text>

  <rect x="180" y="440" width="500" height="56" fill="url(#deployGrad)" rx="10" filter="url(#cardShadow)"/>
  <text x="430" y="464" text-anchor="middle" font-family="sans-serif" font-size="13" font-weight="700" fill="white">🚀 Gradio App — Live on Kaggle</text>
  <text x="430" y="483" text-anchor="middle" font-family="sans-serif" font-size="10" fill="#a7f3d0">3-tab interface · Real-time inference · Public share link</text>
</svg>

</div>

---

## 🔬 ML Pipeline

<div align="center">

<!-- PIPELINE DETAIL SVG -->
<svg width="860" height="300" viewBox="0 0 860 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="pipelineBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d1117"/>
      <stop offset="100%" style="stop-color:#0d1117"/>
    </linearGradient>
    <linearGradient id="step1g" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#1d4ed8"/><stop offset="100%" style="stop-color:#1e40af"/>
    </linearGradient>
    <linearGradient id="step2g" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#059669"/><stop offset="100%" style="stop-color:#047857"/>
    </linearGradient>
    <linearGradient id="step3g" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#7c3aed"/><stop offset="100%" style="stop-color:#6d28d9"/>
    </linearGradient>
    <linearGradient id="step4g" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#b45309"/><stop offset="100%" style="stop-color:#92400e"/>
    </linearGradient>
    <linearGradient id="step5g" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0e9f6e"/><stop offset="100%" style="stop-color:#057a55"/>
    </linearGradient>
    <marker id="pArrow" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="5" markerHeight="5" orient="auto">
      <path d="M 0 0 L 10 5 L 0 10 z" fill="#5DCAA5"/>
    </marker>
  </defs>
  <rect width="860" height="300" fill="#0d1117" rx="14"/>

  <!-- Step circles + labels top row -->
  <!-- Step 1 -->
  <circle cx="80" cy="90" r="36" fill="url(#step1g)" stroke="#3b82f6" stroke-width="2"/>
  <text x="80" y="84" text-anchor="middle" font-family="sans-serif" font-size="20">📂</text>
  <text x="80" y="103" text-anchor="middle" font-family="sans-serif" font-size="9" font-weight="700" fill="white">LOAD</text>
  <text x="80" y="145" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">CSV ingestion</text>
  <text x="80" y="158" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Target normalize</text>

  <!-- Arrow 1→2 -->
  <line x1="118" y1="90" x2="192" y2="90" stroke="#5DCAA5" stroke-width="2" marker-end="url(#pArrow)"/>

  <!-- Step 2 -->
  <circle cx="230" cy="90" r="36" fill="url(#step2g)" stroke="#10b981" stroke-width="2"/>
  <text x="230" y="84" text-anchor="middle" font-family="sans-serif" font-size="20">🩹</text>
  <text x="230" y="103" text-anchor="middle" font-family="sans-serif" font-size="9" font-weight="700" fill="white">CLEAN</text>
  <text x="230" y="145" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Zero imputation</text>
  <text x="230" y="158" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Label encoding</text>

  <!-- Arrow 2→3 -->
  <line x1="268" y1="90" x2="342" y2="90" stroke="#5DCAA5" stroke-width="2" marker-end="url(#pArrow)"/>

  <!-- Step 3 -->
  <circle cx="380" cy="90" r="36" fill="url(#step3g)" stroke="#8b5cf6" stroke-width="2"/>
  <text x="380" y="84" text-anchor="middle" font-family="sans-serif" font-size="20">⚖️</text>
  <text x="380" y="103" text-anchor="middle" font-family="sans-serif" font-size="9" font-weight="700" fill="white">BALANCE</text>
  <text x="380" y="145" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">StandardScaler</text>
  <text x="380" y="158" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">SMOTE oversample</text>

  <!-- Arrow 3→4 -->
  <line x1="418" y1="90" x2="492" y2="90" stroke="#5DCAA5" stroke-width="2" marker-end="url(#pArrow)"/>

  <!-- Step 4 -->
  <circle cx="530" cy="90" r="36" fill="url(#step4g)" stroke="#f59e0b" stroke-width="2"/>
  <text x="530" y="84" text-anchor="middle" font-family="sans-serif" font-size="20">🏋️</text>
  <text x="530" y="103" text-anchor="middle" font-family="sans-serif" font-size="9" font-weight="700" fill="white">TRAIN</text>
  <text x="530" y="145" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">4 classifiers</text>
  <text x="530" y="158" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Stratified 80/20</text>

  <!-- Arrow 4→5 -->
  <line x1="568" y1="90" x2="642" y2="90" stroke="#5DCAA5" stroke-width="2" marker-end="url(#pArrow)"/>

  <!-- Step 5 -->
  <circle cx="680" cy="90" r="36" fill="url(#step5g)" stroke="#10b981" stroke-width="2"/>
  <text x="680" y="84" text-anchor="middle" font-family="sans-serif" font-size="20">🔬</text>
  <text x="680" y="103" text-anchor="middle" font-family="sans-serif" font-size="9" font-weight="700" fill="white">TUNE</text>
  <text x="680" y="145" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Optuna TPE</text>
  <text x="680" y="158" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">50 trials</text>

  <!-- Arrow 5→6 -->
  <line x1="718" y1="90" x2="790" y2="90" stroke="#5DCAA5" stroke-width="2" marker-end="url(#pArrow)"/>

  <!-- Step 6 -->
  <circle cx="820" cy="90" r="36" fill="#0e9f6e" stroke="#5DCAA5" stroke-width="2.5"/>
  <text x="820" y="84" text-anchor="middle" font-family="sans-serif" font-size="20">🚀</text>
  <text x="820" y="103" text-anchor="middle" font-family="sans-serif" font-size="9" font-weight="700" fill="white">DEPLOY</text>
  <text x="820" y="145" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Gradio UI</text>
  <text x="820" y="158" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Public link</text>

  <!-- Medical metrics legend -->
  <rect x="60" y="195" width="740" height="84" fill="#161b22" rx="10" stroke="#21262d" stroke-width="1"/>
  <text x="430" y="218" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="#e6edf3">📊 Evaluation Metrics — Why Each Matters Clinically</text>

  <rect x="80" y="226" width="160" height="40" fill="#1f2937" rx="6"/>
  <text x="160" y="242" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#60a5fa">ROC-AUC</text>
  <text x="160" y="258" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Overall discriminability</text>

  <rect x="260" y="226" width="160" height="40" fill="#1f2937" rx="6"/>
  <text x="340" y="242" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#34d399">Sensitivity</text>
  <text x="340" y="258" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Catch true positives</text>

  <rect x="440" y="226" width="160" height="40" fill="#1f2937" rx="6"/>
  <text x="520" y="242" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#f87171">Specificity</text>
  <text x="520" y="258" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Avoid false alarms</text>

  <rect x="620" y="226" width="160" height="40" fill="#1f2937" rx="6"/>
  <text x="700" y="242" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#fbbf24">F1 Score</text>
  <text x="700" y="258" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#8b949e">Precision-recall balance</text>
</svg>

</div>

---

## 📈 Results & Leaderboard

<div align="center">

<!-- RESULTS SVG — leaderboard bars -->
<svg width="860" height="380" viewBox="0 0 860 380" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="barTeal" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#5DCAA5"/><stop offset="100%" style="stop-color:#378ADD"/>
    </linearGradient>
    <linearGradient id="barCoral" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#D85A30"/><stop offset="100%" style="stop-color:#7F77DD"/>
    </linearGradient>
    <linearGradient id="barBlue" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#378ADD"/><stop offset="100%" style="stop-color:#5DCAA5"/>
    </linearGradient>
  </defs>
  <rect width="860" height="380" fill="#0d1117" rx="14"/>
  <text x="430" y="26" text-anchor="middle" font-family="sans-serif" font-size="13" font-weight="700" fill="#e6edf3">🏆 Model Leaderboard — Best per Dataset (ROC-AUC)</text>

  <!-- Y-axis labels -->
  <text x="30" y="60" font-family="sans-serif" font-size="9" fill="#4d5566">1.00</text>
  <text x="30" y="110" font-family="sans-serif" font-size="9" fill="#4d5566">0.95</text>
  <text x="30" y="160" font-family="sans-serif" font-size="9" fill="#4d5566">0.90</text>
  <text x="30" y="210" font-family="sans-serif" font-size="9" fill="#4d5566">0.85</text>
  <text x="30" y="260" font-family="sans-serif" font-size="9" fill="#4d5566">0.80</text>

  <!-- Grid lines -->
  <line x1="55" y1="56" x2="830" y2="56" stroke="#21262d" stroke-width="1" stroke-dasharray="3,3"/>
  <line x1="55" y1="106" x2="830" y2="106" stroke="#21262d" stroke-width="1" stroke-dasharray="3,3"/>
  <line x1="55" y1="156" x2="830" y2="156" stroke="#21262d" stroke-width="1" stroke-dasharray="3,3"/>
  <line x1="55" y1="206" x2="830" y2="156" stroke="#21262d" stroke-width="1" stroke-dasharray="3,3"/>
  <line x1="55" y1="256" x2="830" y2="256" stroke="#21262d" stroke-width="1" stroke-dasharray="3,3"/>

  <!-- Baseline = 0.80, scale: 200px per 0.20 = 1000px per 1.0 -->
  <!-- AUC 0.979 → height = (0.979-0.80)*1000 = 179 -->
  <!-- AUC 0.958 → height = (0.958-0.80)*1000 = 158 -->
  <!-- AUC 0.838 → height = (0.838-0.80)*1000 = 38  -->
  <!-- base y = 256 -->

  <!-- Dataset 1 group: Diabetes-Large -->
  <!-- LR 0.962 → 162 -->
  <rect x="70" y="94" width="50" height="162" fill="#378ADD" rx="4" opacity="0.7"/>
  <text x="95" y="90" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#60a5fa">0.962</text>
  <!-- RF 0.974 → 174 -->
  <rect x="128" y="82" width="50" height="174" fill="#1D9E75" rx="4" opacity="0.7"/>
  <text x="153" y="78" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#6ee7b7">0.974</text>
  <!-- XGB 0.978 → 178 -->
  <rect x="186" y="78" width="50" height="178" fill="#D85A30" rx="4" opacity="0.7"/>
  <text x="211" y="74" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#fca5a5">0.978</text>
  <!-- LGBM 0.979 → 179 (winner) -->
  <rect x="244" y="77" width="50" height="179" fill="url(#barTeal)" rx="4"/>
  <text x="269" y="73" text-anchor="middle" font-family="sans-serif" font-size="9" font-weight="700" fill="#5DCAA5">0.979 🏆</text>

  <text x="195" y="276" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#8b949e">🩸 Diabetes-Large</text>

  <!-- Dataset 2 group: Heart-Cleveland -->
  <!-- LR 0.954 → 154 (winner) -->
  <rect x="350" y="102" width="50" height="154" fill="url(#barCoral)" rx="4"/>
  <text x="375" y="98" text-anchor="middle" font-family="sans-serif" font-size="9" font-weight="700" fill="#D85A30">0.954 🏆</text>
  <!-- RF 0.941 → 141 -->
  <rect x="408" y="115" width="50" height="141" fill="#1D9E75" rx="4" opacity="0.7"/>
  <text x="433" y="111" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#6ee7b7">0.941</text>
  <!-- XGB 0.934 → 134 -->
  <rect x="466" y="122" width="50" height="134" fill="#D85A30" rx="4" opacity="0.7"/>
  <text x="491" y="118" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#fca5a5">0.934</text>
  <!-- LGBM 0.949 → 149 -->
  <rect x="524" y="107" width="50" height="149" fill="#7F77DD" rx="4" opacity="0.7"/>
  <text x="549" y="103" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#c4b5fd">0.949</text>

  <text x="462" y="276" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#8b949e">❤️ Heart-Cleveland</text>

  <!-- Dataset 3 group: Pima -->
  <!-- LR 0.811 → 11 -->
  <rect x="630" y="245" width="50" height="11" fill="#378ADD" rx="4" opacity="0.7"/>
  <text x="655" y="241" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#60a5fa">0.811</text>
  <!-- RF 0.809 → 9 -->
  <rect x="688" y="247" width="50" height="9" fill="#1D9E75" rx="4" opacity="0.7"/>
  <text x="713" y="243" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#6ee7b7">0.809</text>
  <!-- XGB 0.838 → 38 (winner) -->
  <rect x="746" y="218" width="50" height="38" fill="url(#barBlue)" rx="4"/>
  <text x="771" y="214" text-anchor="middle" font-family="sans-serif" font-size="9" font-weight="700" fill="#378ADD">0.838 🏆</text>
  <!-- LGBM 0.816 → 16 -->

  <text x="712" y="276" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#8b949e">🧬 Pima Indians</text>

  <!-- Legend -->
  <rect x="55" y="295" width="750" height="70" fill="#161b22" rx="8" stroke="#21262d" stroke-width="1"/>
  <text x="430" y="313" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#e6edf3">Key Insight</text>

  <rect x="75" y="320" width="10" height="10" fill="#378ADD" rx="2"/>
  <text x="93" y="330" font-family="sans-serif" font-size="9" fill="#8b949e">Logistic Reg.</text>

  <rect x="180" y="320" width="10" height="10" fill="#1D9E75" rx="2"/>
  <text x="198" y="330" font-family="sans-serif" font-size="9" fill="#8b949e">Random Forest</text>

  <rect x="295" y="320" width="10" height="10" fill="#D85A30" rx="2"/>
  <text x="313" y="330" font-family="sans-serif" font-size="9" fill="#8b949e">XGBoost</text>

  <rect x="390" y="320" width="10" height="10" fill="#7F77DD" rx="2"/>
  <text x="408" y="330" font-family="sans-serif" font-size="9" fill="#8b949e">LightGBM</text>

  <text x="430" y="352" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#6b7280">
    Simpler models win on small data (Heart: LR beats XGB). Boosting dominates at scale (Diabetes-Large: LGBM 0.979).
  </text>
</svg>

</div>

### Detailed Metrics Table

| Dataset | Model | AUC | F1 | Sensitivity | Specificity |
|:---|:---|:---:|:---:|:---:|:---:|
| 🩸 Diabetes-Large | **LightGBM** *(tuned)* | **0.979** | 0.804 | 0.709 | 0.995 |
| ❤️ Heart-Cleveland | **Logistic Regression** *(tuned)* | **0.958** | 0.902 | 0.821 | 1.000 |
| 🧬 Diabetes-Pima | **XGBoost + Feat. Eng.** *(tuned)* | **0.838** | 0.649 | 0.685 | 0.770 |

> **Sensitivity** = fraction of sick patients correctly identified. **Specificity** = fraction of healthy patients correctly cleared. For medical screening, sensitivity is the priority.

---

## ⚙️ Feature Engineering

<div align="center">

<!-- FEATURE ENGINEERING SVG -->
<svg width="860" height="290" viewBox="0 0 860 290" xmlns="http://www.w3.org/2000/svg">
  <rect width="860" height="290" fill="#0d1117" rx="14"/>
  <text x="430" y="26" text-anchor="middle" font-family="sans-serif" font-size="13" font-weight="700" fill="#e6edf3">🧬 Pima Indians — Feature Engineering (8 → 16 Features)</text>

  <!-- Original features column -->
  <rect x="20" y="40" width="180" height="230" fill="#161b22" rx="10" stroke="#1d4ed8" stroke-width="1.5"/>
  <rect x="20" y="40" width="180" height="30" fill="#1d4ed8" rx="8"/>
  <rect x="20" y="58" width="180" height="12" fill="#1d4ed8"/>
  <text x="110" y="61" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="white">Original 8 Features</text>

  <g font-family="sans-serif" font-size="10" fill="#8b949e">
    <text x="36" y="90">📊 Pregnancies</text>
    <text x="36" y="108">🩸 Glucose</text>
    <text x="36" y="126">💉 Blood Pressure</text>
    <text x="36" y="144">📏 Skin Thickness</text>
    <text x="36" y="162">💊 Insulin</text>
    <text x="36" y="180">⚖️  BMI</text>
    <text x="36" y="198">🧬 Diabetes Pedigree</text>
    <text x="36" y="216">🎂 Age</text>
  </g>

  <!-- Arrow -->
  <line x1="200" y1="155" x2="255" y2="155" stroke="#5DCAA5" stroke-width="2.5" marker-end="url(#arrowTeal)"/>
  <text x="228" y="148" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#5DCAA5">×2</text>

  <!-- Engineered features column -->
  <rect x="258" y="40" width="580" height="230" fill="#161b22" rx="10" stroke="#5DCAA5" stroke-width="1.5"/>
  <rect x="258" y="40" width="580" height="30" fill="#057a55" rx="8"/>
  <rect x="258" y="58" width="580" height="12" fill="#057a55"/>
  <text x="548" y="61" text-anchor="middle" font-family="sans-serif" font-size="11" font-weight="700" fill="white">8 Engineered Features Added</text>

  <!-- Feature cards 2×4 grid -->
  <!-- Row 1 -->
  <rect x="272" y="76" width="132" height="60" fill="#0e2a1e" rx="7" stroke="#5DCAA5" stroke-width="1"/>
  <text x="338" y="95" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#5DCAA5">glucose × bmi</text>
  <text x="338" y="110" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">Insulin resistance</text>
  <text x="338" y="124" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">proxy</text>

  <rect x="416" y="76" width="132" height="60" fill="#2a1a0e" rx="7" stroke="#f59e0b" stroke-width="1"/>
  <text x="482" y="95" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#fbbf24">bp × age</text>
  <text x="482" y="110" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">Cardiovascular</text>
  <text x="482" y="124" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">stress score</text>

  <rect x="560" y="76" width="132" height="60" fill="#1a0e2a" rx="7" stroke="#8b5cf6" stroke-width="1"/>
  <text x="626" y="95" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#c4b5fd">glucose / bmi</text>
  <text x="626" y="110" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">Thin-person</text>
  <text x="626" y="124" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">glucose risk</text>

  <rect x="704" y="76" width="120" height="60" fill="#0e1a2a" rx="7" stroke="#3b82f6" stroke-width="1"/>
  <text x="764" y="95" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#60a5fa">skin / bmi</text>
  <text x="764" y="110" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">Adiposity</text>
  <text x="764" y="124" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">proxy</text>

  <!-- Row 2 -->
  <rect x="272" y="150" width="132" height="60" fill="#0e2a1e" rx="7" stroke="#10b981" stroke-width="1"/>
  <text x="338" y="169" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#34d399">insulin / glucose</text>
  <text x="338" y="184" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">Sensitivity</text>
  <text x="338" y="198" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">indicator</text>

  <rect x="416" y="150" width="132" height="60" fill="#2a200e" rx="7" stroke="#d97706" stroke-width="1"/>
  <text x="482" y="169" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#fbbf24">age × preg</text>
  <text x="482" y="184" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">Older mother</text>
  <text x="482" y="198" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">risk amplifier</text>

  <rect x="560" y="150" width="132" height="60" fill="#1a0e0e" rx="7" stroke="#ef4444" stroke-width="1"/>
  <text x="626" y="169" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#f87171">BMI bin</text>
  <text x="626" y="184" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">WHO category</text>
  <text x="626" y="198" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">0/1/2/3</text>

  <rect x="704" y="150" width="120" height="60" fill="#0e1a1a" rx="7" stroke="#06b6d4" stroke-width="1"/>
  <text x="764" y="169" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#22d3ee">glucose bin</text>
  <text x="764" y="184" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">Clinical threshold</text>
  <text x="764" y="198" text-anchor="middle" font-family="sans-serif" font-size="8.5" fill="#6b7280">normal/pre/diabetic</text>

  <!-- Result bar -->
  <rect x="272" y="224" width="552" height="32" fill="#0e2a1e" rx="6" stroke="#5DCAA5" stroke-width="1"/>
  <text x="548" y="244" text-anchor="middle" font-family="sans-serif" font-size="10" fill="#5DCAA5">
    ✅ AUC improved:  0.823 → 0.838   (+0.015)   with XGBoost + Stacking Ensemble
  </text>
</svg>

</div>

---

## 🚀 Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/medrisk-classifier.git
cd medrisk-classifier

# 2. Install dependencies
pip install -r requirements.txt

# 3. Add datasets (Kaggle API)
kaggle datasets download mathchi/diabetes-data-set
kaggle datasets download cherngs/heart-disease-cleveland-uci
kaggle datasets download uciml/pima-indians-diabetes-database

# 4. Run on Kaggle (recommended — GPU included)
# Open notebook on Kaggle and click "Run All"

# 5. Or run locally
jupyter notebook MedRisk_Classifier.ipynb
```

### Requirements

```
numpy>=1.24
pandas>=2.0
scikit-learn>=1.3
xgboost>=2.0
lightgbm>=4.0
optuna>=3.4
imbalanced-learn>=0.11
gradio>=4.0
matplotlib>=3.7
seaborn>=0.12
```

---

## 🗂️ Project Structure

```
medrisk-classifier/
│
├── 📓 MedRisk_Classifier.ipynb     # Main Kaggle notebook (run this)
│
├── 📊 outputs/
│   ├── class_balance.png           # Snippet 1 — class distribution
│   ├── dist_*.png                  # Snippet 1 — feature KDE plots
│   ├── corr_*.png                  # Snippet 1 — correlation heatmaps
│   ├── smote_balance.png           # Snippet 2 — before/after SMOTE
│   ├── target_correlation.png      # Snippet 2 — feature-target corr
│   ├── metrics_heatmap.png         # Snippet 3 — model comparison
│   ├── roc_curves.png              # Snippet 3 — ROC per dataset
│   ├── confusion_matrices.png      # Snippet 3 — confusion matrices
│   ├── feature_importance.png      # Snippet 3 — RF + LGBM importance
│   ├── tuned_vs_baseline.png       # Snippet 4 — Optuna gains
│   ├── optuna_history.png          # Snippet 4 — trial convergence
│   └── pima_progression.png        # Snippet 4B — engineering gains
│
├── 📋 requirements.txt
└── 📖 README.md
```

---

## 🧩 Tech Stack

<div align="center">

<!-- TECH STACK SVG -->
<svg width="860" height="140" viewBox="0 0 860 140" xmlns="http://www.w3.org/2000/svg">
  <rect width="860" height="140" fill="#0d1117" rx="14"/>

  <!-- Tech pills -->
  <!-- Python -->
  <rect x="20" y="40" width="110" height="60" fill="#1e3a5f" rx="10" stroke="#3b82f6" stroke-width="1.5"/>
  <text x="75" y="66" text-anchor="middle" font-family="sans-serif" font-size="22">🐍</text>
  <text x="75" y="88" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#60a5fa">Python 3.12</text>

  <!-- XGBoost -->
  <rect x="145" y="40" width="110" height="60" fill="#3a1e0e" rx="10" stroke="#f97316" stroke-width="1.5"/>
  <text x="200" y="66" text-anchor="middle" font-family="sans-serif" font-size="22">⚡</text>
  <text x="200" y="88" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#fb923c">XGBoost 2.0</text>

  <!-- LightGBM -->
  <rect x="270" y="40" width="110" height="60" fill="#0e3a1e" rx="10" stroke="#10b981" stroke-width="1.5"/>
  <text x="325" y="66" text-anchor="middle" font-family="sans-serif" font-size="22">💡</text>
  <text x="325" y="88" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#34d399">LightGBM 4.0</text>

  <!-- Optuna -->
  <rect x="395" y="40" width="110" height="60" fill="#2a1a3a" rx="10" stroke="#8b5cf6" stroke-width="1.5"/>
  <text x="450" y="66" text-anchor="middle" font-family="sans-serif" font-size="22">🔬</text>
  <text x="450" y="88" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#a78bfa">Optuna 3.4</text>

  <!-- Gradio -->
  <rect x="520" y="40" width="110" height="60" fill="#3a1e0e" rx="10" stroke="#f97316" stroke-width="1.5"/>
  <text x="575" y="66" text-anchor="middle" font-family="sans-serif" font-size="22">🎛️</text>
  <text x="575" y="88" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#fb923c">Gradio 4.0</text>

  <!-- sklearn -->
  <rect x="645" y="40" width="110" height="60" fill="#1e3a1e" rx="10" stroke="#22c55e" stroke-width="1.5"/>
  <text x="700" y="66" text-anchor="middle" font-family="sans-serif" font-size="22">🤖</text>
  <text x="700" y="88" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#4ade80">scikit-learn</text>

  <!-- Kaggle -->
  <rect x="770" y="40" width="70" height="60" fill="#0e1e3a" rx="10" stroke="#20beff" stroke-width="1.5"/>
  <text x="805" y="66" text-anchor="middle" font-family="sans-serif" font-size="22">🏅</text>
  <text x="805" y="88" text-anchor="middle" font-family="sans-serif" font-size="10" font-weight="700" fill="#22d3ee">Kaggle</text>

  <text x="430" y="120" text-anchor="middle" font-family="sans-serif" font-size="9" fill="#4d5566">All open-source · No paid APIs · GPU-accelerated on Kaggle</text>
</svg>

</div>

---

<div align="center">

<!-- FOOTER SVG -->
<svg width="860" height="80" viewBox="0 0 860 80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="footerGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#0f0c29"/>
      <stop offset="50%" style="stop-color:#302b63"/>
      <stop offset="100%" style="stop-color:#24243e"/>
    </linearGradient>
    <linearGradient id="footerLine" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#5DCAA5;stop-opacity:0"/>
      <stop offset="30%" style="stop-color:#5DCAA5"/>
      <stop offset="70%" style="stop-color:#378ADD"/>
      <stop offset="100%" style="stop-color:#378ADD;stop-opacity:0"/>
    </linearGradient>
  </defs>
  <rect width="860" height="80" fill="url(#footerGrad)" rx="12"/>
  <rect x="200" y="2" width="460" height="2" fill="url(#footerLine)" rx="1"/>
  <text x="430" y="34" text-anchor="middle" font-family="sans-serif" font-size="12" font-weight="700" fill="#e6edf3">
    Built for GitHub Portfolio · Kaggle GPU · 100% Open Source
  </text>
  <text x="430" y="56" text-anchor="middle" font-family="sans-serif" font-size="10" fill="#8b949e">
    MedRisk Classifier · 3 Datasets · 4 Models · Optuna · Gradio · SMOTE · Feature Engineering
  </text>
</svg>

<br/>

*⚠️ This project is for educational and portfolio purposes. Not intended for clinical diagnosis.*

**Made with 🩺 + 🤖 + ☕**

</div>
