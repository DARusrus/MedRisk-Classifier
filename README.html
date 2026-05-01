<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>MedRisk Classifier — README</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Mono:wght@400;500&family=Outfit:wght@300;400;500;600;700&display=swap" rel="stylesheet"/>
<style>
:root {
  --teal-50:#E1F5EE; --teal-100:#9FE1CB; --teal-200:#5DCAA5; --teal-400:#1D9E75; --teal-600:#0F6E56; --teal-800:#085041; --teal-900:#04342C;
  --coral-50:#FAECE7; --coral-100:#F5C4B3; --coral-200:#F0997B; --coral-400:#D85A30; --coral-600:#993C1D; --coral-800:#712B13;
  --amber-50:#FAEEDA; --amber-100:#FAC775; --amber-200:#EF9F27; --amber-400:#BA7517; --amber-600:#854F0B;
  --blue-50:#E6F1FB; --blue-100:#B5D4F4; --blue-200:#85B7EB; --blue-400:#378ADD; --blue-600:#185FA5; --blue-800:#0C447C;
  --purple-50:#EEEDFE; --purple-100:#CECBF6; --purple-200:#AFA9EC; --purple-400:#7F77DD; --purple-600:#534AB7; --purple-800:#3C3489;
  --gray-50:#F1EFE8; --gray-100:#D3D1C7; --gray-200:#B4B2A9; --gray-400:#888780; --gray-600:#5F5E5A; --gray-800:#444441;
  --ink:#1a1a1a; --ink2:#3d3d3a; --ink3:#73726c; --paper:#fafaf8;
}
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:'Outfit',sans-serif;background:var(--paper);color:var(--ink);line-height:1.7;overflow-x:hidden}

/* ── HERO ── */
.hero{background:var(--teal-600);color:#fff;text-align:center;padding:80px 40px 100px;position:relative;overflow:hidden}
.hero::before{content:'';position:absolute;inset:0;background:repeating-linear-gradient(45deg,transparent,transparent 60px,rgba(255,255,255,.03) 60px,rgba(255,255,255,.03) 61px)}
.hero-tag{display:inline-block;background:rgba(255,255,255,.15);border:1px solid rgba(255,255,255,.25);border-radius:999px;padding:6px 18px;font-size:12px;letter-spacing:.12em;text-transform:uppercase;font-weight:500;margin-bottom:28px}
.hero h1{font-family:'DM Serif Display',serif;font-size:clamp(48px,8vw,88px);line-height:1.0;letter-spacing:-1px;margin-bottom:16px}
.hero h1 em{font-style:italic;color:var(--teal-100)}
.hero-sub{font-size:18px;color:rgba(255,255,255,.75);max-width:560px;margin:0 auto 48px;font-weight:300;line-height:1.6}
.badge-row{display:flex;flex-wrap:wrap;justify-content:center;gap:10px;margin-bottom:36px}
.badge{background:rgba(255,255,255,.12);border:1px solid rgba(255,255,255,.2);border-radius:8px;padding:8px 16px;font-size:12px;font-weight:500;color:#fff;letter-spacing:.04em;display:flex;align-items:center;gap:6px}
.badge .dot{width:6px;height:6px;border-radius:50%;background:var(--teal-100);flex-shrink:0}
.cta-row{display:flex;justify-content:center;gap:14px;flex-wrap:wrap}
.btn-primary{background:#fff;color:var(--teal-600);padding:14px 32px;border-radius:999px;font-weight:600;font-size:15px;text-decoration:none;display:inline-flex;align-items:center;gap:8px}
.btn-secondary{background:transparent;color:#fff;border:1.5px solid rgba(255,255,255,.4);padding:14px 32px;border-radius:999px;font-weight:500;font-size:15px;text-decoration:none;display:inline-flex;align-items:center;gap:8px}
.wave{display:block;margin-top:-1px}

/* ── NAV STRIP ── */
.nav-strip{background:var(--teal-900);display:flex;justify-content:center;flex-wrap:wrap;gap:0}
.nav-strip a{color:var(--teal-100);text-decoration:none;font-size:12px;letter-spacing:.06em;text-transform:uppercase;font-weight:500;padding:14px 20px;border-right:1px solid rgba(255,255,255,.06)}
.nav-strip a:hover{background:rgba(255,255,255,.06);color:#fff}

/* ── SECTION WRAPPERS ── */
section{padding:80px 0}
.container{max-width:900px;margin:0 auto;padding:0 32px}
.section-tag{display:inline-flex;align-items:center;gap:8px;background:var(--teal-50);color:var(--teal-600);border-radius:999px;padding:5px 14px;font-size:11px;font-weight:600;letter-spacing:.1em;text-transform:uppercase;margin-bottom:20px}
.section-tag .icon{font-size:14px}
h2.section-title{font-family:'DM Serif Display',serif;font-size:clamp(32px,5vw,48px);line-height:1.1;color:var(--ink);margin-bottom:16px}
.section-lead{font-size:17px;color:var(--ink3);max-width:640px;margin:0 auto 56px;line-height:1.7}

/* ── ALT SECTION ── */
section.alt{background:var(--gray-50)}
section.dark{background:var(--teal-900);color:#fff}
section.dark h2.section-title{color:#fff}
section.dark .section-tag{background:rgba(255,255,255,.1);color:var(--teal-100)}
section.dark .section-lead{color:rgba(255,255,255,.65)}

/* ── DATASET CARDS ── */
.dataset-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-bottom:48px}
.ds-card{border-radius:16px;padding:28px 24px;position:relative;overflow:hidden}
.ds-card.a{background:var(--teal-50);border:1.5px solid var(--teal-100)}
.ds-card.b{background:var(--coral-50);border:1.5px solid var(--coral-100)}
.ds-card.c{background:var(--purple-50);border:1.5px solid var(--purple-100)}
.ds-card .ds-icon{font-size:32px;margin-bottom:16px;display:block}
.ds-card h3{font-size:16px;font-weight:600;margin-bottom:6px;color:var(--ink)}
.ds-card .ds-source{font-size:11px;color:var(--ink3);margin-bottom:20px;font-family:'DM Mono',monospace}
.ds-stats{display:flex;gap:16px;flex-wrap:wrap}
.ds-stat{display:flex;flex-direction:column;gap:2px}
.ds-stat .val{font-size:20px;font-weight:700;line-height:1}
.ds-stat .lbl{font-size:10px;text-transform:uppercase;letter-spacing:.08em;color:var(--ink3);font-weight:500}
.ds-card.a .val{color:var(--teal-600)}
.ds-card.b .val{color:var(--coral-600)}
.ds-card.c .val{color:var(--purple-600)}
.imbalance-badge{position:absolute;top:16px;right:16px;font-size:10px;font-weight:600;padding:4px 10px;border-radius:999px}
.ds-card.a .imbalance-badge{background:var(--amber-50);color:var(--amber-600);border:1px solid var(--amber-100)}
.ds-card.b .imbalance-badge{background:var(--teal-50);color:var(--teal-600);border:1px solid var(--teal-100)}
.ds-card.c .imbalance-badge{background:var(--teal-50);color:var(--teal-600);border:1px solid var(--teal-100)}

/* ── DIAGRAM CONTAINERS ── */
.diagram-wrap{border-radius:20px;overflow:hidden;border:1.5px solid var(--gray-100);margin:40px 0;background:#fff}
.diagram-header{background:var(--gray-50);padding:16px 24px;border-bottom:1px solid var(--gray-100);display:flex;align-items:center;justify-content:space-between}
.diagram-header .dtitle{font-size:12px;font-weight:600;letter-spacing:.08em;text-transform:uppercase;color:var(--ink3)}
.diagram-header .dpills{display:flex;gap:6px}
.diagram-header .dpill{width:10px;height:10px;border-radius:50%}
.diagram-body{padding:32px}

/* ── PIPELINE SVG layout ── */
.pipeline-wrap{width:100%;overflow:auto}

/* ── MODEL TABLE ── */
.model-table-wrap{overflow-x:auto;border-radius:16px;border:1.5px solid var(--gray-100);margin:32px 0}
table.model-table{width:100%;border-collapse:collapse;font-size:14px}
table.model-table thead tr{background:var(--teal-900);color:#fff}
table.model-table thead th{padding:14px 16px;text-align:left;font-weight:500;font-size:12px;letter-spacing:.06em;text-transform:uppercase}
table.model-table tbody tr:nth-child(even){background:var(--gray-50)}
table.model-table tbody tr.winner{background:var(--teal-50)}
table.model-table td{padding:13px 16px;border-bottom:1px solid var(--gray-100);color:var(--ink2)}
table.model-table td.num{font-family:'DM Mono',monospace;font-size:13px}
table.model-table .star{color:var(--teal-400);font-weight:700}
.table-group-head td{background:var(--teal-800);color:var(--teal-100);font-size:11px;font-weight:600;letter-spacing:.08em;text-transform:uppercase;padding:8px 16px}

/* ── LEADERBOARD ── */
.leaderboard{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin:40px 0}
.lb-card{border-radius:16px;padding:28px 24px;text-align:center;border:2px solid}
.lb-card.gold{background:linear-gradient(135deg,var(--teal-50),var(--teal-100));border-color:var(--teal-200)}
.lb-card .lb-rank{font-size:28px;margin-bottom:12px}
.lb-card .lb-dataset{font-size:11px;text-transform:uppercase;letter-spacing:.1em;color:var(--ink3);font-weight:600;margin-bottom:6px}
.lb-card .lb-model{font-size:17px;font-weight:700;color:var(--teal-600);margin-bottom:20px}
.lb-card .lb-metrics{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.lb-metric{display:flex;flex-direction:column;gap:3px}
.lb-metric .mv{font-family:'DM Mono',monospace;font-size:18px;font-weight:500;color:var(--ink)}
.lb-metric .mk{font-size:10px;text-transform:uppercase;letter-spacing:.08em;color:var(--ink3)}

/* ── FEAT ENG ── */
.fe-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;margin:32px 0}
.fe-card{border-radius:14px;padding:22px 20px;border:1.5px solid}
.fe-card.original{background:var(--gray-50);border-color:var(--gray-100)}
.fe-card.interaction{background:var(--teal-50);border-color:var(--teal-100)}
.fe-card.ratio{background:var(--amber-50);border-color:var(--amber-100)}
.fe-card.binned{background:var(--purple-50);border-color:var(--purple-100)}
.fe-card h4{font-size:13px;font-weight:700;letter-spacing:.08em;text-transform:uppercase;margin-bottom:14px}
.fe-card.original h4{color:var(--gray-600)}
.fe-card.interaction h4{color:var(--teal-600)}
.fe-card.ratio h4{color:var(--amber-600)}
.fe-card.binned h4{color:var(--purple-600)}
.fe-tag{display:inline-block;font-family:'DM Mono',monospace;font-size:11px;padding:3px 8px;border-radius:6px;margin:3px}
.fe-card.original .fe-tag{background:var(--gray-100);color:var(--gray-800)}
.fe-card.interaction .fe-tag{background:var(--teal-100);color:var(--teal-800)}
.fe-card.ratio .fe-tag{background:var(--amber-100);color:var(--amber-600)}
.fe-card.binned .fe-tag{background:var(--purple-100);color:var(--purple-800)}
.fe-card .fe-note{font-size:11px;color:var(--ink3);margin-top:10px;font-style:italic;line-height:1.5}

/* ── TUNING COMPARISON ── */
.tune-compare{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin:32px 0}
.tc-card{border-radius:14px;padding:22px 20px;background:#fff;border:1.5px solid var(--gray-100);text-align:center}
.tc-card h4{font-size:12px;text-transform:uppercase;letter-spacing:.08em;color:var(--ink3);margin-bottom:6px}
.tc-card .tc-model{font-size:14px;font-weight:600;color:var(--ink);margin-bottom:16px}
.tc-bar-wrap{height:6px;background:var(--gray-100);border-radius:999px;margin:4px 0 2px;position:relative;overflow:visible}
.tc-bar-base{height:6px;background:var(--gray-200);border-radius:999px}
.tc-bar-tuned{height:6px;border-radius:999px;position:absolute;top:0;left:0}
.tc-nums{display:flex;justify-content:space-between;font-size:11px;font-family:'DM Mono',monospace;color:var(--ink3);margin-top:4px}
.tc-delta{font-size:22px;font-weight:700;color:var(--teal-400);font-family:'DM Mono',monospace;margin-top:12px}
.tc-delta-lbl{font-size:11px;color:var(--ink3);text-transform:uppercase;letter-spacing:.06em}

/* ── HOW TO RUN ── */
.steps-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:20px;margin:32px 0}
.step-card{border-radius:16px;padding:28px 24px;border:1.5px solid var(--gray-100);background:#fff}
.step-card .step-num{font-size:32px;font-weight:700;color:var(--teal-100);font-family:'DM Serif Display',serif;line-height:1;margin-bottom:12px}
.step-card h3{font-size:16px;font-weight:600;margin-bottom:8px;color:var(--ink)}
.step-card p{font-size:14px;color:var(--ink3);line-height:1.6}
code.inline{font-family:'DM Mono',monospace;font-size:12px;background:var(--gray-50);border:1px solid var(--gray-100);padding:2px 6px;border-radius:4px;color:var(--ink2)}
pre.code-block{background:var(--teal-900);border-radius:14px;padding:24px;font-family:'DM Mono',monospace;font-size:12px;color:var(--teal-100);overflow-x:auto;line-height:1.8;margin:16px 0}
pre.code-block .kw{color:var(--teal-200)}
pre.code-block .cm{color:rgba(255,255,255,.3);font-style:italic}

/* ── DEPS ── */
.dep-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:14px;margin:24px 0}
.dep-item{display:flex;align-items:center;gap:12px;padding:14px 16px;background:rgba(255,255,255,.05);border-radius:12px;border:1px solid rgba(255,255,255,.08)}
.dep-name{font-family:'DM Mono',monospace;font-size:13px;font-weight:500;color:var(--teal-100);flex:0 0 130px}
.dep-desc{font-size:12px;color:rgba(255,255,255,.5)}

/* ── REFS ── */
.ref-list{margin:24px 0}
.ref-item{padding:16px 0;border-bottom:1px solid var(--gray-100);display:flex;gap:16px;align-items:flex-start}
.ref-num{font-family:'DM Mono',monospace;font-size:12px;color:var(--teal-400);font-weight:600;flex-shrink:0;margin-top:2px;width:24px}
.ref-text{font-size:14px;color:var(--ink3);line-height:1.6}
.ref-text strong{color:var(--ink);font-weight:600}

/* ── FOOTER ── */
.footer{background:var(--teal-900);color:rgba(255,255,255,.5);text-align:center;padding:60px 32px;font-size:13px}
.footer strong{color:#fff}

/* ── PROGRESS BAR ANIMATION ── */
@keyframes fillBar{from{width:0}to{width:var(--w)}}
.animate-bar{animation:fillBar .8s ease-out forwards}

/* ── CENTERED UTIL ── */
.text-center{text-align:center}

/* ── METRIC PILL ── */
.metric-pill{display:inline-flex;align-items:center;gap:6px;background:var(--teal-50);border:1px solid var(--teal-100);border-radius:999px;padding:6px 14px;font-size:13px;font-weight:500;color:var(--teal-600);font-family:'DM Mono',monospace}
.metric-pill .arrow{color:var(--teal-400)}
</style>
</head>
<body>

<!-- ═══ HERO ═══ -->
<div class="hero">
  <div class="hero-tag">College Portfolio Project</div>
  <h1>MedRisk<br/><em>Classifier</em></h1>
  <p class="hero-sub">A generalizable machine learning pipeline for chronic disease prediction across three independent clinical datasets — zero cost, fully open source.</p>
  <div class="badge-row">
    <span class="badge"><span class="dot"></span>Python 3.12</span>
    <span class="badge"><span class="dot"></span>XGBoost · LightGBM</span>
    <span class="badge"><span class="dot"></span>Optuna HPO</span>
    <span class="badge"><span class="dot"></span>SMOTE Balancing</span>
    <span class="badge"><span class="dot"></span>Gradio App</span>
    <span class="badge"><span class="dot"></span>Kaggle GPU T4</span>
  </div>
  <div class="cta-row">
    <a href="YOUR_GRADIO_LINK" class="btn-primary">&#x1F680; Live Demo</a>
    <a href="YOUR_KAGGLE_LINK" class="btn-secondary">&#x1F4D3; Open in Kaggle</a>
  </div>
</div>

<!-- ── WAVE DIVIDER ── -->
<svg class="wave" viewBox="0 0 1440 40" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none" style="background:var(--teal-900);margin-top:-1px"><path d="M0 0 Q360 40 720 20 Q1080 0 1440 30 L1440 40 L0 40Z" fill="#fafaf8"/></svg>

<!-- ── NAV ── -->
<nav class="nav-strip">
  <a href="#overview">Overview</a>
  <a href="#datasets">Datasets</a>
  <a href="#pipeline">Pipeline</a>
  <a href="#features">Features</a>
  <a href="#results">Results</a>
  <a href="#tuning">Tuning</a>
  <a href="#demo">Demo</a>
  <a href="#run">How to Run</a>
</nav>

<!-- ═══ OVERVIEW ═══ -->
<section id="overview">
  <div class="container text-center">
    <div class="section-tag"><span class="icon">&#x1F9E0;</span>Project Overview</div>
    <h2 class="section-title">One pipeline.<br/>Three datasets.</h2>
    <p class="section-lead">MedRisk Classifier demonstrates that a single well-engineered ML codebase can adapt to any tabular clinical dataset — handling class imbalance, missing values, categorical encoding, and heterogeneous feature schemas automatically.</p>

    <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin:48px 0">
      <div style="background:var(--teal-50);border:1.5px solid var(--teal-100);border-radius:16px;padding:32px 20px">
        <div style="font-size:40px;font-weight:700;color:var(--teal-400);font-family:'DM Mono',monospace;margin-bottom:8px">0.979</div>
        <div style="font-size:13px;font-weight:600;color:var(--teal-600);margin-bottom:4px">Best AUC Achieved</div>
        <div style="font-size:12px;color:var(--ink3)">LightGBM · Diabetes-Large</div>
      </div>
      <div style="background:var(--coral-50);border:1.5px solid var(--coral-100);border-radius:16px;padding:32px 20px">
        <div style="font-size:40px;font-weight:700;color:var(--coral-600);font-family:'DM Mono',monospace;margin-bottom:8px">101k</div>
        <div style="font-size:13px;font-weight:600;color:var(--coral-600);margin-bottom:4px">Total Patient Records</div>
        <div style="font-size:12px;color:var(--ink3)">Across all 3 datasets</div>
      </div>
      <div style="background:var(--purple-50);border:1.5px solid var(--purple-100);border-radius:16px;padding:32px 20px">
        <div style="font-size:40px;font-weight:700;color:var(--purple-600);font-family:'DM Mono',monospace;margin-bottom:8px">12</div>
        <div style="font-size:13px;font-weight:600;color:var(--purple-600);margin-bottom:4px">Models Trained</div>
        <div style="font-size:12px;color:var(--ink3)">4 classifiers × 3 datasets</div>
      </div>
    </div>

    <div style="background:var(--teal-900);border-radius:16px;padding:32px;text-align:left;margin-top:20px">
      <div style="font-size:11px;font-weight:600;letter-spacing:.1em;text-transform:uppercase;color:var(--teal-200);margin-bottom:16px">Why Sensitivity matters more than Accuracy</div>
      <p style="color:rgba(255,255,255,.7);font-size:15px;line-height:1.7">In medical classification, <span style="color:var(--teal-200);font-weight:600">a false negative costs more than a false positive</span>. Missing a diabetic patient is worse than over-referring a healthy one. This pipeline explicitly tracks and reports Sensitivity (true positive rate) alongside Specificity so the clinical tradeoff is always visible — not hidden inside a single accuracy number.</p>
    </div>
  </div>
</section>

<!-- ═══ DATASETS ═══ -->
<section id="datasets" class="alt">
  <div class="container text-center">
    <div class="section-tag"><span class="icon">&#x1F4CA;</span>Datasets</div>
    <h2 class="section-title">Three datasets.<br/>Three challenges.</h2>
    <p class="section-lead">Chosen for complementary properties — different sizes, class balances, and clinical domains — to stress-test generalizability.</p>

    <div class="dataset-grid">
      <div class="ds-card a">
        <span class="imbalance-badge">&#x26A0;&#xFE0F; 8.5% positive</span>
        <span class="ds-icon">&#x1FA78;</span>
        <h3>Diabetes Prediction</h3>
        <div class="ds-source">iammustafatz / Kaggle</div>
        <div class="ds-stats">
          <div class="ds-stat"><span class="val">100k</span><span class="lbl">Rows</span></div>
          <div class="ds-stat"><span class="val">8</span><span class="lbl">Features</span></div>
          <div class="ds-stat"><span class="val">LightGBM</span><span class="lbl">Winner</span></div>
        </div>
      </div>
      <div class="ds-card b">
        <span class="imbalance-badge">&#x2705; 46.1% positive</span>
        <span class="ds-icon">&#x2764;&#xFE0F;</span>
        <h3>Heart Disease Cleveland</h3>
        <div class="ds-source">cherngs / UCI ML Repo</div>
        <div class="ds-stats">
          <div class="ds-stat"><span class="val">297</span><span class="lbl">Rows</span></div>
          <div class="ds-stat"><span class="val">13</span><span class="lbl">Features</span></div>
          <div class="ds-stat"><span class="val">Log. Reg.</span><span class="lbl">Winner</span></div>
        </div>
      </div>
      <div class="ds-card c">
        <span class="imbalance-badge">&#x2705; 34.9% positive</span>
        <span class="ds-icon">&#x1F9EC;</span>
        <h3>Pima Indians Diabetes</h3>
        <div class="ds-source">uciml / UCI ML Repo</div>
        <div class="ds-stats">
          <div class="ds-stat"><span class="val">768</span><span class="lbl">Rows</span></div>
          <div class="ds-stat"><span class="val">8→16</span><span class="lbl">Features</span></div>
          <div class="ds-stat"><span class="val">XGBoost</span><span class="lbl">Winner</span></div>
        </div>
      </div>
    </div>

    <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:14px;text-align:left">
      <div style="background:#fff;border-radius:14px;padding:20px 18px;border:1.5px solid var(--gray-100)">
        <div style="font-size:11px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--amber-600);margin-bottom:8px">&#x26A0; Challenge: Imbalance</div>
        <p style="font-size:13px;color:var(--ink3);line-height:1.6">Diabetes-Large is 91.5% negative. SMOTE applied on training set only — test set stays untouched to reflect real-world distribution.</p>
      </div>
      <div style="background:#fff;border-radius:14px;padding:20px 18px;border:1.5px solid var(--gray-100)">
        <div style="font-size:11px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--coral-600);margin-bottom:8px">&#x26A0; Challenge: Small data</div>
        <p style="font-size:13px;color:var(--ink3);line-height:1.6">Heart-Cleveland has only 237 training rows. Complex ensembles overfit — Logistic Regression wins, confirming that simpler models generalize better on small data.</p>
      </div>
      <div style="background:#fff;border-radius:14px;padding:20px 18px;border:1.5px solid var(--gray-100)">
        <div style="font-size:11px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--purple-600);margin-bottom:8px">&#x26A0; Challenge: Impossible zeros</div>
        <p style="font-size:13px;color:var(--ink3);line-height:1.6">Pima's Glucose, BMI, and BloodPressure have biological zeros — physically impossible values used as missing-value codes. Replaced with column medians before any processing.</p>
      </div>
    </div>
  </div>
</section>

<!-- ═══ PIPELINE ═══ -->
<section id="pipeline">
  <div class="container text-center">
    <div class="section-tag"><span class="icon">&#x1F3D7;&#xFE0F;</span>Architecture</div>
    <h2 class="section-title">The full pipeline.</h2>
    <p class="section-lead">From raw CSV to deployed Gradio app — every step, in order.</p>

    <div class="diagram-wrap">
      <div class="diagram-header">
        <span class="dtitle">Pipeline — end-to-end flow</span>
        <div class="dpills"><div class="dpill" style="background:#FF6058"></div><div class="dpill" style="background:#FFBE2E"></div><div class="dpill" style="background:#2ACA44"></div></div>
      </div>
      <div class="diagram-body" style="padding:24px 16px">
        <svg width="100%" viewBox="0 0 840 560" role="img" xmlns="http://www.w3.org/2000/svg">
          <title>MedRisk pipeline architecture</title>
          <defs>
            <marker id="arr" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
              <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
            </marker>
          </defs>

          <!-- ROW 0: RAW DATA -->
          <rect x="310" y="10" width="220" height="44" rx="10" fill="#085041" stroke="#0F6E56" stroke-width="1"/>
          <text x="420" y="37" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="13" font-weight="600" fill="#9FE1CB">Raw CSV Files — 3 Datasets</text>

          <!-- arrow down -->
          <line x1="420" y1="54" x2="420" y2="80" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- ROW 1: 3 DATASET NODES -->
          <rect x="60" y="82" width="200" height="52" rx="10" fill="#E1F5EE" stroke="#5DCAA5" stroke-width="1"/>
          <text x="160" y="103" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#085041">Diabetes-Large</text>
          <text x="160" y="121" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#0F6E56">100k rows · 8 features</text>

          <rect x="310" y="82" width="220" height="52" rx="10" fill="#FAECE7" stroke="#F0997B" stroke-width="1"/>
          <text x="420" y="103" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#712B13">Heart-Cleveland</text>
          <text x="420" y="121" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#993C1D">297 rows · 13 features</text>

          <rect x="580" y="82" width="200" height="52" rx="10" fill="#EEEDFE" stroke="#AFA9EC" stroke-width="1"/>
          <text x="680" y="103" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#26215C">Pima Indians</text>
          <text x="680" y="121" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#534AB7">768 rows · 8 features</text>

          <!-- fan arrows from raw -->
          <path d="M420 54 L160 82" fill="none" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
          <path d="M420 54 L680 82" fill="none" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- ROW 2: PER-DATASET PREP -->
          <rect x="60" y="162" width="200" height="48" rx="10" fill="#FAEEDA" stroke="#FAC775" stroke-width="1"/>
          <text x="160" y="181" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" font-weight="600" fill="#633806">Encode categoricals</text>
          <text x="160" y="197" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#854F0B">gender + smoking_history</text>

          <rect x="310" y="162" width="220" height="48" rx="10" fill="#FAEEDA" stroke="#FAC775" stroke-width="1"/>
          <text x="420" y="181" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" font-weight="600" fill="#633806">Binarize target</text>
          <text x="420" y="197" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#854F0B">condition 0-4 → 0/1</text>

          <rect x="580" y="162" width="200" height="48" rx="10" fill="#FAEEDA" stroke="#FAC775" stroke-width="1"/>
          <text x="680" y="181" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" font-weight="600" fill="#633806">Impute zeros</text>
          <text x="680" y="197" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#854F0B">median replacement</text>

          <!-- down arrows -->
          <line x1="160" y1="134" x2="160" y2="162" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
          <line x1="420" y1="134" x2="420" y2="162" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
          <line x1="680" y1="134" x2="680" y2="162" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- MERGE ARROW into shared box -->
          <path d="M160 210 L160 248 L420 248" fill="none" stroke="#B4B2A9" stroke-width="1"/>
          <path d="M420 210 L420 248" fill="none" stroke="#B4B2A9" stroke-width="1"/>
          <path d="M680 210 L680 248 L420 248" fill="none" stroke="#B4B2A9" stroke-width="1"/>
          <line x1="420" y1="248" x2="420" y2="268" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- ROW 3: SHARED STEPS (3 boxes side by side) -->
          <rect x="100" y="270" width="180" height="52" rx="10" fill="#E6F1FB" stroke="#85B7EB" stroke-width="1"/>
          <text x="190" y="289" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#042C53">80/20 Split</text>
          <text x="190" y="307" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#185FA5">stratified by target</text>

          <rect x="320" y="270" width="200" height="52" rx="10" fill="#E6F1FB" stroke="#85B7EB" stroke-width="1"/>
          <text x="420" y="289" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#042C53">StandardScaler</text>
          <text x="420" y="307" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#185FA5">fit on train only</text>

          <rect x="560" y="270" width="180" height="52" rx="10" fill="#E6F1FB" stroke="#85B7EB" stroke-width="1"/>
          <text x="650" y="289" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#042C53">SMOTE</text>
          <text x="650" y="307" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#185FA5">training set only</text>

          <!-- arrows between shared steps -->
          <line x1="280" y1="296" x2="320" y2="296" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
          <line x1="520" y1="296" x2="560" y2="296" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- down from SMOTE block center -->
          <line x1="420" y1="322" x2="420" y2="358" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- ROW 4: MODELS -->
          <rect x="80" y="360" width="138" height="48" rx="10" fill="#085041" stroke="#1D9E75" stroke-width="1"/>
          <text x="149" y="388" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#9FE1CB">Logistic Reg.</text>

          <rect x="238" y="360" width="138" height="48" rx="10" fill="#085041" stroke="#1D9E75" stroke-width="1"/>
          <text x="307" y="388" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#9FE1CB">Random Forest</text>

          <rect x="396" y="360" width="138" height="48" rx="10" fill="#085041" stroke="#1D9E75" stroke-width="1"/>
          <text x="465" y="388" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#9FE1CB">XGBoost</text>

          <rect x="554" y="360" width="138" height="48" rx="10" fill="#085041" stroke="#1D9E75" stroke-width="1"/>
          <text x="623" y="388" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#9FE1CB">LightGBM</text>

          <!-- arrows from above into model row -->
          <path d="M420 358 L149 360" fill="none" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
          <path d="M420 358 L307 360" fill="none" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
          <path d="M420 358 L465 360" fill="none" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>
          <path d="M420 358 L623 360" fill="none" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- collect arrows -->
          <path d="M149 408 L149 448 L420 448" fill="none" stroke="#B4B2A9" stroke-width="1"/>
          <path d="M307 408 L307 448 L420 448" fill="none" stroke="#B4B2A9" stroke-width="1"/>
          <path d="M465 408 L465 448 L420 448" fill="none" stroke="#B4B2A9" stroke-width="1"/>
          <path d="M623 408 L623 448 L420 448" fill="none" stroke="#B4B2A9" stroke-width="1"/>
          <line x1="420" y1="448" x2="420" y2="466" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- ROW 5: EVALUATE + OPTUNA -->
          <rect x="220" y="468" width="180" height="48" rx="10" fill="#FAECE7" stroke="#F0997B" stroke-width="1"/>
          <text x="310" y="487" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#712B13">Evaluate</text>
          <text x="310" y="503" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#993C1D">AUC · F1 · Sens · Spec</text>

          <rect x="440" y="468" width="180" height="48" rx="10" fill="#FAECE7" stroke="#F0997B" stroke-width="1"/>
          <text x="530" y="487" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="12" font-weight="600" fill="#712B13">Optuna Tuning</text>
          <text x="530" y="503" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="11" fill="#993C1D">50–100 trials per model</text>

          <line x1="400" y1="492" x2="440" y2="492" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- Final arrow to deploy -->
          <path d="M530 516 L530 540 L420 540" fill="none" stroke="#B4B2A9" stroke-width="1" marker-end="url(#arr)"/>

          <!-- ROW 6: DEPLOY -->
          <rect x="300" y="516" width="240" height="40" rx="10" fill="#D85A30" stroke="#993C1D" stroke-width="1"/>
          <text x="420" y="536" text-anchor="middle" dominant-baseline="central" font-family="'Outfit',sans-serif" font-size="13" font-weight="700" fill="#fff">Gradio App — Kaggle Deploy</text>
        </svg>
      </div>
    </div>
  </div>
</section>

<!-- ═══ FEATURE ENGINEERING ═══ -->
<section id="features" class="alt">
  <div class="container text-center">
    <div class="section-tag"><span class="icon">&#x2699;&#xFE0F;</span>Feature Engineering</div>
    <h2 class="section-title">Raw features weren't enough.<br/>So we built better ones.</h2>
    <p class="section-lead">Applied exclusively to Pima Indians — the weakest performer — using clinical domain knowledge to construct 8 new features from the original 8.</p>

    <div class="fe-grid">
      <div class="fe-card original">
        <h4>Original features (8)</h4>
        <span class="fe-tag">Pregnancies</span><span class="fe-tag">Glucose</span><span class="fe-tag">BloodPressure</span>
        <span class="fe-tag">SkinThickness</span><span class="fe-tag">Insulin</span><span class="fe-tag">BMI</span>
        <span class="fe-tag">DiabetesPedigreeFunction</span><span class="fe-tag">Age</span>
        <p class="fe-note">After zero-imputation with column medians (374 impossible insulin values, 227 skin values replaced).</p>
      </div>
      <div class="fe-card interaction">
        <h4>Interaction features (4)</h4>
        <span class="fe-tag">glucose_bmi</span><span class="fe-tag">bp_age</span>
        <span class="fe-tag">age_pregnancies</span><span class="fe-tag">insulin_glucose</span>
        <p class="fe-note">Clinically motivated products and ratios — glucose×BMI captures insulin resistance, BP×Age captures cardiovascular stress.</p>
      </div>
      <div class="fe-card ratio">
        <h4>Ratio features (2)</h4>
        <span class="fe-tag">glucose_bmi_ratio</span><span class="fe-tag">skin_bmi_ratio</span>
        <p class="fe-note">Thin patients with high glucose have a distinct risk profile invisible to either feature alone. Skin-to-BMI ratio is an adiposity proxy.</p>
      </div>
      <div class="fe-card binned">
        <h4>Clinical bins (2)</h4>
        <span class="fe-tag">bmi_bin</span><span class="fe-tag">glucose_bin</span>
        <p class="fe-note">WHO BMI thresholds (under/normal/over/obese) and clinical glucose thresholds (normal / pre-diabetic / diabetic) encoded as ordinal integers.</p>
      </div>
    </div>

    <div style="background:#fff;border-radius:16px;padding:28px;border:1.5px solid var(--gray-100);text-align:left;margin-top:8px">
      <div style="font-size:12px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--ink3);margin-bottom:16px">AUC progression on Pima</div>
      <div style="display:flex;flex-direction:column;gap:14px">
        <div>
          <div style="display:flex;justify-content:space-between;font-size:13px;color:var(--ink2);margin-bottom:6px"><span>Baseline XGBoost (8 features)</span><span style="font-family:'DM Mono',monospace;font-weight:600">0.823</span></div>
          <div style="height:8px;background:var(--gray-100);border-radius:999px"><div style="height:8px;background:var(--gray-300);border-radius:999px;width:82.3%"></div></div>
        </div>
        <div>
          <div style="display:flex;justify-content:space-between;font-size:13px;color:var(--ink2);margin-bottom:6px"><span>Tuned XGBoost (8 features)</span><span style="font-family:'DM Mono',monospace;font-weight:600">0.825</span></div>
          <div style="height:8px;background:var(--gray-100);border-radius:999px"><div style="height:8px;background:var(--teal-200);border-radius:999px;width:82.5%"></div></div>
        </div>
        <div>
          <div style="display:flex;justify-content:space-between;font-size:13px;color:var(--teal-600);font-weight:600;margin-bottom:6px"><span>Tuned XGBoost (16 engineered features)</span><span style="font-family:'DM Mono',monospace">0.838</span></div>
          <div style="height:8px;background:var(--gray-100);border-radius:999px"><div style="height:8px;background:var(--teal-400);border-radius:999px;width:83.8%"></div></div>
        </div>
      </div>
      <p style="font-size:12px;color:var(--ink3);margin-top:16px;font-style:italic">Feature engineering (+0.015 AUC) outperformed hyperparameter tuning alone (+0.002) — domain knowledge beats search.</p>
    </div>
  </div>
</section>

<!-- ═══ RESULTS ═══ -->
<section id="results">
  <div class="container text-center">
    <div class="section-tag"><span class="icon">&#x1F3C6;</span>Results</div>
    <h2 class="section-title">Every model.<br/>Every metric.</h2>
    <p class="section-lead">Four classifiers trained per dataset. Evaluated on Accuracy, ROC-AUC, F1, Sensitivity, and Specificity.</p>

    <!-- LEADERBOARD -->
    <div class="leaderboard">
      <div class="lb-card gold">
        <div class="lb-rank">&#x1FA78;</div>
        <div class="lb-dataset">Diabetes-Large</div>
        <div class="lb-model">LightGBM</div>
        <div class="lb-metrics">
          <div class="lb-metric"><span class="mv">0.979</span><span class="mk">AUC</span></div>
          <div class="lb-metric"><span class="mv">0.804</span><span class="mk">F1</span></div>
          <div class="lb-metric"><span class="mv">0.709</span><span class="mk">Sensitivity</span></div>
          <div class="lb-metric"><span class="mv">0.995</span><span class="mk">Specificity</span></div>
        </div>
      </div>
      <div class="lb-card gold">
        <div class="lb-rank">&#x2764;&#xFE0F;</div>
        <div class="lb-dataset">Heart-Cleveland</div>
        <div class="lb-model">Logistic Regression</div>
        <div class="lb-metrics">
          <div class="lb-metric"><span class="mv">0.958</span><span class="mk">AUC</span></div>
          <div class="lb-metric"><span class="mv">0.902</span><span class="mk">F1</span></div>
          <div class="lb-metric"><span class="mv">0.821</span><span class="mk">Sensitivity</span></div>
          <div class="lb-metric"><span class="mv">1.000</span><span class="mk">Specificity</span></div>
        </div>
      </div>
      <div class="lb-card gold">
        <div class="lb-rank">&#x1F9EC;</div>
        <div class="lb-dataset">Pima Indians</div>
        <div class="lb-model">XGBoost + FE</div>
        <div class="lb-metrics">
          <div class="lb-metric"><span class="mv">0.838</span><span class="mk">AUC</span></div>
          <div class="lb-metric"><span class="mv">0.649</span><span class="mk">F1</span></div>
          <div class="lb-metric"><span class="mv">0.685</span><span class="mk">Sensitivity</span></div>
          <div class="lb-metric"><span class="mv">0.770</span><span class="mk">Specificity</span></div>
        </div>
      </div>
    </div>

    <!-- FULL TABLES -->
    <div style="text-align:left">
      <div class="diagram-wrap">
        <div class="diagram-header">
          <span class="dtitle">Full model comparison — all datasets</span>
          <div class="dpills"><div class="dpill" style="background:#1D9E75"></div><div class="dpill" style="background:#D85A30"></div><div class="dpill" style="background:#378ADD"></div></div>
        </div>
        <div style="overflow-x:auto">
          <table class="model-table">
            <thead><tr><th>Dataset</th><th>Model</th><th>AUC</th><th>F1</th><th>Sensitivity</th><th>Specificity</th><th>Train Time</th></tr></thead>
            <tbody>
              <tr class="table-group-head"><td colspan="7">&#x1FA78; Diabetes-Large — 100k rows · 8 features · LightGBM T4 GPU</td></tr>
              <tr><td>Diabetes-Large</td><td>Logistic Regression</td><td class="num">0.962</td><td class="num">0.571</td><td class="num">0.888</td><td class="num">0.887</td><td class="num">0.3s</td></tr>
              <tr><td>Diabetes-Large</td><td>Random Forest</td><td class="num">0.974</td><td class="num">0.686</td><td class="num">0.834</td><td class="num">0.945</td><td class="num">11.7s</td></tr>
              <tr><td>Diabetes-Large</td><td>XGBoost</td><td class="num">0.978</td><td class="num">0.780</td><td class="num">0.762</td><td class="num">0.982</td><td class="num">1.1s</td></tr>
              <tr class="winner"><td>Diabetes-Large</td><td><span class="star">&#x2B50;</span> LightGBM</td><td class="num" style="color:var(--teal-600);font-weight:700">0.978</td><td class="num" style="color:var(--teal-600);font-weight:700">0.804</td><td class="num">0.709</td><td class="num" style="color:var(--teal-600);font-weight:700">0.995</td><td class="num">2.0s</td></tr>
              <tr class="table-group-head"><td colspan="7">&#x2764;&#xFE0F; Heart-Cleveland — 297 rows · 13 features · LR wins on small data</td></tr>
              <tr class="winner"><td>Heart-Cleveland</td><td><span class="star">&#x2B50;</span> Logistic Regression</td><td class="num" style="color:var(--teal-600);font-weight:700">0.954</td><td class="num" style="color:var(--teal-600);font-weight:700">0.902</td><td class="num">0.821</td><td class="num" style="color:var(--teal-600);font-weight:700">1.000</td><td class="num">0.0s</td></tr>
              <tr><td>Heart-Cleveland</td><td>LightGBM</td><td class="num">0.949</td><td class="num">0.852</td><td class="num">0.821</td><td class="num">0.906</td><td class="num">0.1s</td></tr>
              <tr><td>Heart-Cleveland</td><td>XGBoost</td><td class="num">0.934</td><td class="num">0.846</td><td class="num">0.786</td><td class="num">0.938</td><td class="num">0.1s</td></tr>
              <tr><td>Heart-Cleveland</td><td>Random Forest</td><td class="num">0.941</td><td class="num">0.800</td><td class="num">0.714</td><td class="num">0.938</td><td class="num">0.6s</td></tr>
              <tr class="table-group-head"><td colspan="7">&#x1F9EC; Pima Indians — 768 rows · 8→16 features · Feature engineering applied</td></tr>
              <tr class="winner"><td>Pima Indians</td><td><span class="star">&#x2B50;</span> XGBoost + FE</td><td class="num" style="color:var(--teal-600);font-weight:700">0.838</td><td class="num">0.649</td><td class="num">0.685</td><td class="num">0.770</td><td class="num">14.4s</td></tr>
              <tr><td>Pima Indians</td><td>LightGBM</td><td class="num">0.816</td><td class="num">0.637</td><td class="num">0.667</td><td class="num">0.770</td><td class="num">0.2s</td></tr>
              <tr><td>Pima Indians</td><td>XGBoost baseline</td><td class="num">0.823</td><td class="num">0.649</td><td class="num">0.685</td><td class="num">0.770</td><td class="num">0.2s</td></tr>
              <tr><td>Pima Indians</td><td>Logistic Regression</td><td class="num">0.811</td><td class="num">0.621</td><td class="num">0.667</td><td class="num">0.740</td><td class="num">0.0s</td></tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

    <div style="background:var(--teal-50);border:1.5px solid var(--teal-100);border-radius:14px;padding:22px 24px;text-align:left;margin-top:8px">
      <p style="font-size:14px;color:var(--teal-800);line-height:1.7"><strong>Key insight — dataset size dictates model choice.</strong> On Heart-Cleveland with only 237 training rows, Logistic Regression outperformed every ensemble method. Pima's ceiling of 0.838 AUC reflects genuine data limitations (1988 dataset, noisy measurements, 768 samples) — not a pipeline failure. Honest results are more valuable than inflated ones.</p>
    </div>
  </div>
</section>

<!-- ═══ TUNING ═══ -->
<section id="tuning" class="alt">
  <div class="container text-center">
    <div class="section-tag"><span class="icon">&#x1F52C;</span>Hyperparameter Tuning</div>
    <h2 class="section-title">Optuna TPE.<br/>50–100 trials each.</h2>
    <p class="section-lead">Tree-structured Parzen Estimator — probabilistic search that learns from past trials to focus on promising regions of the hyperparameter space.</p>

    <div class="tune-compare">
      <div class="tc-card">
        <h4>Diabetes-Large</h4>
        <div class="tc-model">LightGBM</div>
        <div style="font-size:11px;color:var(--ink3);text-align:left;margin-bottom:12px">ROC-AUC</div>
        <div style="position:relative;height:6px;background:var(--gray-100);border-radius:999px;margin-bottom:4px">
          <div style="position:absolute;top:0;left:0;height:6px;background:var(--gray-300);border-radius:999px;width:97.81%"></div>
        </div>
        <div style="position:relative;height:6px;background:var(--gray-100);border-radius:999px">
          <div style="position:absolute;top:0;left:0;height:6px;background:var(--teal-400);border-radius:999px;width:97.92%"></div>
        </div>
        <div class="tc-nums"><span style="color:var(--gray-400)">0.9781</span><span style="color:var(--teal-600)">0.9792</span></div>
        <div class="tc-delta">+0.0011</div>
        <div class="tc-delta-lbl">AUC gain</div>
      </div>
      <div class="tc-card">
        <h4>Heart-Cleveland</h4>
        <div class="tc-model">Logistic Regression</div>
        <div style="font-size:11px;color:var(--ink3);text-align:left;margin-bottom:12px">ROC-AUC</div>
        <div style="position:relative;height:6px;background:var(--gray-100);border-radius:999px;margin-bottom:4px">
          <div style="position:absolute;top:0;left:0;height:6px;background:var(--gray-300);border-radius:999px;width:95.42%"></div>
        </div>
        <div style="position:relative;height:6px;background:var(--gray-100);border-radius:999px">
          <div style="position:absolute;top:0;left:0;height:6px;background:var(--teal-400);border-radius:999px;width:95.76%"></div>
        </div>
        <div class="tc-nums"><span style="color:var(--gray-400)">0.9542</span><span style="color:var(--teal-600)">0.9576</span></div>
        <div class="tc-delta">+0.0034</div>
        <div class="tc-delta-lbl">AUC gain</div>
      </div>
      <div class="tc-card">
        <h4>Pima Indians</h4>
        <div class="tc-model">XGBoost + FE</div>
        <div style="font-size:11px;color:var(--ink3);text-align:left;margin-bottom:12px">ROC-AUC</div>
        <div style="position:relative;height:6px;background:var(--gray-100);border-radius:999px;margin-bottom:4px">
          <div style="position:absolute;top:0;left:0;height:6px;background:var(--gray-300);border-radius:999px;width:82.30%"></div>
        </div>
        <div style="position:relative;height:6px;background:var(--gray-100);border-radius:999px">
          <div style="position:absolute;top:0;left:0;height:6px;background:var(--teal-400);border-radius:999px;width:83.83%"></div>
        </div>
        <div class="tc-nums"><span style="color:var(--gray-400)">0.8230</span><span style="color:var(--teal-600)">0.8383</span></div>
        <div class="tc-delta">+0.0153</div>
        <div class="tc-delta-lbl">AUC gain (incl. FE)</div>
      </div>
    </div>
  </div>
</section>

<!-- ═══ LIVE DEMO ═══ -->
<section id="demo" class="dark">
  <div class="container text-center">
    <div class="section-tag"><span class="icon">&#x1F680;</span>Live Demo</div>
    <h2 class="section-title">Try it right now.</h2>
    <p class="section-lead">Three-tab Gradio app deployed on Kaggle. No login required.</p>

    <div style="background:rgba(255,255,255,.06);border:1.5px solid rgba(255,255,255,.12);border-radius:20px;padding:40px;margin:32px 0">
      <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-bottom:36px">
        <div style="background:rgba(255,255,255,.05);border-radius:14px;padding:24px 20px">
          <div style="font-size:28px;margin-bottom:12px">&#x1FA78;</div>
          <div style="font-size:14px;font-weight:600;color:#fff;margin-bottom:6px">Diabetes Risk</div>
          <div style="font-size:12px;color:rgba(255,255,255,.5)">LightGBM · 8 inputs</div>
        </div>
        <div style="background:rgba(255,255,255,.05);border-radius:14px;padding:24px 20px">
          <div style="font-size:28px;margin-bottom:12px">&#x2764;&#xFE0F;</div>
          <div style="font-size:14px;font-weight:600;color:#fff;margin-bottom:6px">Heart Disease</div>
          <div style="font-size:12px;color:rgba(255,255,255,.5)">Logistic Reg. · 13 inputs</div>
        </div>
        <div style="background:rgba(255,255,255,.05);border-radius:14px;padding:24px 20px">
          <div style="font-size:28px;margin-bottom:12px">&#x1F9EC;</div>
          <div style="font-size:14px;font-weight:600;color:#fff;margin-bottom:6px">Pima Diabetes</div>
          <div style="font-size:12px;color:rgba(255,255,255,.5)">XGBoost · 8 inputs</div>
        </div>
      </div>
      <div style="display:flex;flex-direction:column;gap:10px;text-align:left;margin-bottom:32px">
        <div style="display:flex;align-items:center;gap:12px;font-size:14px;color:rgba(255,255,255,.7)"><span style="width:24px;height:24px;background:var(--teal-400);border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;color:#fff;flex-shrink:0">1</span>Pick a tab for your use case</div>
        <div style="display:flex;align-items:center;gap:12px;font-size:14px;color:rgba(255,255,255,.7)"><span style="width:24px;height:24px;background:var(--teal-400);border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;color:#fff;flex-shrink:0">2</span>Adjust the clinical sliders to match patient values</div>
        <div style="display:flex;align-items:center;gap:12px;font-size:14px;color:rgba(255,255,255,.7)"><span style="width:24px;height:24px;background:var(--teal-400);border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;color:#fff;flex-shrink:0">3</span>Click Predict — get a color-coded risk score instantly</div>
      </div>
      <div style="display:flex;gap:12px;justify-content:center;flex-wrap:wrap;margin-bottom:24px">
        <div style="background:rgba(29,158,117,.2);border:1px solid rgba(29,158,117,.4);border-radius:10px;padding:12px 20px;font-size:13px;color:#9FE1CB">&#x1F7E2; &lt; 20% — Low Risk</div>
        <div style="background:rgba(186,117,23,.2);border:1px solid rgba(186,117,23,.4);border-radius:10px;padding:12px 20px;font-size:13px;color:#FAC775">&#x1F7E1; 20–50% — Moderate Risk</div>
        <div style="background:rgba(216,90,48,.2);border:1px solid rgba(216,90,48,.4);border-radius:10px;padding:12px 20px;font-size:13px;color:#F0997B">&#x1F534; &gt; 50% — High Risk</div>
      </div>
      <a href="YOUR_GRADIO_LINK" class="btn-primary" style="display:inline-flex">&#x1F680; Launch Live Demo</a>
      <p style="font-size:11px;color:rgba(255,255,255,.3);margin-top:16px">For educational purposes only. Not a medical device. Consult a qualified healthcare professional.</p>
    </div>
  </div>
</section>

<!-- ═══ HOW TO RUN ═══ -->
<section id="run">
  <div class="container text-center">
    <div class="section-tag"><span class="icon">&#x25B6;&#xFE0F;</span>How to Run</div>
    <h2 class="section-title">Up and running<br/>in minutes.</h2>
    <p class="section-lead">Two paths — Kaggle (recommended, free GPU included) or local.</p>

    <div class="steps-grid">
      <div class="step-card" style="border-color:var(--teal-100)">
        <div class="step-num" style="color:var(--teal-200)">A</div>
        <h3>Kaggle — Recommended</h3>
        <p>Open the notebook, fork it, click Run All. GPU T4 included free. The Gradio app launches in the last cell output with a public link.</p>
        <div style="margin-top:16px;display:flex;flex-direction:column;gap:6px">
          <code class="inline">iammustafatz/diabetes-prediction-dataset</code>
          <code class="inline">cherngs/heart-disease-cleveland-uci</code>
          <code class="inline">uciml/pima-indians-diabetes-database</code>
        </div>
      </div>
      <div class="step-card">
        <div class="step-num">B</div>
        <h3>Local Setup</h3>
        <p>Clone the repo, install dependencies, update dataset paths in Snippet 1, run the notebook.</p>
        <pre class="code-block" style="margin-top:16px"><span class="kw">pip install</span> numpy pandas matplotlib seaborn \
          scikit-learn imbalanced-learn \
          xgboost lightgbm optuna gradio</pre>
      </div>
    </div>

    <div style="margin-top:8px;background:var(--teal-900);border-radius:16px;padding:32px;text-align:left">
      <div style="font-size:11px;font-weight:600;letter-spacing:.1em;text-transform:uppercase;color:var(--teal-200);margin-bottom:20px">Dependencies</div>
      <div class="dep-grid">
        <div class="dep-item"><span class="dep-name">scikit-learn</span><span class="dep-desc">Preprocessing, metrics, Stacking</span></div>
        <div class="dep-item"><span class="dep-name">xgboost</span><span class="dep-desc">Gradient boosting with GPU (CUDA hist)</span></div>
        <div class="dep-item"><span class="dep-name">lightgbm</span><span class="dep-desc">Histogram-based boosting, fast at scale</span></div>
        <div class="dep-item"><span class="dep-name">imbalanced-learn</span><span class="dep-desc">SMOTE oversampling</span></div>
        <div class="dep-item"><span class="dep-name">optuna</span><span class="dep-desc">Bayesian HPO via TPE sampler</span></div>
        <div class="dep-item"><span class="dep-name">gradio</span><span class="dep-desc">Interactive web app + share link</span></div>
        <div class="dep-item"><span class="dep-name">pandas / numpy</span><span class="dep-desc">Data manipulation</span></div>
        <div class="dep-item"><span class="dep-name">matplotlib / seaborn</span><span class="dep-desc">All visualizations (13 plot files)</span></div>
      </div>
    </div>
  </div>
</section>

<!-- ═══ REFERENCES ═══ -->
<section class="alt">
  <div class="container">
    <div class="text-center" style="margin-bottom:40px">
      <div class="section-tag"><span class="icon">&#x1F4DA;</span>References</div>
      <h2 class="section-title">Standing on the<br/>shoulders of giants.</h2>
    </div>
    <div class="ref-list">
      <div class="ref-item"><span class="ref-num">[1]</span><span class="ref-text"><strong>Smith, J.W. et al. (1988).</strong> Using the ADAP learning algorithm to forecast the onset of diabetes mellitus. Proceedings of the Annual Symposium on Computer Application in Medical Care. <em>Pima Indians Diabetes Database — UCI ML Repository.</em></span></div>
      <div class="ref-item"><span class="ref-num">[2]</span><span class="ref-text"><strong>Detrano, R. et al. (1989).</strong> International application of a new probability algorithm for the diagnosis of coronary artery disease. <em>American Journal of Cardiology, 64(5), 304–310.</em> Heart Disease Cleveland UCI Dataset.</span></div>
      <div class="ref-item"><span class="ref-num">[3]</span><span class="ref-text"><strong>Mustafa, T. (2023).</strong> Diabetes Prediction Dataset — 100,000 patient records. <em>Kaggle.</em> kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset</span></div>
      <div class="ref-item"><span class="ref-num">[4]</span><span class="ref-text"><strong>Chawla, N.V. et al. (2002).</strong> SMOTE: Synthetic Minority Over-sampling Technique. <em>Journal of Artificial Intelligence Research, 16, 321–357.</em></span></div>
      <div class="ref-item"><span class="ref-num">[5]</span><span class="ref-text"><strong>Akiba, T. et al. (2019).</strong> Optuna: A Next-generation Hyperparameter Optimization Framework. <em>Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining.</em></span></div>
    </div>
  </div>
</section>

<!-- ═══ FOOTER ═══ -->
<svg viewBox="0 0 1440 40" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none" style="display:block;background:var(--gray-50);margin-bottom:-1px"><path d="M0 40 Q360 0 720 20 Q1080 40 1440 10 L1440 40 L0 40Z" fill="#04342C"/></svg>
<div class="footer">
  <div style="font-size:28px;margin-bottom:16px">&#x1F3E5;</div>
  <p style="margin-bottom:8px"><strong>MedRisk Classifier</strong> — Built for open science</p>
  <p>All datasets public · All tools free &amp; open source · Kaggle GPU T4</p>
  <div style="margin-top:24px;display:flex;justify-content:center;gap:20px;flex-wrap:wrap">
    <a href="https://github.com/YOUR_USERNAME" style="color:var(--teal-200);text-decoration:none;font-size:13px">GitHub</a>
    <a href="https://kaggle.com/YOUR_USERNAME" style="color:var(--teal-200);text-decoration:none;font-size:13px">Kaggle</a>
    <a href="YOUR_GRADIO_LINK" style="color:var(--teal-200);text-decoration:none;font-size:13px">Live Demo</a>
  </div>
</div>

</body>
</html>
