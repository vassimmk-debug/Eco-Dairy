<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AgriLait — AI-Powered Dairy Consulting Platform</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=Instrument+Sans:wght@400;500;600&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2.39.7/dist/umd/supabase.min.js"></script>
<style>
*{margin:0;padding:0;box-sizing:border-box}
:root{
  --ink:#0e1a0f;--ink2:#3a5a3b;--ink3:#6b8e6c;--surface:#f9faf7;--surface2:#f0f4ed;--surface3:#e5ede0;
  --green:#2d6a2e;--green2:#3d8a3e;--green3:#4caf50;--green4:#c8e6c9;--green5:#e8f5e9;
  --teal:#1b6b5e;--teal2:#c3e6df;--earth2:#f3e9c6;--blue:#1a3c8b;--blue2:#d1dff5;
  --red:#c0392b;--amber:#d4790a;
  --border:rgba(45,106,46,0.15);--border2:rgba(45,106,46,0.25);
  --shadow:0 1px 3px rgba(14,26,15,0.08),0 4px 16px rgba(14,26,15,0.04);
  --shadow2:0 2px 8px rgba(14,26,15,0.12),0 8px 32px rgba(14,26,15,0.06);
}
body{font-family:'Instrument Sans',sans-serif;background:var(--surface);color:var(--ink);font-size:14px;line-height:1.6;overflow-x:hidden}

/* NAV */
nav{background:rgba(249,250,247,0.96);backdrop-filter:blur(12px);border-bottom:1px solid var(--border);padding:0 32px;display:flex;align-items:center;gap:28px;height:60px;position:sticky;top:0;z-index:100}
.logo{display:flex;align-items:center;gap:10px;cursor:pointer;flex-shrink:0}
.logo-mark{width:32px;height:32px;background:var(--green);border-radius:8px;display:flex;align-items:center;justify-content:center}
.logo-text{font-family:'DM Serif Display',serif;font-size:18px;color:var(--ink)}
.logo-text span{color:var(--green2)}
nav a{font-size:13px;color:var(--ink2);text-decoration:none;font-weight:500;padding:4px 0;border-bottom:2px solid transparent;transition:all .2s;cursor:pointer;white-space:nowrap}
nav a:hover,nav a.active{color:var(--green);border-bottom-color:var(--green)}
.nav-right{margin-left:auto;display:flex;align-items:center;gap:10px;flex-shrink:0}
.lang-switcher{display:flex;gap:4px;background:var(--surface2);border-radius:6px;padding:3px}
.lang-btn{padding:3px 8px;border-radius:4px;font-size:11px;font-weight:600;cursor:pointer;border:none;background:transparent;color:var(--ink3);transition:all .2s}
.lang-btn.active{background:#fff;color:var(--green);box-shadow:var(--shadow)}
.btn-ghost{padding:6px 14px;border:1px solid var(--border2);border-radius:6px;font-size:13px;font-weight:500;color:var(--ink2);background:transparent;cursor:pointer;transition:all .2s;font-family:'Instrument Sans',sans-serif}
.btn-ghost:hover{background:var(--surface2)}
.btn-primary{padding:7px 16px;background:var(--green);border:none;border-radius:6px;font-size:13px;font-weight:600;color:#fff;cursor:pointer;transition:all .2s;font-family:'Instrument Sans',sans-serif}
.btn-primary:hover{background:var(--green2)}
.user-pill{display:flex;align-items:center;gap:8px;padding:5px 12px;background:var(--green5);border:1px solid var(--green4);border-radius:100px;font-size:12px;font-weight:600;color:var(--green)}
.user-dot{width:7px;height:7px;background:var(--green3);border-radius:50%}

/* TABS */
.tab-bar{background:var(--surface);border-bottom:1px solid var(--border);padding:0 32px;display:flex;gap:0;overflow-x:auto}
.tab{padding:14px 20px;font-size:13px;font-weight:500;color:var(--ink3);cursor:pointer;border-bottom:2px solid transparent;white-space:nowrap;transition:all .2s}
.tab.active{color:var(--green);border-bottom-color:var(--green)}

/* VIEWS */
.view{display:none;animation:fadeIn .3s ease}
.view.active{display:block}
@keyframes fadeIn{from{opacity:0;transform:translateY(4px)}to{opacity:1;transform:translateY(0)}}

/* MODAL */
.modal-overlay{position:fixed;inset:0;background:rgba(14,26,15,0.6);backdrop-filter:blur(4px);z-index:200;display:flex;align-items:center;justify-content:center;opacity:0;pointer-events:none;transition:opacity .2s}
.modal-overlay.open{opacity:1;pointer-events:all}
.modal{background:var(--surface);border-radius:16px;padding:36px;width:420px;max-width:92vw;box-shadow:var(--shadow2);transform:translateY(8px);transition:transform .2s;position:relative}
.modal-overlay.open .modal{transform:translateY(0)}
.modal-title{font-family:'DM Serif Display',serif;font-size:26px;color:var(--ink);margin-bottom:6px}
.modal-sub{font-size:13px;color:var(--ink3);margin-bottom:24px}
.modal-tabs{display:flex;gap:0;border-bottom:1px solid var(--border);margin-bottom:24px}
.modal-tab{padding:8px 20px;font-size:13px;font-weight:500;color:var(--ink3);cursor:pointer;border-bottom:2px solid transparent;transition:all .2s}
.modal-tab.active{color:var(--green);border-bottom-color:var(--green)}
.modal-close{position:absolute;top:14px;right:14px;width:28px;height:28px;border-radius:50%;border:none;background:var(--surface2);cursor:pointer;font-size:14px;color:var(--ink3)}
.fg{display:flex;flex-direction:column;gap:6px;margin-bottom:14px}
.fg label{font-size:12px;font-weight:600;color:var(--ink2)}
.fg input,.fg select,.fg textarea{padding:10px 14px;border:1px solid var(--border2);border-radius:8px;font-size:13px;font-family:'Instrument Sans',sans-serif;color:var(--ink);background:#fff;outline:none;transition:all .2s;width:100%}
.fg input:focus,.fg select:focus,.fg textarea:focus{border-color:var(--green3);box-shadow:0 0 0 3px rgba(76,175,80,0.12)}
.auth-btn{width:100%;padding:11px;background:var(--green);border:none;border-radius:8px;font-size:14px;font-weight:600;color:#fff;cursor:pointer;font-family:'Instrument Sans',sans-serif;transition:all .2s;margin-top:4px}
.auth-btn:hover{background:var(--green2)}
.auth-btn:disabled{opacity:0.6;cursor:not-allowed}
.msg{font-size:12px;text-align:center;margin-top:10px;padding:8px 12px;border-radius:6px;display:none}
.msg.error{background:#ffebee;color:#c62828;display:block}
.msg.success{background:var(--green5);color:var(--green);display:block}

/* TOAST */
.toast{position:fixed;bottom:24px;right:24px;background:var(--ink);color:#fff;padding:12px 20px;border-radius:10px;font-size:13px;font-weight:500;z-index:300;transform:translateY(80px);opacity:0;transition:all .3s;max-width:300px}
.toast.show{transform:translateY(0);opacity:1}
.toast.green{background:var(--green)}

/* HERO */
.hero{background:linear-gradient(145deg,#0e1a0f 0%,#1a3a1b 40%,#1b6b5e 100%);padding:80px 32px;position:relative;overflow:hidden;min-height:480px;display:flex;align-items:center}
.hero-bg{position:absolute;inset:0;opacity:0.04;background-image:radial-gradient(circle at 2px 2px,#fff 1px,transparent 0);background-size:28px 28px}
.hero-orb{position:absolute;right:-80px;top:-80px;width:480px;height:480px;border-radius:50%;background:radial-gradient(circle,rgba(76,175,80,0.18) 0%,transparent 70%)}
.hero-orb2{position:absolute;right:200px;bottom:-100px;width:300px;height:300px;border-radius:50%;background:radial-gradient(circle,rgba(27,107,94,0.2) 0%,transparent 70%)}
.hero-content{position:relative;z-index:1;max-width:580px}

.hero-eyebrow{display:inline-flex;align-items:center;gap:8px;background:rgba(76,175,80,0.15);border:1px solid rgba(76,175,80,0.3);border-radius:100px;padding:5px 14px;font-size:12px;font-weight:600;color:#81c784;letter-spacing:0.5px;margin-bottom:24px}
.hero-dot{width:6px;height:6px;background:#4caf50;border-radius:50%;animation:pulse 2s infinite}
@keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:0.5;transform:scale(0.8)}}
.hero h1{font-family:'DM Serif Display',serif;font-size:48px;line-height:1.1;color:#fff;letter-spacing:-1px;margin-bottom:20px}
.hero h1 em{font-style:italic;color:#81c784}
.hero p{font-size:16px;color:rgba(255,255,255,0.65);line-height:1.7;margin-bottom:36px;max-width:500px}
.hero-cta{display:flex;gap:12px;flex-wrap:wrap}
.btn-hero{padding:12px 28px;background:#4caf50;border:none;border-radius:8px;font-size:14px;font-weight:600;color:#fff;cursor:pointer;font-family:'Instrument Sans',sans-serif;transition:all .2s}
.btn-hero:hover{background:#66bb6a;transform:translateY(-1px)}
.btn-hero-outline{padding:12px 28px;background:rgba(255,255,255,0.08);border:1px solid rgba(255,255,255,0.2);border-radius:8px;font-size:14px;font-weight:500;color:rgba(255,255,255,0.8);cursor:pointer;font-family:'Instrument Sans',sans-serif;transition:all .2s}
.btn-hero-outline:hover{background:rgba(255,255,255,0.14)}
.hero-stats{display:flex;gap:48px;margin-top:48px;padding-top:32px;border-top:1px solid rgba(255,255,255,0.1)}
.hero-stat-num{font-family:'DM Serif Display',serif;font-size:28px;color:#fff}
.hero-stat-label{font-size:12px;color:rgba(255,255,255,0.5)}

/* SECTIONS */
.section{padding:56px 32px}
.section-eyebrow{font-size:11px;font-weight:600;color:var(--green2);letter-spacing:1px;text-transform:uppercase;margin-bottom:8px}
.section-title{font-family:'DM Serif Display',serif;font-size:34px;color:var(--ink);letter-spacing:-0.5px;margin-bottom:12px}
.section-sub{font-size:15px;color:var(--ink3);max-width:520px;line-height:1.6;margin-bottom:40px}
.flow-steps{display:flex}
.flow-step{flex:1;padding:28px 24px;background:var(--surface);border:1px solid var(--border);position:relative;transition:all .2s}
.flow-step:first-child{border-radius:12px 0 0 12px}
.flow-step:last-child{border-radius:0 12px 12px 0}
.flow-step:not(:first-child){border-left:none}
.flow-step:hover{background:var(--surface2)}
.flow-step::after{content:'→';position:absolute;right:-14px;top:50%;transform:translateY(-50%);color:var(--green3);font-size:18px;z-index:2;background:var(--surface);padding:2px}
.flow-step:last-child::after{display:none}
.step-num{width:28px;height:28px;background:var(--green5);border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:700;color:var(--green2);margin-bottom:12px}
.step-icon{font-size:22px;margin-bottom:10px}
.step-title{font-size:13px;font-weight:600;color:var(--ink);margin-bottom:4px}
.step-desc{font-size:12px;color:var(--ink3);line-height:1.5}
.features-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
.feat-card{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:24px;transition:all .25s;cursor:pointer}
.feat-card:hover{border-color:var(--green3);box-shadow:var(--shadow2);transform:translateY(-2px)}
.feat-icon{width:40px;height:40px;border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:18px;margin-bottom:14px}
.feat-title{font-size:14px;font-weight:600;color:var(--ink);margin-bottom:6px}
.feat-desc{font-size:12px;color:var(--ink3);line-height:1.55}

/* DASHBOARD */
.dashboard-header{padding:24px 32px 0;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:12px}
.farm-avatar{width:44px;height:44px;background:var(--green);border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:18px;flex-shrink:0}
.farm-score-badge{background:var(--green5);border:1px solid var(--green4);border-radius:8px;padding:8px 16px;text-align:center}
.score-num-big{font-family:'DM Serif Display',serif;font-size:28px;color:var(--green);line-height:1}
.dash-grid{padding:20px 32px;display:grid;grid-template-columns:repeat(4,1fr);gap:14px}
.kpi-card{background:var(--surface);border:1px solid var(--border);border-radius:10px;padding:16px;transition:all .2s}
.kpi-card:hover{box-shadow:var(--shadow)}
.kpi-label{font-size:11px;font-weight:600;color:var(--ink3);text-transform:uppercase;letter-spacing:0.4px;margin-bottom:6px}
.kpi-num{font-family:'DM Serif Display',serif;font-size:26px;color:var(--ink);line-height:1.1}
.kpi-unit{font-family:'Instrument Sans',sans-serif;font-size:12px;color:var(--ink3);margin-left:2px}
.kpi-trend{font-size:11px;margin-top:4px}
.trend-up{color:#2e7d32}.trend-down{color:var(--red)}.trend-neutral{color:var(--ink3)}
.dash-main{padding:0 32px 20px;display:grid;grid-template-columns:1fr 1fr 340px;gap:16px}
.chart-card{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:20px}
.chart-title{font-size:13px;font-weight:600;color:var(--ink);margin-bottom:4px}
.chart-sub{font-size:11px;color:var(--ink3);margin-bottom:16px}
.scores-section{padding:0 32px 20px}
.scores-row{display:grid;grid-template-columns:repeat(7,1fr);gap:10px}
.score-card{background:var(--surface);border:1px solid var(--border);border-radius:10px;padding:14px;text-align:center;transition:all .2s}
.score-card:hover{border-color:var(--green3)}
.score-ring{width:60px;height:60px;margin:0 auto 8px;position:relative}
.score-ring svg{transform:rotate(-90deg)}
.score-ring-label{position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);font-family:'DM Serif Display',serif;font-size:16px;color:var(--ink);line-height:1}
.score-name{font-size:10px;font-weight:600;color:var(--ink3);text-transform:uppercase;letter-spacing:0.3px}
.alert-card{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:20px}
.alert-item{display:flex;align-items:flex-start;gap:12px;padding:10px 0;border-bottom:1px solid var(--border)}
.alert-item:last-child{border-bottom:none;padding-bottom:0}
.alert-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0;margin-top:5px}
.alert-text{font-size:12px;color:var(--ink2);line-height:1.5}
.alert-time{font-size:11px;color:var(--ink3);margin-top:2px}

/* NO DATA STATE */
.no-data{text-align:center;padding:60px 32px}
.no-data-icon{font-size:48px;margin-bottom:16px}
.no-data-title{font-family:'DM Serif Display',serif;font-size:22px;color:var(--ink);margin-bottom:8px}
.no-data-sub{font-size:14px;color:var(--ink3);margin-bottom:24px;max-width:400px;margin-left:auto;margin-right:auto}

/* AI ADVISOR */
.advisor-layout{padding:24px 32px;display:grid;grid-template-columns:300px 1fr;gap:20px}
.advisor-sidebar{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:20px;display:flex;flex-direction:column;gap:12px}
.advisor-context{background:var(--green5);border:1px solid var(--green4);border-radius:8px;padding:14px}
.context-label{font-size:10px;font-weight:700;color:var(--green2);text-transform:uppercase;letter-spacing:0.5px;margin-bottom:8px}
.context-item{display:flex;justify-content:space-between;font-size:12px;color:var(--ink2);padding:3px 0}
.context-val{font-weight:600;color:var(--ink)}
.chip{padding:8px 12px;border:1px solid var(--border);border-radius:8px;font-size:12px;color:var(--ink2);cursor:pointer;transition:all .2s;line-height:1.4}
.chip:hover,.chip.active{background:var(--green5);border-color:var(--green3);color:var(--green)}
.advisor-main{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:24px}
.ai-badge{display:inline-flex;align-items:center;gap:6px;background:var(--green5);border:1px solid var(--green4);border-radius:6px;padding:4px 10px;font-size:11px;font-weight:600;color:var(--green2)}
.ai-pulse{width:6px;height:6px;background:var(--green3);border-radius:50%;animation:pulse 1.5s infinite}
.rec-list{display:flex;flex-direction:column;gap:12px;margin-top:20px}
.rec-item{background:var(--surface2);border:1px solid var(--border);border-radius:10px;padding:16px;transition:all .2s}
.rec-item:hover{border-color:var(--green3)}
.rec-header{display:flex;align-items:flex-start;justify-content:space-between;gap:12px;margin-bottom:8px}
.rec-priority{padding:2px 8px;border-radius:4px;font-size:10px;font-weight:700;letter-spacing:0.3px;white-space:nowrap}
.p-high{background:#ffebee;color:#c62828}.p-med{background:#fff8e1;color:#e65100}.p-low{background:#e8f5e9;color:#2e7d32}
.rec-title{font-size:13px;font-weight:600;color:var(--ink)}
.rec-body{font-size:12px;color:var(--ink2);line-height:1.6;margin-bottom:10px}
.rec-impact{font-size:11px;font-weight:600;color:var(--teal);background:var(--teal2);padding:4px 10px;border-radius:4px;display:inline-block}
.ai-loading{text-align:center;padding:40px;color:var(--ink3);font-size:13px}
.ai-spinner{width:32px;height:32px;border:3px solid var(--green4);border-top-color:var(--green);border-radius:50%;animation:spin .8s linear infinite;margin:0 auto 12px}
@keyframes spin{to{transform:rotate(360deg)}}

/* ONBOARDING */
.onboarding-layout{padding:24px 32px;display:grid;grid-template-columns:220px 1fr;gap:20px}
.onboarding-steps{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:16px;height:fit-content}
.step-nav-item{display:flex;align-items:center;gap:12px;padding:10px 12px;border-radius:8px;cursor:pointer;transition:all .2s}
.step-nav-item:hover,.step-nav-item.active{background:var(--green5)}
.step-num-sm{width:24px;height:24px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;flex-shrink:0}
.s-complete{background:var(--green);color:#fff}.s-active{background:var(--green5);color:var(--green);border:1.5px solid var(--green3)}.s-pending{background:var(--surface3);color:var(--ink3)}
.step-nav-name{font-size:12px;font-weight:500;color:var(--ink2)}
.step-nav-item.active .step-nav-name{color:var(--green);font-weight:600}
.form-section{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:28px}
.form-title{font-size:18px;font-weight:600;color:var(--ink);margin-bottom:4px}
.form-sub{font-size:13px;color:var(--ink3);margin-bottom:24px}
.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px}
.fg.full{grid-column:1/-1}
.form-footer{margin-top:24px;display:flex;justify-content:flex-end;gap:10px;padding-top:20px;border-top:1px solid var(--border)}
.btn-sm{padding:8px 18px;border-radius:7px;font-size:13px;font-weight:600;font-family:'Instrument Sans',sans-serif;cursor:pointer;transition:all .2s;border:none}
.btn-green{background:var(--green);color:#fff}.btn-green:hover{background:var(--green2)}
.btn-outline-sm{background:transparent;border:1px solid var(--border2)!important;color:var(--ink2)}.btn-outline-sm:hover{background:var(--surface2)}

/* BENCHMARK */
.benchmark-layout{padding:24px 32px;display:flex;flex-direction:column;gap:16px}
.bench-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px}
.bench-card{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:20px}
.bench-label{font-size:13px;font-weight:600;color:var(--ink);margin-bottom:16px}
.bench-bar-row{display:flex;align-items:center;gap:10px;margin-bottom:10px}
.bench-bar-label{font-size:11px;color:var(--ink3);width:90px;text-align:right;flex-shrink:0}
.bench-bar-track{flex:1;height:8px;background:var(--surface3);border-radius:4px;overflow:hidden}
.bench-bar-fill{height:100%;border-radius:4px;transition:width .6s ease}
.bench-bar-val{font-size:11px;font-weight:600;color:var(--ink);width:54px;text-align:right;flex-shrink:0}
.your-bar{background:var(--green2)}.region-bar{background:#81c784}

/* SUSTAINABILITY */
.sust-layout{padding:24px 32px;display:grid;grid-template-columns:1fr 1fr 1fr;gap:16px}
.sust-card{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:20px}
.sust-bar{height:6px;background:var(--surface3);border-radius:3px;margin-top:10px;overflow:hidden}
.sust-bar-fill{height:100%;border-radius:3px}

/* PROGRESS BAR */
.progress-bar{height:4px;background:var(--green4);border-radius:2px;margin-bottom:0}
.progress-fill{height:100%;background:var(--green);border-radius:2px;transition:width .3s}

@media(max-width:900px){
  .features-grid,.scores-row{grid-template-columns:repeat(2,1fr)}
  .dash-grid{grid-template-columns:1fr 1fr}
  .dash-main,.advisor-layout,.onboarding-layout,.sust-layout{grid-template-columns:1fr}
  .form-grid{grid-template-columns:1fr}
  .bench-grid{grid-template-columns:1fr}
  .hero h1{font-size:32px}
  .flow-steps{flex-direction:column}
  .flow-step{border-radius:0!important;border-left:1px solid var(--border)!important}
  .flow-step::after{display:none}
  nav{gap:16px;padding:0 16px}
  nav a{font-size:12px}
}
</style>
</head>
<body>

<div class="toast" id="toast"></div>

<!-- AUTH MODAL -->
<div class="modal-overlay" id="authModal">
  <div class="modal">
    <button class="modal-close" onclick="closeModal()">✕</button>
    <div class="modal-title" data-i18n="welcome">Welcome to AgriLait</div>
    <div class="modal-sub" data-i18n="platform_tagline">Your farm intelligence platform</div>
    <div class="modal-tabs">
      <div class="modal-tab active" onclick="switchAuthTab('login')" data-i18n="login">Log In</div>
      <div class="modal-tab" onclick="switchAuthTab('register')" data-i18n="create_account">Create Account</div>
    </div>
    <div id="loginForm">
      <div class="fg"><label data-i18n="email">Email</label><input type="email" id="loginEmail" placeholder="your@email.com"></div>
      <div class="fg"><label data-i18n="password">Password</label><input type="password" id="loginPassword" placeholder="••••••••"></div>
      <button class="auth-btn" onclick="handleLogin()" data-i18n="login">Log In</button>
      <div class="msg" id="loginMsg"></div>
    </div>
    <div id="registerForm" style="display:none">
      <div class="fg"><label data-i18n="full_name">Full Name</label><input type="text" id="regName" placeholder="Your full name"></div>
      <div class="fg"><label data-i18n="email">Email</label><input type="email" id="regEmail" placeholder="your@email.com"></div>
      <div class="fg"><label data-i18n="password">Password</label><input type="password" id="regPassword" placeholder="Min. 6 characters"></div>
      <button class="auth-btn" onclick="handleRegister()" data-i18n="create_account">Create Account</button>
      <div class="msg" id="registerMsg"></div>
    </div>
  </div>
</div>

<!-- NAV -->
<nav>
  <div class="logo" onclick="showView('home')">
    <div class="logo-mark"><svg width="18" height="18" viewBox="0 0 18 18" fill="none"><path d="M9 2L14 6V12L9 16L4 12V6L9 2Z" stroke="#fff" stroke-width="1.5" fill="none"/><circle cx="9" cy="9" r="2" fill="#fff"/></svg></div>
    <span class="logo-text">Agri<span>Lait</span></span>
  </div>
  <a onclick="showView('home')" id="nav-home" class="active" data-i18n="platform">Platform</a>
  <a onclick="requireAuth('dashboard')" id="nav-dashboard" data-i18n="dashboard">Dashboard</a>
  <a onclick="requireAuth('advisor')" id="nav-advisor" data-i18n="ai_advisor">AI Advisor</a>
  <a onclick="requireAuth('benchmark')" id="nav-benchmark" data-i18n="benchmarking">Benchmarking</a>
  <a onclick="requireAuth('sustainability')" id="nav-sustainability" data-i18n="sustainability">Sustainability</a>
  <div class="nav-right">
    <div class="lang-switcher">
      <button class="lang-btn active" onclick="setLang('en')">EN</button>
      <button class="lang-btn" onclick="setLang('fr')">FR</button>
      <button class="lang-btn" onclick="setLang('ar')">AR</button>
    </div>
    <div id="navRight">
      <button class="btn-ghost" onclick="showView('onboarding')" data-i18n="register_farm">Register Farm</button>
      <button class="btn-primary" onclick="openModal()" data-i18n="login">Log In</button>
    </div>
  </div>
</nav>

<div class="tab-bar" id="tab-bar" style="display:none">
  <div class="tab active" data-i18n="overview">Overview</div>
  <div class="tab" data-i18n="herd">Herd Management</div>
  <div class="tab" data-i18n="milk">Milk Production</div>
  <div class="tab" data-i18n="feeding">Feeding</div>
  <div class="tab" data-i18n="reproduction">Reproduction</div>
  <div class="tab" data-i18n="health">Animal Health</div>
  <div class="tab" data-i18n="financials">Financials</div>
  <div class="tab" data-i18n="reports">Reports</div>
</div>

<!-- HOME -->
<div class="view active" id="view-home">
  <div class="hero">
    <div class="hero-bg"></div><div class="hero-orb"></div><div class="hero-orb2"></div>
    <div class="hero-content">
      <div class="hero-eyebrow"><span class="hero-dot"></span><span data-i18n="hero_eyebrow">AI-Powered Dairy Consulting</span></div>
      <h1 data-i18n="hero_title">Transform Farm Data<br>into <em>Better Decisions</em></h1>
      <p data-i18n="hero_sub">The world's most advanced dairy farm intelligence platform. Real-time analytics, AI-driven recommendations, and expert consulting — built for tomorrow's farmer.</p>
      <div class="hero-cta">
        <button class="btn-hero" onclick="openModal()" data-i18n="start_free">Start Free — Create Account</button>
        <button class="btn-hero-outline" onclick="requireAuth('dashboard')" data-i18n="explore_dashboard">Explore Dashboard →</button>
      </div>
      <div class="hero-stats">
        <div><div class="hero-stat-num" id="statFarms">0</div><div class="hero-stat-label" data-i18n="farms_analyzed">Farms Registered</div></div>
        <div><div class="hero-stat-num">18%</div><div class="hero-stat-label" data-i18n="yield_increase">Avg. Yield Increase</div></div>
        <div><div class="hero-stat-num">3</div><div class="hero-stat-label" data-i18n="countries">Countries</div></div>
      </div>
    </div>
  </div>
  <div class="section" style="background:var(--surface2);border-bottom:1px solid var(--border)">
    <div class="section-eyebrow" data-i18n="how_it_works_label">How It Works</div>
    <div class="section-title" data-i18n="how_it_works_title">From Raw Data to Real Results</div>
    <div class="section-sub" data-i18n="how_it_works_sub">Five integrated stages that transform your farm's data into actionable intelligence.</div>
    <div class="flow-steps">
      <div class="flow-step"><div class="step-num">1</div><div class="step-icon">📊</div><div class="step-title" data-i18n="step1_title">Data Collection</div><div class="step-desc" data-i18n="step1_desc">Structured onboarding covers 10 farm dimensions</div></div>
      <div class="flow-step"><div class="step-num">2</div><div class="step-icon">🔬</div><div class="step-title" data-i18n="step2_title">Farm Analysis</div><div class="step-desc" data-i18n="step2_desc">AI processes 200+ indicators against regional data</div></div>
      <div class="flow-step"><div class="step-num">3</div><div class="step-icon">🧠</div><div class="step-title" data-i18n="step3_title">AI Recommendations</div><div class="step-desc" data-i18n="step3_desc">Personalized action plans ranked by impact</div></div>
      <div class="flow-step"><div class="step-num">4</div><div class="step-icon">👨‍🌾</div><div class="step-title" data-i18n="step4_title">Expert Support</div><div class="step-desc" data-i18n="step4_desc">On-demand access to certified consultants</div></div>
      <div class="flow-step"><div class="step-num">5</div><div class="step-icon">📈</div><div class="step-title" data-i18n="step5_title">Continuous Monitoring</div><div class="step-desc" data-i18n="step5_desc">Real-time KPI tracking with early warning alerts</div></div>
    </div>
  </div>
  <div class="section">
    <div class="section-eyebrow" data-i18n="capabilities_label">Platform Capabilities</div>
    <div class="section-title" data-i18n="capabilities_title">Everything Your Farm Intelligence Needs</div>
    <div class="features-grid">
      <div class="feat-card" onclick="requireAuth('dashboard')"><div class="feat-icon" style="background:var(--green5)">📊</div><div class="feat-title" data-i18n="feat1_title">Smart Dashboard</div><div class="feat-desc" data-i18n="feat1_desc">Real-time KPI monitoring with 7 performance scores and custom alerts.</div></div>
      <div class="feat-card" onclick="requireAuth('advisor')"><div class="feat-icon" style="background:#fff8e1">🤖</div><div class="feat-title" data-i18n="feat2_title">AI Farm Advisor</div><div class="feat-desc" data-i18n="feat2_desc">Personalized recommendations covering nutrition, reproduction, health, and costs.</div></div>
      <div class="feat-card" onclick="requireAuth('benchmark')"><div class="feat-icon" style="background:var(--blue2)">📍</div><div class="feat-title" data-i18n="feat3_title">Benchmarking</div><div class="feat-desc" data-i18n="feat3_desc">Anonymous peer comparison against regional farms with similar herd sizes.</div></div>
      <div class="feat-card"><div class="feat-icon" style="background:#fce4ec">⚠️</div><div class="feat-title" data-i18n="feat4_title">Early Warning System</div><div class="feat-desc" data-i18n="feat4_desc">Predictive alerts for heat stress, mastitis risk, fertility decline, and financial stress.</div></div>
      <div class="feat-card" onclick="requireAuth('sustainability')"><div class="feat-icon" style="background:var(--teal2)">🌿</div><div class="feat-title" data-i18n="feat5_title">Sustainability Module</div><div class="feat-desc" data-i18n="feat5_desc">Carbon and water footprint per liter of milk. ISO 14040/44 LCA methodology.</div></div>
      <div class="feat-card"><div class="feat-icon" style="background:var(--earth2)">💰</div><div class="feat-title" data-i18n="feat6_title">Economic Simulator</div><div class="feat-desc" data-i18n="feat6_desc">Model scenarios with projected ROI and break-even analysis for any investment.</div></div>
    </div>
  </div>
</div>

<!-- DASHBOARD -->
<div class="view" id="view-dashboard">
  <div id="dashContent"></div>
</div>

<!-- AI ADVISOR -->
<div class="view" id="view-advisor">
  <div id="advisorContent"></div>
</div>

<!-- ONBOARDING -->
<div class="view" id="view-onboarding">
  <div class="onboarding-layout">
    <div class="onboarding-steps">
      <div style="font-size:13px;font-weight:600;color:var(--ink);margin-bottom:16px;padding:0 4px" data-i18n="farm_registration">Farm Registration</div>
      <div class="step-nav-item active"><div class="step-num-sm s-active">1</div><div class="step-nav-name" data-i18n="farm_profile">Farm Profile</div></div>
      <div class="step-nav-item"><div class="step-num-sm s-pending">2</div><div class="step-nav-name" data-i18n="herd">Herd Management</div></div>
      <div class="step-nav-item"><div class="step-num-sm s-pending">3</div><div class="step-nav-name" data-i18n="milk">Milk Production</div></div>
      <div class="step-nav-item"><div class="step-num-sm s-pending">4</div><div class="step-nav-name" data-i18n="feeding">Feeding</div></div>
      <div class="step-nav-item"><div class="step-num-sm s-pending">5</div><div class="step-nav-name" data-i18n="health">Animal Health</div></div>
      <div class="step-nav-item"><div class="step-num-sm s-pending">6</div><div class="step-nav-name" data-i18n="reproduction">Reproduction</div></div>
      <div class="step-nav-item"><div class="step-num-sm s-pending">7</div><div class="step-nav-name" data-i18n="infrastructure">Infrastructure</div></div>
      <div class="step-nav-item"><div class="step-num-sm s-pending">8</div><div class="step-nav-name" data-i18n="financials">Financials</div></div>
    </div>
    <div class="form-section">
      <div class="form-title" data-i18n="farm_profile">Farm Profile</div>
      <div class="form-sub" data-i18n="farm_profile_sub">Basic information about your farm. Log in to save your data permanently.</div>
      <div class="form-grid">
        <div class="fg"><label data-i18n="farm_name">Farm Name *</label><input type="text" id="f_name" placeholder="e.g. Ferme Benamar"></div>
        <div class="fg"><label data-i18n="owner_name">Owner / Manager *</label><input type="text" id="f_owner" placeholder="Full name"></div>
        <div class="fg"><label data-i18n="country">Country *</label><select id="f_country"><option>Algeria</option><option>Morocco</option><option>Tunisia</option><option>Egypt</option><option>France</option><option>Other</option></select></div>
        <div class="fg"><label data-i18n="region">Region / Wilaya</label><input type="text" id="f_region" placeholder="e.g. Annaba"></div>
        <div class="fg"><label data-i18n="farm_area">Farm Area (ha) *</label><input type="number" id="f_area" placeholder="e.g. 280"></div>
        <div class="fg"><label data-i18n="years_op">Years Operating *</label><input type="number" id="f_years" placeholder="e.g. 15"></div>
        <div class="fg"><label data-i18n="prod_type">Production Type</label><select id="f_production"><option>Intensive (zero-grazing)</option><option>Semi-intensive</option><option>Extensive (grazing)</option><option>Organic</option></select></div>
        <div class="fg"><label data-i18n="ownership">Ownership</label><select id="f_ownership"><option>Owner-operator</option><option>Tenant farmer</option><option>Cooperative member</option><option>Corporate farm</option></select></div>
        <div class="fg"><label data-i18n="total_animals">Total Animals</label><input type="number" id="f_animals" placeholder="e.g. 320"></div>
        <div class="fg"><label data-i18n="lactating">Lactating Cows</label><input type="number" id="f_lactating" placeholder="e.g. 273"></div>
        <div class="fg"><label data-i18n="daily_yield">Daily Yield (L)</label><input type="number" id="f_yield" placeholder="e.g. 7840"></div>
        <div class="fg"><label data-i18n="conception_rate">Conception Rate (%)</label><input type="number" id="f_conception" placeholder="e.g. 58"></div>
        <div class="fg"><label data-i18n="scc">SCC (k cells/mL)</label><input type="number" id="f_scc" placeholder="e.g. 198"></div>
        <div class="fg"><label data-i18n="feed_cost">Feed Cost / L (local currency)</label><input type="number" id="f_feedcost" placeholder="e.g. 14.2"></div>
        <div class="fg full"><label data-i18n="description">Farm Description</label><textarea id="f_desc" rows="3" placeholder="Describe your farm's main activities, challenges, or goals..."></textarea></div>
      </div>
      <div class="form-footer">
        <button class="btn-sm btn-outline-sm" onclick="showView('home')" data-i18n="cancel">Cancel</button>
        <button class="btn-sm btn-green" onclick="saveFarmProfile()" data-i18n="save_profile">Save Farm Profile →</button>
      </div>
      <div class="msg" id="farmMsg" style="margin-top:12px"></div>
    </div>
  </div>
</div>

<!-- BENCHMARK -->
<div class="view" id="view-benchmark">
  <div class="benchmark-layout">
    <div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:12px">
      <div><div class="section-eyebrow" data-i18n="anon_benchmark">Anonymous Benchmarking</div><div style="font-size:18px;font-weight:600;color:var(--ink)" data-i18n="your_farm_vs">Your Farm vs. Regional Peers</div><div style="font-size:12px;color:var(--ink3);margin-top:4px" id="benchSubtitle">Loading farm data...</div></div>
      <button class="btn-primary" onclick="requireAuth('dashboard')" data-i18n="view_dashboard">View Dashboard</button>
    </div>
    <div class="bench-grid" id="benchGrid">
      <div class="bench-card"><div class="bench-label">🥛 Milk Production</div>
        <div class="bench-bar-row"><div class="bench-bar-label" data-i18n="your_farm">Your farm</div><div class="bench-bar-track"><div class="bench-bar-fill your-bar" id="b_yield_you" style="width:0%"></div></div><div class="bench-bar-val" id="b_yield_you_val">—</div></div>
        <div class="bench-bar-row"><div class="bench-bar-label" data-i18n="regional_avg">Regional avg</div><div class="bench-bar-track"><div class="bench-bar-fill region-bar" style="width:60%"></div></div><div class="bench-bar-val">24.1 L</div></div>
        <div style="height:10px"></div>
        <div class="bench-bar-row"><div class="bench-bar-label">SCC</div><div class="bench-bar-track"><div class="bench-bar-fill your-bar" id="b_scc_you" style="width:0%"></div></div><div class="bench-bar-val" id="b_scc_you_val">—</div></div>
        <div class="bench-bar-row"><div class="bench-bar-label" data-i18n="regional_avg">Regional avg</div><div class="bench-bar-track"><div class="bench-bar-fill region-bar" style="width:75%"></div></div><div class="bench-bar-val">248k</div></div>
      </div>
      <div class="bench-card"><div class="bench-label">🐄 Reproduction</div>
        <div class="bench-bar-row"><div class="bench-bar-label" data-i18n="your_farm">Your farm</div><div class="bench-bar-track"><div class="bench-bar-fill your-bar" id="b_conc_you" style="width:0%"></div></div><div class="bench-bar-val" id="b_conc_you_val">—</div></div>
        <div class="bench-bar-row"><div class="bench-bar-label" data-i18n="regional_avg">Regional avg</div><div class="bench-bar-track"><div class="bench-bar-fill region-bar" style="width:62%"></div></div><div class="bench-bar-val">62%</div></div>
      </div>
      <div class="bench-card"><div class="bench-label">💰 Feed Efficiency</div>
        <div class="bench-bar-row"><div class="bench-bar-label" data-i18n="your_farm">Your farm</div><div class="bench-bar-track"><div class="bench-bar-fill your-bar" id="b_feed_you" style="width:0%"></div></div><div class="bench-bar-val" id="b_feed_you_val">—</div></div>
        <div class="bench-bar-row"><div class="bench-bar-label" data-i18n="regional_avg">Regional avg</div><div class="bench-bar-track"><div class="bench-bar-fill region-bar" style="width:60%"></div></div><div class="bench-bar-val">Avg</div></div>
      </div>
      <div class="bench-card"><div style="position:relative;height:220px"><canvas id="radarChart"></canvas></div></div>
    </div>
  </div>
</div>

<!-- SUSTAINABILITY -->
<div class="view" id="view-sustainability">
  <div style="padding:24px 32px 0">
    <div class="section-eyebrow" data-i18n="env_intelligence">Environmental Intelligence</div>
    <div style="font-size:22px;font-weight:600;font-family:'DM Serif Display',serif;color:var(--ink);margin-bottom:4px" data-i18n="sust_title">Sustainability & Carbon Analysis</div>
    <div style="font-size:13px;color:var(--ink3);margin-bottom:24px">LCA-based · ISO 14040/44 · Functional unit: 1 kg FPCM</div>
  </div>
  <div class="sust-layout">
    <div class="sust-card">
      <div class="chart-title" data-i18n="carbon_footprint">Carbon Footprint</div>
      <div style="text-align:center;padding:20px 0"><div style="font-family:'DM Serif Display',serif;font-size:42px;color:var(--ink)" id="sust_carbon">—</div><div style="font-size:13px;color:var(--ink3)">kg CO₂eq / kg FPCM</div></div>
      <div class="sust-bar"><div class="sust-bar-fill" id="sust_carbon_bar" style="width:0%;background:#2d6a2e"></div></div>
      <div style="font-size:11px;color:var(--ink3);margin-top:6px;display:flex;justify-content:space-between"><span data-i18n="your_farm">Your farm</span><span>MENA avg: 2.14</span></div>
      <div style="margin-top:16px;font-size:12px;color:var(--ink2)">
        <div style="display:flex;justify-content:space-between;padding:5px 0;border-bottom:1px solid var(--border)"><span>Enteric fermentation</span><span style="font-weight:600">42%</span></div>
        <div style="display:flex;justify-content:space-between;padding:5px 0;border-bottom:1px solid var(--border)"><span>Manure management</span><span style="font-weight:600">23%</span></div>
        <div style="display:flex;justify-content:space-between;padding:5px 0;border-bottom:1px solid var(--border)"><span>Feed production</span><span style="font-weight:600">28%</span></div>
        <div style="display:flex;justify-content:space-between;padding:5px 0"><span>Energy & transport</span><span style="font-weight:600">7%</span></div>
      </div>
    </div>
    <div class="sust-card">
      <div class="chart-title" data-i18n="water_footprint">Water Footprint</div>
      <div style="text-align:center;padding:20px 0"><div style="font-family:'DM Serif Display',serif;font-size:42px;color:var(--ink)" id="sust_water">—</div><div style="font-size:13px;color:var(--ink3)">L water / L milk</div></div>
      <div class="sust-bar"><div class="sust-bar-fill" id="sust_water_bar" style="width:0%;background:#1b6b5e"></div></div>
      <div style="font-size:11px;color:var(--ink3);margin-top:6px;display:flex;justify-content:space-between"><span data-i18n="your_farm">Your farm</span><span>Regional avg: 590 L</span></div>
      <div style="margin-top:20px;padding:14px;background:var(--green5);border:1px solid var(--green4);border-radius:8px;font-size:12px;color:var(--ink2)" id="sust_note">Enter your farm data to see your sustainability scores.</div>
    </div>
    <div class="sust-card">
      <div class="chart-title" data-i18n="resource_efficiency">Resource Efficiency</div>
      <div style="display:flex;flex-direction:column;gap:16px;margin-top:16px">
        <div><div style="display:flex;justify-content:space-between;font-size:12px;margin-bottom:5px"><span style="color:var(--ink2)" data-i18n="feed_conversion">Feed conversion</span><span style="font-weight:600" id="sust_fcr">—</span></div><div class="sust-bar"><div class="sust-bar-fill" id="sust_fcr_bar" style="width:0%;background:#2d6a2e"></div></div></div>
        <div><div style="display:flex;justify-content:space-between;font-size:12px;margin-bottom:5px"><span style="color:var(--ink2)">Milk efficiency</span><span style="font-weight:600" id="sust_eff">—</span></div><div class="sust-bar"><div class="sust-bar-fill" id="sust_eff_bar" style="width:0%;background:#3d8a3e"></div></div></div>
        <div><div style="display:flex;justify-content:space-between;font-size:12px;margin-bottom:5px"><span style="color:var(--ink2)">Herd utilization</span><span style="font-weight:600" id="sust_herd">—</span></div><div class="sust-bar"><div class="sust-bar-fill" id="sust_herd_bar" style="width:0%;background:#1b6b5e"></div></div></div>
      </div>
      <div style="margin-top:20px;padding:12px;background:var(--green5);border:1px solid var(--green4);border-radius:8px;font-size:12px;color:var(--ink2)">🌱 <span id="sust_score_text" data-i18n="sust_score_placeholder">Complete your farm profile to get your sustainability score.</span></div>
    </div>
  </div>
</div>

<script>
// ── SUPABASE ──
const SUPABASE_URL = 'https://prmlvxufcgeadvsmffzs.supabase.co';
const SUPABASE_KEY = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InBybWx2eHVmY2dlYWR2c21mZnpzIiwicm9sZSI6ImFub24iLCJpYXQiOjE3ODA3NzYxMzAsImV4cCI6MjA5NjM1MjEzMH0.LXRfU3j_7fsOOdjNA6r-UU5B9sCF6v6rixB0h11J7Jg';
const sb = supabase.createClient(SUPABASE_URL, SUPABASE_KEY);
let currentUser = null;
let farmData = null;

// ── TRANSLATIONS ──
const i18n = {
  en: {
    welcome:'Welcome to AgriLait',platform_tagline:'Your farm intelligence platform',
    login:'Log In',create_account:'Create Account',email:'Email',password:'Password',full_name:'Full Name',
    platform:'Platform',dashboard:'Dashboard',ai_advisor:'AI Advisor',benchmarking:'Benchmarking',sustainability:'Sustainability',
    register_farm:'Register Farm',hero_eyebrow:'AI-Powered Dairy Consulting',
    hero_title:'Transform Farm Data<br>into <em>Better Decisions</em>',
    hero_sub:"The world's most advanced dairy farm intelligence platform.",
    start_free:'Start Free — Create Account',explore_dashboard:'Explore Dashboard →',
    farms_analyzed:'Farms Registered',yield_increase:'Avg. Yield Increase',countries:'Countries',
    how_it_works_label:'How It Works',how_it_works_title:'From Raw Data to Real Results',
    how_it_works_sub:"Five integrated stages that transform your farm's data into actionable intelligence.",
    step1_title:'Data Collection',step1_desc:'Structured onboarding covers 10 farm dimensions',
    step2_title:'Farm Analysis',step2_desc:'AI processes 200+ indicators against regional data',
    step3_title:'AI Recommendations',step3_desc:'Personalized action plans ranked by impact',
    step4_title:'Expert Support',step4_desc:'On-demand access to certified consultants',
    step5_title:'Continuous Monitoring',step5_desc:'Real-time KPI tracking with early warning alerts',
    capabilities_label:'Platform Capabilities',capabilities_title:'Everything Your Farm Intelligence Needs',
    feat1_title:'Smart Dashboard',feat1_desc:'Real-time KPI monitoring with 7 performance scores.',
    feat2_title:'AI Farm Advisor',feat2_desc:'Personalized recommendations covering nutrition, reproduction, health.',
    feat3_title:'Benchmarking',feat3_desc:'Anonymous peer comparison against regional farms.',
    feat4_title:'Early Warning System',feat4_desc:'Predictive alerts for heat stress, mastitis risk.',
    feat5_title:'Sustainability Module',feat5_desc:'Carbon and water footprint per liter of milk.',
    feat6_title:'Economic Simulator',feat6_desc:'Model scenarios with projected ROI and break-even analysis.',
    farm_registration:'Farm Registration',farm_profile:'Farm Profile',herd:'Herd Management',
    milk:'Milk Production',feeding:'Feeding',health:'Animal Health',reproduction:'Reproduction',
    infrastructure:'Infrastructure',financials:'Financials',reports:'Reports',overview:'Overview',
    farm_profile_sub:'Basic information about your farm. Log in to save your data permanently.',
    farm_name:'Farm Name *',owner_name:'Owner / Manager *',country:'Country *',region:'Region / Wilaya',
    farm_area:'Farm Area (ha) *',years_op:'Years Operating *',prod_type:'Production Type',
    ownership:'Ownership',total_animals:'Total Animals',lactating:'Lactating Cows',
    daily_yield:'Daily Yield (L)',conception_rate:'Conception Rate (%)',scc:'SCC (k cells/mL)',
    feed_cost:'Feed Cost / L',description:'Farm Description',cancel:'Cancel',save_profile:'Save Farm Profile →',
    anon_benchmark:'Anonymous Benchmarking',your_farm_vs:'Your Farm vs. Regional Peers',
    your_farm:'Your farm',regional_avg:'Regional avg',view_dashboard:'View Dashboard',
    env_intelligence:'Environmental Intelligence',sust_title:'Sustainability & Carbon Analysis',
    carbon_footprint:'Carbon Footprint',water_footprint:'Water Footprint',resource_efficiency:'Resource Efficiency',
    feed_conversion:'Feed conversion',sust_score_placeholder:'Complete your farm profile to get your sustainability score.',
    no_farm_title:'No Farm Data Yet',no_farm_sub:'Register your farm to see your personalized dashboard.',
    register_now:'Register Farm Now',ai_recs:'AI-Powered Recommendations',ai_sub:'Based on your farm data · Updated on save',
    perf_scores:'Performance Scores',active_alerts:'Active Alerts',
  },
  fr: {
    welcome:'Bienvenue sur AgriLait',platform_tagline:'Votre plateforme d\'intelligence agricole',
    login:'Se connecter',create_account:'Créer un compte',email:'Email',password:'Mot de passe',full_name:'Nom complet',
    platform:'Plateforme',dashboard:'Tableau de bord',ai_advisor:'Conseiller IA',benchmarking:'Benchmarking',sustainability:'Durabilité',
    register_farm:'Inscrire ma ferme',hero_eyebrow:'Conseil laitier assisté par IA',
    hero_title:'Transformez vos données<br>en <em>Meilleures Décisions</em>',
    hero_sub:'La plateforme d\'intelligence agricole la plus avancée au monde.',
    start_free:'Commencer gratuitement',explore_dashboard:'Explorer le tableau de bord →',
    farms_analyzed:'Fermes inscrites',yield_increase:'Augmentation moy. du rendement',countries:'Pays',
    how_it_works_label:'Comment ça marche',how_it_works_title:'Des données brutes aux résultats concrets',
    how_it_works_sub:'Cinq étapes intégrées qui transforment vos données en intelligence actionnable.',
    step1_title:'Collecte de données',step1_desc:'Onboarding structuré couvrant 10 dimensions',
    step2_title:'Analyse de la ferme',step2_desc:'L\'IA traite 200+ indicateurs',
    step3_title:'Recommandations IA',step3_desc:'Plans d\'action personnalisés',
    step4_title:'Soutien d\'experts',step4_desc:'Accès à la demande aux consultants',
    step5_title:'Suivi continu',step5_desc:'Suivi des KPI en temps réel',
    capabilities_label:'Fonctionnalités',capabilities_title:'Tout ce dont votre ferme a besoin',
    feat1_title:'Tableau de bord intelligent',feat1_desc:'Surveillance des KPI en temps réel.',
    feat2_title:'Conseiller IA',feat2_desc:'Recommandations personnalisées.',
    feat3_title:'Benchmarking',feat3_desc:'Comparaison anonyme avec des fermes régionales.',
    feat4_title:'Système d\'alerte précoce',feat4_desc:'Alertes prédictives.',
    feat5_title:'Module durabilité',feat5_desc:'Empreinte carbone par litre de lait.',
    feat6_title:'Simulateur économique',feat6_desc:'Modélisation de scénarios avec ROI projeté.',
    farm_registration:'Inscription de la ferme',farm_profile:'Profil de la ferme',herd:'Gestion du troupeau',
    milk:'Production laitière',feeding:'Alimentation',health:'Santé animale',reproduction:'Reproduction',
    infrastructure:'Infrastructure',financials:'Finance',reports:'Rapports',overview:'Vue d\'ensemble',
    farm_profile_sub:'Informations de base sur votre ferme.',
    farm_name:'Nom de la ferme *',owner_name:'Propriétaire / Gérant *',country:'Pays *',region:'Région / Wilaya',
    farm_area:'Surface (ha) *',years_op:'Années d\'exploitation *',prod_type:'Type de production',
    ownership:'Statut juridique',total_animals:'Animaux total',lactating:'Vaches en lactation',
    daily_yield:'Rendement journalier (L)',conception_rate:'Taux de conception (%)',scc:'SCC (k cellules/mL)',
    feed_cost:'Coût alimentation / L',description:'Description',cancel:'Annuler',save_profile:'Enregistrer →',
    anon_benchmark:'Benchmarking anonyme',your_farm_vs:'Votre ferme vs. les pairs régionaux',
    your_farm:'Votre ferme',regional_avg:'Moy. régionale',view_dashboard:'Voir le tableau de bord',
    env_intelligence:'Intelligence environnementale',sust_title:'Analyse durabilité & carbone',
    carbon_footprint:'Empreinte carbone',water_footprint:'Empreinte eau',resource_efficiency:'Efficacité des ressources',
    feed_conversion:'Conversion alimentaire',sust_score_placeholder:'Complétez votre profil pour voir votre score.',
    no_farm_title:'Aucune donnée de ferme',no_farm_sub:'Inscrivez votre ferme pour voir votre tableau de bord.',
    register_now:'Inscrire ma ferme',ai_recs:'Recommandations IA',ai_sub:'Basées sur vos données · Mises à jour à chaque sauvegarde',
    perf_scores:'Scores de performance',active_alerts:'Alertes actives',
  },
  ar: {
    welcome:'مرحباً بك في AgriLait',platform_tagline:'منصة الذكاء الزراعي الخاصة بك',
    login:'تسجيل الدخول',create_account:'إنشاء حساب',email:'البريد الإلكتروني',password:'كلمة المرور',full_name:'الاسم الكامل',
    platform:'المنصة',dashboard:'لوحة التحكم',ai_advisor:'المستشار الذكي',benchmarking:'المقارنة المرجعية',sustainability:'الاستدامة',
    register_farm:'تسجيل المزرعة',hero_eyebrow:'استشارات الألبان بالذكاء الاصطناعي',
    hero_title:'حوّل بيانات مزرعتك<br>إلى <em>قرارات أفضل</em>',
    hero_sub:'أكثر منصات استخبارات المزارع الألبانية تقدماً في العالم.',
    start_free:'ابدأ مجاناً',explore_dashboard:'استعرض لوحة التحكم →',
    farms_analyzed:'المزارع المسجلة',yield_increase:'متوسط زيادة الإنتاج',countries:'دول',
    how_it_works_label:'كيف يعمل',how_it_works_title:'من البيانات الخام إلى نتائج حقيقية',
    how_it_works_sub:'خمس مراحل متكاملة تحول بيانات مزرعتك إلى ذكاء قابل للتطبيق.',
    step1_title:'جمع البيانات',step1_desc:'تغطي 10 أبعاد للمزرعة',
    step2_title:'تحليل المزرعة',step2_desc:'يعالج الذكاء الاصطناعي أكثر من 200 مؤشر',
    step3_title:'توصيات الذكاء الاصطناعي',step3_desc:'خطط عمل مخصصة',
    step4_title:'دعم الخبراء',step4_desc:'وصول فوري إلى المستشارين',
    step5_title:'المراقبة المستمرة',step5_desc:'تتبع مؤشرات الأداء الرئيسية في الوقت الفعلي',
    capabilities_label:'إمكانيات المنصة',capabilities_title:'كل ما تحتاجه مزرعتك',
    feat1_title:'لوحة تحكم ذكية',feat1_desc:'مراقبة مؤشرات الأداء في الوقت الفعلي.',
    feat2_title:'المستشار الزراعي الذكي',feat2_desc:'توصيات مخصصة تشمل التغذية والتكاثر والصحة.',
    feat3_title:'المقارنة المرجعية',feat3_desc:'مقارنة مجهولة مع المزارع الإقليمية.',
    feat4_title:'نظام الإنذار المبكر',feat4_desc:'تنبيهات تنبؤية.',
    feat5_title:'وحدة الاستدامة',feat5_desc:'البصمة الكربونية لكل لتر حليب.',
    feat6_title:'محاكي اقتصادي',feat6_desc:'نمذجة السيناريوهات مع توقعات العائد على الاستثمار.',
    farm_registration:'تسجيل المزرعة',farm_profile:'ملف المزرعة',herd:'إدارة القطيع',
    milk:'إنتاج الحليب',feeding:'التغذية',health:'صحة الحيوان',reproduction:'التكاثر',
    infrastructure:'البنية التحتية',financials:'الشؤون المالية',reports:'التقارير',overview:'نظرة عامة',
    farm_profile_sub:'المعلومات الأساسية عن مزرعتك.',
    farm_name:'اسم المزرعة *',owner_name:'المالك / المدير *',country:'البلد *',region:'المنطقة / الولاية',
    farm_area:'مساحة المزرعة (هكتار) *',years_op:'سنوات التشغيل *',prod_type:'نوع الإنتاج',
    ownership:'حالة الملكية',total_animals:'إجمالي الحيوانات',lactating:'الأبقار الحلوب',
    daily_yield:'الإنتاج اليومي (لتر)',conception_rate:'معدل الحمل (%)',scc:'SCC (ألف خلية/مل)',
    feed_cost:'تكلفة العلف / لتر',description:'وصف المزرعة',cancel:'إلغاء',save_profile:'حفظ ملف المزرعة →',
    anon_benchmark:'المقارنة المرجعية المجهولة',your_farm_vs:'مزرعتك مقابل الأقران الإقليميين',
    your_farm:'مزرعتك',regional_avg:'المتوسط الإقليمي',view_dashboard:'عرض لوحة التحكم',
    env_intelligence:'الذكاء البيئي',sust_title:'تحليل الاستدامة والكربون',
    carbon_footprint:'البصمة الكربونية',water_footprint:'البصمة المائية',resource_efficiency:'كفاءة الموارد',
    feed_conversion:'معدل تحويل العلف',sust_score_placeholder:'أكمل ملف مزرعتك للحصول على درجة الاستدامة.',
    no_farm_title:'لا توجد بيانات مزرعة بعد',no_farm_sub:'سجّل مزرعتك لرؤية لوحة التحكم الشخصية.',
    register_now:'تسجيل المزرعة الآن',ai_recs:'توصيات الذكاء الاصطناعي',ai_sub:'بناءً على بيانات مزرعتك',
    perf_scores:'درجات الأداء',active_alerts:'التنبيهات النشطة',
  }
};
let currentLang = 'en';

function setLang(lang) {
  currentLang = lang;
  document.querySelectorAll('.lang-btn').forEach(b => b.classList.toggle('active', b.textContent.toLowerCase() === lang));
  document.dir = lang === 'ar' ? 'rtl' : 'ltr';
  document.querySelectorAll('[data-i18n]').forEach(el => {
    const key = el.getAttribute('data-i18n');
    if (i18n[lang][key]) {
      if (el.tagName === 'INPUT' || el.tagName === 'TEXTAREA') el.placeholder = i18n[lang][key];
      else el.innerHTML = i18n[lang][key];
    }
  });
}

function t(key) { return i18n[currentLang][key] || i18n['en'][key] || key; }

// ── AUTH STATE ──
sb.auth.onAuthStateChange(async (event, session) => {
  currentUser = session?.user || null;
  updateNavUI();
  if (event === 'SIGNED_IN') {
    closeModal();
    showToast('👋 ' + (currentUser.user_metadata?.full_name || 'Welcome back!'), 'green');
    await loadFarmData();
    updateLiveStats();
  }
  if (event === 'SIGNED_OUT') {
    farmData = null;
    showView('home');
    showToast('Logged out');
  }
});

async function loadFarmData() {
  if (!currentUser) return;
  const { data, error } = await sb.from('farms').select('*').eq('user_id', currentUser.id).order('created_at', { ascending: false }).limit(1);
  if (!error && data && data.length > 0) {
    farmData = data[0];
    updateDashboard();
    updateBenchmark();
    updateSustainability();
  }
}

async function updateLiveStats() {
  const { count } = await sb.from('farms').select('*', { count: 'exact', head: true });
  if (count) document.getElementById('statFarms').textContent = count;
}

// ── DASHBOARD RENDER ──
function calcScore(farm) {
  let score = 50;
  const ypc = farm.lactating_cows && farm.daily_yield_liters ? farm.daily_yield_liters / farm.lactating_cows : 0;
  if (ypc > 20) score += 10; else if (ypc > 12) score += 6; else if (ypc > 6) score += 2;
  if (farm.scc_thousands && farm.scc_thousands < 200) score += 8; else if (farm.scc_thousands && farm.scc_thousands < 400) score += 4;
  if (farm.conception_rate_pct > 60) score += 8; else if (farm.conception_rate_pct > 45) score += 4; else if (farm.conception_rate_pct > 0) score -= 3;
  if (farm.lactating_cows && farm.total_animals && (farm.lactating_cows / farm.total_animals) > 0.8) score += 6;
  else if (farm.lactating_cows && farm.total_animals && (farm.lactating_cows / farm.total_animals) > 0.65) score += 3;
  if (farm.feed_cost_per_liter && farm.feed_cost_per_liter > 0) score += 5;
  return Math.min(100, Math.max(0, score));
}

function calcScores(f) {
  const ypc = f.lactating_cows && f.daily_yield_liters ? f.daily_yield_liters / f.lactating_cows : 0;
  const nutr = f.feed_cost_per_liter > 0 ? Math.min(100, Math.max(30, 85 - (f.feed_cost_per_liter / 500) * 40)) : 50;
  const repro = f.conception_rate_pct > 0 ? Math.min(100, Math.max(0, (f.conception_rate_pct / 65) * 100)) : 50;
  const health = f.scc_thousands > 0 ? Math.min(100, Math.max(20, 100 - (f.scc_thousands / 600) * 80)) : 50;
  const milk = ypc > 0 ? Math.min(100, Math.max(10, (ypc / 20) * 100)) : 50;
  const sust = Math.round(55 + (health > 70 ? 12 : health > 50 ? 6 : 0) + (milk > 50 ? 8 : 0));
  const econ = f.feed_cost_per_liter > 0 ? Math.min(100, Math.max(20, 90 - (f.feed_cost_per_liter / 400) * 60)) : 50;
  return { nutr: Math.round(nutr), repro: Math.round(repro), health: Math.round(health), milk: Math.round(milk), sust: Math.min(100, sust), econ: Math.round(econ) };
}

function updateDashboard() {
  const f = farmData;
  if (!f) return;
  const overall = calcScore(f);
  const {nutr, repro, health, milk, sust, econ} = calcScores(f);

  const yieldPerCow = f.lactating_cows && f.daily_yield_liters ? (f.daily_yield_liters / f.lactating_cows).toFixed(1) : '—';
  const herdPct = f.lactating_cows && f.total_animals ? ((f.lactating_cows / f.total_animals) * 100).toFixed(1) : '—';

  document.getElementById('dashContent').innerHTML = `
    <div class="dashboard-header">
      <div style="display:flex;align-items:center;gap:14px">
        <div class="farm-avatar">🐄</div>
        <div>
          <div style="font-size:16px;font-weight:600;color:var(--ink)">${f.farm_name} — ${f.region || f.country}</div>
          <div style="font-size:12px;color:var(--ink3)">${f.farm_area_ha ? f.farm_area_ha + ' ha · ' : ''}${f.total_animals || '—'} animals · ${f.production_type || ''}</div>
        </div>
      </div>
      <div style="display:flex;align-items:center;gap:12px">
        <div style="font-size:12px;color:var(--ink3)">Last updated: <strong>${new Date(f.updated_at || f.created_at).toLocaleDateString()}</strong></div>
        <div class="farm-score-badge"><div class="score-num-big">${overall}</div><div style="font-size:11px;color:var(--ink3);margin-top:2px">Farm Score</div></div>
      </div>
    </div>
    <div class="dash-grid">
      <div class="kpi-card"><div class="kpi-label">🥛 Daily Production</div><div class="kpi-num">${f.daily_yield_liters ? f.daily_yield_liters.toLocaleString() : '—'}<span class="kpi-unit">L</span></div><div class="kpi-trend trend-neutral">Enter data to track trends</div></div>
      <div class="kpi-card"><div class="kpi-label">🐄 Yield / Cow</div><div class="kpi-num">${yieldPerCow}<span class="kpi-unit">L/day</span></div><div class="kpi-trend ${f.daily_yield_liters / f.lactating_cows > 25 ? 'trend-up' : 'trend-down'}">${f.lactating_cows ? (f.daily_yield_liters / f.lactating_cows > 25 ? '↑ Above average' : '↓ Below average') : '—'}</div></div>
      <div class="kpi-card"><div class="kpi-label">🔬 SCC</div><div class="kpi-num">${f.scc_thousands || '—'}<span class="kpi-unit">k cells/mL</span></div><div class="kpi-trend ${f.scc_thousands < 200 ? 'trend-up' : 'trend-down'}">${f.scc_thousands ? (f.scc_thousands < 200 ? '✓ Good — target <200k' : '⚠ Above target') : '—'}</div></div>
      <div class="kpi-card"><div class="kpi-label">📋 Conception Rate</div><div class="kpi-num">${f.conception_rate_pct || '—'}<span class="kpi-unit">%</span></div><div class="kpi-trend ${f.conception_rate_pct >= 65 ? 'trend-up' : 'trend-down'}">${f.conception_rate_pct ? (f.conception_rate_pct >= 65 ? '✓ On target' : '↓ Below target (65%)') : '—'}</div></div>
      <div class="kpi-card"><div class="kpi-label">💰 Feed Cost / L</div><div class="kpi-num">${f.feed_cost_per_liter || '—'}<span class="kpi-unit">${f.country === 'Algeria' ? 'DZD' : 'MAD'}</span></div><div class="kpi-trend trend-neutral">→ ${f.feed_cost_per_liter ? 'Stable' : 'Not entered'}</div></div>
      <div class="kpi-card"><div class="kpi-label">🌿 Lactating Cows</div><div class="kpi-num">${f.lactating_cows || '—'}<span class="kpi-unit">/ ${f.total_animals || '?'}</span></div><div class="kpi-trend ${herdPct > 80 ? 'trend-up' : 'trend-neutral'}">${herdPct !== '—' ? herdPct + '% in milk' : '—'}</div></div>
      <div class="kpi-card"><div class="kpi-label">🏗 Farm Size</div><div class="kpi-num">${f.farm_area_ha || '—'}<span class="kpi-unit">ha</span></div><div class="kpi-trend trend-neutral">${f.years_operation ? f.years_operation + ' years operating' : '—'}</div></div>
      <div class="kpi-card"><div class="kpi-label">🌍 Location</div><div class="kpi-num" style="font-size:16px;margin-top:4px">${f.country}</div><div class="kpi-trend trend-neutral">${f.production_type || '—'}</div></div>
    </div>
    <div class="scores-section">
      <div style="font-size:13px;font-weight:600;color:var(--ink);margin-bottom:12px">${t('perf_scores')}</div>
      <div class="scores-row">
        ${scoreRing(overall,'#2d6a2e','Overall')}
        ${scoreRing(Math.round(nutr),'#3d8a3e','Nutrition')}
        ${scoreRing(Math.round(repro),'#d4790a','Repro')}
        ${scoreRing(Math.round(health),'#3d8a3e','Health')}
        ${scoreRing(Math.round(milk),'#3d8a3e','Milk')}
        ${scoreRing(Math.round(sust),'#1b6b5e','Sustain.')}
        ${scoreRing(Math.round(econ),'#1a3c8b','Economic')}
      </div>
    </div>
    <div style="padding:0 32px 32px">
      <div class="alert-card">
        <div class="chart-title" style="margin-bottom:14px">⚠️ ${t('active_alerts')}</div>
        ${generateAlerts(f)}
      </div>
    </div>
  `;
}

function scoreRing(val, color, name) {
  const r = 22, circ = 2 * Math.PI * r;
  const offset = circ - (val / 100) * circ;
  return `<div class="score-card">
    <div class="score-ring">
      <svg width="60" height="60" viewBox="0 0 60 60"><circle cx="30" cy="30" r="${r}" fill="none" stroke="#e5ede0" stroke-width="5"/><circle cx="30" cy="30" r="${r}" fill="none" stroke="${color}" stroke-width="5" stroke-dasharray="${circ}" stroke-dashoffset="${offset}" stroke-linecap="round" style="transform:rotate(-90deg);transform-origin:center"/></svg>
      <div class="score-ring-label">${val}</div>
    </div>
    <div class="score-name">${name}</div>
  </div>`;
}

function generateAlerts(f) {
  let alerts = [];
  if (f.conception_rate_pct && f.conception_rate_pct < 60) alerts.push({color:'#c0392b',text:`Conception rate at ${f.conception_rate_pct}% — below 65% target. Review AI protocol.`,time:'High priority'});
  if (f.scc_thousands && f.scc_thousands > 250) alerts.push({color:'#d4790a',text:`SCC at ${f.scc_thousands}k — above premium threshold. Check for mastitis.`,time:'Medium priority'});
  if (f.lactating_cows && f.total_animals && (f.lactating_cows/f.total_animals) < 0.75) alerts.push({color:'#d4790a',text:`Only ${((f.lactating_cows/f.total_animals)*100).toFixed(0)}% of herd in milk — below 80% target.`,time:'Medium priority'});
  if (alerts.length === 0) alerts.push({color:'#2d6a2e',text:'No critical alerts. Farm data looks healthy. Add more data for detailed analysis.',time:'Info'});
  return alerts.map(a => `<div class="alert-item"><div class="alert-dot" style="background:${a.color}"></div><div><div class="alert-text">${a.text}</div><div class="alert-time">${a.time}</div></div></div>`).join('');
}

// ── AI ADVISOR ──
function updateAdvisor() {
  if (!farmData) {
    document.getElementById('advisorContent').innerHTML = noDataHTML();
    return;
  }
  const f = farmData;
  const recs = generateRecommendations(f);
  document.getElementById('advisorContent').innerHTML = `
    <div class="advisor-layout">
      <div class="advisor-sidebar">
        <div style="font-size:13px;font-weight:600;color:var(--ink)">Farm Context</div>
        <div class="advisor-context">
          <div class="context-label">Current Profile</div>
          <div style="display:flex;justify-content:space-between;font-size:12px;color:var(--ink2);padding:3px 0"><span>Farm</span><span style="font-weight:600;color:var(--ink)">${f.farm_name}</span></div>
          <div style="display:flex;justify-content:space-between;font-size:12px;color:var(--ink2);padding:3px 0"><span>Animals</span><span style="font-weight:600;color:var(--ink)">${f.total_animals || '—'}</span></div>
          <div style="display:flex;justify-content:space-between;font-size:12px;color:var(--ink2);padding:3px 0"><span>Yield/day</span><span style="font-weight:600;color:var(--ink)">${f.daily_yield_liters || '—'} L</span></div>
          <div style="display:flex;justify-content:space-between;font-size:12px;color:var(--ink2);padding:3px 0"><span>Conception</span><span style="font-weight:600;color:${f.conception_rate_pct < 60 ? 'var(--red)' : 'var(--ink)'}">${f.conception_rate_pct || '—'}%</span></div>
          <div style="display:flex;justify-content:space-between;font-size:12px;color:var(--ink2);padding:3px 0"><span>SCC</span><span style="font-weight:600;color:var(--ink)">${f.scc_thousands || '—'}k</span></div>
        </div>
        <div style="font-size:12px;font-weight:600;color:var(--ink2)">Focus Areas</div>
        <div style="display:flex;flex-direction:column;gap:6px">
          ${recs.map((r,i) => `<div class="chip ${i===0?'active':''}">${r.icon} ${r.area}</div>`).join('')}
        </div>
        <button class="btn-sm btn-green" style="margin-top:auto" onclick="requireAuth('onboarding')">Update Farm Data</button>
      </div>
      <div class="advisor-main">
        <div style="display:flex;align-items:center;justify-content:space-between">
          <div><div style="font-size:16px;font-weight:600;color:var(--ink)">${t('ai_recs')}</div><div style="font-size:12px;color:var(--ink3);margin-top:2px">${t('ai_sub')}</div></div>
          <div class="ai-badge"><span class="ai-pulse"></span>AI Active</div>
        </div>
        <div class="rec-list">${recs.map(r => `
          <div class="rec-item">
            <div class="rec-header"><div class="rec-title">${r.icon} ${r.title}</div><span class="rec-priority ${r.pClass}">${r.priority}</span></div>
            <div class="rec-body">${r.body}</div>
            <div class="rec-impact">${r.impact}</div>
          </div>`).join('')}
        </div>
      </div>
    </div>`;
  document.querySelectorAll('.chip').forEach(c => c.addEventListener('click', function(){ document.querySelectorAll('.chip').forEach(x=>x.classList.remove('active')); this.classList.add('active') }));
}

function generateRecommendations(f) {
  const recs = [];
  if (f.conception_rate_pct && f.conception_rate_pct < 65) {
    recs.push({icon:'🔴',area:'Reproduction',title:`Improve Conception Rate (currently ${f.conception_rate_pct}%)`,priority:'HIGH',pClass:'p-high',body:`Your conception rate of ${f.conception_rate_pct}% is ${65 - f.conception_rate_pct} points below the 65% target. Recommend shifting inseminations to early morning (05:00–07:00), increasing water access points, and adding 200g/cow/day rumen-protected fat to improve energy balance during estrus.`,impact:`Projected gain: +${Math.round((65-f.conception_rate_pct)*0.6)}–${Math.round((65-f.conception_rate_pct)*0.9)}% conception rate within 60 days`});
  }
  if (f.scc_thousands && f.scc_thousands > 200) {
    recs.push({icon:'💊',area:'Mastitis Control',title:`Reduce SCC from ${f.scc_thousands}k`,priority:'HIGH',pClass:'p-high',body:`SCC of ${f.scc_thousands}k cells/mL exceeds the premium milk threshold of 200k. Implement post-milking teat dipping with an approved disinfectant, check milking machine settings, and isolate high-SCC cows for targeted treatment.`,impact:`Projected gain: Premium milk price bonus + reduced antibiotic costs`});
  }
  if (f.daily_yield_liters && f.lactating_cows && (f.daily_yield_liters/f.lactating_cows) < 25) {
    const ypc = (f.daily_yield_liters/f.lactating_cows).toFixed(1);
    recs.push({icon:'🌾',area:'Nutrition',title:`Increase yield per cow from ${ypc} L/day`,priority:'MEDIUM',pClass:'p-med',body:`Average yield of ${ypc} L/cow/day is below the regional target of 25–30 L. Review your total mixed ration (TMR) for energy density, ensure NDF is between 28–32% of dry matter, and consider adding bypass protein supplement at 150–200g/cow/day.`,impact:`Projected gain: +2–4 L/cow/day with ration optimization`});
  }
  if (f.feed_cost_per_liter && f.feed_cost_per_liter > 16) {
    recs.push({icon:'💰',area:'Cost Reduction',title:`Reduce Feed Cost (${f.feed_cost_per_liter}/L)`,priority:'MEDIUM',pClass:'p-med',body:`Feed cost of ${f.feed_cost_per_liter} per liter is above the efficient benchmark. Consider increasing homegrown forage proportion, negotiating bulk purchase contracts with feed suppliers, and using a precision feeding approach to reduce waste.`,impact:`Projected saving: 10–18% reduction in feed costs per liter`});
  }
  if (f.lactating_cows && f.total_animals && (f.lactating_cows/f.total_animals) < 0.80) {
    const pct = ((f.lactating_cows/f.total_animals)*100).toFixed(0);
    recs.push({icon:'📈',area:'Herd Efficiency',title:`Improve herd utilization (${pct}% in milk)`,priority:'LOW',pClass:'p-low',body:`Only ${pct}% of your herd is currently in milk, below the 80–85% efficiency target. Review your culling strategy, pregnancy monitoring protocol, and transition cow management to reduce dry period length.`,impact:`Projected gain: +${Math.round((0.82 - f.lactating_cows/f.total_animals) * f.total_animals)} additional lactating cows`});
  }
  if (recs.length === 0) {
    recs.push({icon:'✅',area:'General',title:'Farm performing well — continue monitoring',priority:'GOOD',pClass:'p-low',body:`Based on the data entered, your farm is performing at or above targets. Continue monitoring key indicators and update your data regularly to receive more precise recommendations.`,impact:'Keep tracking: add more data for deeper insights'});
  }
  return recs;
}

// ── BENCHMARK ──
function updateBenchmark() {
  if (!farmData) return;
  const f = farmData;
  const yieldPct = f.daily_yield_liters && f.lactating_cows ? Math.min(100, ((f.daily_yield_liters/f.lactating_cows)/35)*100) : 0;
  const sccPct = f.scc_thousands ? Math.min(100, Math.max(0, ((400-f.scc_thousands)/400)*100)) : 0;
  const concPct = f.conception_rate_pct ? Math.min(100, f.conception_rate_pct) : 0;
  const feedPct = f.feed_cost_per_liter ? Math.min(100, Math.max(0, 100-(f.feed_cost_per_liter/25)*100)) : 0;
  document.getElementById('benchSubtitle').textContent = `Farm: ${f.farm_name} · ${f.country}`;
  document.getElementById('b_yield_you').style.width = yieldPct + '%';
  document.getElementById('b_yield_you_val').textContent = f.daily_yield_liters && f.lactating_cows ? (f.daily_yield_liters/f.lactating_cows).toFixed(1)+' L' : '—';
  document.getElementById('b_scc_you').style.width = sccPct + '%';
  document.getElementById('b_scc_you_val').textContent = f.scc_thousands ? f.scc_thousands+'k' : '—';
  document.getElementById('b_conc_you').style.width = concPct + '%';
  document.getElementById('b_conc_you_val').textContent = f.conception_rate_pct ? f.conception_rate_pct+'%' : '—';
  document.getElementById('b_feed_you').style.width = feedPct + '%';
  document.getElementById('b_feed_you_val').textContent = f.feed_cost_per_liter ? f.feed_cost_per_liter : '—';
  initBench(f);
}

// ── SUSTAINABILITY CALC ──
function updateSustainability() {
  if (!farmData) return;
  const f = farmData;
  if (!f.daily_yield_liters || !f.total_animals) return;
  const ypc = f.daily_yield_liters / (f.lactating_cows || f.total_animals * 0.8);
  const carbon = (2.4 - (ypc / 30) * 0.8).toFixed(2);
  const water = Math.round(600 - (ypc / 30) * 200);
  const fcr = (1.4 - (ypc / 30) * 0.3).toFixed(2);
  const milkEff = Math.min(100, (ypc / 35) * 100).toFixed(0);
  const herdEff = f.lactating_cows && f.total_animals ? ((f.lactating_cows/f.total_animals)*100).toFixed(0) : '—';
  document.getElementById('sust_carbon').textContent = carbon;
  document.getElementById('sust_carbon_bar').style.width = Math.min(100, (2.5-carbon)/2.5*100) + '%';
  document.getElementById('sust_water').textContent = water;
  document.getElementById('sust_water_bar').style.width = Math.min(100, (650-water)/650*100) + '%';
  document.getElementById('sust_fcr').textContent = fcr + ' kg DM/L';
  document.getElementById('sust_fcr_bar').style.width = Math.min(100, (1.5-fcr)/1.5*100) + '%';
  document.getElementById('sust_eff').textContent = milkEff + '%';
  document.getElementById('sust_eff_bar').style.width = milkEff + '%';
  document.getElementById('sust_herd').textContent = herdEff + '%';
  document.getElementById('sust_herd_bar').style.width = herdEff + '%';
  const sustScore = Math.round(60 + (ypc/35)*25 + (f.scc_thousands < 200 ? 10 : 0));
  document.getElementById('sust_score_text').textContent = `🌱 Sustainability Score: ${sustScore}/100 — Your carbon intensity is ${carbon} kg CO₂eq/kg FPCM vs MENA avg 2.14`;
  document.getElementById('sust_note').textContent = `Your water footprint is ${water} L/L milk — ${water < 400 ? 'better than' : 'close to'} regional average of 590 L/L milk.`;
}

function noDataHTML() {
  return `<div class="no-data">
    <div class="no-data-icon">🌾</div>
    <div class="no-data-title">${t('no_farm_title')}</div>
    <div class="no-data-sub">${t('no_farm_sub')}</div>
    <button class="btn-primary" onclick="showView('onboarding')">${t('register_now')}</button>
  </div>`;
}

// ── SAVE FARM ──
async function saveFarmProfile() {
  const msg = document.getElementById('farmMsg');
  if (!currentUser) { showMsg(msg, 'Please log in first to save your data.', 'error'); openModal(); return; }
  const data = {
    user_id: currentUser.id,
    farm_name: document.getElementById('f_name').value,
    owner_name: document.getElementById('f_owner').value,
    country: document.getElementById('f_country').value,
    region: document.getElementById('f_region').value,
    farm_area_ha: parseFloat(document.getElementById('f_area').value) || null,
    years_operation: parseInt(document.getElementById('f_years').value) || null,
    production_type: document.getElementById('f_production').value,
    ownership_status: document.getElementById('f_ownership').value,
    description: document.getElementById('f_desc').value,
    total_animals: parseInt(document.getElementById('f_animals').value) || null,
    lactating_cows: parseInt(document.getElementById('f_lactating').value) || null,
    daily_yield_liters: parseFloat(document.getElementById('f_yield').value) || null,
    conception_rate_pct: parseFloat(document.getElementById('f_conception').value) || null,
    scc_thousands: parseFloat(document.getElementById('f_scc').value) || null,
    feed_cost_per_liter: parseFloat(document.getElementById('f_feedcost').value) || null,
    updated_at: new Date().toISOString()
  };
  if (!data.farm_name) { showMsg(msg, 'Farm name is required.', 'error'); return; }
  const btn = document.querySelector('.form-footer .btn-green');
  btn.disabled = true; btn.textContent = 'Saving...';
  const existing = await sb.from('farms').select('id').eq('user_id', currentUser.id).limit(1);
  let error;
  if (existing.data && existing.data.length > 0) {
    ({ error } = await sb.from('farms').update(data).eq('id', existing.data[0].id));
  } else {
    ({ error } = await sb.from('farms').insert([data]));
  }
  btn.disabled = false; btn.textContent = t('save_profile');
  if (error) showMsg(msg, 'Error: ' + error.message, 'error');
  else {
    showMsg(msg, '✓ Farm saved successfully!', 'success');
    showToast('Farm data saved! 🌾', 'green');
    await loadFarmData();
    await updateLiveStats();
  }
}

// ── AUTH ──
async function handleLogin() {
  const email = document.getElementById('loginEmail').value;
  const pass = document.getElementById('loginPassword').value;
  const msg = document.getElementById('loginMsg');
  if (!email || !pass) { showMsg(msg, 'Please fill in all fields.', 'error'); return; }
  const btn = document.querySelector('#loginForm .auth-btn');
  btn.disabled = true; btn.textContent = 'Logging in...';
  const { error } = await sb.auth.signInWithPassword({ email, password: pass });
  btn.disabled = false; btn.textContent = t('login');
  if (error) showMsg(msg, error.message, 'error');
}

async function handleRegister() {
  const name = document.getElementById('regName').value;
  const email = document.getElementById('regEmail').value;
  const pass = document.getElementById('regPassword').value;
  const msg = document.getElementById('registerMsg');
  if (!name || !email || !pass) { showMsg(msg, 'Please fill in all fields.', 'error'); return; }
  if (pass.length < 6) { showMsg(msg, 'Password must be at least 6 characters.', 'error'); return; }
  const btn = document.querySelector('#registerForm .auth-btn');
  btn.disabled = true; btn.textContent = 'Creating account...';
  const { error } = await sb.auth.signUp({ email, password: pass, options: { data: { full_name: name } } });
  btn.disabled = false; btn.textContent = t('create_account');
  if (error) showMsg(msg, error.message, 'error');
  else showMsg(msg, '✓ Account created! Check your email to confirm, then log in.', 'success');
}

async function handleLogout() { await sb.auth.signOut(); }

function updateNavUI() {
  const navRight = document.getElementById('navRight');
  if (currentUser) {
    const name = currentUser.user_metadata?.full_name || currentUser.email.split('@')[0];
    navRight.innerHTML = `<div class="user-pill"><div class="user-dot"></div>${name}</div><button class="btn-ghost" onclick="handleLogout()">Log Out</button>`;
  } else {
    navRight.innerHTML = `<button class="btn-ghost" onclick="showView('onboarding')" data-i18n="register_farm">Register Farm</button><button class="btn-primary" onclick="openModal()" data-i18n="login">Log In</button>`;
  }
}

// ── NAVIGATION ──
function showView(v) {
  document.querySelectorAll('.view').forEach(el => el.classList.remove('active'));
  document.getElementById('view-'+v).classList.add('active');
  document.querySelectorAll('nav a[id^="nav-"]').forEach(el => el.classList.remove('active'));
  const n = document.getElementById('nav-'+v); if(n) n.classList.add('active');
  document.getElementById('tab-bar').style.display = v==='dashboard' ? 'flex' : 'none';
  window.scrollTo(0,0);
  if (v==='dashboard') { farmData ? updateDashboard() : document.getElementById('dashContent').innerHTML = noDataHTML(); }
  if (v==='advisor') { updateAdvisor(); }
  if (v==='benchmark') { if(farmData) updateBenchmark(); initBench(farmData); }
  if (v==='sustainability') { if(farmData) updateSustainability(); initSust(); }
}

function requireAuth(v) {
  if (currentUser) showView(v);
  else { openModal(); showToast('Please log in to access this section'); }
}

// ── MODAL ──
function openModal() { document.getElementById('authModal').classList.add('open') }
function closeModal() { document.getElementById('authModal').classList.remove('open') }
function switchAuthTab(tab) {
  document.querySelectorAll('.modal-tab').forEach((t,i) => t.classList.toggle('active', (tab==='login'&&i===0)||(tab==='register'&&i===1)));
  document.getElementById('loginForm').style.display = tab==='login'?'block':'none';
  document.getElementById('registerForm').style.display = tab==='register'?'block':'none';
}
document.getElementById('authModal').addEventListener('click', e => { if(e.target===e.currentTarget) closeModal() });

// ── HELPERS ──
function showMsg(el, text, type) { el.textContent=text; el.className='msg '+type; el.style.display='block'; }
function showToast(msg, type='') { const t=document.getElementById('toast'); t.textContent=msg; t.className='toast '+type+' show'; setTimeout(()=>t.classList.remove('show'),3000); }

// ── CHARTS ──
let bi=false,si=false;
function initBench(f) {
  if(bi) return; bi=true;
  const yours = f ? [
    Math.round(f.daily_yield_liters&&f.lactating_cows?(f.daily_yield_liters/f.lactating_cows/35)*100:50),
    f.feed_cost_per_liter?Math.round(100-(f.feed_cost_per_liter/25)*100):50,
    f.conception_rate_pct?Math.round(f.conception_rate_pct):50,
    f.scc_thousands?Math.round(((400-f.scc_thousands)/400)*100):50,
    65,60
  ] : [50,50,50,50,65,60];
  new Chart(document.getElementById('radarChart'),{type:'radar',data:{labels:['Milk','Cost Eff.','Repro','Health','Sustain.','Economic'],datasets:[{label:'Your Farm',data:yours,borderColor:'#2d6a2e',backgroundColor:'rgba(45,106,46,0.12)',pointBackgroundColor:'#2d6a2e'},{label:'Regional Avg',data:[68,65,62,70,58,65],borderColor:'#81c784',backgroundColor:'rgba(129,199,132,0.08)',pointBackgroundColor:'#81c784',borderDash:[4,4]}]},options:{responsive:true,maintainAspectRatio:false,plugins:{legend:{labels:{font:{size:10},color:'#3a5a3b'}}},scales:{r:{grid:{color:'rgba(0,0,0,0.06)'},pointLabels:{font:{size:10},color:'#3a5a3b'},ticks:{display:false},min:0,max:100}}}});
}
function initSust(){
  if(si)return;si=true;
  const wc = document.getElementById('waterChart');
  if(wc) new Chart(wc,{type:'bar',data:{labels:['Green','Blue','Grey'],datasets:[{label:'Your farm',data:[164,68,53],backgroundColor:['#3d8a3e','#1a3c8b','#81c784']},{label:'Regional avg',data:[340,150,100],backgroundColor:['rgba(129,199,132,0.3)','rgba(26,60,139,0.2)','rgba(61,138,62,0.2)']}]},options:{responsive:true,maintainAspectRatio:false,plugins:{legend:{labels:{font:{size:10},color:'#3a5a3b'}}},scales:{y:{grid:{color:'rgba(0,0,0,0.04)'},ticks:{font:{size:9},color:'#6b8e6c'}},x:{grid:{display:false},ticks:{font:{size:9},color:'#6b8e6c'}}}}});
}

// ── TABS & STEPS ──
// ── TAB SWITCHING WITH CONTENT ──
const tabNames = ['overview','herd','milk','feeding','reproduction','health','financials','reports'];
document.querySelectorAll('.tab').forEach((tab, i) => {
  tab.addEventListener('click', function() {
    document.querySelectorAll('.tab').forEach(x => x.classList.remove('active'));
    this.classList.add('active');
    renderDashTab(tabNames[i]);
  });
});

function renderDashTab(tab) {
  const f = farmData;
  if (!f) { document.getElementById('dashContent').innerHTML = noDataHTML(); return; }
  if (tab === 'overview') { updateDashboard(); return; }
  const currency = f.country === 'Algeria' ? 'DZD' : f.country === 'Morocco' ? 'MAD' : 'Local';
  const ypc = f.lactating_cows && f.daily_yield_liters ? (f.daily_yield_liters / f.lactating_cows).toFixed(1) : '—';
  const herdPct = f.lactating_cows && f.total_animals ? ((f.lactating_cows / f.total_animals) * 100).toFixed(0) : '—';

  const tabContent = {
    herd: `
      <div style="padding:24px 32px">
        <div style="font-family:'DM Serif Display',serif;font-size:22px;color:var(--ink);margin-bottom:4px">Herd Management</div>
        <div style="font-size:13px;color:var(--ink3);margin-bottom:24px">Overview of your herd composition and structure</div>
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-bottom:20px">
          ${kpiCard('🐄','Total Animals', f.total_animals || '—', 'head', 'trend-neutral', 'All livestock')}
          ${kpiCard('🥛','Lactating Cows', f.lactating_cows || '—', 'cows', herdPct > 80 ? 'trend-up' : 'trend-neutral', herdPct !== '—' ? herdPct + '% of herd in milk' : '—')}
          ${kpiCard('🌿','Dry Cows', f.total_animals && f.lactating_cows ? f.total_animals - f.lactating_cows : '—', 'cows', 'trend-neutral', 'Not currently milking')}
          ${kpiCard('📊','Herd Utilization', herdPct, '%', herdPct > 80 ? 'trend-up' : 'trend-neutral', herdPct > 80 ? '✓ Good (target >80%)' : 'Target: >80%')}
        </div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
          <div class="chart-card">
            <div class="chart-title">Herd Composition</div>
            <div class="chart-sub">Breakdown of your ${f.total_animals || '—'} animals</div>
            ${f.total_animals && f.lactating_cows ? `
            <div style="display:flex;flex-direction:column;gap:12px;margin-top:8px">
              ${herdBar('Lactating Cows', f.lactating_cows, f.total_animals, '#2d6a2e')}
              ${herdBar('Dry Cows', Math.max(0, f.total_animals - f.lactating_cows), f.total_animals, '#81c784')}
            </div>` : '<div style="color:var(--ink3);font-size:13px;padding:20px 0">Enter herd data in Farm Registration to see breakdown</div>'}
          </div>
          <div class="chart-card">
            <div class="chart-title">Farm Details</div>
            <div class="chart-sub">Key farm parameters</div>
            <div style="display:flex;flex-direction:column;gap:8px;margin-top:8px">
              ${infoRow('Production Type', f.production_type || '—')}
              ${infoRow('Farm Size', f.farm_area_ha ? f.farm_area_ha + ' ha' : '—')}
              ${infoRow('Years Operating', f.years_operation ? f.years_operation + ' years' : '—')}
              ${infoRow('Ownership', f.ownership_status || '—')}
              ${infoRow('Region', f.region || f.country || '—')}
            </div>
          </div>
        </div>
      </div>`,

    milk: `
      <div style="padding:24px 32px">
        <div style="font-family:'DM Serif Display',serif;font-size:22px;color:var(--ink);margin-bottom:4px">Milk Production</div>
        <div style="font-size:13px;color:var(--ink3);margin-bottom:24px">Production performance and milk quality indicators</div>
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-bottom:20px">
          ${kpiCard('🥛','Daily Production', f.daily_yield_liters || '—', 'L', 'trend-neutral', 'Total liters per day')}
          ${kpiCard('🐄','Yield per Cow', ypc, 'L/day', ypc > 15 ? 'trend-up' : ypc > 8 ? 'trend-neutral' : 'trend-down', ypc > 15 ? '↑ Good performance' : ypc > 8 ? '→ Average' : '↓ Below average')}
          ${kpiCard('🔬','SCC', f.scc_thousands || '—', 'k cells/mL', f.scc_thousands < 200 ? 'trend-up' : 'trend-down', f.scc_thousands < 200 ? '✓ Premium quality' : f.scc_thousands < 400 ? '⚠ Acceptable' : '⛔ Poor quality')}
          ${kpiCard('💰','Milk Price', f.milk_price_per_liter || '—', currency + '/L', 'trend-neutral', 'Selling price per liter')}
        </div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
          <div class="chart-card">
            <div class="chart-title">Production Summary</div>
            <div class="chart-sub">Key performance vs targets</div>
            <div style="display:flex;flex-direction:column;gap:14px;margin-top:12px">
              ${progressBar('Yield / cow vs target (20 L)', ypc > 0 ? Math.min(100,(ypc/20)*100) : 0, ypc + ' L / 20 L target', '#2d6a2e')}
              ${progressBar('SCC quality vs threshold (200k)', f.scc_thousands > 0 ? Math.min(100,((400-f.scc_thousands)/400)*100) : 0, f.scc_thousands + 'k / 200k target', f.scc_thousands < 200 ? '#2d6a2e' : '#d4790a')}
              ${progressBar('Herd in milk vs target (80%)', herdPct > 0 ? Math.min(100, herdPct) : 0, herdPct + '% / 80% target', herdPct > 80 ? '#2d6a2e' : '#d4790a')}
            </div>
          </div>
          <div class="chart-card">
            <div class="chart-title">Quality Assessment</div>
            <div class="chart-sub">Milk quality grade based on SCC</div>
            <div style="text-align:center;padding:20px 0">
              <div style="font-family:'DM Serif Display',serif;font-size:48px;color:${f.scc_thousands < 200 ? 'var(--green)' : f.scc_thousands < 400 ? 'var(--amber)' : 'var(--red)'}">
                ${f.scc_thousands < 200 ? 'A+' : f.scc_thousands < 300 ? 'A' : f.scc_thousands < 400 ? 'B' : 'C'}
              </div>
              <div style="font-size:13px;color:var(--ink3);margin-top:8px">
                ${f.scc_thousands < 200 ? 'Premium quality — eligible for quality bonuses' : f.scc_thousands < 400 ? 'Standard quality — improvement recommended' : 'Below standard — mastitis risk detected'}
              </div>
            </div>
          </div>
        </div>
      </div>`,

    feeding: `
      <div style="padding:24px 32px">
        <div style="font-family:'DM Serif Display',serif;font-size:22px;color:var(--ink);margin-bottom:4px">Feeding Management</div>
        <div style="font-size:13px;color:var(--ink3);margin-bottom:24px">Feed costs, efficiency and nutrition overview</div>
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-bottom:20px">
          ${kpiCard('💰','Feed Cost / L', f.feed_cost_per_liter || '—', currency, 'trend-neutral', 'Cost per liter of milk')}
          ${kpiCard('📦','Daily Feed Cost', f.feed_cost_per_liter && f.daily_yield_liters ? (f.feed_cost_per_liter * f.daily_yield_liters).toLocaleString() : '—', currency, 'trend-neutral', 'Estimated daily feed spend')}
          ${kpiCard('📈','Monthly Feed Cost', f.feed_cost_per_liter && f.daily_yield_liters ? (f.feed_cost_per_liter * f.daily_yield_liters * 30).toLocaleString() : '—', currency, 'trend-neutral', 'Estimated monthly spend')}
          ${kpiCard('⚖️','Feed Efficiency', ypc > 0 && f.feed_cost_per_liter > 0 ? (ypc / f.feed_cost_per_liter * 100).toFixed(1) : '—', 'L/unit cost', 'trend-neutral', 'Liters per unit feed cost')}
        </div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
          <div class="chart-card">
            <div class="chart-title">Cost Analysis</div>
            <div class="chart-sub">Feed cost breakdown and benchmarks</div>
            <div style="display:flex;flex-direction:column;gap:14px;margin-top:12px">
              ${infoRow('Feed cost per liter', f.feed_cost_per_liter ? f.feed_cost_per_liter + ' ' + currency : 'Not entered')}
              ${infoRow('Daily production', f.daily_yield_liters ? f.daily_yield_liters + ' L' : '—')}
              ${infoRow('Daily feed cost estimate', f.feed_cost_per_liter && f.daily_yield_liters ? (f.feed_cost_per_liter * f.daily_yield_liters).toLocaleString() + ' ' + currency : '—')}
              ${infoRow('Annual feed cost estimate', f.feed_cost_per_liter && f.daily_yield_liters ? (f.feed_cost_per_liter * f.daily_yield_liters * 365).toLocaleString() + ' ' + currency : '—')}
            </div>
          </div>
          <div class="chart-card">
            <div class="chart-title">Feeding Recommendations</div>
            <div class="chart-sub">Based on your farm data</div>
            <div style="display:flex;flex-direction:column;gap:10px;margin-top:8px">
              ${ypc < 15 ? recBox('🌾', 'Review ration energy density', 'Yield per cow suggests the TMR may be low in energy. Consider increasing bypass fat or starch content.', 'high') : recBox('✅', 'Yield is adequate', 'Continue current feeding program and monitor trends monthly.', 'low')}
              ${f.feed_cost_per_liter > 200 ? recBox('💰', 'High feed cost detected', 'Feed cost per liter appears high. Consider bulk purchasing or increasing homegrown forage proportion.', 'medium') : ''}
            </div>
          </div>
        </div>
      </div>`,

    reproduction: `
      <div style="padding:24px 32px">
        <div style="font-family:'DM Serif Display',serif;font-size:22px;color:var(--ink);margin-bottom:4px">Reproduction Management</div>
        <div style="font-size:13px;color:var(--ink3);margin-bottom:24px">Fertility performance and breeding efficiency</div>
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-bottom:20px">
          ${kpiCard('📋','Conception Rate', f.conception_rate_pct || '—', '%', f.conception_rate_pct >= 65 ? 'trend-up' : f.conception_rate_pct >= 45 ? 'trend-neutral' : 'trend-down', f.conception_rate_pct >= 65 ? '✓ On target (≥65%)' : f.conception_rate_pct >= 45 ? '→ Below target (65%)' : '↓ Critical — review protocol')}
          ${kpiCard('🔄','Target Rate', '65', '%', 'trend-neutral', 'Industry benchmark')}
          ${kpiCard('📉','Gap to Target', f.conception_rate_pct > 0 ? Math.max(0, 65 - f.conception_rate_pct) : '—', 'pts', f.conception_rate_pct >= 65 ? 'trend-up' : 'trend-down', f.conception_rate_pct >= 65 ? '✓ Target achieved' : 'Points below target')}
          ${kpiCard('🐄','Breeding Cows', f.lactating_cows || '—', 'eligible', 'trend-neutral', 'Lactating cows eligible')}
        </div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
          <div class="chart-card">
            <div class="chart-title">Fertility Score</div>
            <div class="chart-sub">Conception rate vs regional benchmarks</div>
            <div style="display:flex;flex-direction:column;gap:14px;margin-top:12px">
              ${progressBar('Your conception rate', f.conception_rate_pct || 0, (f.conception_rate_pct || 0) + '%', f.conception_rate_pct >= 65 ? '#2d6a2e' : '#d4790a')}
              ${progressBar('Regional average', 62, '62%', '#81c784')}
              ${progressBar('Target', 65, '65%', '#1b6b5e')}
            </div>
          </div>
          <div class="chart-card">
            <div class="chart-title">Reproduction Recommendations</div>
            <div class="chart-sub">Targeted interventions</div>
            <div style="display:flex;flex-direction:column;gap:10px;margin-top:8px">
              ${f.conception_rate_pct < 50 ? recBox('🔴', 'Critical: Low conception rate', 'Shift AI timing to early morning (05:00-07:00), check bull fertility, increase water access points, and consider rumen-protected fat supplement at 200g/cow/day.', 'high') : f.conception_rate_pct < 65 ? recBox('🟡', 'Below target: Improve conception', 'Consider reviewing heat detection accuracy, AI timing protocol, and energy balance around breeding.', 'medium') : recBox('✅', 'Good fertility performance', 'Conception rate is at or above target. Maintain current protocol and monitor monthly.', 'low')}
            </div>
          </div>
        </div>
      </div>`,

    health: `
      <div style="padding:24px 32px">
        <div style="font-family:'DM Serif Display',serif;font-size:22px;color:var(--ink);margin-bottom:4px">Animal Health</div>
        <div style="font-size:13px;color:var(--ink3);margin-bottom:24px">Udder health, disease prevention and welfare indicators</div>
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-bottom:20px">
          ${kpiCard('🔬','SCC Level', f.scc_thousands || '—', 'k cells/mL', f.scc_thousands < 200 ? 'trend-up' : 'trend-down', f.scc_thousands < 200 ? '✓ Excellent udder health' : '⚠ Review milking hygiene')}
          ${kpiCard('🎯','Target SCC', '<200', 'k cells/mL', 'trend-neutral', 'Premium milk threshold')}
          ${kpiCard('🏥','Health Risk', f.scc_thousands > 400 ? 'HIGH' : f.scc_thousands > 200 ? 'MEDIUM' : 'LOW', '', f.scc_thousands > 400 ? 'trend-down' : f.scc_thousands > 200 ? 'trend-neutral' : 'trend-up', 'Based on SCC level')}
          ${kpiCard('💊','Mastitis Risk', f.scc_thousands > 400 ? 'Elevated' : f.scc_thousands > 200 ? 'Moderate' : 'Low', '', f.scc_thousands > 400 ? 'trend-down' : f.scc_thousands > 200 ? 'trend-neutral' : 'trend-up', 'SCC-based assessment')}
        </div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
          <div class="chart-card">
            <div class="chart-title">Udder Health Status</div>
            <div class="chart-sub">SCC analysis and milk quality grade</div>
            <div style="text-align:center;padding:16px 0">
              <div style="font-family:'DM Serif Display',serif;font-size:52px;color:${f.scc_thousands < 200 ? 'var(--green)' : f.scc_thousands < 400 ? 'var(--amber)' : 'var(--red)'}">
                ${f.scc_thousands || '—'}k
              </div>
              <div style="font-size:12px;color:var(--ink3);margin-top:4px">cells/mL</div>
              <div style="margin-top:16px">
                ${progressBar('SCC vs premium threshold (200k)', f.scc_thousands > 0 ? Math.min(100, (f.scc_thousands/600)*100) : 0, '', f.scc_thousands < 200 ? '#2d6a2e' : '#c0392b')}
              </div>
              <div style="font-size:12px;margin-top:12px;padding:8px 12px;background:${f.scc_thousands < 200 ? 'var(--green5)' : 'var(--earth2)'};border-radius:6px;color:var(--ink2)">
                ${f.scc_thousands < 200 ? '✓ Eligible for premium milk pricing' : f.scc_thousands < 400 ? '⚠ Not eligible for premium — investigate subclinical mastitis' : '⛔ High SCC — immediate veterinary review recommended'}
              </div>
            </div>
          </div>
          <div class="chart-card">
            <div class="chart-title">Health Action Plan</div>
            <div class="chart-sub">Recommended interventions</div>
            <div style="display:flex;flex-direction:column;gap:10px;margin-top:8px">
              ${f.scc_thousands > 400 ? recBox('🔴', 'Urgent: Mastitis risk', 'SCC above 400k indicates active mastitis. Identify and treat affected cows immediately. Review milking machine settings and post-milking teat dipping.', 'high') : f.scc_thousands > 200 ? recBox('🟡', 'Subclinical mastitis likely', 'SCC between 200-400k suggests subclinical mastitis in some cows. Consider individual cow SCC testing and targeted treatment.', 'medium') : recBox('✅', 'Excellent udder health', 'SCC below 200k — continue current milking hygiene protocol and teat dipping program.', 'low')}
              ${recBox('💉', 'Vaccination reminder', 'Ensure all cows are up to date on FMD, BVD, and leptospirosis vaccinations. Record dates in farm journal.', 'low')}
            </div>
          </div>
        </div>
      </div>`,

    financials: `
      <div style="padding:24px 32px">
        <div style="font-family:'DM Serif Display',serif;font-size:22px;color:var(--ink);margin-bottom:4px">Financial Performance</div>
        <div style="font-size:13px;color:var(--ink3);margin-bottom:24px">Revenue, costs and profitability analysis</div>
        <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-bottom:20px">
          ${kpiCard('💵','Daily Revenue Est.', f.daily_yield_liters && f.milk_price_per_liter ? (f.daily_yield_liters * f.milk_price_per_liter).toLocaleString() : '—', currency, 'trend-neutral', 'Based on yield × price')}
          ${kpiCard('📦','Daily Feed Cost', f.feed_cost_per_liter && f.daily_yield_liters ? (f.feed_cost_per_liter * f.daily_yield_liters).toLocaleString() : '—', currency, 'trend-neutral', 'Feed cost estimate')}
          ${kpiCard('📈','Monthly Revenue Est.', f.daily_yield_liters && f.milk_price_per_liter ? (f.daily_yield_liters * f.milk_price_per_liter * 30).toLocaleString() : '—', currency, 'trend-neutral', '30-day estimate')}
          ${kpiCard('⚖️','Cost per Liter', f.feed_cost_per_liter || '—', currency, 'trend-neutral', 'Feed cost only')}
        </div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
          <div class="chart-card">
            <div class="chart-title">Financial Summary</div>
            <div class="chart-sub">Estimated based on available data</div>
            <div style="display:flex;flex-direction:column;gap:8px;margin-top:12px">
              ${infoRow('Daily production', f.daily_yield_liters ? f.daily_yield_liters + ' L' : 'Not entered')}
              ${infoRow('Milk price / L', f.milk_price_per_liter ? f.milk_price_per_liter + ' ' + currency : 'Not entered')}
              ${infoRow('Daily revenue (est.)', f.daily_yield_liters && f.milk_price_per_liter ? (f.daily_yield_liters * f.milk_price_per_liter).toLocaleString() + ' ' + currency : '—')}
              ${infoRow('Monthly revenue (est.)', f.daily_yield_liters && f.milk_price_per_liter ? (f.daily_yield_liters * f.milk_price_per_liter * 30).toLocaleString() + ' ' + currency : '—')}
              ${infoRow('Feed cost / L', f.feed_cost_per_liter ? f.feed_cost_per_liter + ' ' + currency : 'Not entered')}
              ${infoRow('Daily feed cost (est.)', f.feed_cost_per_liter && f.daily_yield_liters ? (f.feed_cost_per_liter * f.daily_yield_liters).toLocaleString() + ' ' + currency : '—')}
            </div>
            <div style="margin-top:16px;padding:12px;background:var(--green5);border:1px solid var(--green4);border-radius:8px;font-size:12px;color:var(--ink2)">
              💡 Add your milk selling price in the farm profile to enable full financial analysis.
            </div>
          </div>
          <div class="chart-card">
            <div class="chart-title">Financial Recommendations</div>
            <div class="chart-sub">Opportunities to improve profitability</div>
            <div style="display:flex;flex-direction:column;gap:10px;margin-top:8px">
              ${f.scc_thousands < 200 ? recBox('💰', 'Premium milk pricing opportunity', 'Your SCC qualifies you for premium milk pricing. Negotiate with your dairy processor for a quality bonus.', 'low') : recBox('📉', 'SCC reducing your milk value', 'Improving SCC below 200k could qualify you for premium pricing bonuses on every liter sold.', 'medium')}
              ${recBox('📊', 'Track all costs for better analysis', 'Enter your milk selling price and complete the financial section to get full profitability analysis.', 'low')}
            </div>
          </div>
        </div>
      </div>`,

    reports: `
      <div style="padding:24px 32px">
        <div style="font-family:'DM Serif Display',serif;font-size:22px;color:var(--ink);margin-bottom:4px">Farm Reports</div>
        <div style="font-size:13px;color:var(--ink3);margin-bottom:24px">Automated farm assessment and audit reports</div>
        <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:16px">
          <div class="chart-card" style="cursor:pointer" onclick="window.print()">
            <div style="font-size:24px;margin-bottom:12px">📋</div>
            <div class="chart-title">Farm Performance Report</div>
            <div style="font-size:12px;color:var(--ink3);margin:8px 0 16px">Full overview of all performance scores, KPIs, and recommendations</div>
            <div style="padding:8px 16px;background:var(--green);border-radius:6px;font-size:13px;font-weight:600;color:#fff;text-align:center">Print / Save PDF</div>
          </div>
          <div class="chart-card" style="opacity:0.6">
            <div style="font-size:24px;margin-bottom:12px">🌿</div>
            <div class="chart-title">Sustainability Report</div>
            <div style="font-size:12px;color:var(--ink3);margin:8px 0 16px">Carbon footprint, water usage, and LCA analysis report</div>
            <div style="padding:8px 16px;background:var(--surface3);border-radius:6px;font-size:13px;font-weight:500;color:var(--ink3);text-align:center">Coming Soon</div>
          </div>
          <div class="chart-card" style="opacity:0.6">
            <div style="font-size:24px;margin-bottom:12px">💰</div>
            <div class="chart-title">Financial Analysis Report</div>
            <div style="font-size:12px;color:var(--ink3);margin:8px 0 16px">Revenue projections, cost breakdown and ROI analysis</div>
            <div style="padding:8px 16px;background:var(--surface3);border-radius:6px;font-size:13px;font-weight:500;color:var(--ink3);text-align:center">Coming Soon</div>
          </div>
        </div>
        <div style="margin-top:20px" class="chart-card">
          <div class="chart-title" style="margin-bottom:16px">📊 Quick Farm Summary — ${f.farm_name}</div>
          <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:16px;font-size:13px">
            <div>
              <div style="font-weight:600;color:var(--ink2);margin-bottom:8px">Production</div>
              ${infoRow('Daily yield', f.daily_yield_liters ? f.daily_yield_liters + ' L' : '—')}
              ${infoRow('Yield / cow', ypc + ' L/day')}
              ${infoRow('Lactating cows', f.lactating_cows || '—')}
            </div>
            <div>
              <div style="font-weight:600;color:var(--ink2);margin-bottom:8px">Quality & Health</div>
              ${infoRow('SCC', f.scc_thousands ? f.scc_thousands + 'k' : '—')}
              ${infoRow('Conception rate', f.conception_rate_pct ? f.conception_rate_pct + '%' : '—')}
              ${infoRow('Herd utilization', herdPct + '%')}
            </div>
            <div>
              <div style="font-weight:600;color:var(--ink2);margin-bottom:8px">Economics</div>
              ${infoRow('Feed cost/L', f.feed_cost_per_liter || '—')}
              ${infoRow('Farm size', f.farm_area_ha ? f.farm_area_ha + ' ha' : '—')}
              ${infoRow('Location', f.region || f.country || '—')}
            </div>
          </div>
        </div>
      </div>`
  };

  document.getElementById('dashContent').innerHTML = tabContent[tab] || '';
}

function kpiCard(icon, label, value, unit, trendClass, trendText) {
  return `<div class="kpi-card"><div class="kpi-label">${icon} ${label}</div><div class="kpi-num">${value}<span class="kpi-unit">${unit}</span></div><div class="kpi-trend ${trendClass}">${trendText}</div></div>`;
}
function infoRow(label, value) {
  return `<div style="display:flex;justify-content:space-between;padding:5px 0;border-bottom:1px solid var(--border);font-size:12px"><span style="color:var(--ink3)">${label}</span><span style="font-weight:600;color:var(--ink)">${value}</span></div>`;
}
function herdBar(label, value, total, color) {
  const pct = total > 0 ? Math.round((value/total)*100) : 0;
  return `<div><div style="display:flex;justify-content:space-between;font-size:12px;margin-bottom:4px"><span style="color:var(--ink2)">${label}</span><span style="font-weight:600;color:var(--ink)">${value} (${pct}%)</span></div><div style="height:8px;background:var(--surface3);border-radius:4px;overflow:hidden"><div style="width:${pct}%;height:100%;background:${color};border-radius:4px;transition:width .6s"></div></div></div>`;
}
function progressBar(label, pct, valueText, color) {
  return `<div><div style="display:flex;justify-content:space-between;font-size:12px;margin-bottom:4px"><span style="color:var(--ink2)">${label}</span><span style="font-weight:600;color:var(--ink)">${valueText}</span></div><div style="height:8px;background:var(--surface3);border-radius:4px;overflow:hidden"><div style="width:${Math.min(100,pct)}%;height:100%;background:${color};border-radius:4px;transition:width .6s"></div></div></div>`;
}
function recBox(icon, title, body, priority) {
  const colors = { high: {bg:'#ffebee',border:'rgba(192,57,43,0.2)',tc:'#c62828'}, medium: {bg:'#fff8e1',border:'rgba(212,121,10,0.2)',tc:'#e65100'}, low: {bg:'var(--green5)',border:'rgba(45,106,46,0.2)',tc:'var(--green)'} };
  const c = colors[priority] || colors.low;
  return `<div style="background:${c.bg};border:1px solid ${c.border};border-radius:8px;padding:12px"><div style="font-size:12px;font-weight:600;color:${c.tc};margin-bottom:4px">${icon} ${title}</div><div style="font-size:11px;color:var(--ink2);line-height:1.5">${body}</div></div>`;
}
document.querySelectorAll('.step-nav-item').forEach((item,i) => item.addEventListener('click', function(){ document.querySelectorAll('.step-nav-item').forEach((s,j)=>{ s.classList.remove('active'); s.querySelector('.step-num-sm').className='step-num-sm '+(j<i?'s-complete':j===i?'s-active':'s-pending') }); this.classList.add('active') }));

// ── INIT ──
updateLiveStats();
</script>
</body>
</html>
