<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Sopaan · CMGGA 2026 · Mock Paper 1</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,500;9..144,700&family=Source+Sans+3:wght@400;600;700&family=IBM+Plex+Mono:wght@500;600&display=swap">
<style>
  html,body{margin:0;} img{max-width:100%;} [hidden]{display:none !important;}
  :root{
    --navy:#16264A; --navy-2:#1F3B6B; --gold:#C79A3E; --gold-soft:#F3E7C9;
    --paper:#FBF9F4; --paper-2:#F1EAD8; --card:#FFFFFF;
    --ink:#211E1A; --ink-soft:#655D4C; --rule:#E4DCC8;
    --success:#2E8B57; --success-soft:#E1F2E7;
    --danger:#BF4B45; --danger-soft:#FAE3E1;
    --locked:#C7BEA9;
    --focus:#1F3B6B;
    --accent-text:#1F3B6B; --retry-text:#8A661F;
    color-scheme:light;
  }
  @media (prefers-color-scheme: dark){
    :root:not([data-theme="light"]){
      --navy:#0E1830; --navy-2:#16264A; --gold:#E0B75B; --gold-soft:#3A2F16;
      --paper:#141210; --paper-2:#1C1914; --card:#1C1914;
      --ink:#EDE7DA; --ink-soft:#B2A996; --rule:#3A342A;
      --success:#7BC79A; --success-soft:#1B2E22;
      --danger:#E38884; --danger-soft:#331D1B;
      --locked:#4A4436;
      --focus:#E0B75B;
      --accent-text:#E0B75B; --retry-text:#E0B75B;
      color-scheme:dark;
    }
  }
  :root[data-theme="dark"]{
    --navy:#0E1830; --navy-2:#16264A; --gold:#E0B75B; --gold-soft:#3A2F16;
    --paper:#141210; --paper-2:#1C1914; --card:#1C1914;
    --ink:#EDE7DA; --ink-soft:#B2A996; --rule:#3A342A;
    --success:#7BC79A; --success-soft:#1B2E22;
    --danger:#E38884; --danger-soft:#331D1B;
    --locked:#4A4436;
    --focus:#E0B75B;
    --accent-text:#E0B75B; --retry-text:#E0B75B;
    color-scheme:dark;
  }

  *{box-sizing:border-box;}
  body{background:var(--paper); color:var(--ink); font-family:'Source Sans 3',-apple-system,'Segoe UI',sans-serif; padding-inline:0; padding-block:0;}
  h1,h2,h3{font-family:'Fraunces',Georgia,serif; text-wrap:balance; margin:0;}
  .num{font-family:'IBM Plex Mono',ui-monospace,monospace; font-variant-numeric:tabular-nums;}

  header.brand{
    background:linear-gradient(155deg,var(--navy) 0%, var(--navy-2) 100%);
    color:#F4EFDF; padding-block:calc(20px + env(safe-area-inset-top,0px)) 18px; padding-inline:20px;
  }
  .brand-row{display:flex; align-items:center; gap:12px; max-width:900px; margin:0 auto;}
  .crest{
    width:42px; height:42px; border-radius:10px; background:var(--gold); color:var(--navy);
    display:flex; align-items:center; justify-content:center; font-family:'Fraunces',serif; font-weight:700; font-size:18px; flex-shrink:0;
  }
  .brand-name{font-size:12px; letter-spacing:.08em; text-transform:uppercase; color:var(--gold); font-weight:700;}
  .series-name{font-size:19px; font-weight:700; font-family:'Fraunces',serif;}
  .chapter-eyebrow{max-width:900px; margin:14px auto 0; font-size:12px; letter-spacing:.06em; text-transform:uppercase; color:#AEB9D6;}
  .chapter-title{font-size:28px; max-width:900px; margin:2px auto 0;}
  .chapter-sub{font-size:14.5px; color:var(--gold); font-weight:700; max-width:900px; margin:3px auto 0;}

  .chapter-progress{max-width:900px; margin:14px auto 0; display:flex; align-items:center; gap:10px;}
  .cp-track{flex:1; height:6px; border-radius:99px; background:rgba(255,255,255,.18); overflow:hidden;}
  .cp-fill{height:100%; background:var(--gold); border-radius:99px; transition:width .3s ease;}
  .cp-label{font-size:11.5px; color:#CFD7EA; white-space:nowrap;}

  .tabbar{position:sticky; top:env(safe-area-inset-top,0px); z-index:15; background:var(--paper); border-bottom:1px solid var(--rule); overflow-x:auto; white-space:nowrap;}
  .tabbar-inner{max-width:900px; margin:0 auto; display:flex; padding-inline:16px;}
  .tab-btn{font-family:inherit; font-size:14px; font-weight:600; color:var(--ink-soft); background:none; border:none; padding:13px 16px; cursor:pointer; position:relative; flex-shrink:0;}
  .tab-btn.active{color:var(--accent-text);}
  .tab-btn.active::after{content:''; position:absolute; left:12px; right:12px; bottom:0; height:3px; background:var(--gold); border-radius:3px 3px 0 0;}
  .tab-count{font-size:11px; color:var(--ink-soft); margin-left:5px;}

  .slide-progress{max-width:900px; margin:0 auto; padding:10px 16px 0; display:flex; align-items:center; gap:10px;}
  .sp-track{flex:1; height:5px; border-radius:99px; background:var(--rule); overflow:hidden;}
  .sp-fill{height:100%; background:var(--accent-text); border-radius:99px; transition:width .3s ease;}
  .sp-label{font-size:12px; color:var(--ink-soft); white-space:nowrap; font-weight:600;}

  .wrap{max-width:900px; margin:0 auto; padding:16px 16px calc(110px + env(safe-area-inset-bottom,0px));}

  .qcard{background:var(--card); border:1px solid var(--rule); border-radius:14px; padding:18px;}
  .qhead{display:flex; align-items:flex-start; gap:10px; margin-bottom:10px;}
  .qnum{width:32px; height:32px; border-radius:8px; background:var(--gold-soft); color:var(--accent-text); display:flex; align-items:center; justify-content:center; font-weight:700; font-family:'Fraunces',serif; flex-shrink:0; font-size:14px;}
  .qtext{font-size:16px; line-height:1.55; flex:1;}
  .qtag{font-size:10.5px; color:var(--gold); background:var(--gold-soft); padding:2px 7px; border-radius:99px; font-weight:700; margin-left:6px; white-space:nowrap;}
  .marks-pill{font-size:11px; font-weight:700; color:var(--ink-soft); border:1px solid var(--rule); padding:3px 9px; border-radius:99px; margin-left:auto; flex-shrink:0; white-space:nowrap;}
  .step-badge{font-size:11px; font-weight:700; color:var(--accent-text); background:var(--paper-2); border:1px solid var(--rule); padding:3px 9px; border-radius:99px; display:inline-block; margin-bottom:12px;}

  .options{display:flex; flex-direction:column; gap:8px; margin-top:10px;}
  .opt{display:flex; align-items:center; gap:10px; padding:11px 12px; border:1.5px solid var(--rule); border-radius:10px; cursor:pointer; font-size:15px; background:var(--paper);}
  .opt input{accent-color:var(--navy-2);}
  .opt.is-correct{border-color:var(--success); background:var(--success-soft);}
  .opt.is-wrong{border-color:var(--danger); background:var(--danger-soft);}
  .opt.locked{cursor:not-allowed;}

  .subpart-label{font-weight:700; font-size:12.5px; color:var(--accent-text); text-transform:uppercase; letter-spacing:.03em; margin:14px 0 6px;}
  .or-divider{text-align:center; font-size:11px; font-weight:700; letter-spacing:.08em; color:var(--ink-soft); margin:8px 0;}

  .steps{display:flex; flex-direction:column; gap:10px;}
  .step-line{font-size:14.5px; line-height:1.9; background:var(--paper); border:1px dashed var(--rule); border-radius:10px; padding:9px 12px;}
  .step-line.resolved{opacity:.9;}
  .blank-input{font-family:'IBM Plex Mono',monospace; font-size:14px; border:1.5px solid var(--rule); border-radius:6px; padding:3px 8px; width:120px; background:var(--card); color:var(--ink); margin:0 2px;}
  .blank-input:focus{outline:none; border-color:var(--focus); box-shadow:0 0 0 3px var(--gold-soft);}
  .blank-input.is-correct{border-color:var(--success); background:var(--success-soft);}
  .blank-input.is-wrong{border-color:var(--danger); background:var(--danger-soft);}
  .blank-input[disabled]{opacity:.85;}
  .reveal-note{font-size:12px; color:var(--danger); padding-left:2px; margin-top:-2px;}

  .feedback{font-size:13.5px; padding:10px 12px; border-radius:9px; margin-top:14px; display:none;}
  .feedback.show{display:block;}
  .feedback.ok{background:var(--success-soft); color:var(--success);}
  .feedback.retry{background:var(--gold-soft); color:var(--retry-text);}
  .feedback.reveal{background:var(--danger-soft); color:var(--danger);}
  .feedback.err{background:var(--danger-soft); color:var(--danger);}
  .attempts-dots{display:inline-flex; gap:4px; margin-left:2px;}
  .attempts-dots span{width:6px; height:6px; border-radius:50%; background:var(--ink-soft); opacity:.3; display:inline-block;}
  .attempts-dots span.used{opacity:1; background:var(--danger);}

  .ar-box{background:var(--paper-2); border-radius:10px; padding:10px 12px; margin-bottom:12px; font-size:13px; color:var(--ink-soft);}

  .navbar{
    position:fixed; left:0; right:0; bottom:0; z-index:30; background:var(--paper);
    border-top:1px solid var(--rule); padding:10px 16px calc(10px + env(safe-area-inset-bottom,0px));
  }
  .navbar-inner{max-width:900px; margin:0 auto; display:flex; gap:8px; flex-wrap:wrap; align-items:center;}
  .btn{font-family:inherit; font-size:13.5px; font-weight:700; padding:10px 14px; border-radius:9px; border:1.5px solid var(--rule); background:var(--card); color:var(--ink); cursor:pointer;}
  .btn:hover{border-color:var(--navy-2);}
  .btn:disabled{opacity:.4; cursor:not-allowed;}
  .btn-primary{background:var(--navy-2); color:#fff; border-color:var(--navy-2);}
  .navbar .spacer{flex:1;}

  .fab{position:fixed; right:16px; bottom:calc(74px + env(safe-area-inset-bottom,0px)); background:var(--gold); color:var(--navy); border:none; border-radius:999px; padding:11px 16px; font-family:inherit; font-weight:700; font-size:13px; display:flex; align-items:center; gap:7px; cursor:pointer; box-shadow:0 6px 16px rgba(0,0,0,.18); z-index:35;}
  .fab-badge{background:rgba(255,255,255,.55); border-radius:99px; padding:1px 7px; font-size:11px;}

  .overlay{position:fixed; inset:0; background:rgba(20,18,14,.45); z-index:50; display:none; align-items:flex-end; justify-content:center;}
  .overlay.show{display:flex;}
  .palette{background:var(--card); width:min(480px,100%); max-height:78vh; overflow-y:auto; border-radius:18px 18px 0 0; padding:18px 18px calc(18px + env(safe-area-inset-bottom,0px)); border:1px solid var(--rule); border-bottom:none;}
  @media (min-width:640px){ .overlay{align-items:center;} .palette{border-radius:18px; border-bottom:1px solid var(--rule); max-height:74vh;} }
  .palette-head{display:flex; align-items:center; justify-content:space-between; margin-bottom:6px;}
  .palette-head h2{font-size:16px;}
  .palette-close{background:none; border:none; font-size:20px; color:var(--ink-soft); cursor:pointer; padding:4px;}
  .palette-legend{display:flex; gap:12px; flex-wrap:wrap; font-size:11px; color:var(--ink-soft); margin:10px 0 14px;}
  .palette-legend span{display:inline-flex; align-items:center; gap:5px;}
  .dot{width:9px; height:9px; border-radius:50%; display:inline-block;}
  .dot.correct{background:var(--success);} .dot.revealed{background:var(--danger);}
  .dot.skipped{background:var(--gold);} .dot.locked{background:var(--locked);}
  .dot.current{background:var(--navy-2);}
  .chip-grid{display:grid; grid-template-columns:repeat(auto-fill,minmax(48px,1fr)); gap:8px;}
  .chip{border:1.5px solid var(--rule); border-radius:9px; padding:8px 4px; text-align:center; font-family:'IBM Plex Mono',monospace; font-size:12.5px; font-weight:600; cursor:pointer; background:var(--paper); color:var(--ink);}
  .chip[data-status="correct"]{border-color:var(--success); background:var(--success-soft); color:var(--success);}
  .chip[data-status="revealed"]{border-color:var(--danger); background:var(--danger-soft); color:var(--danger);}
  .chip[data-status="skipped"]{border-color:var(--gold); background:var(--gold-soft); color:var(--retry-text);}
  .chip[data-status="locked"]{border-color:var(--rule); color:var(--locked); cursor:not-allowed; background:var(--paper-2);}
  .chip[data-status="current"]{outline:2px solid var(--navy-2); outline-offset:1px;}

  .toast{position:fixed; left:50%; bottom:calc(140px + env(safe-area-inset-bottom,0px)); transform:translateX(-50%); background:var(--ink); color:var(--paper); padding:9px 16px; border-radius:99px; font-size:13px; opacity:0; pointer-events:none; transition:opacity .25s ease; z-index:60;}
  .toast.show{opacity:1;}

  .done-card{text-align:center; padding:36px 20px;}
  .done-card .big{font-size:38px; margin-bottom:6px;}
  .score-pills{display:flex; gap:10px; justify-content:center; flex-wrap:wrap; margin:16px 0;}
  .score-pill{padding:8px 16px; border-radius:99px; font-size:13px; font-weight:700;}

  footer.brandfoot{max-width:900px; margin:14px auto 0; padding:0 16px calc(110px + env(safe-area-inset-bottom,0px)); text-align:center; font-size:12px; color:var(--ink-soft);}

  .mode-pill{font-family:inherit; font-size:12.5px; font-weight:700; color:var(--navy); background:var(--gold); border:none; border-radius:99px; padding:6px 14px; cursor:pointer; margin-top:12px; display:inline-flex; align-items:center; gap:6px;}
  .mode-pick{display:flex; flex-direction:column; gap:14px; padding:8px 0 24px;}
  .mode-card{background:var(--card); border:1.5px solid var(--rule); border-radius:16px; padding:22px; cursor:pointer; text-align:left;}
  .mode-card:hover{border-color:var(--navy-2);}
  .mode-card .mode-icon{font-size:26px; margin-bottom:8px;}
  .mode-card h3{font-size:18px; margin-bottom:6px;}
  .mode-card p{font-size:13.5px; color:var(--ink-soft); line-height:1.5; margin:0;}
  .quiz-hint{font-size:12.5px; color:var(--ink-soft); background:var(--paper-2); border-radius:9px; padding:8px 12px; margin-bottom:14px;}
  .review-row{border:1px solid var(--rule); border-radius:10px; padding:11px 13px; margin-bottom:10px;}
  .review-tag{font-size:11.5px; font-weight:700; margin-bottom:4px; display:block;}
  .review-tag.ok{color:var(--success);} .review-tag.bad{color:var(--danger);} .review-tag.na{color:var(--ink-soft);}
  .review-q{font-size:13.5px; margin-bottom:6px; color:var(--ink-soft);}
  .review-ans{font-size:13px; margin-bottom:2px;}

  .who-row{max-width:900px; margin:12px auto 0; display:flex; flex-wrap:wrap; gap:8px; align-items:center;}
  .who-row .mode-pill{margin-top:0;}
  .who{display:inline-flex; flex-wrap:wrap; align-items:center; gap:6px; font-size:12.5px; color:#CFD7EA;}
  .who b{color:#F4EFDF;}
  .who button{font-family:inherit; font-size:12px; font-weight:700; color:#F4EFDF; background:rgba(255,255,255,.12); border:1px solid rgba(255,255,255,.22); border-radius:99px; padding:5px 11px; cursor:pointer;}
  .who button:hover{background:rgba(255,255,255,.2);}
  .login-card{max-width:460px; margin:8px auto 0; background:var(--card); border:1px solid var(--rule); border-radius:16px; padding:22px;}
  .login-card h2{font-size:21px; margin-bottom:4px;}
  .login-card p.lead{font-size:13.5px; color:var(--ink-soft); margin:0 0 16px; line-height:1.5;}
  .fld{display:flex; flex-direction:column; gap:5px; margin-bottom:12px;}
  .fld label{font-size:12px; font-weight:700; letter-spacing:.04em; text-transform:uppercase; color:var(--ink-soft);}
  .fld input{font-family:inherit; font-size:15px; padding:10px 12px; border:1.5px solid var(--rule); border-radius:9px; background:var(--paper); color:var(--ink);}
  .fld input:focus{outline:none; border-color:var(--focus); box-shadow:0 0 0 3px var(--gold-soft);}
  .fld-row{display:grid; grid-template-columns:1fr 1fr; gap:10px;}
  .login-err{font-size:13px; color:var(--danger); background:var(--danger-soft); border-radius:8px; padding:8px 10px; margin-bottom:12px;}
  .login-note{font-size:12px; color:var(--ink-soft); margin-top:12px; line-height:1.5;}
  .known{margin:0 0 16px; display:flex; flex-direction:column; gap:6px;}
  .known-label{font-size:12px; font-weight:700; letter-spacing:.04em; text-transform:uppercase; color:var(--ink-soft);}
  .known-btn{display:flex; justify-content:space-between; align-items:center; gap:10px; text-align:left; font-family:inherit; font-size:14.5px; padding:10px 12px; border:1.5px solid var(--rule); border-radius:10px; background:var(--paper); color:var(--ink); cursor:pointer;}
  .known-btn:hover{border-color:var(--navy-2);}
  .known-btn small{font-size:12px; color:var(--ink-soft);}
  .rec-card{background:var(--card); border:1px solid var(--rule); border-radius:14px; padding:18px; margin-bottom:14px;}
  .rec-card h2{font-size:19px; margin-bottom:10px;}
  .rec-card h3{font-size:15px; margin:4px 0 8px;}
  .rec-table-wrap{overflow-x:auto;}
  .rec-table{width:100%; border-collapse:collapse; font-size:13.5px; font-variant-numeric:tabular-nums;}
  .rec-table th{text-align:left; font-size:11.5px; text-transform:uppercase; letter-spacing:.04em; color:var(--ink-soft); padding:6px 8px; border-bottom:1px solid var(--rule); white-space:nowrap;}
  .rec-table td{padding:8px; border-bottom:1px solid var(--rule); white-space:nowrap;}
  .rec-bar{display:inline-block; width:70px; height:6px; border-radius:99px; background:var(--rule); overflow:hidden; vertical-align:middle; margin-right:6px;}
  .rec-bar i{display:block; height:100%; background:var(--success);}
  .rec-empty{font-size:13.5px; color:var(--ink-soft);}
  .sec-sub{max-width:900px; margin:0 auto; padding:10px 16px 0; font-size:12.5px; font-weight:700; color:var(--accent-text); letter-spacing:.02em;}
  .opt{flex-wrap:wrap;}
  .opt-l{font-family:'IBM Plex Mono',monospace; font-size:13px; font-weight:600; color:var(--ink-soft);}
  .opt-t{flex:1; min-width:0;}
  .opt.is-chosen:not(.is-correct):not(.is-wrong){border-color:var(--navy-2); background:var(--gold-soft);}
  .opt-tag{font-size:11px; font-weight:700; padding:2px 8px; border-radius:99px; background:var(--card); border:1px solid currentColor; white-space:nowrap;}
  .opt.is-correct .opt-tag{color:var(--success);} .opt.is-wrong .opt-tag{color:var(--danger);} .opt.is-chosen:not(.is-correct):not(.is-wrong) .opt-tag{color:var(--accent-text);}
  .chosen{font-size:13.5px; margin-top:10px; padding:8px 12px; border-radius:9px;}
  .chosen.ok{background:var(--success-soft); color:var(--success);} .chosen.bad{background:var(--danger-soft); color:var(--danger);}
  .chosen + .chosen{margin-top:6px;}
  .solution{margin-top:14px; border:1px solid var(--rule); border-left:4px solid var(--gold); background:var(--paper-2); border-radius:10px; padding:12px 14px;}
  .sol-h{font-family:'Fraunces',Georgia,serif; font-weight:700; font-size:14px; color:var(--accent-text); margin-bottom:6px;}
  .sol-line{font-size:14.5px; line-height:1.7;}
  .rev-sol summary{cursor:pointer; font-size:12.5px; font-weight:700; color:var(--accent-text); margin-top:6px;}
  .rev-sol .solution{margin-top:8px;}
  .chapter-credit{max-width:900px; margin:4px auto 0; font-size:12px; color:#CFD7EA;}
  footer.brandfoot a{color:inherit;}
  .blank-input.wide{width:260px; max-width:100%; font-family:'Source Sans 3',sans-serif;}
  .blank-input.expr{width:170px; max-width:100%;}
  /*fix-layout*/ .cp-fill,.sp-fill{width:0;} .fld{min-width:0;} .fld input{width:100%; min-width:0; box-sizing:border-box;}
  .fig{margin:6px 0 10px; display:flex; justify-content:center;}
  .figsvg{width:100%; max-width:340px; height:auto; overflow:visible;}
  .figsvg .ln,.figsvg .arm{stroke:var(--ink); stroke-width:1.6; fill:none;}
  .figsvg .arm{stroke:var(--accent-text); stroke-width:2;}
  .figsvg .pt{fill:var(--ink);}
  .figsvg .lb{fill:var(--ink); font:600 13px 'Source Sans 3',sans-serif;}
  .figsvg .al{fill:var(--accent-text); font:700 12px 'Source Sans 3',sans-serif;}
  .figsvg .wg{fill:var(--gold-soft); stroke:var(--gold); stroke-width:1.2;}
  .figsvg .wg2{fill:rgba(199,154,62,.35); stroke:var(--gold); stroke-width:1.2;}
  .figsvg .ra{fill:none; stroke:var(--ink); stroke-width:1.2;}
  .figsvg .ahd{fill:var(--ink);}
  .figsvg .pr{fill:var(--paper-2); stroke:var(--ink-soft); stroke-width:1.2;}
  .figsvg .tk{stroke:var(--ink-soft); stroke-width:.8;}
  .figsvg .po{fill:var(--ink); font:600 8.5px 'IBM Plex Mono',monospace;}
  .figsvg .pi{fill:var(--danger); font:600 7.5px 'IBM Plex Mono',monospace;}
  .figsvg .sh{fill:var(--gold-soft); stroke:var(--ink); stroke-width:1.5; stroke-linejoin:round;}
  .figsvg .sh2{fill:rgba(199,154,62,.38); stroke:var(--ink); stroke-width:1.5; stroke-linejoin:round;}
  .figsvg .sh3{fill:rgba(199,154,62,.22); stroke:var(--ink); stroke-width:1.5; stroke-linejoin:round;}
  .figsvg .none{fill:none;}
  .figsvg .hid{stroke-dasharray:5 4; fill:none;}
  .figsvg .tick{stroke:var(--ink); stroke-width:1.4; fill:none;}
  .figsvg .shd{fill:var(--accent-text); fill-opacity:.55;}
  .figsvg .cell{fill:var(--card); stroke:var(--ink); stroke-width:1.1;}
  .figsvg .dr{fill:var(--danger);} .figsvg .dw{fill:var(--card); stroke:var(--ink); stroke-width:1.2;}
  .figsvg .dotfill{fill:var(--danger);}
  .tt{border-collapse:collapse; font-size:13.5px; margin:4px auto; font-variant-numeric:tabular-nums;} .tt th,.tt td{border:1px solid var(--rule); padding:4px 9px; text-align:left;} .tt th{background:var(--paper-2); font-weight:700;} .ttw{overflow-x:auto; max-width:100%;}
  .fq{display:inline-flex; flex-direction:column; vertical-align:middle; text-align:center; font-size:.82em; line-height:1.12; margin:0 2px;}
  .fq>span:first-child{border-bottom:1.5px solid currentColor; padding:0 2px;}
  .fq>span:last-child{padding:0 2px;}
  .mx{white-space:nowrap;}
  .blank-input.fr{width:110px;}
  @media (prefers-reduced-motion:reduce){ *{transition:none !important;} }
.datline{display:block;margin-top:8px;padding:8px 10px;border-radius:8px;background:var(--paper-2);font:500 14px/1.7 'IBM Plex Mono',monospace;word-spacing:2px;overflow-wrap:anywhere;}

  .theory{display:flex;flex-direction:column;gap:16px;padding-bottom:40px;}
  .hub{display:grid;grid-template-columns:1fr;gap:12px;}
  @media (min-width:640px){ .hub{grid-template-columns:repeat(3,1fr);} }
  .hub-card{background:var(--card);border:1px solid var(--rule);border-radius:14px;padding:16px;display:flex;flex-direction:column;gap:8px;}
  .hub-card h3{font-family:'Fraunces',serif;font-size:18px;margin:0;color:var(--accent-text);}
  .hub-card p{margin:0;font-size:14px;color:var(--ink-soft);line-height:1.5;}
  .hub-btns{display:flex;flex-wrap:wrap;gap:8px;margin-top:auto;}
  .hub-btn{min-height:40px;border:1.5px solid var(--rule);background:var(--paper-2);color:var(--ink);border-radius:10px;padding:8px 12px;font:600 14px 'Source Sans 3',sans-serif;cursor:pointer;text-align:left;}
  .hub-btn:hover{border-color:var(--gold);}
  .hub-btn.primary{background:var(--navy);color:#F4EFDF;border-color:var(--navy);}
  .note{background:var(--card);border:1px solid var(--rule);border-radius:14px;padding:18px;scroll-margin-top:120px;}
  .note h2{font-family:'Fraunces',serif;font-size:22px;margin:0 0 4px;color:var(--ink);}
  .note .lt{font-size:13.5px;color:var(--ink-soft);margin:0 0 12px;}
  .note .lt b{color:var(--accent-text);}
  .note h4{font:700 15px 'Source Sans 3',sans-serif;margin:16px 0 6px;color:var(--accent-text);}
  .note p,.note li{font-size:15.5px;line-height:1.6;}
  .note ul{padding-left:20px;margin:6px 0;}
  .keybox{background:var(--gold-soft);border-left:4px solid var(--gold);border-radius:8px;padding:10px 12px;margin:10px 0;font-size:15px;line-height:1.6;}
  .keybox b{color:var(--ink);}
  .ex{background:var(--paper-2);border-radius:10px;padding:12px;margin:10px 0;}
  .ex .exh{font-family:'Fraunces',serif;font-weight:700;color:var(--accent-text);margin-bottom:4px;}
  .ex .exl{font-size:15px;line-height:1.7;}
  .ttab{width:100%;border-collapse:collapse;font-size:14.5px;margin:8px 0;}
  .ttab th,.ttab td{border:1px solid var(--rule);padding:7px 8px;text-align:left;vertical-align:top;}
  .ttab th{background:var(--paper-2);}
  .tscroll{overflow-x:auto;}
  .mono{font-family:'IBM Plex Mono',monospace;font-size:.92em;}
  @media (max-width:480px){ .ttab{font-size:13.5px;} .ttab th,.ttab td{padding:6px;} }
  .note .figsvg{max-width:100%;height:auto;display:block;margin:8px auto;}


  .rep-top{display:flex;flex-wrap:wrap;gap:18px;align-items:center;justify-content:center;margin-top:8px;}
  .rep-legend{flex:1;min-width:220px;display:flex;flex-direction:column;gap:8px;}
  .rep-cap{font:700 13px 'Source Sans 3',sans-serif;color:var(--ink-soft);text-transform:uppercase;letter-spacing:.05em;}
  .rep-li{display:flex;align-items:center;gap:6px;font-size:15px;}
  .rep-n{margin-left:auto;white-space:nowrap;padding-left:8px;font-family:'IBM Plex Mono',monospace;font-weight:600;}
  .sw{display:inline-block;width:12px;height:12px;border-radius:3px;flex:none;}
  .rep-grid{display:grid;grid-template-columns:1fr;gap:12px;}
  @media (min-width:640px){ .rep-grid{grid-template-columns:1fr 1fr;} }
  .rep-card{background:var(--card);border:1px solid var(--rule);border-radius:14px;padding:14px;display:flex;flex-direction:column;gap:10px;}
  .rep-h{display:flex;align-items:center;gap:8px;font:700 16px 'Source Sans 3',sans-serif;}
  .crit{display:inline-grid;place-items:center;width:28px;height:28px;border-radius:50%;color:var(--card);font:700 15px Fraunces,serif;flex:none;}
  .rep-row{display:flex;gap:14px;align-items:center;}
  .rep-stats{display:flex;flex-direction:column;gap:5px;font-size:14.5px;}
  .rep-stats div{display:flex;align-items:center;gap:6px;}
  .rep-lvl{margin-top:4px;color:var(--accent-text);} .rep-lvl span{color:var(--ink-soft);font-size:13px;}
  .rep-note{font-size:13px;color:var(--ink-soft);}


  .skip-chips{display:flex;flex-wrap:wrap;gap:8px;justify-content:center;margin:12px 0;}
  .skip-chips .chip{min-width:48px;min-height:40px;cursor:pointer;border:1.5px solid var(--gold);background:var(--gold-soft);color:var(--retry-text);border-radius:10px;font:600 14px 'IBM Plex Mono',monospace;}
  .skip-btns{display:flex;flex-wrap:wrap;gap:10px;justify-content:center;margin-top:12px;}


  .kb-toggle{border:none;background:transparent;font-size:15px;cursor:pointer;padding:0 2px;vertical-align:middle;opacity:.7;}
  .vkb{position:fixed;left:0;right:0;bottom:0;z-index:80;background:var(--paper-2);border-top:1px solid var(--rule);box-shadow:0 -6px 20px rgba(0,0,0,.12);padding:6px 6px 8px;display:none;}
  .vkb.show{display:block;}
  .vkb-top{display:flex;justify-content:space-between;align-items:center;max-width:640px;margin:0 auto 4px;font:600 12px 'Source Sans 3',sans-serif;color:var(--ink-soft);}
  .vkb-link{border:none;background:none;color:var(--accent-text);font:600 12px 'Source Sans 3',sans-serif;cursor:pointer;text-decoration:underline;}
  .vkb-row{display:flex;gap:5px;max-width:640px;margin:0 auto 5px;}
  .vkb-k{flex:1;min-height:42px;border:1px solid var(--rule);border-radius:8px;background:var(--card);color:var(--ink);font:600 17px 'IBM Plex Mono',monospace;cursor:pointer;padding:0;}
  .vkb-k.fn{font:600 13px 'Source Sans 3',sans-serif;background:var(--gold-soft);}
  .vkb-k.done{background:var(--navy);color:#F4EFDF;border-color:var(--navy);}
  .vkb-k:active{transform:scale(.96);}
  body.kb-open .wrap{padding-bottom:360px;}
  body.kb-open .fab{display:none;}
  .tool-bar{display:flex;gap:8px;flex-wrap:wrap;margin:-4px 0 10px;}
  .tool-btn{min-height:36px;border:1.5px solid var(--gold);background:var(--gold-soft);color:var(--ink);border-radius:18px;padding:4px 12px;font:600 13.5px 'Source Sans 3',sans-serif;cursor:pointer;}
  .tool-panel{position:fixed;z-index:85;background:var(--card);border:1px solid var(--rule);border-radius:14px;box-shadow:0 10px 30px rgba(0,0,0,.25);display:none;}
  .tool-panel.show{display:block;}
  .tp-head{display:flex;align-items:center;gap:8px;padding:8px 10px;border-bottom:1px solid var(--rule);font:600 14px 'Source Sans 3',sans-serif;}
  .tp-note{font-size:12px;color:var(--ink-soft);font-weight:500;}
  .tp-x{margin-left:auto;border:1px solid var(--rule);background:var(--paper-2);color:var(--ink);border-radius:8px;min-height:32px;padding:2px 10px;cursor:pointer;font:600 13px 'Source Sans 3',sans-serif;}
  .tp-x + .tp-x{margin-left:0;}
  .calc{right:12px;bottom:84px;width:min(330px,calc(100vw - 24px));}
  body.calc-open .wrap{padding-bottom:440px;}
  body.calc-open .fab{display:none;}
  @media (max-width:640px){ .calc{left:6px;right:6px;width:auto;} .calc-keys button{min-height:36px;} }
  .calc-disp{padding:8px 12px;text-align:right;background:var(--paper-2);}
  .calc-expr{font:500 13px 'IBM Plex Mono',monospace;color:var(--ink-soft);min-height:18px;word-break:break-all;}
  .calc-res{font:600 24px 'IBM Plex Mono',monospace;color:var(--ink);word-break:break-all;}
  .calc-keys{display:grid;grid-template-columns:repeat(6,1fr);gap:5px;padding:8px;}
  .calc-keys button{min-height:40px;border:1px solid var(--rule);border-radius:8px;background:var(--card);color:var(--ink);font:600 14px 'IBM Plex Mono',monospace;cursor:pointer;padding:0;}
  .calc-keys button.fn{background:var(--gold-soft);font-family:'Source Sans 3',sans-serif;font-size:13px;}
  .calc-keys button.eq{grid-column:span 2;background:var(--navy);color:#F4EFDF;border-color:var(--navy);}
  .desmos{left:50%;top:50%;transform:translate(-50%,-50%);width:min(760px,calc(100vw - 16px));height:min(560px,calc(100vh - 90px));flex-direction:column;}
  .desmos.show{display:flex;}
  #desmosBox{flex:1;min-height:0;border-radius:0 0 14px 14px;overflow:hidden;}
  .desmos-msg{padding:24px;text-align:center;color:var(--ink-soft);}
  .chip[data-status="skipped"]{cursor:pointer;}
  .chip[data-status="answered"]{border-color:var(--accent-text);color:var(--accent-text);}


  button.crest-home{border:none;padding:0;position:relative;cursor:pointer;transition:transform .15s ease;}
  button.crest-home:hover,button.crest-home:focus-visible{transform:scale(1.06);outline:2px solid var(--gold);outline-offset:2px;}
  .crest-h{position:absolute;right:-7px;bottom:-7px;width:18px;height:18px;border-radius:50%;background:#F4EFDF;color:var(--navy);font:700 12px/18px 'Source Sans 3',sans-serif;text-align:center;box-shadow:0 1px 3px rgba(0,0,0,.3);}
  .brand .brand-row{position:relative;}
  .bmasw{position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);display:flex;flex-shrink:0;white-space:nowrap;align-items:center;gap:6px;background:rgba(255,255,255,.12);border:1px solid rgba(255,255,255,.25);border-radius:99px;padding:5px 14px;color:#F4EFDF;}
  .bmasw-ic{font-size:16px;} .bmasw-t{font:600 20px 'IBM Plex Mono',monospace;letter-spacing:.02em;min-width:62px;text-align:center;}
  .bmasw-b{border:none;background:rgba(255,255,255,.18);color:#F4EFDF;border-radius:50%;width:30px;height:30px;cursor:pointer;font-size:13px;}
  .bmasw.off{display:none;}
  @media (max-width:560px){ .bmasw{position:static;transform:none;margin-left:auto;padding:4px 5px 4px 8px;gap:4px;} .bmasw-ic{display:none;} .bmasw-t{font-size:16px;min-width:48px;} .bmasw-b{width:26px;height:26px;} .brand .series-name{font-size:15px;} .brand .brand-name{font-size:10.5px;} .brand .brand-row>div:not(.bmasw){min-width:0;} }
  .bmasw-done{font:600 15px 'IBM Plex Mono',monospace;color:var(--accent-text);margin:4px 0 8px;}
  .sp-fab{position:fixed;left:14px;bottom:84px;z-index:60;border:1.5px solid var(--navy-2);background:var(--card);color:var(--ink);border-radius:99px;padding:9px 14px;font:700 14px 'Source Sans 3',sans-serif;box-shadow:0 4px 14px rgba(0,0,0,.15);cursor:pointer;}
  .sp-fab.on{background:var(--navy);color:#F4EFDF;}
  body.kb-open .sp-fab{display:none;}
  .sp-canvas{position:absolute;z-index:55;display:none;touch-action:none;cursor:crosshair;}
  .sp-canvas.passive{pointer-events:none;cursor:default;}
  .sp-bar{position:fixed;top:8px;left:8px;right:8px;margin:0 auto;width:max-content;z-index:90;display:none;align-items:center;gap:6px;background:var(--card);border:1px solid var(--rule);border-radius:14px;padding:6px 8px;box-shadow:0 6px 20px rgba(0,0,0,.2);max-width:calc(100vw - 16px);flex-wrap:wrap;justify-content:center;}
  .sp-lbl{font:700 13px 'Source Sans 3',sans-serif;color:var(--ink-soft);margin-right:2px;}
  .sp-pen,.sp-tool{width:38px;height:38px;border-radius:10px;border:1.5px solid var(--rule);background:var(--paper);cursor:pointer;display:inline-flex;align-items:center;justify-content:center;font-size:17px;padding:0;color:var(--ink);}
  .sp-pen i{width:20px;height:20px;border-radius:50%;display:block;}
  .sp-pen.on,.sp-tool.on{border-color:var(--navy-2);box-shadow:0 0 0 3px var(--gold-soft);}
  @media (max-width:560px){ .sp-lbl{display:none;} .sp-pen,.sp-tool{width:34px;height:34px;} .sp-fab span{display:none;} }

  /* larger reading sizes */
  .chapter-eyebrow{font-size:13.5px;}
  .chapter-title{font-size:36px;line-height:1.15;}
  .chapter-sub{font-size:16.5px;}
  .tab-btn{font-size:15.5px;}
  .sec-sub{font-size:15px;}
  .qtext{font-size:19px;line-height:1.55;}
  .qnum{width:36px;height:36px;font-size:16px;}
  .opt{font-size:17.5px;padding:12px 14px;}
  .step-line{font-size:17.5px;line-height:2;}
  .blank-input{font-size:16px;}
  .sol-line{font-size:16.5px;}
  .feedback{font-size:15px;}
  .note h2{font-size:28px;}
  .note h4{font-size:19px;}
  .note p,.note li{font-size:17.5px;line-height:1.65;}
  .note .lt{font-size:15.5px;}
  .ex .exh{font-size:18px;} .ex .exl{font-size:16.5px;}
  .keybox{font-size:16.5px;}
  .ttab{font-size:15.5px;}
  .hub-card h3{font-size:21px;} .hub-card p{font-size:15.5px;} .hub-btn{font-size:15px;}
  @media (max-width:480px){ .chapter-title{font-size:30px;} .qtext{font-size:18px;} .opt,.step-line{font-size:16.5px;} .note h2{font-size:24px;} .note p,.note li{font-size:16.5px;} }

  /* v4 celebration */
  .v4conf{position:fixed;inset:0;width:100vw;height:100vh;pointer-events:none;z-index:9999;}
  .v4ban{background:linear-gradient(135deg,var(--gold-soft),var(--card));border:2px solid var(--gold);border-radius:18px;padding:18px 14px 16px;margin:-4px 0 18px;text-align:center;animation:v4pop .55s cubic-bezier(.2,1.6,.4,1);}
  @keyframes v4pop{0%{transform:scale(.6);opacity:0}100%{transform:scale(1);opacity:1}}
  .v4trophy{font-size:54px;line-height:1;animation:v4bob 1.4s ease-in-out infinite;}
  @keyframes v4bob{0%,100%{transform:translateY(0) rotate(-6deg)}50%{transform:translateY(-6px) rotate(6deg)}}
  .v4h{font-size:28px;font-weight:800;color:var(--accent-text);margin-top:6px;}
  .v4m{font-size:19px;color:var(--ink);margin-top:4px;}
  .v4pills{display:flex;flex-wrap:wrap;gap:8px;justify-content:center;margin-top:12px;}
  .v4p{font-size:16px;font-weight:700;border-radius:999px;padding:6px 12px;}
  .v4p.g{background:var(--success-soft);color:var(--success);} .v4p.o{background:var(--gold-soft);color:var(--retry-text);}
  .v4p.r{background:var(--danger-soft);color:var(--danger);} .v4p.s{background:var(--rule);color:var(--ink);}
  .v4next{margin-top:14px;} .v4go{font-size:18px !important;padding:13px 20px !important;}
  .v4rec td.v4g{color:var(--success);font-weight:700;} .v4rec td.v4o{color:var(--retry-text);font-weight:700;} .v4rec td.v4r{color:var(--danger);font-weight:700;}
  .v4rec tr.v4tot td{font-weight:800;border-top:2px solid var(--rule);}
  .v4rec th{font-size:12.5px;padding:6px 3px !important;white-space:nowrap;} .v4rec td{font-size:15px;padding:7px 3px !important;text-align:center;}
  .v4rec td:first-child,.v4rec th:first-child{text-align:left;white-space:normal;min-width:92px;max-width:150px;font-size:14.5px;}
  @media(max-width:460px){ .v4left{display:none;} }
  .v4leg{font-size:14.5px;color:var(--ink-soft);margin:2px 0 8px;line-height:1.5;}
  body.v4done .fab-q,body.v4done #qFab{display:none;}
  .v4sum{font-size:16px;margin-top:10px;}
  /* v4 larger reading sizes */
  body{font-size:18px;}
  .chapter-title{font-size:38px !important;line-height:1.15;}
  .chapter-sub{font-size:17px !important;}
  .tab-btn{font-size:16.5px !important;}
  .sec-sub{font-size:16.5px !important;}
  .qtext{font-size:21px !important;line-height:1.6 !important;}
  .qnum{width:38px !important;height:38px !important;font-size:17px !important;}
  .opt{font-size:19.5px !important;padding:13px 15px !important;}
  .step-line{font-size:19.5px !important;line-height:2.1 !important;}
  .blank-input{font-size:18px !important;min-height:40px;}
  .sol-line{font-size:18px !important;line-height:1.6;}
  .feedback{font-size:16.5px !important;}
  .note h2{font-size:29px !important;}
  .note h3{font-size:22px !important;}
  .note h4{font-size:20px !important;}
  .note p,.note li,.note td,.note th{font-size:18.5px !important;line-height:1.7 !important;}
  .ex .exh{font-size:19px !important;} .ex .exl{font-size:18px !important;}
  .keybox{font-size:18px !important;}
  .hub-card p{font-size:17.5px !important;} .hub-btn{font-size:16.5px !important;}
  .review-q,.review-ans{font-size:17.5px !important;}
  .rec-table td{font-size:16px;}
  .vkb-k{font-size:19px !important;}
  .fq{font-size:0.95em;}

  /* v5 plotters */
  .plotw{background:var(--card);border:1px solid var(--rule);border-radius:12px;padding:10px;margin:6px 0 4px;}
  .plotw svg{display:block;margin:0 auto;cursor:crosshair;}
  .plw-msg{font-size:15px;color:var(--ink-soft);margin:6px 2px;}
  .plw-tools{display:flex;gap:8px;flex-wrap:wrap;margin-top:6px;}
  .plw-tools button,.plw-row button{font:600 14px 'Source Sans 3',sans-serif;border:1px solid var(--rule);background:var(--paper-2);color:var(--ink);border-radius:8px;padding:7px 10px;cursor:pointer;min-height:36px;}
  .plw-row{display:flex;align-items:center;gap:6px;flex-wrap:wrap;padding:6px;border-radius:8px;margin-top:6px;border:1px solid transparent;}
  .plw-row.sel{border-color:var(--gold);background:var(--gold-soft);}
  .plw-sw{width:14px;height:14px;border-radius:4px;display:inline-block;}
  .plw-eq{font:600 16px 'IBM Plex Mono',monospace;margin-right:4px;}
  .plw-sum{font-size:16px;margin-top:8px;} .plw-key{font-size:15px;margin-top:6px;color:var(--ink);}

  /* v6 accuracy meter */
  .accm{max-width:900px;margin:6px auto 0;padding:6px 16px;display:flex;align-items:center;gap:10px;}
  .accg{width:64px;height:38px;flex:0 0 auto;}
  .acct{display:flex;flex-direction:column;line-height:1.25;font-size:14.5px;color:var(--ink-soft);}
  .acct b{font-size:16px;color:var(--ink);} .accp{font:700 18px 'IBM Plex Mono',monospace;margin-left:4px;}
  .accp.g{color:var(--success);} .accp.o{color:var(--retry-text);} .accp.r{color:var(--danger);}
  /* v6 observations */
  .v6obs{text-align:left;background:var(--card);border:1px solid var(--rule);border-left:5px solid var(--accent-text);border-radius:14px;padding:14px 16px;margin:0 0 16px;}
  .v6h{font:700 21px 'Fraunces',Georgia,serif;color:var(--accent-text);margin-bottom:6px;}
  .v6lvl{font-size:17px;font-weight:700;padding:8px 10px;border-radius:10px;margin-bottom:8px;}
  .v6lvl.g{background:var(--success-soft);color:var(--success);} .v6lvl.o{background:var(--gold-soft);color:var(--retry-text);} .v6lvl.r{background:var(--danger-soft);color:var(--danger);}
  .v6sub{font-weight:800;font-size:15px;text-transform:uppercase;letter-spacing:.04em;color:var(--ink-soft);margin:10px 0 4px;}
  .v6ul{margin:0;padding-left:20px;} .v6ul li{font-size:17px;line-height:1.55;margin:3px 0;} .v6p{font-size:17px;margin:2px 0;}
  .v6q{font:700 14px 'IBM Plex Mono',monospace;border:1px solid var(--danger);color:var(--danger);background:var(--danger-soft);border-radius:8px;padding:3px 8px;cursor:pointer;margin:2px 2px;}
  .v6btns{display:flex;flex-direction:column;gap:6px;} .v6btns button{text-align:left;font:600 16px 'Source Sans 3',sans-serif;border:1px solid var(--rule);background:var(--paper-2);color:var(--ink);border-radius:10px;padding:9px 12px;cursor:pointer;}
  /* v6 whiteboard */
  .wb-fab{position:fixed;left:14px;bottom:calc(140px + env(safe-area-inset-bottom,0px));z-index:40;border:1px solid var(--rule);background:var(--card);color:var(--ink);border-radius:999px;padding:9px 14px;font:700 15px 'Source Sans 3',sans-serif;box-shadow:0 2px 8px rgba(0,0,0,.15);cursor:pointer;}
  @media(max-width:520px){ .wb-fab span{display:none;} .wb-fab{padding:9px 11px;} }
  .wbov{position:fixed;inset:0;z-index:9000;background:#f3f4f6;display:none;flex-direction:column;}
  .wbov.show{display:flex;} body.wb-open{overflow:hidden;}
  .wbbar{display:flex;flex-wrap:nowrap;overflow-x:auto;-webkit-overflow-scrolling:touch;align-items:center;gap:4px;padding:6px 8px;background:#fff;border-bottom:1px solid #e5e7eb;box-shadow:0 1px 4px rgba(0,0,0,.06);}
  .wbbar button{flex:0 0 auto;min-width:38px;height:38px;border:1px solid #e5e7eb;background:#fff;border-radius:9px;font:600 17px sans-serif;color:#111;cursor:pointer;}
  .wbbar button.on{border-color:#2563eb;background:#dbeafe;} .wbc{min-width:26px!important;width:26px;height:26px!important;border-radius:50%!important;border:2px solid #d1d5db!important;}
  .wbc.on{outline:3px solid #2563eb;outline-offset:1px;} .wbsep{flex:0 0 auto;width:1px;height:26px;background:#e5e7eb;margin:0 3px;}
  .wbsz{width:90px;flex:0 0 auto;} .wbpg{font:600 14px sans-serif;color:#374151;min-width:44px;text-align:center;} .wbx{padding:0 10px;font-size:15px!important;}
  .wbcv{flex:1;width:100%;min-width:0;min-height:0;touch-action:none;cursor:crosshair;display:block;background:#fff;}
  .wbbody{flex:1;display:flex;flex-direction:column;min-height:0;}
  .wbq{background:var(--paper);color:var(--ink);border-bottom:3px solid var(--gold);max-height:40vh;overflow:auto;padding:8px 12px 10px;flex:0 0 auto;}
  .wbqh{display:flex;align-items:center;justify-content:space-between;gap:8px;font-size:15px;color:var(--accent-text);margin-bottom:6px;position:sticky;top:-8px;background:var(--paper);padding:4px 0;z-index:1;}
  .wbqt{font:600 14px 'Source Sans 3',sans-serif;border:1px solid var(--rule);background:var(--card);color:var(--ink);border-radius:8px;padding:5px 10px;cursor:pointer;}
  .wbq.min{max-height:none;} .wbq.min .wbqc{display:none;}
  .wbqc .qcard{margin:0;box-shadow:none;} .wbqc .qtext{font-size:19px !important;} .wbqc input{pointer-events:none;}
  @media(min-width:860px){ .wbbody{flex-direction:row;} .wbq{width:40%;max-width:520px;max-height:none;border-bottom:0;border-right:3px solid var(--gold);} .wbq.min{width:auto;} }
  .wbin{position:fixed;z-index:9001;font:20px 'Source Sans 3',sans-serif;border:1px dashed #2563eb;background:rgba(255,255,255,.9);padding:2px 6px;min-width:140px;}

  .scatw{background:var(--card);border:1px solid var(--rule);border-radius:12px;padding:8px;margin:6px 0 4px;}
  .scatw svg{display:block;margin:0 auto;cursor:crosshair;}
  .scw-sum{font-size:15.5px;margin-top:6px;}

  .gp-hidden{position:absolute !important;width:2px !important;height:2px !important;padding:0 !important;border:0 !important;opacity:0 !important;overflow:hidden;}
  .gp-box{margin:8px 0 4px;padding:10px;border:1px solid var(--rule);border-radius:12px;background:var(--card);}
  .gp-help{font-size:15px;color:var(--ink-soft);margin-bottom:6px;line-height:1.4;}
  .gp-svg{display:block;margin:0 auto;width:100%;max-width:380px;user-select:none;-webkit-user-select:none;cursor:crosshair;}
  .gp-tools{display:flex;flex-wrap:wrap;gap:6px;align-items:center;margin-top:8px;}
  .gp-tools.gp-n{display:block;line-height:2.6;}
  .gp-b{font:600 15px 'Source Sans 3',sans-serif;border:1.5px solid var(--rule);background:var(--paper);color:var(--ink);border-radius:999px;padding:6px 12px;cursor:pointer;margin:0 3px 0 0;}
  .gp-b.on{border-color:var(--accent-text);background:var(--gold-soft);color:var(--accent-text);}
  .gp-lab{font-weight:700;margin-right:6px;}
  .gp-in{font:16px 'IBM Plex Mono',monospace;width:90px;border:1.5px solid var(--rule);border-radius:6px;padding:4px 6px;margin-right:6px;background:var(--card);color:var(--ink);}
  .gp-stat{font-size:15px;margin-top:6px;color:var(--accent-text);font-weight:600;}
  .ineq-grapher{border:2px solid var(--gold);border-radius:14px;padding:12px;margin:14px 0;background:var(--card);}
  .gr-head{font:700 19px 'Fraunces',serif;color:var(--accent-text);margin-bottom:6px;}
  .gr-row{display:flex;gap:8px;} .gr-in{flex:1;min-width:0;font:16px 'IBM Plex Mono',monospace;border:1.5px solid var(--rule);border-radius:8px;padding:8px;background:var(--paper);color:var(--ink);}
  .gr-hint{font-size:14.5px;color:var(--ink-soft);margin:6px 0;}
  .gr-cv{width:100%;max-width:420px;display:block;margin:6px auto;border:1px solid var(--rule);border-radius:8px;}
  .gr-msg{font-size:15px;color:var(--accent-text);font-weight:600;}

  header.brand{background:linear-gradient(180deg,rgba(20,20,20,.55),rgba(20,20,20,.78)),url('data:image/jpeg;base64,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') center/cover no-repeat, #2b2b2b !important;}
  .crest,button.crest-home{width:58px !important;height:54px !important;background:transparent !important;border-radius:12px !important;}
  .crest img{width:58px;height:53px;display:block;filter:drop-shadow(0 1px 2px rgba(0,0,0,.5));}
  button.crest-home .crest-h{right:-4px;bottom:-4px;}
  .brand-name{color:#F4EFDF !important;font-family:'Fraunces',Georgia,serif;font-size:13px !important;letter-spacing:.06em;}
  .series-name{color:#E8D9A8;}
  .chapter-eyebrow{color:#D9D4C7 !important;}
  .chapter-sub{color:#F1D58A !important;}

  .ex-sum{background:var(--gold-soft);border:2px solid var(--gold);border-radius:16px;padding:14px 16px;margin:10px 0 16px;text-align:center;}
  .ex-big{font:800 44px 'Fraunces',Georgia,serif;color:var(--accent-text);line-height:1.1;} .ex-big span{font-size:22px;color:var(--ink-soft);}
  .ex-lab{font-size:15px;color:var(--ink-soft);margin-top:2px;}
  .ex-row{display:flex;flex-wrap:wrap;gap:8px 16px;justify-content:center;margin-top:10px;font-size:16px;}
  .ex-tip{margin-top:10px;font-size:15.5px;color:var(--ink);}
  .fig{flex-direction:column;align-items:center;} .fig>*{max-width:100%;} .fig>.fig{width:100%;}
  .ex-small .ex-big{font-size:34px;} .ex-net{font-size:15.5px;} .ex-net span{color:var(--ink-soft);font-size:13.5px;}
</style>
</head>
<body>
<header class="brand">
  <div class="brand-row">
    <div class="crest"><img src="data:image/png;base64,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" alt="Brain and Mind"></div>
    <div>
      <div class="brand-name">Brain &amp; Mind Academy</div>
      <div class="series-name">Sopaan <span style="font-weight:400;font-size:14px;color:#CFD7EA;">Practice Series</span></div>
    </div>
  </div>
  <div class="chapter-eyebrow">CMGGA 2026 · Written examination practice</div>
  <div class="chapter-title">CMGGA 2026 · Mock Paper 1</div>
  <div class="chapter-sub">100 Questions · Parts A–E · Negative marking</div><div class="chapter-credit">Theory · Step-by-step practice · Learning assessment</div>
  <div class="chapter-progress">
    <div class="cp-track"><div class="cp-fill" id="cpFill"></div></div>
    <div class="cp-label" id="cpLabel">0% complete</div>
  </div>
  <div class="who-row"><button class="mode-pill" id="modePill" hidden>Choose a mode</button><span class="who" id="whoBar" hidden></span></div>
</header>

<nav class="tabbar"><div class="tabbar-inner" id="tabbar"></div></nav>
<div class="sec-sub" id="secSub"></div><div class="slide-progress"><div class="sp-track"><div class="sp-fill" id="spFill"></div></div><div class="sp-label" id="spLabel">Question 1 of 49</div></div>
<div class="wrap" id="wrap"></div>
<footer class="brandfoot">Brain &amp; Mind Academy · Sopaan Practice Series<br>Original mock paper written by Brain &amp; Mind Academy for the CMGGA 2026 written examination. Not an official paper.</footer>

<div class="navbar"><div class="navbar-inner" id="navbarInner"></div></div>
<button class="fab" id="paletteFab"><span>Questions</span><span class="fab-badge" id="fabBadge">0/49</span></button>

<div class="overlay" id="overlay">
  <div class="palette" role="dialog" aria-label="Question palette">
    <div class="palette-head"><h2 id="paletteTitle">Question palette</h2><button class="palette-close" id="paletteClose">&times;</button></div>
    <div class="palette-legend">
      <span><i class="dot current"></i>Current</span><span><i class="dot correct"></i>Correct</span>
      <span><i class="dot revealed"></i>Revealed</span><span><i class="dot skipped"></i>Skipped</span>
      <span><i class="dot locked"></i>Locked</span>
    </div>
    <div class="chip-grid" id="paletteBody"></div>
  </div>
</div>
<div class="toast" id="toast"></div>

<script>
(function(){
"use strict";

/* ================= audio ================= */
var audioCtx=null;
function ensureAudio(){ if(!audioCtx){ try{ audioCtx=new (window.AudioContext||window.webkitAudioContext)(); }catch(e){} } return audioCtx; }
function playTone(freqs,dur,type){
  var ctx=ensureAudio(); if(!ctx) return;
  try{
    var t0=ctx.currentTime;
    freqs.forEach(function(f,i){
      var o=ctx.createOscillator(), g=ctx.createGain();
      o.type=type||'sine'; o.frequency.value=f;
      var start=t0+i*dur;
      g.gain.setValueAtTime(0.0001,start);
      g.gain.exponentialRampToValueAtTime(0.16,start+0.02);
      g.gain.exponentialRampToValueAtTime(0.0001,start+dur);
      o.connect(g); g.connect(ctx.destination);
      o.start(start); o.stop(start+dur+0.02);
    });
  }catch(e){}
}
function playSuccess(){ playTone([523.25,659.25,783.99],0.11,'sine'); }
function playWrong(){ playTone([220,185],0.14,'square'); }
function playReveal(){ playTone([300,220],0.16,'triangle'); }

/* ================= helpers ================= */
function norm(s){
  return String(s===undefined||s===null?'':s).trim().toLowerCase().replace(/\s+/g,'')
    .replace(/[×∗*·]/g,'x').replace(/÷/g,'/').replace(/–|—|−/g,'-')
    .replace(/[²]/g,'^2').replace(/[³]/g,'^3').replace(/[⁴]/g,'^4').replace(/[⁵]/g,'^5')
    .replace(/[⁶]/g,'^6').replace(/[⁷]/g,'^7').replace(/[⁸]/g,'^8').replace(/[⁹]/g,'^9')
    .replace(/\^/g,'');
}
function parseNum(s){
  if(s===undefined||s===null) return null;
  var t=String(s).trim().replace(/,/g,'').replace(/[−–—]/g,'-').replace(/\s+/g,''); if(t==='') return null;
  var neg=false; if(t[0]==='-'){neg=true;t=t.slice(1);}
  var m=t.match(/^(\d+)\/(\d+)$/);
  if(m){ var v=parseInt(m[1],10)/parseInt(m[2],10); return neg?-v:v; }
  if(/^\d+(\.\d+)?$/.test(t)){ var v2=parseFloat(t); return neg?-v2:v2; }
  return null;
}
/* ---- expression checker: compares answers like (P-2w)/2 and P/2-w at random values ---- */
function exprPrep(s){
  return String(s).toLowerCase().replace(/\s+/g,'').replace(/^[a-z]\(x\)=/i,'').replace(/^[a-z]=/i,'').replace(/[×∗·]/g,'*').replace(/÷/g,'/').replace(/[−–—]/g,'-')
    .replace(/²/g,'^2').replace(/³/g,'^3').replace(/⁴/g,'^4').replace(/⁵/g,'^5').replace(/⁶/g,'^6').replace(/⁷/g,'^7').replace(/⁸/g,'^8').replace(/⁹/g,'^9').replace(/π/g,'#').replace(/pi/gi,'#').replace(/½/g,'(1/2)');
}
function exprCompile(src){
  var s=exprPrep(src), i=0, toks=[], absDepth=0;
  while(i<s.length){
    var ch=s[i];
    if(/[0-9.]/.test(ch)){ var j=i; while(j<s.length && /[0-9.]/.test(s[j])) j++; toks.push({k:'n',v:parseFloat(s.slice(i,j))}); i=j; continue; }
    if(/[a-zA-Z#]/.test(ch)){ toks.push({k:'v',v:ch}); i++; continue; }
    if(ch==='|'){ var pv=toks[toks.length-1]; var opn=(absDepth===0)||!pv||('+-*/^(['.indexOf(pv.k)>=0); if(opn){ absDepth++; toks.push({k:'['}); } else { absDepth--; toks.push({k:']'}); } i++; continue; }
    if('+-*/^()'.indexOf(ch)>=0){ toks.push({k:ch}); i++; continue; }
    return null;
  }
  var out=[];
  for(var t=0;t<toks.length;t++){
    var a=toks[t], b=out[out.length-1];
    if(b && (b.k==='n'||b.k==='v'||b.k===')'||b.k===']') && (a.k==='n'||a.k==='v'||a.k==='('||a.k==='[')) out.push({k:'&'});
    out.push(a);
  }
  var p=0;
  function peek(){ return out[p]; }
  function parseE(){ var n=parseT(); while(peek() && (peek().k==='+'||peek().k==='-')){ var o=out[p++].k, r=parseT(); n=(function(l,r,o){return function(e){ return o==='+'?l(e)+r(e):l(e)-r(e); };})(n,r,o); } return n; }
  function parseI(){ var n=parseU(); while(peek() && peek().k==='&'){ p++; var r=parseP(); n=(function(l,r){return function(e){ return l(e)*r(e); };})(n,r); } return n; }
  function parseT(){ var n=parseI(); while(peek() && (peek().k==='*'||peek().k==='/')){ var o=out[p++].k, r=parseI(); n=(function(l,r,o){return function(e){ return o==='*'?l(e)*r(e):l(e)/r(e); };})(n,r,o); } return n; }
  function parseU(){ if(peek() && peek().k==='-'){ p++; var u=parseU(); return function(e){ return -u(e); }; } if(peek() && peek().k==='+'){ p++; return parseU(); } return parseP(); }
  function parseP(){ var b=parseA(); if(peek() && peek().k==='^'){ p++; var x=parseU(); return function(e){ return Math.pow(b(e),x(e)); }; } return b; }
  function parseA(){
    var t=out[p++]; if(!t) throw 0;
    if(t.k==='n') return function(){ return t.v; };
    if(t.k==='v') return t.v==='#' ? function(){ return Math.PI; } : function(e){ return e[t.v]; };
    if(t.k==='('){ var n=parseE(); if(!peek()||peek().k!==')') throw 0; p++; return n; }
    if(t.k==='['){ var m=parseE(); if(!peek()||peek().k!==']') throw 0; p++; return function(e){ return Math.abs(m(e)); }; }
    throw 0;
  }
  try{ var f=parseE(); if(p!==out.length) return null; return f; }catch(e){ return null; }
}
function exprEqual(input,answer){
  var f=exprCompile(input), g=exprCompile(answer); if(!f||!g) return false;
  var hits=0;
  for(var trial=0;trial<8;trial++){
    var env={}; 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'.split('').forEach(function(c){ env[c]=1.3+Math.random()*4.1; });
    var x=f(env), y=g(env);
    if(!isFinite(x)||!isFinite(y)) continue;
    if(Math.abs(x-y)>1e-7*Math.max(1,Math.abs(x),Math.abs(y))) return false;
    hits++;
  }
  return hits>=3;
}
function wordsNorm(s){ return String(s||'').toLowerCase().replace(/\band\b/g,' ').replace(/[^a-z]/g,''); }
function listNorm(s){ return (String(s||'').replace(/[−–—]/g,'-').replace(/(\d) (?=\d{3}\b)/g,'$1').match(/-?\d+(\.\d+)?/g)||[]).join(','); }
function powNorm(s){ return String(s||'').toLowerCase().replace(/\s+/g,'').replace(/[×∗*·.]/g,'x').replace(/[⁰¹²³⁴⁵⁶⁷⁸⁹]+/g,function(m){ return '^'+m.split('').map(function(c){ return '⁰¹²³⁴⁵⁶⁷⁸⁹'.indexOf(c); }).join(''); }).replace(/\^1(?!\d)/g,''); }
function fr(s){ return String(s).replace(/\{(\d+) (\d+)\/(\d+)\}/g,'<span class="mx">$1<span class="fq"><span>$2</span><span>$3</span></span></span>').replace(/\{(\d+)\/(\d+)\}/g,'<span class="fq"><span>$1</span><span>$2</span></span>'); }
function gcdI(a,b){ a=Math.abs(a); b=Math.abs(b); while(b){ var t=a%b; a=b; b=t; } return a; }
function fracParse(s){ s=String(s===undefined||s===null?'':s).trim().replace(/[\u2044\u2215\u00f7]/g,'/').replace(/\s+/g,' ').replace(/\s*\/\s*/g,'/'); var m;
  if((m=s.match(/^(-?\d+)$/))) return {v:+m[1],form:'int',n:+m[1],d:1};
  if((m=s.match(/^(-?\d+)\/(\d+)$/))){ if(+m[2]===0) return null; return {v:m[1]/m[2],form:'frac',n:+m[1],d:+m[2]}; }
  if((m=s.match(/^(-?)(\d+)(?: |\+)(\d+)\/(\d+)$/))){ if(+m[4]===0) return null; var sg=m[1]?-1:1; return {v:sg*(+m[2]+m[3]/m[4]),form:'mixed',w:sg*m[2],n:+m[3],d:+m[4]}; }
  if((m=s.match(/^-?\d*\.\d+$/))) return {v:parseFloat(s),form:'dec'};
  return null; }
function fracOK(mode,input,answer){
  if(mode==='flist'){ var A=String(input).split(/[,;]/).map(function(x){return x.trim();}).filter(Boolean), K=String(answer).split(/[,;]/).map(function(x){return x.trim();});
    if(A.length!==K.length) return false; return A.every(function(x,i){ var a=fracParse(x), k=fracParse(K[i]); return a&&k&&Math.abs(a.v-k.v)<1e-9; }); }
  var a=fracParse(input), k=fracParse(answer); if(!a||!k) return false;
  var same=Math.abs(a.v-k.v)<1e-9; if(!same) return false;
  if(mode==='fv') return true;
  if(mode==='dec') return a.form==='dec'||a.form==='int';
  if(mode==='fe') return (a.form==='frac'&&k.form==='frac'&&a.n===k.n&&a.d===k.d)||(a.form==='int'&&k.form==='int');
  if(mode==='fi') return a.form==='frac'||(a.form==='int'&&k.form==='int');
  if(mode==='fl') return a.form==='int'||(a.form==='frac'&&gcdI(a.n,a.d)===1)||(a.form==='mixed'&&a.n<a.d&&gcdI(a.n,a.d)===1);
  if(mode==='fm') return a.form==='int'||(a.form==='mixed'&&a.n>0&&a.n<a.d&&gcdI(a.n,a.d)===1);
  return false; }
function answerMatches(input,answer,accept,expr){
  if(expr==='dec'||expr==='fv'||expr==='fe'||expr==='fl'||expr==='fm'||expr==='fi'||expr==='flist'){ if(input===undefined||input===null||String(input).trim()==='') return false; return fracOK(expr,input,answer); }
  if(input===undefined||input===null||String(input).trim()==='') return false;
  if(expr==='words'){ return [answer].concat(accept||[]).some(function(a){ if(/\d/.test(a)) return norm(a)===norm(input); var w=wordsNorm(a); return w!=='' && w===wordsNorm(input); }); }
  if(expr==='list'){ return [answer].concat(accept||[]).some(function(a){ return listNorm(a)===listNorm(input); }); }
  if(expr==='pow'){ return [answer].concat(accept||[]).some(function(a){ return powNorm(a)===powNorm(input); }); }
  if(expr==='time'){ var tn=function(x){ var t=String(x).toLowerCase().replace(/[\s.]/g,'').replace(/[:h]/g,''); if(/^\d{3}(am|pm)?$/.test(t)) t='0'+t; return t; }; return [answer].concat(accept||[]).some(function(a){ return tn(a)===tn(input); }); }
  if(expr==='glist'){ var gn=function(x){ return String(x).toUpperCase().split(/[\s,;]+/).filter(Boolean).sort().join(','); }; return [answer].concat(accept||[]).some(function(a){ return gn(a)===gn(input); }); }
  if(expr==='coord'){ var cn=function(x){ return String(x).replace(/[\u2212\u2013\u2014]/g,'-').replace(/[\s()\[\]]/g,''); }; return [answer].concat(accept||[]).some(function(a){ return cn(a)===cn(input); }); }
  if(expr==='dlist'){ var dn=function(x){ return (String(x).replace(/[−–—]/g,'-').match(/-?\d*\.?\d+/g)||[]).map(Number).join(','); }; return [answer].concat(accept||[]).some(function(a){ return dn(a)===dn(input); }); }
  if(expr==='set'){ var sn=function(x){ return (String(x).match(/-?\d+/g)||[]).map(Number).sort(function(a,b){return a-b;}).join(','); }; return [answer].concat(accept||[]).some(function(a){ return sn(a)===sn(input); }); }
  if(expr==='primes'){ var pn=function(x){ var t=powNorm(x).replace(/[^0-9x^]/g,''); var out=[]; t.split('x').forEach(function(tok){ if(!tok) return; var m=tok.split('^'); var b=+m[0], e=m[1]?+m[1]:1; for(var i=0;i<e;i++) out.push(b); }); return out.sort(function(a,b){return a-b;}).join(','); }; return [answer].concat(accept||[]).some(function(a){ return pn(a)===pn(input); }); }
  if(expr==='angle'){ var an=function(x){ return String(x).toUpperCase().replace(/[^A-Z]/g,''); }; var k=an(answer), v=an(input); return v===k || v===k.split('').reverse().join(''); }
  if(expr==='trans'){ var tv=function(x){ var s=String(x).toLowerCase().replace(/[−–—]/g,'-').replace(/\b(units?|squares?|and|then|steps?|to|the|a)\b/g,' ').replace(/[,;.]/g,' '); var re=/(\d+)\s*(right|left|up|down|r|l|u|d)\b/g, m, dx=0, dy=0, n=0; while((m=re.exec(s))){ var v=+m[1], d=m[2][0]; if(d==='r')dx+=v; else if(d==='l')dx-=v; else if(d==='u')dy+=v; else dy-=v; n++; } if(!n||s.replace(re,'').replace(/\s+/g,'')!=='') return null; return dx+','+dy; }; var ti=tv(input); return ti!==null && [answer].concat(accept||[]).some(function(a){ return tv(a)===ti; }); }
  if(expr==='rot'){ var rv=function(x){ var s=String(x).toLowerCase().replace(/quarter[\s-]*turn/g,'90').replace(/half[\s-]*turn/g,'180').replace(/three[\s-]*quarter[\s-]*turn/g,'270'); var m=s.match(/\b(90|180|270)\b/); if(!m) return null; var a=+m[1]; if(a===180) return '180'; var dir=/anti|counter|acw|ccw/.test(s)?-1:(/clockwise|\bcw\b/.test(s)?1:0); if(!dir) return null; return String(((a*dir)%360+360)%360); }; var ri=rv(input); return ri!==null && ri===rv(answer); }
  if(expr==='expanded'){ var f=function(x){ return String(x).replace(/\s+/g,'').replace(/,/g,''); }; return [answer].concat(accept||[]).some(function(a){ return f(a)===f(input); }); }
  if(expr===true && input!==undefined && input!==null && String(input).trim()!==''){
    if(exprEqual(input,answer)) return true;
    var alt=String(input).replace(/\/\s*(\d+(?:\.\d+)?)\s*([a-zA-Z(])/g,'/$1*$2'); if(alt!==String(input) && exprEqual(alt,answer)) return true;
    return (accept||[]).some(function(a){ return exprEqual(input,a); });
  }
  if(input===undefined||input===null||String(input).trim()==='') return false;
  var n1=parseNum(input), n2=parseNum(answer);
  if(n1!==null && n2!==null){ if(Math.abs(n1-n2)<1e-3) return true; return (accept||[]).some(function(a){ var n3=parseNum(a); return n3!==null && Math.abs(n1-n3)<1e-3; }); }
  var cands=[answer].concat(accept||[]); var ni=norm(input);
  for(var i=0;i<cands.length;i++){ if(norm(cands[i])===ni) return true; }
  return false;
}
function esc(s){ return String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;'); }

/* ================= DATA ================= */
var AR_OPTIONS = ["Both A and R are true, and R is the correct explanation of A","Both A and R are true, but R is NOT the correct explanation of A","A is true but R is false","A is false but R is true"];
var THEORY = "<div class=\"hub\"><div class=\"hub-card\"><h3>📝 CMGGA 2026 · Mock Paper 1</h3><p>100 objective questions in five parts, exactly like the written examination. Marking: <b>+1</b> correct, <b>−0.33</b> wrong, <b>0</b> unattempted.</p><div class=\"hub-btns\"><button class=\"hub-btn\" data-go=\"s1\">Part A · 15 Q</button><button class=\"hub-btn\" data-go=\"s2\">Part B · 25 Q</button><button class=\"hub-btn\" data-go=\"s3\">Part C · 25 Q</button><button class=\"hub-btn\" data-go=\"s4\">Part D · 15 Q</button><button class=\"hub-btn\" data-go=\"s5\">Part E · 20 Q</button><button class=\"hub-btn primary\" data-go=\"report\">📊 Score report</button></div></div></div><section class=\"note\" id=\"nintro\"><h2>How to take this mock paper</h2><div class=\"tscroll\"><table class=\"ttab\"><tr><th>Part</th><th>Domain</th><th>Questions</th><th>Marks</th></tr><tr><td>A</td><td>Governance, Haryana and public systems</td><td>15</td><td>15</td></tr><tr><td>B</td><td>Quantitative aptitude and data interpretation</td><td>25</td><td>25</td></tr><tr><td>C</td><td>Logical, analytical and critical reasoning</td><td>25</td><td>25</td></tr><tr><td>D</td><td>English and Hindi communication</td><td>15</td><td>15</td></tr><tr><td>E</td><td>Behavioural and administrative judgement</td><td>20</td><td>20</td></tr><tr><td></td><td><b>Total</b></td><td><b>100</b></td><td><b>100</b></td></tr></table></div><ol><li><b>Exam practice:</b> switch to <b>📝 Quiz Mode</b> (mode pill in the header). Answer the parts in any order; nothing is marked until you finish a part. The clock in the header shows time since you signed in — aim for about <b>1 minute per question</b> and check your admit card for the exact paper duration.</li><li><b>Score:</b> after each part you see your net score for that part; the <b>📊 Score report</b> tab adds them up with negative marking.</li><li><b>Learn from mistakes:</b> every question has a worked explanation. Use <b>📘 Learning Sheet</b> mode afterwards to retry with instant feedback.</li><li><b>Negative marking strategy:</b> a wrong answer costs a third of a mark, so guess only when you can eliminate at least one or two options.</li></ol><p style=\"font-size:15px;color:var(--ink-soft)\">Indicative syllabus: CMGGA 2026 examination pattern (Stage 2, written examination, 23 October 2026). Questions, passages and explanations are original practice material written by Brain &amp; Mind Academy; they are not official questions.</p></section>";
var REPORT = [["s1", "A", "Governance, Haryana and public systems"], ["s2", "B", "Quantitative aptitude and data interpretation"], ["s3", "C", "Logical, analytical and critical reasoning"], ["s4", "D", "English and Hindi communication"], ["s5", "E", "Behavioural and administrative judgement"]];
var SECTIONS = [{"id": "s1", "label": "Part A", "sub": "Governance, Haryana and public systems · 15 questions · 15 marks", "slides": [{"kind": "mcq", "text": "The 73rd Constitutional Amendment makes some features of Panchayati Raj compulsory for every state and leaves others to the state legislature. Which of the following is left to the <b>discretion of the state legislature</b>?", "opts": ["Constituting a State Finance Commission to review the finances of panchayats", "Handing over all 29 subjects of the Eleventh Schedule to the panchayats", "Holding panchayat elections through a State Election Commission", "Reserving at least one-third of seats in panchayats for women"], "correct": 1, "tag": "", "sol": "Article 243G says the state legislature <i>may</i> give panchayats powers and functions, including those on the Eleventh Schedule's 29 subjects. How much is actually handed over is therefore up to each state. A State Finance Commission (243I), a State Election Commission (243K) and at least one-third of seats for women (243D) are all compulsory. The common trap is to think the 29 subjects pass to panchayats automatically. The Schedule only lists subjects a state can devolve."}, {"kind": "mcq", "text": "A Haryana municipal council argues that it should get a fixed share of the stamp duty the state collects inside its limits. Which body is constitutionally responsible for recommending how state taxes and duties are shared between the state and its municipalities?", "opts": ["The Finance Commission of India constituted under Article 280", "The GST Council constituted under Article 279A", "The State Finance Commission under Article 243Y read with Article 243I", "The District Planning Committee under Article 243ZD"], "correct": 2, "tag": "", "sol": "Article 243Y requires the State Finance Commission set up under Article 243I to review municipal finances. It also recommends how the state's taxes, duties, tolls and fees should be shared between the state and its municipalities. The Union Finance Commission recommends how taxes are shared between the Centre and the states. It only proposes measures to boost a state's funds for local bodies, using the SFC's recommendations. The GST Council deals only with GST, and the DPC consolidates plans; neither of them shares out revenue."}, {"kind": "mcq", "text": "An NGO asks a High Court to order the state to supply hot cooked meals in every school. Its only ground is Article 47, which deals with nutrition and public health. Which statement best describes how Directive Principles like Article 47 work?", "opts": ["Courts cannot enforce them on their own, but they are fundamental to governance and the state must apply them when making laws", "Courts can enforce them directly, just like Fundamental Rights, through a writ petition", "They bind only the Union government, so state governments are not covered", "They take effect only after the Finance Commission recommends funds for them"], "correct": 0, "tag": "", "sol": "Article 37 says Directive Principles cannot be enforced by any court. It also declares them fundamental in the governance of the country and puts the state under a duty to apply them in making laws. They therefore reach citizens through laws and schemes. The NFSA's meal and ration entitlements are an example, and those can be enforced because a statute creates them. Option (b) mixes up DPSPs with Fundamental Rights. Option (c) is wrong because 'State' in Part IV covers state governments too."}, {"kind": "mcq", "text": "A farmer in Kaithal cannot complete his <i>Meri Fasal Mera Byora</i> registration because the land area shown for him does not match what he cultivates. The portal draws land details from the Revenue Department's records. What is the correct way to resolve this?", "opts": ["Ask the Block Development and Panchayat Officer to edit the area directly on the portal", "Ask the Gram Sabha to pass a resolution certifying the cultivated area", "Ask the mandi's market committee to accept his produce without registration", "Get the land record corrected through the patwari and tehsil revenue office so that correct data reaches the portal"], "correct": 3, "tag": "", "sol": "MFMB takes land and holding details from the Revenue Department's land-record system (Web-HALRIS). The lasting fix is to correct the source record at the revenue field level, through the patwari and the tehsil office. The BDPO handles development and panchayat work, not land records. A Gram Sabha resolution cannot override revenue records. Selling without registration does not fix the data. The same mismatch would block MSP payment and other benefits linked to the portal."}, {"kind": "mcq", "text": "Which sequence correctly arranges the territorial units of general and revenue administration in Haryana from the <b>largest to the smallest</b>?", "opts": ["District → Tehsil → Sub-division → Patwar circle", "District → Sub-division → Tehsil → Patwar circle", "Sub-division → District → Tehsil → Patwar circle", "District → Patwar circle → Tehsil → Sub-division"], "correct": 1, "tag": "", "sol": "A district, headed by the Deputy Commissioner, is divided into sub-divisions headed by SDMs. Each sub-division contains one or more tehsils under a Tehsildar, and each tehsil is divided into patwar circles, where the patwari keeps village land records. The usual trap is to put the tehsil above the sub-division. The SDM supervises the tehsils within the sub-division, not the other way round."}, {"kind": "mcq", "text": "Several villages in one block need a shared drain and a link road that crosses all of their boundaries. Under Haryana's three-tier Panchayati Raj structure, which body's plan should normally include this work?", "opts": ["The Panchayat Samiti, constituted at the block level", "The Gram Panchayat of the largest village, which should carry out the whole work", "The Zila Parishad alone, since any shared asset is a district subject", "The Gram Sabha of each village separately, with no coordination"], "correct": 0, "tag": "", "sol": "Haryana's Panchayati Raj Act, 1994 sets up a Gram Panchayat for the village, a Panchayat Samiti for the block and a Zila Parishad for the district. Work that spans several villages of one block belongs at the middle tier, the Panchayat Samiti. That level matches the area the work covers. One village panchayat cannot plan for its neighbours. Sending a block-level job straight to the Zila Parishad skips the intermediate tier."}, {"kind": "mcq", "text": "Under Part IXA of the Constitution, introduced by the 74th Amendment, which municipalities <b>must</b> set up Wards Committees?", "opts": ["Every Nagar Panchayat in a transitional area", "Only municipal corporations of state capitals", "Municipalities with a population of three lakh or more", "Only those municipalities whose councillors request it by resolution"], "correct": 2, "tag": "", "sol": "Article 243S requires Wards Committees, made up of one or more wards, in the area of every municipality with a population of three lakh or more. The state legislature decides their composition and territorial area. The obligation depends on population, not on a municipality's status as a capital or on a council resolution. Smaller municipalities may still set up ward-level bodies if state law allows it."}, {"kind": "mcq", "text": "A district reviews its nutrition programme for children under six who attend anganwadi centres. Which of the following is an <b>outcome</b> indicator rather than an output indicator?", "opts": ["Number of take-home ration packets distributed in the quarter", "Number of anganwadi workers trained in growth monitoring", "Percentage of anganwadi centres that submitted monthly reports on time", "Change in the percentage of under-five children who are underweight"], "correct": 3, "tag": "", "sol": "Outputs are the goods and services a programme directly produces, such as packets distributed, workers trained and reports filed. Outcomes are the changes those outputs are meant to bring about in people's lives, such as a lower share of underweight children. Options (a)–(c) can all improve while children stay malnourished. That is why monitoring and evaluation must track outcomes and not only outputs."}, {"kind": "mcq", "text": "A pilot of SMS reminders for immunisation runs in 2 blocks of a district. Full-immunisation coverage in these blocks rises from 70% to 82% in a year. Which evidence would <b>most strengthen</b> the claim that the SMS pilot caused the rise?", "opts": ["Similar blocks of the same district that did not get the pilot rose only from 71% to 73% over the same year", "Health workers in the pilot blocks said in interviews that they found the SMS system useful", "The pilot blocks are among the best-performing blocks in the district on most indicators", "The number of SMS messages sent rose every month during the pilot"], "correct": 0, "tag": "", "sol": "To claim the pilot caused the rise, you need the counterfactual: what would have happened without it. Similar non-pilot blocks that rose by only 2 points suggest that about 10 of the 12 points came from the pilot. This is a difference-in-differences comparison. Worker opinions and SMS volumes are process or output evidence and do not show impact. Option (c) actually weakens the claim, because strong blocks may have improved anyway. That is selection bias."}, {"kind": "mcq", "text": "Under the National Food Security Act, 2013, a <b>Priority Household</b> of 4 members and an <b>Antyodaya Anna Yojana (AAY)</b> household of 4 members are each entitled to how much foodgrain per month?", "opts": ["Priority: 35 kg; AAY: 20 kg", "Priority: 20 kg; AAY: 35 kg", "Priority: 20 kg; AAY: 20 kg", "Priority: 25 kg; AAY: 35 kg"], "correct": 1, "tag": "", "sol": "NFSA gives Priority Households 5 kg per person per month, so a family of 4 gets 4 × 5 = 20 kg. AAY households, the poorest of the poor, get a flat 35 kg per household per month, whatever their size. The trap is to apply the per-person rule to AAY. For a 4-member family, the AAY entitlement of 35 kg is more than the per-person total of 20 kg."}, {"kind": "mcq", "text": "Which of the following is <b>not</b> one of the six services traditionally delivered through anganwadi centres under ICDS?", "opts": ["Supplementary nutrition", "Pre-school non-formal education", "Registration and issue of caste certificates", "Immunisation, health check-ups and referral services"], "correct": 2, "tag": "", "sol": "The ICDS package has six services: supplementary nutrition, pre-school non-formal education, nutrition and health education, immunisation, health check-ups and referral services. Immunisation, check-ups and referral are delivered together with the health system. Caste certificates are a revenue-administration service applied for through the e-services or SARAL platform. They are not an anganwadi function."}, {"kind": "mcq", "text": "A citizen files an RTI application with a district office. The information is needed because a family member's release from custody depends on it. Under the RTI Act, 2005, within what time must the information normally be supplied, and to whom does a first appeal lie if it is not?", "opts": ["Within 30 days; first appeal to the State Information Commission", "Within 15 days; first appeal to the Deputy Commissioner in every case", "Within 48 hours; first appeal directly to the High Court", "Within 48 hours; first appeal to an officer senior in rank to the PIO in the same authority"], "correct": 3, "tag": "", "sol": "Section 7(1) sets 30 days as the normal limit. Where the information concerns a person's life or liberty, it must be supplied within 48 hours. Under Section 19(1), a first appeal goes to an officer senior in rank to the PIO in the same public authority. The Information Commission hears the second appeal. Option (a) uses the general timeline and skips the first appeal stage. Courts are not the first appellate forum under the Act."}, {"kind": "mcq", "text": "Under the Haryana Right to Service Act, 2014, a designated officer fails to deliver a notified service within its time limit. With the Auto Appeal System (AAS) on the SARAL platform, what happens next?", "opts": ["The application is escalated automatically to the First Grievance Redressal Authority, and can go on to the Second Authority and the Right to Service Commission", "The citizen must first file an RTI application to find out why the service was delayed", "The case goes straight to the Chief Minister's office for disciplinary action", "The application lapses and the citizen must apply again with fresh documents"], "correct": 0, "tag": "", "sol": "Under the Act, a citizen whose service is delayed or wrongly refused can appeal to the First and then the Second Grievance Redressal Authority. The Haryana Right to Service Commission sits above them. The Auto Appeal System, built by NIC for the Commission, files these appeals automatically when the time limit is missed. The citizen does not have to start the process. The Second Authority and the Commission can impose a penalty on the defaulting officer, and part of it can go to the citizen as compensation. RTI, CM-office referral and lapse are not part of this mechanism."}, {"kind": "mcq", "text": "Haryana has started old-age pensions for some eligible citizens without a separate application. Which feature of the Parivar Pehchan Patra (PPP) system mainly makes this proactive delivery possible?", "opts": ["Every family receiving a printed PPP card that must be shown at the pension office", "A verified family database checked against other government records, which lets the system find people who meet the age and income criteria", "A rule that old-age pension can be claimed only through CM Window", "Making it mandatory for all pensioners to open accounts in a single state-owned bank"], "correct": 1, "tag": "", "sol": "PPP keeps a continuously updated database of families. Self-declared data is verified electronically against other records, and physically where needed. Births, deaths and marriages are linked to it. Because date of birth and income can be checked within the system, eligible citizens can be identified automatically and their pensions started. A printed card or a single bank does nothing to identify eligibility. CM Window is a grievance channel, not a benefit-delivery platform."}, {"kind": "mcq", "text": "Which pairing correctly matches each citizen need to the Haryana platform designed for it?", "opts": ["Applying for a domicile certificate → CM Window; complaining that a drain has not been cleaned for weeks → SARAL", "Both needs → Haryana Kaushal Rozgar Nigam portal", "Applying for a domicile certificate → SARAL; complaining that a drain has not been cleaned for weeks → CM Window", "Both needs → Meri Fasal Mera Byora portal"], "correct": 2, "tag": "", "sol": "Antyodaya SARAL is the single platform for applying for government schemes and services, with Right to Service timelines and status tracking. CM Window, running since 25 December 2014, is the state's grievance redressal and monitoring system. Citizens register complaints and track them with a registration number. Option (a) reverses the roles. HKRN deploys contractual manpower and MFMB handles crop registration, so neither suits these needs."}]}, {"id": "s2", "label": "Part B", "sub": "Quantitative aptitude and data interpretation · 25 questions · 25 marks", "slides": [{"kind": "mcq", "text": "Study the table and answer the question. In which district is the share of women among all beneficiaries of both schemes taken together the highest?", "opts": ["Hisar", "Rohtak", "Sirsa", "Karnal"], "correct": 1, "tag": "", "sol": "Women ÷ all beneficiaries: Hisar 530/1200 = 44.2%, Rohtak 660/1200 = 55%, Karnal 460/1200 = 38.3%, Sirsa 490/900 = 54.4%. Rohtak is highest.\nTrap: Sirsa has the highest female share within SEL alone (170/300 = 56.7%), but the question asks about both schemes together.", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink)\">Beneficiaries of two state schemes, 2025–26 (ST = Skill Training, SEL = Self-Employment Loan)</div><div class=\"tscroll\"><table class=\"ttab\"><tr><th>District</th><th>ST – Male</th><th>ST – Female</th><th>SEL – Male</th><th>SEL – Female</th></tr><tr><td>Hisar</td><td>420</td><td>380</td><td>250</td><td>150</td></tr><tr><td>Rohtak</td><td>360</td><td>440</td><td>180</td><td>220</td></tr><tr><td>Karnal</td><td>500</td><td>300</td><td>240</td><td>160</td></tr><tr><td>Sirsa</td><td>280</td><td>320</td><td>130</td><td>170</td></tr></table></div>"}, {"kind": "mcq", "text": "Study the table and answer the question. By what percentage does the total number of Skill Training beneficiaries in Karnal exceed that in Sirsa?", "opts": ["25%", "20%", "40%", "33.3%"], "correct": 3, "tag": "", "sol": "ST total: Karnal 500 + 300 = 800, Sirsa 280 + 320 = 600. Excess = 200, and the base is Sirsa: 200/600 × 100 = 33.3%.\nTrap: 25% divides 200 by Karnal's 800 (wrong base).", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink)\">Beneficiaries of two state schemes, 2025–26 (ST = Skill Training, SEL = Self-Employment Loan)</div><div class=\"tscroll\"><table class=\"ttab\"><tr><th>District</th><th>ST – Male</th><th>ST – Female</th><th>SEL – Male</th><th>SEL – Female</th></tr><tr><td>Hisar</td><td>420</td><td>380</td><td>250</td><td>150</td></tr><tr><td>Rohtak</td><td>360</td><td>440</td><td>180</td><td>220</td></tr><tr><td>Karnal</td><td>500</td><td>300</td><td>240</td><td>160</td></tr><tr><td>Sirsa</td><td>280</td><td>320</td><td>130</td><td>170</td></tr></table></div>"}, {"kind": "mcq", "text": "Study the table and answer the question. Each ST beneficiary costs ₹12,000 and each SEL beneficiary is given a loan of ₹40,000. What is the total outlay for Hisar under both schemes?", "opts": ["₹2.56 crore", "₹25.6 crore", "₹2.56 lakh", "₹1.60 crore"], "correct": 0, "tag": "", "sol": "Hisar: ST = 420 + 380 = 800 → 800 × 12,000 = ₹96 lakh; SEL = 250 + 150 = 400 → 400 × 40,000 = ₹1.6 crore. Total = ₹2,56,00,000 = ₹2.56 crore.\nTrap: ₹1.60 crore counts only the SEL loans; ₹25.6 crore misplaces the crore (1 crore = 100 lakh).", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink)\">Beneficiaries of two state schemes, 2025–26 (ST = Skill Training, SEL = Self-Employment Loan)</div><div class=\"tscroll\"><table class=\"ttab\"><tr><th>District</th><th>ST – Male</th><th>ST – Female</th><th>SEL – Male</th><th>SEL – Female</th></tr><tr><td>Hisar</td><td>420</td><td>380</td><td>250</td><td>150</td></tr><tr><td>Rohtak</td><td>360</td><td>440</td><td>180</td><td>220</td></tr><tr><td>Karnal</td><td>500</td><td>300</td><td>240</td><td>160</td></tr><tr><td>Sirsa</td><td>280</td><td>320</td><td>130</td><td>170</td></tr></table></div>"}, {"kind": "mcq", "text": "Study the bar chart and answer the question. In which year was the resolution rate (resolved ÷ received) the highest?", "opts": ["2024", "2025", "2023", "2022"], "correct": 0, "tag": "", "sol": "Rates: 2021 75%, 2022 83.3%, 2023 85%, 2024 60/66 = 90.9%, 2025 63/72 = 87.5%. Highest is 2024.\nTrap: 2025 has the most grievances resolved (63 thousand), but also more received, so its rate is lower.", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink);text-align:center\">Grievances on a district portal (in thousands)</div><div class=\"fig\"><svg class=\"figsvg\" viewBox=\"0 0 340 250\" style=\"width:100%;max-width:340px;height:auto\" xmlns=\"http://www.w3.org/2000/svg\"><line x1=\"42\" y1=\"200.0\" x2=\"330\" y2=\"200.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"204.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">0</text><line x1=\"42\" y1=\"155.0\" x2=\"330\" y2=\"155.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"159.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">20</text><line x1=\"42\" y1=\"110.0\" x2=\"330\" y2=\"110.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"114.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">40</text><line x1=\"42\" y1=\"65.0\" x2=\"330\" y2=\"65.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"69.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">60</text><line x1=\"42\" y1=\"20.0\" x2=\"330\" y2=\"20.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"24.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">80</text><rect x=\"52.4\" y=\"110.0\" width=\"18.4\" height=\"90.0\" fill=\"var(--accent-text)\"/><text x=\"61.6\" y=\"107.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">40</text><rect x=\"70.8\" y=\"132.5\" width=\"18.4\" height=\"67.5\" fill=\"var(--gold)\"/><text x=\"80.0\" y=\"129.5\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">30</text><text x=\"70.8\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2021</text><rect x=\"110.0\" y=\"92.0\" width=\"18.4\" height=\"108.0\" fill=\"var(--accent-text)\"/><text x=\"119.2\" y=\"89.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">48</text><rect x=\"128.4\" y=\"110.0\" width=\"18.4\" height=\"90.0\" fill=\"var(--gold)\"/><text x=\"137.6\" y=\"107.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">40</text><text x=\"128.4\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2022</text><rect x=\"167.6\" y=\"65.0\" width=\"18.4\" height=\"135.0\" fill=\"var(--accent-text)\"/><text x=\"176.8\" y=\"62.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">60</text><rect x=\"186.0\" y=\"85.2\" width=\"18.4\" height=\"114.8\" fill=\"var(--gold)\"/><text x=\"195.2\" y=\"82.2\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">51</text><text x=\"186.0\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2023</text><rect x=\"225.2\" y=\"51.5\" width=\"18.4\" height=\"148.5\" fill=\"var(--accent-text)\"/><text x=\"234.4\" y=\"48.5\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">66</text><rect x=\"243.6\" y=\"65.0\" width=\"18.4\" height=\"135.0\" fill=\"var(--gold)\"/><text x=\"252.8\" y=\"62.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">60</text><text x=\"243.6\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2024</text><rect x=\"282.8\" y=\"38.0\" width=\"18.4\" height=\"162.0\" fill=\"var(--accent-text)\"/><text x=\"292.0\" y=\"35.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">72</text><rect x=\"301.2\" y=\"58.2\" width=\"18.4\" height=\"141.8\" fill=\"var(--gold)\"/><text x=\"310.4\" y=\"55.2\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">63</text><text x=\"301.2\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2025</text><line x1=\"42\" y1=\"200\" x2=\"330\" y2=\"200\" stroke=\"var(--ink)\" stroke-width=\"1\"/><line x1=\"42\" y1=\"200\" x2=\"42\" y2=\"14\" stroke=\"var(--ink)\" stroke-width=\"1\"/><text x=\"12\" y=\"110.0\" transform=\"rotate(-90 12 110.0)\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Thousands</text><rect x=\"70\" y=\"226\" width=\"11\" height=\"11\" fill=\"var(--accent-text)\"/><text x=\"85\" y=\"236\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Received</text><rect x=\"190\" y=\"226\" width=\"11\" height=\"11\" fill=\"var(--gold)\"/><text x=\"205\" y=\"236\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Resolved</text></svg></div>"}, {"kind": "mcq", "text": "Study the bar chart and answer the question. What is the percentage increase in grievances received from 2022 to 2024?", "opts": ["27.3%", "18%", "37.5%", "32.5%"], "correct": 2, "tag": "", "sol": "2022: 48 thousand; 2024: 66 thousand. Increase = 18; 18/48 × 100 = 37.5%.\nTrap: 27.3% uses 2024 (66) as the base; 18% is just the absolute increase in thousands.", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink);text-align:center\">Grievances on a district portal (in thousands)</div><div class=\"fig\"><svg class=\"figsvg\" viewBox=\"0 0 340 250\" style=\"width:100%;max-width:340px;height:auto\" xmlns=\"http://www.w3.org/2000/svg\"><line x1=\"42\" y1=\"200.0\" x2=\"330\" y2=\"200.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"204.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">0</text><line x1=\"42\" y1=\"155.0\" x2=\"330\" y2=\"155.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"159.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">20</text><line x1=\"42\" y1=\"110.0\" x2=\"330\" y2=\"110.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"114.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">40</text><line x1=\"42\" y1=\"65.0\" x2=\"330\" y2=\"65.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"69.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">60</text><line x1=\"42\" y1=\"20.0\" x2=\"330\" y2=\"20.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"24.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">80</text><rect x=\"52.4\" y=\"110.0\" width=\"18.4\" height=\"90.0\" fill=\"var(--accent-text)\"/><text x=\"61.6\" y=\"107.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">40</text><rect x=\"70.8\" y=\"132.5\" width=\"18.4\" height=\"67.5\" fill=\"var(--gold)\"/><text x=\"80.0\" y=\"129.5\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">30</text><text x=\"70.8\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2021</text><rect x=\"110.0\" y=\"92.0\" width=\"18.4\" height=\"108.0\" fill=\"var(--accent-text)\"/><text x=\"119.2\" y=\"89.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">48</text><rect x=\"128.4\" y=\"110.0\" width=\"18.4\" height=\"90.0\" fill=\"var(--gold)\"/><text x=\"137.6\" y=\"107.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">40</text><text x=\"128.4\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2022</text><rect x=\"167.6\" y=\"65.0\" width=\"18.4\" height=\"135.0\" fill=\"var(--accent-text)\"/><text x=\"176.8\" y=\"62.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">60</text><rect x=\"186.0\" y=\"85.2\" width=\"18.4\" height=\"114.8\" fill=\"var(--gold)\"/><text x=\"195.2\" y=\"82.2\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">51</text><text x=\"186.0\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2023</text><rect x=\"225.2\" y=\"51.5\" width=\"18.4\" height=\"148.5\" fill=\"var(--accent-text)\"/><text x=\"234.4\" y=\"48.5\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">66</text><rect x=\"243.6\" y=\"65.0\" width=\"18.4\" height=\"135.0\" fill=\"var(--gold)\"/><text x=\"252.8\" y=\"62.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">60</text><text x=\"243.6\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2024</text><rect x=\"282.8\" y=\"38.0\" width=\"18.4\" height=\"162.0\" fill=\"var(--accent-text)\"/><text x=\"292.0\" y=\"35.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">72</text><rect x=\"301.2\" y=\"58.2\" width=\"18.4\" height=\"141.8\" fill=\"var(--gold)\"/><text x=\"310.4\" y=\"55.2\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">63</text><text x=\"301.2\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2025</text><line x1=\"42\" y1=\"200\" x2=\"330\" y2=\"200\" stroke=\"var(--ink)\" stroke-width=\"1\"/><line x1=\"42\" y1=\"200\" x2=\"42\" y2=\"14\" stroke=\"var(--ink)\" stroke-width=\"1\"/><text x=\"12\" y=\"110.0\" transform=\"rotate(-90 12 110.0)\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Thousands</text><rect x=\"70\" y=\"226\" width=\"11\" height=\"11\" fill=\"var(--accent-text)\"/><text x=\"85\" y=\"236\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Received</text><rect x=\"190\" y=\"226\" width=\"11\" height=\"11\" fill=\"var(--gold)\"/><text x=\"205\" y=\"236\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Resolved</text></svg></div>"}, {"kind": "mcq", "text": "Study the bar chart and answer the question. In how many of the years 2022–2025 did the number of grievances resolved grow at a faster percentage rate than the number received (each compared with the previous year)?", "opts": ["3", "2", "4", "1"], "correct": 0, "tag": "", "sol": "Received growth: +20%, +25%, +10%, +9.1%. Resolved growth: +33.3%, +27.5%, +17.6%, +5%.\nResolved grew faster in 2022, 2023 and 2024, but not in 2025 (5% < 9.1%). Answer: 3. Trap: counting 2025 because resolved rose in absolute terms.", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink);text-align:center\">Grievances on a district portal (in thousands)</div><div class=\"fig\"><svg class=\"figsvg\" viewBox=\"0 0 340 250\" style=\"width:100%;max-width:340px;height:auto\" xmlns=\"http://www.w3.org/2000/svg\"><line x1=\"42\" y1=\"200.0\" x2=\"330\" y2=\"200.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"204.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">0</text><line x1=\"42\" y1=\"155.0\" x2=\"330\" y2=\"155.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"159.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">20</text><line x1=\"42\" y1=\"110.0\" x2=\"330\" y2=\"110.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"114.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">40</text><line x1=\"42\" y1=\"65.0\" x2=\"330\" y2=\"65.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"69.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">60</text><line x1=\"42\" y1=\"20.0\" x2=\"330\" y2=\"20.0\" stroke=\"var(--rule)\" stroke-width=\"0.6\"/><text x=\"37\" y=\"24.0\" text-anchor=\"end\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">80</text><rect x=\"52.4\" y=\"110.0\" width=\"18.4\" height=\"90.0\" fill=\"var(--accent-text)\"/><text x=\"61.6\" y=\"107.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">40</text><rect x=\"70.8\" y=\"132.5\" width=\"18.4\" height=\"67.5\" fill=\"var(--gold)\"/><text x=\"80.0\" y=\"129.5\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">30</text><text x=\"70.8\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2021</text><rect x=\"110.0\" y=\"92.0\" width=\"18.4\" height=\"108.0\" fill=\"var(--accent-text)\"/><text x=\"119.2\" y=\"89.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">48</text><rect x=\"128.4\" y=\"110.0\" width=\"18.4\" height=\"90.0\" fill=\"var(--gold)\"/><text x=\"137.6\" y=\"107.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">40</text><text x=\"128.4\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2022</text><rect x=\"167.6\" y=\"65.0\" width=\"18.4\" height=\"135.0\" fill=\"var(--accent-text)\"/><text x=\"176.8\" y=\"62.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">60</text><rect x=\"186.0\" y=\"85.2\" width=\"18.4\" height=\"114.8\" fill=\"var(--gold)\"/><text x=\"195.2\" y=\"82.2\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">51</text><text x=\"186.0\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2023</text><rect x=\"225.2\" y=\"51.5\" width=\"18.4\" height=\"148.5\" fill=\"var(--accent-text)\"/><text x=\"234.4\" y=\"48.5\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">66</text><rect x=\"243.6\" y=\"65.0\" width=\"18.4\" height=\"135.0\" fill=\"var(--gold)\"/><text x=\"252.8\" y=\"62.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">60</text><text x=\"243.6\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2024</text><rect x=\"282.8\" y=\"38.0\" width=\"18.4\" height=\"162.0\" fill=\"var(--accent-text)\"/><text x=\"292.0\" y=\"35.0\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">72</text><rect x=\"301.2\" y=\"58.2\" width=\"18.4\" height=\"141.8\" fill=\"var(--gold)\"/><text x=\"310.4\" y=\"55.2\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">63</text><text x=\"301.2\" y=\"215\" text-anchor=\"middle\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">2025</text><line x1=\"42\" y1=\"200\" x2=\"330\" y2=\"200\" stroke=\"var(--ink)\" stroke-width=\"1\"/><line x1=\"42\" y1=\"200\" x2=\"42\" y2=\"14\" stroke=\"var(--ink)\" stroke-width=\"1\"/><text x=\"12\" y=\"110.0\" transform=\"rotate(-90 12 110.0)\" text-anchor=\"middle\" style=\"font:600 10px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Thousands</text><rect x=\"70\" y=\"226\" width=\"11\" height=\"11\" fill=\"var(--accent-text)\"/><text x=\"85\" y=\"236\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Received</text><rect x=\"190\" y=\"226\" width=\"11\" height=\"11\" fill=\"var(--gold)\"/><text x=\"205\" y=\"236\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Resolved</text></svg></div>"}, {"kind": "mcq", "text": "Study the pie chart and answer the question. By how much does spending on Medicines exceed spending on Outreach?", "opts": ["₹13 crore", "₹5.76 crore", "₹6.42 crore", "₹6.24 crore"], "correct": 3, "tag": "", "sol": "Medicines − Outreach = 25% − 12% = 13% of ₹48 crore = 0.13 × 48 = ₹6.24 crore.\nTrap: ₹13 crore reads the 13 percentage points as crore; ₹5.76 crore is 12% of 48 (Outreach alone).", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink);text-align:center\">District health budget 2025–26: ₹48 crore</div><div class=\"fig\"><svg class=\"figsvg\" viewBox=\"0 0 340 200\" style=\"width:100%;max-width:340px;height:auto\" xmlns=\"http://www.w3.org/2000/svg\"><path d=\"M95,100 L95.00,20.00 A80,80 0 0 1 142.02,164.72 Z\" fill=\"var(--accent-text)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><path d=\"M95,100 L142.02,164.72 A80,80 0 0 1 30.28,147.02 Z\" fill=\"var(--gold)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><path d=\"M95,100 L30.28,147.02 A80,80 0 0 1 18.92,75.28 Z\" fill=\"var(--success)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><path d=\"M95,100 L18.92,75.28 A80,80 0 0 1 56.46,29.90 Z\" fill=\"var(--danger)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><path d=\"M95,100 L56.46,29.90 A80,80 0 0 1 95.00,20.00 Z\" fill=\"var(--rule)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><rect x=\"200\" y=\"28\" width=\"12\" height=\"12\" fill=\"var(--accent-text)\"/><text x=\"218\" y=\"38\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Salaries — 40%</text><rect x=\"200\" y=\"56\" width=\"12\" height=\"12\" fill=\"var(--gold)\"/><text x=\"218\" y=\"66\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Medicines — 25%</text><rect x=\"200\" y=\"84\" width=\"12\" height=\"12\" fill=\"var(--success)\"/><text x=\"218\" y=\"94\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Infrastructure — 15%</text><rect x=\"200\" y=\"112\" width=\"12\" height=\"12\" fill=\"var(--danger)\"/><text x=\"218\" y=\"122\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Outreach — 12%</text><rect x=\"200\" y=\"140\" width=\"12\" height=\"12\" fill=\"var(--rule)\"/><text x=\"218\" y=\"150\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Administration — 8%</text></svg></div>"}, {"kind": "mcq", "text": "Study the pie chart and answer the question. Next year the total budget rises to ₹60 crore but the rupee amount for Salaries stays the same. What will be the share of Salaries in the new budget?", "opts": ["32%", "40%", "50%", "30%"], "correct": 0, "tag": "", "sol": "Salaries now = 40% of 48 = ₹19.2 crore. In the new budget: 19.2/60 × 100 = 32%.\nTrap: 40% assumes the share stays fixed, which would need the rupee amount to rise to ₹24 crore.", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink);text-align:center\">District health budget 2025–26: ₹48 crore</div><div class=\"fig\"><svg class=\"figsvg\" viewBox=\"0 0 340 200\" style=\"width:100%;max-width:340px;height:auto\" xmlns=\"http://www.w3.org/2000/svg\"><path d=\"M95,100 L95.00,20.00 A80,80 0 0 1 142.02,164.72 Z\" fill=\"var(--accent-text)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><path d=\"M95,100 L142.02,164.72 A80,80 0 0 1 30.28,147.02 Z\" fill=\"var(--gold)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><path d=\"M95,100 L30.28,147.02 A80,80 0 0 1 18.92,75.28 Z\" fill=\"var(--success)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><path d=\"M95,100 L18.92,75.28 A80,80 0 0 1 56.46,29.90 Z\" fill=\"var(--danger)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><path d=\"M95,100 L56.46,29.90 A80,80 0 0 1 95.00,20.00 Z\" fill=\"var(--rule)\" stroke=\"var(--card)\" stroke-width=\"1.5\"/><rect x=\"200\" y=\"28\" width=\"12\" height=\"12\" fill=\"var(--accent-text)\"/><text x=\"218\" y=\"38\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Salaries — 40%</text><rect x=\"200\" y=\"56\" width=\"12\" height=\"12\" fill=\"var(--gold)\"/><text x=\"218\" y=\"66\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Medicines — 25%</text><rect x=\"200\" y=\"84\" width=\"12\" height=\"12\" fill=\"var(--success)\"/><text x=\"218\" y=\"94\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Infrastructure — 15%</text><rect x=\"200\" y=\"112\" width=\"12\" height=\"12\" fill=\"var(--danger)\"/><text x=\"218\" y=\"122\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Outreach — 12%</text><rect x=\"200\" y=\"140\" width=\"12\" height=\"12\" fill=\"var(--rule)\"/><text x=\"218\" y=\"150\" style=\"font:600 11px 'Source Sans 3',sans-serif\" fill=\"var(--ink)\">Administration — 8%</text></svg></div>"}, {"kind": "mcq", "text": "<b>Data sufficiency.</b> The question is followed by two statements. Decide whether the data in the statements are sufficient to answer it.<br>How many officers are posted in a block office (which has only officers and clerks)?<br><b>I.</b> The ratio of officers to clerks is 2 : 5.<br><b>II.</b> There are 18 more clerks than officers.", "opts": ["Statement I alone is sufficient, but Statement II alone is not", "Statement II alone is sufficient, but Statement I alone is not", "Both statements together are sufficient, but neither alone is", "Both statements together are not sufficient"], "correct": 2, "tag": "", "sol": "I gives only the ratio 2 : 5 (could be 2 and 5, or 4 and 10…). II gives only the difference. Together: officers = 2k, clerks = 5k, 3k = 18 → k = 6, officers = 12. So both are needed.\nTrap: thinking a ratio alone fixes a count."}, {"kind": "mcq", "text": "<b>Data sufficiency.</b> The question is followed by two statements. Decide whether the data in the statements are sufficient to answer it.<br>What was the population of village Bhatla in 2025?<br><b>I.</b> Its population grew by 10% from 2024 to 2025.<br><b>II.</b> Its population in 2024 was 4,000 more than in 2020.", "opts": ["Statement I alone is sufficient, but Statement II alone is not", "Statement II alone is sufficient, but Statement I alone is not", "Both statements together are sufficient, but neither alone is", "Both statements together are not sufficient"], "correct": 3, "tag": "", "sol": "I links 2025 to 2024 only by a percentage; II links 2024 to 2020 only by a difference. No year's actual population is known, so even together the 2025 figure cannot be found.\nTrap: choosing 'both together' because the statements appear to chain years together."}, {"kind": "mcq", "text": "A data-entry check is run on the register extract shown. Which records should be flagged for correction or field verification?", "opts": ["4 only", "4, 5 and 6 only", "5 and 6 only", "1, 4 and 6 only"], "correct": 1, "tag": "", "sol": "Record 4 repeats record 1 exactly (same Family ID and details) — a duplicate. Record 5 shows a 9-year-old as head of family earning an income — implausible. Record 6 shows 0 members though the family has a head — inconsistent.\nTrap: flagging record 1 as well; only one copy of a duplicate pair is removed.", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink)\">Extract from a family survey register</div><div class=\"tscroll\"><table class=\"ttab\"><tr><th>Rec</th><th>Family ID</th><th>Head of family</th><th>Age</th><th>Members</th><th>Income (₹/month)</th></tr><tr><td>1</td><td>HR-1021</td><td>Suresh Kumar</td><td>46</td><td>5</td><td>12,000</td></tr><tr><td>2</td><td>HR-1034</td><td>Kamla Devi</td><td>52</td><td>3</td><td>9,500</td></tr><tr><td>3</td><td>HR-1047</td><td>Ramesh</td><td>38</td><td>4</td><td>15,000</td></tr><tr><td>4</td><td>HR-1021</td><td>Suresh Kumar</td><td>46</td><td>5</td><td>12,000</td></tr><tr><td>5</td><td>HR-1058</td><td>Pooja</td><td>9</td><td>4</td><td>11,000</td></tr><tr><td>6</td><td>HR-1062</td><td>Anil Sharma</td><td>61</td><td>0</td><td>8,000</td></tr></table></div>"}, {"kind": "mcq", "text": "A district office reports the figures shown. What can be concluded about the reported total?", "opts": ["It is correct", "It is understated by 100", "It is overstated by 100", "It is overstated by 10"], "correct": 2, "tag": "", "sol": "1,245 + 987 + 1,532 + 864 = 4,628. The reported 4,728 is 100 more than the true sum, so it is overstated by 100.\nTrap: adding quickly in thousands and missing the hundreds carry.", "fig": "<div style=\"font-weight:600;margin:4px 0;color:var(--ink)\">Monthly report sent by a district office</div><div class=\"tscroll\"><table class=\"ttab\"><tr><th>Block</th><th>New ration cards issued</th></tr><tr><td>A</td><td>1,245</td></tr><tr><td>B</td><td>987</td></tr><tr><td>C</td><td>1,532</td></tr><tr><td>D</td><td>864</td></tr><tr><td><b>Total (as reported)</b></td><td><b>4,728</b></td></tr></table></div>"}, {"kind": "mcq", "text": "Enrolment under a pension scheme rose by 20% in one year and then fell by 15% the next year. What is the net change over the two years?", "opts": ["5% increase", "2% increase", "3% decrease", "No change"], "correct": 1, "tag": "", "sol": "Take 100 → after +20%: 120 → after −15%: 120 × 0.85 = 102. Net = +2%.\nTrap: 20 − 15 = 5% ignores that the 15% fall is on the larger base of 120."}, {"kind": "mcq", "text": "In a recruitment test, 62% of applicants appeared, and 45% of those who appeared qualified. If 2,790 candidates qualified, how many had applied?", "opts": ["6,200", "8,700", "12,400", "10,000"], "correct": 3, "tag": "", "sol": "Qualified = 0.62 × 0.45 × applicants = 0.279 × applicants. Applicants = 2,790 ÷ 0.279 = 10,000.\nTrap: 6,200 = 2,790 ÷ 0.45 gives only the number who appeared."}, {"kind": "mcq", "text": "Wheat procurement at a mandi this season is 25% more than last season. Last season's procurement is what percentage less than this season's?", "opts": ["25%", "20%", "22.5%", "75%"], "correct": 1, "tag": "", "sol": "Let last season = 100, this season = 125. Difference 25 on a base of 125: 25/125 × 100 = 20%.\nTrap: 25% keeps the old base; the comparison is now with this season's figure."}, {"kind": "mcq", "text": "A grant of ₹7.2 crore is received. 10% is kept as a contingency reserve and the rest is divided among three blocks in the ratio of their populations, 4 : 5 : 3. How much does the largest block get?", "opts": ["₹3.0 crore", "₹2.4 crore", "₹2.7 crore", "₹2.16 crore"], "correct": 2, "tag": "", "sol": "Distributable = 90% of 7.2 = ₹6.48 crore. Largest share = 5/12 × 6.48 = ₹2.7 crore.\nTrap: ₹3.0 crore = 5/12 × 7.2 forgets to keep the 10% reserve aside first."}, {"kind": "mcq", "text": "In a government school the ratio of boys to girls is 7 : 5. After 40 more girls are admitted, the ratio becomes 7 : 6. How many boys are there?", "opts": ["280", "240", "320", "200"], "correct": 0, "tag": "", "sol": "Boys = 7k, girls = 5k. 7k / (5k + 40) = 7/6 → 42k = 35k + 280 → k = 40. Boys = 280.\nTrap: 240 treats the 40 new girls as 'one part', which would need the boys to change too."}, {"kind": "mcq", "text": "Three training batches took the same assessment: 40 trainees averaged 72, 35 trainees averaged 80, and 25 trainees averaged 64. What is the average score of all trainees?", "opts": ["72.0", "73.6", "71.4", "72.8"], "correct": 3, "tag": "", "sol": "Total marks = 40×72 + 35×80 + 25×64 = 2,880 + 2,800 + 1,600 = 7,280 for 100 trainees → 72.8.\nTrap: 72.0 is the simple mean of 72, 80, 64, which ignores the different batch sizes."}, {"kind": "mcq", "text": "The average age of 10 field staff in a tehsil is 34 years. A 52-year-old member retires and is replaced by a 27-year-old. What is the new average age?", "opts": ["33.5 years", "31.5 years", "32.5 years", "29.0 years"], "correct": 1, "tag": "", "sol": "The total falls by 52 − 27 = 25 years, so the average falls by 25/10 = 2.5 → 34 − 2.5 = 31.5 years.\nTrap: 29.0 spreads the 25-year drop over 5 people instead of 10 (34 − 5)."}, {"kind": "mcq", "text": "12 enumerators can complete the household survey of a block in 15 days. After 5 days, 3 more enumerators join. In how many days in all is the survey completed?", "opts": ["12 days", "11 days", "13 days", "14 days"], "correct": 2, "tag": "", "sol": "Work = 12 × 15 = 180 enumerator-days. First 5 days: 60 done, 120 left. Now 15 enumerators: 120/15 = 8 days. Total = 5 + 8 = 13 days.\nTrap: 12 days divides all 180 by 15, ignoring the first 5 days at the slower pace."}, {"kind": "mcq", "text": "Inlet pipe A can fill a village overhead tank in 6 hours and inlet B in 9 hours. The supply outlet, if open alone, empties the full tank in 12 hours. With all three open on an empty tank, how long does it take to fill?", "opts": ["3<sup>3</sup>⁄<sub>5</sub> hours", "7<sup>1</sup>⁄<sub>5</sub> hours", "4<sup>4</sup>⁄<sub>7</sub> hours", "5<sup>1</sup>⁄<sub>7</sub> hours"], "correct": 3, "tag": "", "sol": "Net rate = 1/6 + 1/9 − 1/12 = (6 + 4 − 3)/36 = 7/36 tank per hour → time = 36/7 = 5<sup>1</sup>⁄<sub>7</sub> hours.\nTrap: 3<sup>3</sup>⁄<sub>5</sub> h (= 18/5) adds the outlet instead of subtracting it."}, {"kind": "mcq", "text": "2,400 pension files must be verified in 10 working days. A verification officer clears 15 files a day and an assistant clears 10 files a day. If 8 officers are available, what is the minimum number of assistants needed?", "opts": ["12", "16", "8", "24"], "correct": 0, "tag": "", "sol": "Officers clear 8 × 15 × 10 = 1,200 files. Remaining 1,200 files ÷ (10 files × 10 days) = 12 assistants.\nTrap: 24 forgets the officers' share; 16 is 2,400 ÷ 15 ÷ 10 (the officers needed if working alone)."}, {"kind": "mcq", "text": "₹45 lakh + ₹3.2 crore + ₹750 thousand = ?", "opts": ["₹37.25 lakh", "₹4.40 crore", "₹3.725 crore", "₹37.25 crore"], "correct": 2, "tag": "", "sol": "In lakh: 45 + 320 + 7.5 = 372.5 lakh = ₹3.725 crore (1 crore = 100 lakh; 750 thousand = 7.5 lakh).\nTrap: ₹37.25 lakh is ten times too small; ₹4.40 crore treats 750 thousand as 75 lakh (45 + 320 + 75 = 440 lakh)."}, {"kind": "mcq", "text": "Without exact calculation, which value is closest to 39.8% of 1,201 + 19.9 × 50.2?", "opts": ["1,380", "1,480", "1,580", "1,280"], "correct": 1, "tag": "", "sol": "39.8% of 1,201 ≈ 40% of 1,200 = 480; 19.9 × 50.2 ≈ 20 × 50 = 1,000. Sum ≈ 1,480 (exact ≈ 1,477).\nTrap: rounding 39.8% down to 30% or 50.2 down to 45 shifts the answer by ~100."}, {"kind": "mcq", "text": "A state programme spends ₹1.2 lakh crore over five years on a target population of 3 crore people. What is the spending per person over the five years?", "opts": ["₹40,000", "₹4,000", "₹4,00,000", "₹400"], "correct": 0, "tag": "", "sol": "₹1.2 lakh crore = 1.2 × 10<sup>5</sup> × 10<sup>7</sup> = ₹1.2 × 10<sup>12</sup>. Divide by 3 × 10<sup>7</sup> people: 0.4 × 10<sup>5</sup> = ₹40,000.\nTrap: ₹4,000 drops one power of ten when converting lakh crore."}]}, {"id": "s3", "label": "Part C", "sub": "Logical, analytical and critical reasoning · 25 questions · 25 marks", "slides": [{"kind": "mcq", "text": "A district began sending SMS reminders for the second dose of a child vaccine in January 2025. Second-dose completion rose from 71% in 2024 to 84% in 2025. The district health officer concludes that the SMS reminders caused the improvement.<br>Which of the following, if true, most <b>strengthens</b> the officer's conclusion?", "opts": ["Many parents told ASHA workers that they found the SMS reminders useful.", "Most families in the district own at least one mobile phone that can receive SMS.", "In comparable blocks of the same district that did not get SMS reminders, completion stayed near 71% in 2025.", "The SMS reminders cost the district less than ₹1 per beneficiary for the whole year."], "correct": 2, "tag": "", "sol": "A causal claim is strengthened most by a comparison group: similar blocks without SMS showed no rise, so the improvement is less likely due to some district-wide factor. Phone ownership only shows the SMS could be received, and parents liking the messages does not show behaviour changed; cost is irrelevant."}, {"kind": "mcq", "text": "After the state raised the stamp-duty rebate for property registered in a woman's name, the share of registrations in women's names rose sharply. A policy note argues that a further increase in the rebate will therefore increase women's real control over property.<br>Which of the following, if true, most <b>weakens</b> the argument?", "opts": ["Many of the new registrations were in women's names only on paper, with male relatives keeping the documents and taking all decisions about the property.", "Property prices in the state rose during the same period, so the rebate saved buyers more money.", "Several other states also offer a stamp-duty rebate for registrations in women's names.", "The share of registrations in women's names rose more in urban areas than in rural areas."], "correct": 0, "tag": "", "sol": "The argument jumps from 'more registrations in women's names' to 'more real control'. If the registrations are nominal and control stays with men, a bigger rebate may only increase paper ownership. Higher prices or other states' policies do not touch this gap; an urban–rural difference does not weaken it either."}, {"kind": "mcq", "text": "<i>\"The municipal corporation should make online payment the only way to pay property tax. This will cut collection costs and raise the number of owners who pay on time.\"</i><br>The argument above <b>assumes</b> which of the following?", "opts": ["Property-tax rates in the city are lower than in neighbouring cities.", "Online payment systems never face technical failures.", "The corporation's cash counters are currently the main source of errors in tax records.", "Most property owners are able to access and use an online payment facility."], "correct": 3, "tag": "", "sol": "For on-time payment to rise when online is the ONLY channel, owners must be able to pay online; if many cannot, compliance would fall. The argument does not need online systems to be flawless (that is too strong), nor anything about tax rates or the source of record errors."}, {"kind": "mcq", "text": "Read the statements:<br>• Every gram panchayat in the district that has achieved ODF-Plus status has a functioning waste-segregation shed.<br>• Some panchayats with a functioning shed have not yet achieved ODF-Plus status.<br>• No panchayat in Block K has a functioning waste-segregation shed.<br>Which of the following <b>must be true</b>?", "opts": ["Most panchayats with a functioning shed have achieved ODF-Plus status.", "No panchayat in Block K has achieved ODF-Plus status.", "Building a shed in a Block K panchayat will make it ODF-Plus.", "Panchayats outside Block K all have functioning sheds."], "correct": 1, "tag": "", "sol": "Having a shed is a necessary condition for ODF-Plus (every ODF-Plus panchayat has one). Block K has no sheds, so none of its panchayats can be ODF-Plus. A shed is not sufficient (statement 2), so building one does not guarantee status; nothing is said about 'most' or about other blocks."}, {"kind": "mcq", "text": "<i>\"Average waiting time at the tehsil office fell from 95 to 40 minutes after a token system started in March. In the same months, most certificate services moved to the online portal, and daily footfall at the office dropped by more than half. A large part of the fall in waiting time is therefore explained by fewer visitors. So the token system's own effect should be measured separately before it is extended to all tehsils.\"</i><br>Which of the following best expresses the <b>main conclusion</b>?", "opts": ["The token system cut waiting time from 95 to 40 minutes.", "Online services have reduced footfall at the tehsil office by more than half.", "The token system's own effect should be measured before it is extended to all tehsils.", "Fewer visitors explain a large part of the fall in waiting time."], "correct": 2, "tag": "", "sol": "The passage gives facts (waiting time fell; footfall halved) and an intermediate claim (fewer visitors explain much of the fall) to support its final recommendation: measure the token system separately before extending it. Option (d) is a supporting step, not the conclusion; (a) is what the passage questions."}, {"kind": "mcq", "text": "Which of the following could be the order of meetings from Monday to Saturday?", "opts": ["Water, Health, Education, Police, Agriculture, Revenue", "Revenue, Health, Water, Education, Agriculture, Police", "Police, Health, Education, Agriculture, Water, Revenue", "Police, Water, Health, Education, Agriculture, Revenue"], "correct": 3, "tag": "", "sol": "Option (d) meets all six conditions: Revenue on Saturday, Health–Education on Tue–Wed, Police (Mon) not next to Revenue, Water (Tue) before Agriculture (Fri). (a) puts Water on Monday; (b) separates Health and Education; (c) puts Agriculture before Water.", "fig": "<div style=\"border:1px solid var(--rule);border-left:4px solid var(--accent-text);background:var(--card);color:var(--ink);padding:10px 12px;border-radius:6px;font-size:0.95em;line-height:1.5;max-width:100%;box-sizing:border-box\"><b>Caselet — District review meetings</b><br>The Deputy Commissioner will hold six department review meetings — <b>Health (H), Education (E), Agriculture (A), Police (P), Revenue (R)</b> and <b>Water Supply (W)</b> — one per day from Monday to Saturday of the same week, subject to these conditions:<br>1. Revenue is held on Monday or on Saturday.<br>2. Health is held on the day immediately before Education.<br>3. Police is not held on a day immediately before or after Revenue.<br>4. Water Supply is held on some day before Agriculture.<br>5. Water Supply is not held on Monday.<br>6. Agriculture is not held on Saturday.</div>"}, {"kind": "mcq", "text": "If Revenue is held on Monday and Police on Saturday, how many different orders of the six meetings are possible?", "opts": ["2", "3", "4", "5"], "correct": 1, "tag": "", "sol": "Tue–Fri hold H, E, W, A with H immediately before E and W before A. Possible: H E W A, W H E A, W A H E — 3 orders. Orders such as H E A W or A W H E put Agriculture before Water and break condition 4 — counting them is the common slip.", "fig": "<div style=\"border:1px solid var(--rule);border-left:4px solid var(--accent-text);background:var(--card);color:var(--ink);padding:10px 12px;border-radius:6px;font-size:0.95em;line-height:1.5;max-width:100%;box-sizing:border-box\"><b>Caselet — District review meetings</b><br>The Deputy Commissioner will hold six department review meetings — <b>Health (H), Education (E), Agriculture (A), Police (P), Revenue (R)</b> and <b>Water Supply (W)</b> — one per day from Monday to Saturday of the same week, subject to these conditions:<br>1. Revenue is held on Monday or on Saturday.<br>2. Health is held on the day immediately before Education.<br>3. Police is not held on a day immediately before or after Revenue.<br>4. Water Supply is held on some day before Agriculture.<br>5. Water Supply is not held on Monday.<br>6. Agriculture is not held on Saturday.</div>"}, {"kind": "mcq", "text": "If the Health meeting is held on Thursday, on which day is the Water Supply meeting held?", "opts": ["Monday", "Tuesday", "Wednesday", "Saturday"], "correct": 1, "tag": "", "sol": "Health on Thursday puts Education on Friday, leaving Mon, Tue, Wed, Sat. Agriculture cannot be on Saturday and must follow Water, and Water cannot be on Monday, so Water = Tuesday and Agriculture = Wednesday. Revenue and Police then take Monday and Saturday (never adjacent), so Water is fixed on Tuesday.", "fig": "<div style=\"border:1px solid var(--rule);border-left:4px solid var(--accent-text);background:var(--card);color:var(--ink);padding:10px 12px;border-radius:6px;font-size:0.95em;line-height:1.5;max-width:100%;box-sizing:border-box\"><b>Caselet — District review meetings</b><br>The Deputy Commissioner will hold six department review meetings — <b>Health (H), Education (E), Agriculture (A), Police (P), Revenue (R)</b> and <b>Water Supply (W)</b> — one per day from Monday to Saturday of the same week, subject to these conditions:<br>1. Revenue is held on Monday or on Saturday.<br>2. Health is held on the day immediately before Education.<br>3. Police is not held on a day immediately before or after Revenue.<br>4. Water Supply is held on some day before Agriculture.<br>5. Water Supply is not held on Monday.<br>6. Agriculture is not held on Saturday.</div>"}, {"kind": "mcq", "text": "Which of the following <b>cannot</b> be true?", "opts": ["Water Supply is held on Thursday.", "Agriculture is held on Wednesday.", "Education is held on Saturday.", "Police is held on Tuesday."], "correct": 3, "tag": "", "sol": "Police on Tuesday forces Revenue onto Saturday (Monday would be adjacent). Then Mon, Wed, Thu, Fri hold H, E, W, A. Monday cannot be W (cond. 5), A (must follow W) or E (must follow H), so it must be H — but then E must be on Tuesday, which Police occupies. The other three each occur in some valid schedule.", "fig": "<div style=\"border:1px solid var(--rule);border-left:4px solid var(--accent-text);background:var(--card);color:var(--ink);padding:10px 12px;border-radius:6px;font-size:0.95em;line-height:1.5;max-width:100%;box-sizing:border-box\"><b>Caselet — District review meetings</b><br>The Deputy Commissioner will hold six department review meetings — <b>Health (H), Education (E), Agriculture (A), Police (P), Revenue (R)</b> and <b>Water Supply (W)</b> — one per day from Monday to Saturday of the same week, subject to these conditions:<br>1. Revenue is held on Monday or on Saturday.<br>2. Health is held on the day immediately before Education.<br>3. Police is not held on a day immediately before or after Revenue.<br>4. Water Supply is held on some day before Agriculture.<br>5. Water Supply is not held on Monday.<br>6. Agriculture is not held on Saturday.</div>"}, {"kind": "mcq", "text": "<b>Statements:</b> All ward councillors are members of the ward committee. Some members of the ward committee are RWA presidents. No RWA president is a government employee.<br><b>Conclusions:</b> I. Some ward councillors are RWA presidents. II. Some members of the ward committee are not government employees.", "opts": ["Only conclusion I follows", "Only conclusion II follows", "Both I and II follow", "Neither I nor II follows"], "correct": 1, "tag": "", "sol": "The committee members who are RWA presidents cannot be government employees, so II follows. Councillors are only some of the committee members; the RWA presidents in the committee may all be non-councillors, so I does not necessarily follow."}, {"kind": "mcq", "text": "A department's file rules: If a file is approved by the Deputy Commissioner, it goes to the Finance branch. A file that reaches the Finance branch is cleared within 7 days unless an objection is raised on it. File F was <b>not</b> cleared within 7 days.<br>Which of the following <b>must be true</b>?", "opts": ["File F was not approved by the Deputy Commissioner.", "An objection was raised on File F.", "File F never reached the Finance branch.", "If File F was approved by the Deputy Commissioner, an objection was raised on it."], "correct": 3, "tag": "", "sol": "Approval → reaches Finance → (cleared in 7 days OR objection). F was not cleared, so IF it was approved, an objection must have been raised. We cannot tell which of the two actually happened: F may simply not have been approved, or it may have been approved and objected to — so (a), (b), (c) are each possible, not certain."}, {"kind": "mcq", "text": "A state rule says: <i>\"A village can be certified 'fully covered' only if every household in it has a working tap connection.\"</i> In Village Q, every household has a working tap connection.<br>Which of the following follows?", "opts": ["Village Q may or may not be certified 'fully covered'; the rule alone does not decide it.", "Village Q must be certified 'fully covered'.", "Village Q cannot be certified 'fully covered'.", "Every certified village has more tap connections than Village Q."], "correct": 0, "tag": "", "sol": "'Only if' states a necessary condition, not a sufficient one. Q meets the necessary condition, so it is not ruled out, but other requirements (e.g. water quality testing) may exist. Treating 'only if' as 'if' gives the trap answer (b)."}, {"kind": "mcq", "text": "Based on the table, which statement is <b>supported</b>?", "opts": ["Blocks that take longer to approve always approve a smaller share of applications.", "A block with more applications always has a lower approval rate.", "Block D has the highest approval rate among the four blocks.", "The block with the highest approval rate is not the block with the fastest approval."], "correct": 3, "tag": "", "sol": "Approval rates: A 75%, B 90%, C 70%, D 85%. The highest rate (B, 90%) is not the fastest block (C, 12 days), so (d) holds. (a) fails: B and D are slowest yet approve the largest shares. (b) fails: D has fewer applications than B but a lower rate. (c) fails: B (90%) beats D (85%).", "fig": "<div style=\"border:1px solid var(--rule);border-left:4px solid var(--accent-text);background:var(--card);color:var(--ink);padding:10px 12px;border-radius:6px;font-size:0.95em;line-height:1.5;max-width:100%;box-sizing:border-box\"><b>Scholarship applications in four blocks of a district, 2025–26</b></div><div class=\"tscroll\"><table class=\"ttab\"><thead><tr><th>Block</th><th>Applications</th><th>Approved</th><th>Avg. days to approve</th></tr></thead><tbody><tr><td>A</td><td>1,200</td><td>900</td><td>18</td></tr><tr><td>B</td><td>800</td><td>720</td><td>25</td></tr><tr><td>C</td><td>1,500</td><td>1,050</td><td>12</td></tr><tr><td>D</td><td>600</td><td>510</td><td>30</td></tr></tbody></table></div>"}, {"kind": "mcq", "text": "The district report claims: \"Across the four blocks, more than four-fifths of all scholarship applications were approved.\" Based on the table, the claim is:", "opts": ["true, because three of the four blocks approved 75% or more", "false, because the overall approval rate is about 78%", "true, because Blocks B and D both approved more than 80%", "impossible to check without data on rejected applications"], "correct": 1, "tag": "", "sol": "Total approved = 900 + 720 + 1,050 + 510 = 3,180 out of 1,200 + 800 + 1,500 + 600 = 4,100, i.e. about 77.6%, below 80%. Judging by how many blocks cross a threshold (a, c) ignores that the large Block C (70%) pulls the overall rate down. Rejections = applications − approved, so nothing is missing.", "fig": "<div style=\"border:1px solid var(--rule);border-left:4px solid var(--accent-text);background:var(--card);color:var(--ink);padding:10px 12px;border-radius:6px;font-size:0.95em;line-height:1.5;max-width:100%;box-sizing:border-box\"><b>Scholarship applications in four blocks of a district, 2025–26</b></div><div class=\"tscroll\"><table class=\"ttab\"><thead><tr><th>Block</th><th>Applications</th><th>Approved</th><th>Avg. days to approve</th></tr></thead><tbody><tr><td>A</td><td>1,200</td><td>900</td><td>18</td></tr><tr><td>B</td><td>800</td><td>720</td><td>25</td></tr><tr><td>C</td><td>1,500</td><td>1,050</td><td>12</td></tr><tr><td>D</td><td>600</td><td>510</td><td>30</td></tr></tbody></table></div>"}, {"kind": "mcq", "text": "<b>Facts:</b> In 2025, total FIRs registered in District K rose by 20% over 2024. During 2025 the state began allowing vehicle-theft FIRs to be filed online. Vehicle-theft FIRs rose by 60%, while all other FIRs rose by 5%.<br>Which conclusion is <b>best supported</b> by these facts?", "opts": ["Crime in District K increased by 20% in 2025.", "The online FIR facility caused vehicle thefts to increase.", "Part of the rise in registered FIRs may reflect easier registration rather than more crime.", "Police in District K were less effective in 2025 than in 2024."], "correct": 2, "tag": "", "sol": "Registered FIRs measure reporting, not actual crime. The rise is concentrated in the category where filing became easier, so more reporting is a likely part of the explanation. (a) equates FIRs with crime; (b) confuses more reporting of thefts with more thefts; (d) is not supported by any fact given."}, {"kind": "mcq", "text": "Arrange the steps of a public works procurement in the correct order:<br>P. Technical bids are evaluated<br>Q. Administrative approval and expenditure sanction are obtained<br>R. Work order is issued to the selected bidder<br>S. Need is assessed and a cost estimate prepared<br>T. Financial bids of technically qualified bidders are opened<br>U. Tender notice is published", "opts": ["S, Q, U, P, T, R", "Q, S, U, T, P, R", "S, U, Q, P, T, R", "S, Q, U, T, P, R"], "correct": 0, "tag": "", "sol": "A need and estimate come first; sanction is obtained on that estimate; only then is the tender invited. In a two-bid system, technical bids are evaluated first and only qualified bidders' financial bids are opened, after which the work order is issued. (d) opens prices before technical screening — the main trap."}, {"kind": "mcq", "text": "Using the flowchart, what is the outcome for an applicant with complete documents, annual family income ₹1.5 lakh, age 52 years, certified disability 40%, who is a widow?", "opts": ["Disability pension", "Not eligible", "Widow pension", "Old-age pension"], "correct": 2, "tag": "", "sol": "S1 YES → S2 (₹1.5 lakh < ₹1.8 lakh) YES → S3 (52 < 60) NO → S4 (40% < 60%) NO → S5 (widow, adult) YES → Widow pension. Stopping at S4 and choosing 'Disability pension' ignores that her disability is below 60%.", "fig": "<div style=\"border:1px solid var(--rule);border-left:4px solid var(--accent-text);background:var(--card);color:var(--ink);padding:10px 12px;border-radius:6px;font-size:0.95em;line-height:1.5;max-width:100%;box-sizing:border-box\"><b>Pension screening flowchart (illustrative)</b><br><b>S1.</b> Are documents complete? YES → S2. NO → <i>Return to applicant</i>.<br><b>S2.</b> Is annual family income below ₹1.8 lakh? YES → S3. NO → <i>Not eligible</i>.<br><b>S3.</b> Is age 60 years or more? YES → <i>Old-age pension</i>. NO → S4.<br><b>S4.</b> Is certified disability 60% or more? YES → <i>Disability pension</i>. NO → S5.<br><b>S5.</b> Is the applicant a widow aged 18 or more? YES → <i>Widow pension</i>. NO → <i>Not eligible</i>.</div>"}, {"kind": "mcq", "text": "Six officers P, Q, R, S, T and U sit in a row of six chairs facing the dais. T sits third from the left end and U sits immediately to the right of T. R sits at one of the two ends. P and Q sit next to each other, with Q to the left of P. S does not sit at either end and sits somewhere to the left of T.<br>Who sits at the extreme right end?", "opts": ["R", "Q", "U", "P"], "correct": 3, "tag": "", "sol": "T = seat 3, U = seat 4. S is left of T and not at an end, so S = seat 2. Seats 1, 5, 6 remain; P and Q need two adjacent seats, so they take 5–6 with Q on 5 and P on 6, and R takes seat 1. Order: R S T U Q P, so P is at the right end. Choosing R assumes R must be on the right."}, {"kind": "mcq", "text": "A field report shows that in one block, about 30% of ration-card holders have not lifted their monthly foodgrain for three months. Most of them say the local fair-price shop opens irregularly. Which is the <b>most appropriate</b> course of action?", "opts": ["Cancel the ration cards of all holders who have not lifted grain for three months.", "Inspect the shop, enforce fixed opening hours, and help beneficiaries use portability to lift from another shop meanwhile.", "Close all fair-price shops in the block and shift to cash transfers immediately.", "Wait for the next quarterly report to see if the problem continues."], "correct": 1, "tag": "", "sol": "The evidence points to a supply-side failure (irregular opening), so the response should fix the shop and protect access in the meantime. Cancelling cards punishes beneficiaries for the shop's fault; closing all shops is disproportionate; waiting ignores a documented problem affecting food security."}, {"kind": "mcq", "text": "A district introduced a new mid-day meal menu in 50 schools in July and wants to know whether it raised attendance. Which evidence would be <b>most useful</b>?", "opts": ["Attendance in the 50 schools in August compared with July.", "Feedback from cooks on how much children liked the new dishes.", "Change in attendance in the 50 schools versus comparable schools with the old menu, over the same months.", "The number of schools in the state that serve a similar menu."], "correct": 2, "tag": "", "sol": "A before–after comparison alone (a) cannot separate the menu's effect from season, exams or festivals; comparing the change with similar schools on the old menu over the same period controls for those common factors. Liking the food (b) is not attendance, and (d) is irrelevant."}, {"kind": "mcq", "text": "<i>\"Districts with more CCTV cameras per lakh population report fewer road-accident deaths. Therefore, installing more CCTV cameras will reduce road deaths in every district.\"</i><br>Which of the following best identifies the <b>flaw</b> in this reasoning?", "opts": ["It ignores that CCTV cameras are expensive to install and maintain.", "It assumes that all districts have the same number of roads.", "It relies on data about deaths rather than data about injuries.", "It treats an association as causation, though districts with many cameras may also have better roads, lower speeds or quicker trauma care."], "correct": 3, "tag": "", "sol": "The evidence shows only a correlation. A third factor — e.g. more urbanised, better-funded districts having both more cameras and better roads and emergency care — could explain both. Cost (a) is a practical issue, not a flaw in the reasoning; (b) and (c) do not touch the causal leap."}, {"kind": "mcq", "text": "Find the next number in the series: 1, 2, 6, 15, 31, 56, ?", "opts": ["92", "87", "90", "97"], "correct": 0, "tag": "", "sol": "Differences are 1, 4, 9, 16, 25 — the squares 1², 2², 3², 4², 5². The next difference is 6² = 36, so 56 + 36 = 92. Taking differences as growing by 5 or 6 gives the traps 87/90."}, {"kind": "mcq", "text": "In a certain code, WARD is written as ESBX and BLOCK as LDPMC. How will TEHSIL be written in that code?", "opts": ["MJTIFU", "UFITJM", "MJTFIU", "KHRGDS"], "correct": 0, "tag": "", "sol": "Rule: write the word in reverse and shift each letter one step forward. WARD → DRAW → ESBX; BLOCK → KCOLB → LDPMC. TEHSIL → LISHET → MJTIFU. (b) shifts without reversing; (d) reverses but shifts backward."}, {"kind": "mcq", "text": "A survey officer walks 8 km north, turns right and walks 2 km, turns right and walks 3 km, turns left and walks 4 km, and finally turns left and walks 3 km. How far and in which direction is she from the starting point?", "opts": ["10 km, north-east", "14 km, north-east", "10 km, north-west", "8 km, east"], "correct": 0, "tag": "", "sol": "Taking start as (0, 0): north 8 → (0, 8); right = east 2 → (2, 8); right = south 3 → (2, 5); left = east 4 → (6, 5); left = north 3 → (6, 8). Distance = √(6² + 8²) = 10 km, towards the north-east. Adding the net east and north legs (6 + 8 = 14 km, option b) instead of using Pythagoras is the usual trap."}, {"kind": "mcq", "text": "Kavita's mother is the only daughter of Mohan's father. How is Mohan related to Kavita?", "opts": ["Father", "Cousin", "Maternal uncle", "Grandfather"], "correct": 2, "tag": "", "sol": "The only daughter of Mohan's father is Mohan's sister. She is Kavita's mother, so Mohan is the brother of Kavita's mother, i.e. her maternal uncle. Reading 'Mohan's father' as Kavita's grandfather on the father's side leads to wrong options."}]}, {"id": "s4", "label": "Part D", "sub": "English and Hindi communication · 15 questions · 15 marks", "slides": [{"kind": "mcq", "text": "Read the passage (shown above) on crop-diversification incentives and answer the question. Which of the following best states the <b>main argument</b> of the passage?", "opts": ["Farmers in north-western India are by nature unwilling to try new crops, so incentives cannot work.", "Crop-switching incentives fail mainly because they pay for the loss of one crop but not for the loss of the assured market and credit system that comes with it.", "The per-acre incentive offered for leaving paddy is too small and must be raised substantially.", "Groundwater can be protected only by drilling deeper borewells and supplying water by tankers."], "correct": 1, "tag": "", "sol": "The author says the problem lies 'less in the size of the incentive than in what it is attached to': farmers lose procurement, mandis and credit when they leave paddy. The trap is 'farmers are conservative' — the author calls that explanation 'convenient, and mostly wrong'. Raising the incentive is explicitly said to reward mainly those who would switch anyway.", "fig": "<div><div style=\"font-weight:700;margin:0 0 6px;color:var(--accent-text)\">Read the passage</div><div style=\"max-height:320px;overflow:auto;border:1px solid var(--rule);border-radius:10px;padding:10px 12px;background:var(--card)\"><p style=\"margin:0 0 8px;line-height:1.55\">When a state offers farmers a cash incentive to move from paddy to less water-hungry crops, the arithmetic looks irresistible. Every hectare shifted out of transplanted rice saves a large volume of groundwater, and the incentive costs far less than the eventual price of deeper borewells, failed wells and drinking-water tankers. Yet several districts that announced such incentives have found that the area under paddy barely moved. The usual explanation is that farmers are conservative. That explanation is convenient, and mostly wrong.</p><p style=\"margin:0 0 8px;line-height:1.55\">A farmer's choice of crop is not a single decision but the last link in a chain. Paddy and wheat in north-western India are backed by assured public procurement at an announced minimum support price, a dense network of mandis, and commission agents who extend credit against the coming harvest. A farmer who switches to maize or pulses gives up most of this machinery at once. He may receive a one-time payment per acre, but he also faces uncertain buyers, prices that can fall sharply at harvest, and the risk that his dealer will not lend to him next season. Seen from the field, the incentive compensates for the visible loss of one crop while ignoring the invisible loss of an entire support system.</p><p style=\"margin:0 0 8px;line-height:1.55\">This suggests that the problem lies less in the size of the incentive than in what it is attached to. Districts that have made modest progress tended to do three things together. They arranged purchase of the alternative crop, either through a public agency or through a contract with a processor, before the sowing season rather than after it. They worked through farmer producer organisations, so that the risk of a new crop was shared by a group rather than carried by one household. And they paid the incentive in instalments linked to verified sowing, which reduced both leakage and the suspicion that the scheme was a one-season experiment.</p><p style=\"margin:0 0 8px;line-height:1.55\">None of this is glamorous. A press release announcing a higher per-acre payment attracts more attention than an agreement with a starch factory. But groundwater tables do not respond to announcements. They respond to the number of hectares that stop being flooded every June, year after year. A policy that wants that number to fall must make the new crop as boring and predictable to grow and sell as the old one. Until it does, raising the incentive will mostly reward the farmers who were going to switch anyway, and the water table will keep falling.</p></div></div>"}, {"kind": "mcq", "text": "Read the passage (shown above) on crop-diversification incentives and answer the question. Which of the following can be most reasonably <b>inferred</b> from the passage?", "opts": ["Farmer producer organisations buy alternative crops at better prices than public agencies do.", "Paying the incentive in instalments makes the scheme costlier for the government.", "Maize and pulses always fetch a lower price per hectare than paddy at harvest.", "A district that doubles the per-acre incentive but arranges no buyer for the new crop is unlikely to see a large lasting fall in the area under paddy."], "correct": 3, "tag": "", "sol": "The passage says the size of the incentive matters less than assured purchase, and that a higher payment alone 'will mostly reward the farmers who were going to switch anyway'. The other options go beyond the text: it never compares FPO and agency prices, never says instalments raise cost (it says they cut leakage), and speaks only of prices that 'can fall', not that they always are lower.", "fig": "<div><div style=\"font-weight:700;margin:0 0 6px;color:var(--accent-text)\">Read the passage</div><div style=\"max-height:320px;overflow:auto;border:1px solid var(--rule);border-radius:10px;padding:10px 12px;background:var(--card)\"><p style=\"margin:0 0 8px;line-height:1.55\">When a state offers farmers a cash incentive to move from paddy to less water-hungry crops, the arithmetic looks irresistible. Every hectare shifted out of transplanted rice saves a large volume of groundwater, and the incentive costs far less than the eventual price of deeper borewells, failed wells and drinking-water tankers. Yet several districts that announced such incentives have found that the area under paddy barely moved. The usual explanation is that farmers are conservative. That explanation is convenient, and mostly wrong.</p><p style=\"margin:0 0 8px;line-height:1.55\">A farmer's choice of crop is not a single decision but the last link in a chain. Paddy and wheat in north-western India are backed by assured public procurement at an announced minimum support price, a dense network of mandis, and commission agents who extend credit against the coming harvest. A farmer who switches to maize or pulses gives up most of this machinery at once. He may receive a one-time payment per acre, but he also faces uncertain buyers, prices that can fall sharply at harvest, and the risk that his dealer will not lend to him next season. Seen from the field, the incentive compensates for the visible loss of one crop while ignoring the invisible loss of an entire support system.</p><p style=\"margin:0 0 8px;line-height:1.55\">This suggests that the problem lies less in the size of the incentive than in what it is attached to. Districts that have made modest progress tended to do three things together. They arranged purchase of the alternative crop, either through a public agency or through a contract with a processor, before the sowing season rather than after it. They worked through farmer producer organisations, so that the risk of a new crop was shared by a group rather than carried by one household. And they paid the incentive in instalments linked to verified sowing, which reduced both leakage and the suspicion that the scheme was a one-season experiment.</p><p style=\"margin:0 0 8px;line-height:1.55\">None of this is glamorous. A press release announcing a higher per-acre payment attracts more attention than an agreement with a starch factory. But groundwater tables do not respond to announcements. They respond to the number of hectares that stop being flooded every June, year after year. A policy that wants that number to fall must make the new crop as boring and predictable to grow and sell as the old one. Until it does, raising the incentive will mostly reward the farmers who were going to switch anyway, and the water table will keep falling.</p></div></div>"}, {"kind": "mcq", "text": "Read the passage (shown above) on crop-diversification incentives and answer the question. The author calls the explanation that 'farmers are conservative' <i>convenient, and mostly wrong</i> because", "opts": ["it blames farmers' attitudes, whereas their reluctance is a sensible response to losing assured procurement, credit and buyers.", "farmers in fact switch crops readily whenever the per-acre incentive is raised by the state.", "the districts concerned had never actually paid the incentive that they had announced.", "the most conservative farmers were the first to adopt maize and pulses in those districts."], "correct": 0, "tag": "", "sol": "The second paragraph explains that switching means giving up 'an entire support system', so staying with paddy is a rational choice, not mere conservatism; blaming attitudes is 'convenient' because it spares the policy design. The trap (raising incentives makes farmers switch) contradicts the last paragraph; the other two options are not stated anywhere.", "fig": "<div><div style=\"font-weight:700;margin:0 0 6px;color:var(--accent-text)\">Read the passage</div><div style=\"max-height:320px;overflow:auto;border:1px solid var(--rule);border-radius:10px;padding:10px 12px;background:var(--card)\"><p style=\"margin:0 0 8px;line-height:1.55\">When a state offers farmers a cash incentive to move from paddy to less water-hungry crops, the arithmetic looks irresistible. Every hectare shifted out of transplanted rice saves a large volume of groundwater, and the incentive costs far less than the eventual price of deeper borewells, failed wells and drinking-water tankers. Yet several districts that announced such incentives have found that the area under paddy barely moved. The usual explanation is that farmers are conservative. That explanation is convenient, and mostly wrong.</p><p style=\"margin:0 0 8px;line-height:1.55\">A farmer's choice of crop is not a single decision but the last link in a chain. Paddy and wheat in north-western India are backed by assured public procurement at an announced minimum support price, a dense network of mandis, and commission agents who extend credit against the coming harvest. A farmer who switches to maize or pulses gives up most of this machinery at once. He may receive a one-time payment per acre, but he also faces uncertain buyers, prices that can fall sharply at harvest, and the risk that his dealer will not lend to him next season. Seen from the field, the incentive compensates for the visible loss of one crop while ignoring the invisible loss of an entire support system.</p><p style=\"margin:0 0 8px;line-height:1.55\">This suggests that the problem lies less in the size of the incentive than in what it is attached to. Districts that have made modest progress tended to do three things together. They arranged purchase of the alternative crop, either through a public agency or through a contract with a processor, before the sowing season rather than after it. They worked through farmer producer organisations, so that the risk of a new crop was shared by a group rather than carried by one household. And they paid the incentive in instalments linked to verified sowing, which reduced both leakage and the suspicion that the scheme was a one-season experiment.</p><p style=\"margin:0 0 8px;line-height:1.55\">None of this is glamorous. A press release announcing a higher per-acre payment attracts more attention than an agreement with a starch factory. But groundwater tables do not respond to announcements. They respond to the number of hectares that stop being flooded every June, year after year. A policy that wants that number to fall must make the new crop as boring and predictable to grow and sell as the old one. Until it does, raising the incentive will mostly reward the farmers who were going to switch anyway, and the water table will keep falling.</p></div></div>"}, {"kind": "mcq", "text": "Read the passage (shown above) on crop-diversification incentives and answer the question. By saying a policy must make the new crop 'as <i>boring and predictable</i> to grow and sell as the old one', the author means that", "opts": ["the government should promote only crops that need little skill and no new technology to grow.", "the scheme should be run quietly, without press releases or any publicity about the incentive.", "the new crop should carry the same assured buyers, prices and credit that make paddy a low-risk choice.", "farmers should be discouraged from experimenting with crops other than maize and pulses."], "correct": 2, "tag": "", "sol": "'Boring and predictable' is praise here: paddy is attractive because selling it is certain. The author wants the alternative crop to offer the same certainty of market, price and credit. The trap reads 'boring' literally as 'no publicity'; the author contrasts glamour with results but does not ask for secrecy.", "fig": "<div><div style=\"font-weight:700;margin:0 0 6px;color:var(--accent-text)\">Read the passage</div><div style=\"max-height:320px;overflow:auto;border:1px solid var(--rule);border-radius:10px;padding:10px 12px;background:var(--card)\"><p style=\"margin:0 0 8px;line-height:1.55\">When a state offers farmers a cash incentive to move from paddy to less water-hungry crops, the arithmetic looks irresistible. Every hectare shifted out of transplanted rice saves a large volume of groundwater, and the incentive costs far less than the eventual price of deeper borewells, failed wells and drinking-water tankers. Yet several districts that announced such incentives have found that the area under paddy barely moved. The usual explanation is that farmers are conservative. That explanation is convenient, and mostly wrong.</p><p style=\"margin:0 0 8px;line-height:1.55\">A farmer's choice of crop is not a single decision but the last link in a chain. Paddy and wheat in north-western India are backed by assured public procurement at an announced minimum support price, a dense network of mandis, and commission agents who extend credit against the coming harvest. A farmer who switches to maize or pulses gives up most of this machinery at once. He may receive a one-time payment per acre, but he also faces uncertain buyers, prices that can fall sharply at harvest, and the risk that his dealer will not lend to him next season. Seen from the field, the incentive compensates for the visible loss of one crop while ignoring the invisible loss of an entire support system.</p><p style=\"margin:0 0 8px;line-height:1.55\">This suggests that the problem lies less in the size of the incentive than in what it is attached to. Districts that have made modest progress tended to do three things together. They arranged purchase of the alternative crop, either through a public agency or through a contract with a processor, before the sowing season rather than after it. They worked through farmer producer organisations, so that the risk of a new crop was shared by a group rather than carried by one household. And they paid the incentive in instalments linked to verified sowing, which reduced both leakage and the suspicion that the scheme was a one-season experiment.</p><p style=\"margin:0 0 8px;line-height:1.55\">None of this is glamorous. A press release announcing a higher per-acre payment attracts more attention than an agreement with a starch factory. But groundwater tables do not respond to announcements. They respond to the number of hectares that stop being flooded every June, year after year. A policy that wants that number to fall must make the new crop as boring and predictable to grow and sell as the old one. Until it does, raising the incentive will mostly reward the farmers who were going to switch anyway, and the water table will keep falling.</p></div></div>"}, {"kind": "mcq", "text": "Choose the sentence that is grammatically correct and suitable for an official note.", "opts": ["The list of eligible beneficiaries, along with the verification reports, have been forwarded to the Deputy Commissioner.", "The list of eligible beneficiaries along with the verification reports were forwarded to Deputy Commissioner.", "The list of eligible beneficiaries, along with the verification reports, has been forwarded to the Deputy Commissioner.", "The lists of eligible beneficiary, along with verification report, has been forwarded to the Deputy Commissioner."], "correct": 2, "tag": "", "sol": "The subject is 'The list' (singular); a phrase introduced by 'along with' does not make it plural, so the verb must be 'has been'. The trap 'have been' agrees wrongly with 'reports'. The 'were forwarded' option has the same error and drops 'the' before the designation; the 'lists … has' option has a plural subject with a singular verb and 'beneficiary' in the singular."}, {"kind": "mcq", "text": "The sentences P, Q, R and S of a short municipal notice are jumbled. Choose the correct order.<br><b>P</b>: To ensure that no eligible household misses the camp, ward councillors are requested to send lists of residents who still lack ration cards by 10 November.<br><b>Q</b>: The Municipal Committee will hold a special ration-card enrolment camp at the Community Centre, Sector 4, on 15 November.<br><b>R</b>: These reminders will also tell residents to bring an Aadhaar card and proof of residence.<br><b>S</b>: The lists so received will be used to send each listed household an SMS reminder two days before the camp.", "opts": ["P Q S R", "Q P S R", "Q S P R", "Q P R S"], "correct": 1, "tag": "", "sol": "Q announces the camp, so it opens the notice; P refers to 'the camp' and asks for lists; S uses 'the lists so received', so it must follow P; R says 'These reminders', which refers to the SMS reminders in S. Hence Q-P-S-R. 'Q P R S' fails because 'these reminders' would appear before any reminder is mentioned."}, {"kind": "mcq", "text": "A senior citizen has written that his old-age pension for August has not reached his bank account. Which reply is the most appropriate for an official response?", "opts": ["As per records, the delay is due to non-seeding of Aadhaar on your part; necessary action may be taken by you at the earliest.", "Pension delays are common across the state and are being looked into at higher levels. Kindly wait patiently for further orders.", "Your complaint has been noted and will be resolved immediately, positively by tomorrow, without fail and in full.", "We regret the delay. Your account was not linked with Aadhaar, which held up the payment; this has been corrected today and the amount will be credited within seven working days."], "correct": 3, "tag": "", "sol": "A good reply to a citizen is polite, explains the cause in plain words, says what has been done and gives a realistic timeline. The 'non-seeding … on your part' reply is accusatory and pushes the burden back on the citizen; the 'wait patiently' reply is vague and offers no action; the 'without fail' reply over-promises and never explains the cause."}, {"kind": "mcq", "text": "ऊपर दिए गए गद्यांश (गाँव के तालाब) को पढ़कर प्रश्न का उत्तर दीजिए। गद्यांश का <b>मूल संदेश</b> क्या है?", "opts": ["सार्वजनिक संपत्ति का स्थायी संरक्षण तभी संभव है, जब समुदाय उसे अपना माने और उसकी देखरेख में भागीदार बने।", "नलकूप और पाइप से जलापूर्ति आने के बाद गाँवों में तालाबों की कोई उपयोगिता नहीं रह गई है।", "तालाबों को बचाने के लिए प्रशासन को ठेकेदारों के माध्यम से अधिक धनराशि ख़र्च करनी चाहिए।", "मछली-पालन का ठेका देना ही तालाबों के रखरखाव का एकमात्र प्रभावी उपाय है।"], "correct": 0, "tag": "", "sol": "लेखक का केंद्रीय कथन है कि 'केवल धन से तालाब नहीं बचते' और 'उसे जीवित रखने का काम लोगों की भागीदारी से ही संभव है'। 'अधिक धनराशि' वाला विकल्प भ्रामक है, क्योंकि ठेकेदार द्वारा किए गए काम का परिणाम अस्थायी बताया गया है। मछली-पालन केवल एक उदाहरण है, एकमात्र उपाय नहीं।", "fig": "<div lang=\"hi\"><div style=\"font-weight:700;margin:0 0 6px;color:var(--accent-text)\">गद्यांश पढ़िए</div><div style=\"max-height:320px;overflow:auto;border:1px solid var(--rule);border-radius:10px;padding:10px 12px;background:var(--card)\"><p style=\"margin:0 0 8px;line-height:1.55\">एक समय था जब गाँव का तालाब केवल पानी का स्रोत नहीं, बल्कि सामुदायिक जीवन का केंद्र हुआ करता था। पशु वहीं पानी पीते थे, वर्षा का जल वहीं इकट्ठा होता था और आसपास के कुओं का जलस्तर भी उसी से बना रहता था। जब गाँवों में नलकूप लग गए और घरों तक पाइप से पानी पहुँचने लगा, तो लोगों को लगा कि अब तालाब की कोई आवश्यकता नहीं रही। धीरे-धीरे तालाबों में घरों का गंदा पानी गिरने लगा, उनके किनारों पर अतिक्रमण हो गया और कई तालाब कूड़े के ढेर में बदल गए।</p><p style=\"margin:0 0 8px;line-height:1.55\">पिछले कुछ वर्षों में प्रशासन ने तालाबों के जीर्णोद्धार के लिए धनराशि उपलब्ध कराई है। अनुभव बताता है कि केवल धन से तालाब नहीं बचते। जिन गाँवों में ठेकेदार ने खुदाई करके काम पूरा मान लिया, वहाँ दो-तीन वर्षों में स्थिति फिर पहले जैसी हो गई। इसके विपरीत, जिन गाँवों में ग्राम सभा ने स्वयं योजना बनाई, वहाँ परिणाम अधिक स्थायी रहे। ऐसे गाँवों में सबसे पहले यह तय किया गया कि घरों का गंदा पानी तालाब तक पहुँचने से पूर्व कहाँ और कैसे साफ़ होगा। फिर तालाब की देखरेख के लिए एक समिति बनाई गई, जिसमें महिलाओं और युवाओं को भी स्थान मिला। कुछ गाँवों ने तालाब में मछली-पालन का ठेका देकर उससे होने वाली आय को रखरखाव पर ख़र्च करने का नियम बना दिया।</p><p style=\"margin:0 0 8px;line-height:1.55\">इन उदाहरणों से एक बात स्पष्ट होती है। किसी सार्वजनिक संपत्ति की रक्षा तभी होती है, जब समुदाय उसे अपना मानता है और उसकी देखभाल में अपना प्रत्यक्ष लाभ देखता है। सरकारी योजना ढाँचा खड़ा कर सकती है, परंतु उसे जीवित रखने का काम लोगों की भागीदारी से ही संभव है। इसलिए प्रशासन की भूमिका केवल धन देने तक सीमित नहीं होनी चाहिए। उसे ग्राम सभा को तकनीकी सलाह देनी चाहिए, कार्य की गुणवत्ता की निगरानी करनी चाहिए और यह सुनिश्चित करना चाहिए कि निर्णय-प्रक्रिया में गाँव के सभी वर्गों की आवाज़ शामिल हो।</p><p style=\"margin:0 0 8px;line-height:1.55\">तालाबों का प्रश्न वास्तव में जल-प्रबंधन से कहीं बड़ा है। यह इस बात की परीक्षा है कि हम विकास को ऊपर से दिया गया उपहार मानते हैं या मिल-जुलकर निभाई जाने वाली ज़िम्मेदारी।</p></div></div>"}, {"kind": "mcq", "text": "ऊपर दिए गए गद्यांश (गाँव के तालाब) को पढ़कर प्रश्न का उत्तर दीजिए। गद्यांश के आधार पर निम्नलिखित में से कौन-सा <b>निष्कर्ष</b> सबसे उचित है?", "opts": ["जिन गाँवों में समिति में महिलाएँ थीं, वहाँ तालाबों में कभी अतिक्रमण नहीं हुआ।", "प्रशासन को तालाबों के जीर्णोद्धार के लिए धनराशि देना बंद कर देना चाहिए।", "यदि घरों के गंदे पानी की व्यवस्था किए बिना केवल तालाब की खुदाई करा दी जाए, तो उसका लाभ अधिक समय तक नहीं टिकेगा।", "ग्राम सभा द्वारा बनाई गई योजनाओं में तकनीकी सलाह की कोई आवश्यकता नहीं होती।"], "correct": 2, "tag": "", "sol": "गद्यांश के अनुसार केवल खुदाई वाले गाँवों में दो-तीन वर्षों में स्थिति पहले जैसी हो गई, जबकि सफल गाँवों ने सबसे पहले गंदे पानी को साफ़ करने की व्यवस्था तय की। धनराशि बंद करने की बात लेखक नहीं कहता; वह कहता है कि भूमिका 'केवल धन देने तक' सीमित न हो। तकनीकी सलाह को तो प्रशासन का दायित्व बताया गया है।", "fig": "<div lang=\"hi\"><div style=\"font-weight:700;margin:0 0 6px;color:var(--accent-text)\">गद्यांश पढ़िए</div><div style=\"max-height:320px;overflow:auto;border:1px solid var(--rule);border-radius:10px;padding:10px 12px;background:var(--card)\"><p style=\"margin:0 0 8px;line-height:1.55\">एक समय था जब गाँव का तालाब केवल पानी का स्रोत नहीं, बल्कि सामुदायिक जीवन का केंद्र हुआ करता था। पशु वहीं पानी पीते थे, वर्षा का जल वहीं इकट्ठा होता था और आसपास के कुओं का जलस्तर भी उसी से बना रहता था। जब गाँवों में नलकूप लग गए और घरों तक पाइप से पानी पहुँचने लगा, तो लोगों को लगा कि अब तालाब की कोई आवश्यकता नहीं रही। धीरे-धीरे तालाबों में घरों का गंदा पानी गिरने लगा, उनके किनारों पर अतिक्रमण हो गया और कई तालाब कूड़े के ढेर में बदल गए।</p><p style=\"margin:0 0 8px;line-height:1.55\">पिछले कुछ वर्षों में प्रशासन ने तालाबों के जीर्णोद्धार के लिए धनराशि उपलब्ध कराई है। अनुभव बताता है कि केवल धन से तालाब नहीं बचते। जिन गाँवों में ठेकेदार ने खुदाई करके काम पूरा मान लिया, वहाँ दो-तीन वर्षों में स्थिति फिर पहले जैसी हो गई। इसके विपरीत, जिन गाँवों में ग्राम सभा ने स्वयं योजना बनाई, वहाँ परिणाम अधिक स्थायी रहे। ऐसे गाँवों में सबसे पहले यह तय किया गया कि घरों का गंदा पानी तालाब तक पहुँचने से पूर्व कहाँ और कैसे साफ़ होगा। फिर तालाब की देखरेख के लिए एक समिति बनाई गई, जिसमें महिलाओं और युवाओं को भी स्थान मिला। कुछ गाँवों ने तालाब में मछली-पालन का ठेका देकर उससे होने वाली आय को रखरखाव पर ख़र्च करने का नियम बना दिया।</p><p style=\"margin:0 0 8px;line-height:1.55\">इन उदाहरणों से एक बात स्पष्ट होती है। किसी सार्वजनिक संपत्ति की रक्षा तभी होती है, जब समुदाय उसे अपना मानता है और उसकी देखभाल में अपना प्रत्यक्ष लाभ देखता है। सरकारी योजना ढाँचा खड़ा कर सकती है, परंतु उसे जीवित रखने का काम लोगों की भागीदारी से ही संभव है। इसलिए प्रशासन की भूमिका केवल धन देने तक सीमित नहीं होनी चाहिए। उसे ग्राम सभा को तकनीकी सलाह देनी चाहिए, कार्य की गुणवत्ता की निगरानी करनी चाहिए और यह सुनिश्चित करना चाहिए कि निर्णय-प्रक्रिया में गाँव के सभी वर्गों की आवाज़ शामिल हो।</p><p style=\"margin:0 0 8px;line-height:1.55\">तालाबों का प्रश्न वास्तव में जल-प्रबंधन से कहीं बड़ा है। यह इस बात की परीक्षा है कि हम विकास को ऊपर से दिया गया उपहार मानते हैं या मिल-जुलकर निभाई जाने वाली ज़िम्मेदारी।</p></div></div>"}, {"kind": "mcq", "text": "ऊपर दिए गए गद्यांश (गाँव के तालाब) को पढ़कर प्रश्न का उत्तर दीजिए। 'हम विकास को <i>ऊपर से दिया गया उपहार</i> मानते हैं' — इस अंश का <b>आशय</b> है:", "opts": ["विकास को ऐसा कार्य मानना, जो केवल उच्च शिक्षित विशेषज्ञ ही ठीक ढंग से कर सकते हैं।", "विकास को ऐसी योजना मानना, जिसके लिए धन सदैव केंद्र सरकार से ही आना चाहिए।", "विकास को ऐसा पुरस्कार मानना, जो केवल अच्छा काम करने वाले गाँवों को दिया जाता है।", "विकास को ऐसी वस्तु मानना, जो सरकार से मिलती है और जिसकी देखरेख में लोगों की अपनी कोई ज़िम्मेदारी नहीं होती।"], "correct": 3, "tag": "", "sol": "वाक्य में 'उपहार' की तुलना 'मिल-जुलकर निभाई जाने वाली ज़िम्मेदारी' से की गई है; अर्थात् उपहार वह है जिसे लोग बिना भागीदारी के केवल ग्रहण करते हैं। 'पुरस्कार' वाला विकल्प 'उपहार' शब्द का शाब्दिक अर्थ पकड़ता है, आशय नहीं; विशेषज्ञ या केंद्र सरकार की चर्चा गद्यांश में नहीं है।", "fig": "<div lang=\"hi\"><div style=\"font-weight:700;margin:0 0 6px;color:var(--accent-text)\">गद्यांश पढ़िए</div><div style=\"max-height:320px;overflow:auto;border:1px solid var(--rule);border-radius:10px;padding:10px 12px;background:var(--card)\"><p style=\"margin:0 0 8px;line-height:1.55\">एक समय था जब गाँव का तालाब केवल पानी का स्रोत नहीं, बल्कि सामुदायिक जीवन का केंद्र हुआ करता था। पशु वहीं पानी पीते थे, वर्षा का जल वहीं इकट्ठा होता था और आसपास के कुओं का जलस्तर भी उसी से बना रहता था। जब गाँवों में नलकूप लग गए और घरों तक पाइप से पानी पहुँचने लगा, तो लोगों को लगा कि अब तालाब की कोई आवश्यकता नहीं रही। धीरे-धीरे तालाबों में घरों का गंदा पानी गिरने लगा, उनके किनारों पर अतिक्रमण हो गया और कई तालाब कूड़े के ढेर में बदल गए।</p><p style=\"margin:0 0 8px;line-height:1.55\">पिछले कुछ वर्षों में प्रशासन ने तालाबों के जीर्णोद्धार के लिए धनराशि उपलब्ध कराई है। अनुभव बताता है कि केवल धन से तालाब नहीं बचते। जिन गाँवों में ठेकेदार ने खुदाई करके काम पूरा मान लिया, वहाँ दो-तीन वर्षों में स्थिति फिर पहले जैसी हो गई। इसके विपरीत, जिन गाँवों में ग्राम सभा ने स्वयं योजना बनाई, वहाँ परिणाम अधिक स्थायी रहे। ऐसे गाँवों में सबसे पहले यह तय किया गया कि घरों का गंदा पानी तालाब तक पहुँचने से पूर्व कहाँ और कैसे साफ़ होगा। फिर तालाब की देखरेख के लिए एक समिति बनाई गई, जिसमें महिलाओं और युवाओं को भी स्थान मिला। कुछ गाँवों ने तालाब में मछली-पालन का ठेका देकर उससे होने वाली आय को रखरखाव पर ख़र्च करने का नियम बना दिया।</p><p style=\"margin:0 0 8px;line-height:1.55\">इन उदाहरणों से एक बात स्पष्ट होती है। किसी सार्वजनिक संपत्ति की रक्षा तभी होती है, जब समुदाय उसे अपना मानता है और उसकी देखभाल में अपना प्रत्यक्ष लाभ देखता है। सरकारी योजना ढाँचा खड़ा कर सकती है, परंतु उसे जीवित रखने का काम लोगों की भागीदारी से ही संभव है। इसलिए प्रशासन की भूमिका केवल धन देने तक सीमित नहीं होनी चाहिए। उसे ग्राम सभा को तकनीकी सलाह देनी चाहिए, कार्य की गुणवत्ता की निगरानी करनी चाहिए और यह सुनिश्चित करना चाहिए कि निर्णय-प्रक्रिया में गाँव के सभी वर्गों की आवाज़ शामिल हो।</p><p style=\"margin:0 0 8px;line-height:1.55\">तालाबों का प्रश्न वास्तव में जल-प्रबंधन से कहीं बड़ा है। यह इस बात की परीक्षा है कि हम विकास को ऊपर से दिया गया उपहार मानते हैं या मिल-जुलकर निभाई जाने वाली ज़िम्मेदारी।</p></div></div>"}, {"kind": "mcq", "text": "निम्नलिखित में से <b>शुद्ध वाक्य</b> चुनिए।", "opts": ["ग्राम सभा की बैठक में सभी सदस्यों ने अपना-अपना राय दी।", "ग्राम सभा की बैठक में सभी सदस्यों ने अपनी-अपनी राय दी।", "ग्राम सभा के बैठक में सभी सदस्यों ने अपनी-अपनी राय दिया।", "ग्राम सभा की बैठक में सभी सदस्य ने अपनी-अपनी राय दी।"], "correct": 1, "tag": "", "sol": "'बैठक' और 'राय' दोनों स्त्रीलिंग हैं, इसलिए 'की बैठक', 'अपनी-अपनी राय' और 'दी' सही हैं। 'ने' के साथ क्रिया कर्म (राय) के अनुसार चलती है, इसलिए 'राय दिया' अशुद्ध है। 'सभी' के साथ बहुवचन 'सदस्यों' आएगा। पहले विकल्प में 'अपना-अपना राय' लिंग की भूल है।"}, {"kind": "mcq", "text": "निम्नलिखित में से <b>शुद्ध वर्तनी</b> वाला शब्द कौन-सा है?", "opts": ["अनुगृहीत", "प्रशाशनिक", "कवियत्री", "उज्वल"], "correct": 0, "tag": "", "sol": "'अनुगृहीत' (कृतज्ञ) शुद्ध है। अन्य शब्दों के शुद्ध रूप हैं — 'प्रशासनिक' (स, श नहीं), 'कवयित्री' (य के बाद इ की मात्रा), 'उज्ज्वल' (ज् + ज्व)। 'कवियत्री' सबसे आम भूल है, क्योंकि बोलचाल में यही उच्चारण सुनाई देता है।"}, {"kind": "mcq", "text": "कार्यालयी हिंदी में अंग्रेज़ी शब्द <b>'Notification'</b> के लिए उपयुक्त पारिभाषिक शब्द कौन-सा है?", "opts": ["परिपत्र", "ज्ञापन", "अनुस्मारक", "अधिसूचना"], "correct": 3, "tag": "", "sol": "सरकार द्वारा राजपत्र आदि में प्रकाशित औपचारिक घोषणा 'अधिसूचना' (Notification) कहलाती है। 'परिपत्र' = Circular, 'ज्ञापन' = Memorandum और 'अनुस्मारक' = Reminder हैं; 'परिपत्र' भी सूचना देता है, इसलिए यह मुख्य भ्रामक विकल्प है।"}, {"kind": "mcq", "text": "एक नागरिक ने शिकायत की है कि उसके वार्ड से कई दिनों से कूड़ा नहीं उठाया गया। नगर परिषद के उत्तर के लिए <b>सबसे उपयुक्त</b> वाक्य कौन-सा है?", "opts": ["आपकी शिकायत निराधार है, क्योंकि हमारे रिकॉर्ड के अनुसार आपके वार्ड से कूड़ा प्रतिदिन उठाया जा रहा है।", "सफ़ाई कर्मचारियों की भारी कमी चल रही है, इसलिए आपको कुछ और दिन धैर्य रखना ही पड़ेगा।", "आपको हुई असुविधा के लिए खेद है। सफ़ाई निरीक्षक को निर्देश दिए गए हैं कि कल शाम तक आपके वार्ड से कूड़ा उठवाकर आपको सूचित करें।", "आपकी शिकायत पर नियमानुसार यथोचित कार्यवाही यथासमय कर दी जाएगी, कृपया प्रतीक्षा करें।"], "correct": 2, "tag": "", "sol": "नागरिक संवाद में खेद-प्रकाश, स्पष्ट कार्रवाई, ज़िम्मेदार अधिकारी और समय-सीमा होनी चाहिए — ये सब सही विकल्प में हैं। पहला विकल्प बिना जाँच के शिकायत को नकारता है, दूसरा केवल बहाना देता है और चौथा (भ्रामक) औपचारिक तो है, पर अस्पष्ट है — न कार्रवाई बताता है, न समय।"}, {"kind": "mcq", "text": "किसी सूचना के वाक्य P, Q, R, S क्रम में नहीं हैं। <b>सही क्रम</b> चुनिए।<br><b>P</b>: इस शिविर में चिकित्सकों का दल जाँच करके दिव्यांगता प्रमाण-पत्र मौके पर ही जारी करेगा।<br><b>Q</b>: जिला प्रशासन 12 दिसंबर को खंड कार्यालय परिसर में दिव्यांगजनों के लिए एक विशेष शिविर लगाएगा।<br><b>R</b>: प्रमाण-पत्र बनवाने के लिए आवेदक अपने साथ आधार कार्ड और पुराने चिकित्सा-पर्चे अवश्य लाएँ।<br><b>S</b>: यदि किसी आवेदक के पास ये दस्तावेज़ उपलब्ध न हों, तो वह शिविर में बने सहायता-केंद्र से संपर्क कर सकता है।", "opts": ["P Q R S", "Q P R S", "Q R P S", "Q S R P"], "correct": 1, "tag": "", "sol": "Q शिविर की घोषणा करता है, इसलिए पहले आएगा; P 'इस शिविर में' कहकर Q से जुड़ता है; R में दस्तावेज़ों की सूची है और S 'ये दस्तावेज़' कहकर R की ओर संकेत करता है, अतः S, R के ठीक बाद आएगा। 'Q R P S' में 'ये दस्तावेज़' का संबंध P से जुड़ जाता है, जहाँ किसी दस्तावेज़ का उल्लेख नहीं है।"}]}, {"id": "s5", "label": "Part E", "sub": "Behavioural and administrative judgement · 20 questions · 20 marks", "slides": [{"kind": "mcq", "text": "You are a Good Governance Associate (GGA) in the DC's office. The department's MIS shows 98% of household tap connections in a block as functional, but in your visits to 12 villages only about 70% of households reported regular supply. At the DC's review tomorrow, the Executive Engineer asks you not to 'confuse' the meeting with a small sample. What is the <b>MOST</b> appropriate action?", "opts": ["Go with the department's MIS figure, since a 12-village sample cannot overturn official data, and mention your visits only if asked.", "Put both figures before the DC, state your sample size and method clearly, and suggest a quick independent check in randomly chosen villages.", "Replace the MIS figure in the review deck with your field estimate, since direct observation of households is more reliable than self-reported data.", "Ask the Executive Engineer to correct the MIS before the meeting, and drop the point from your note if he agrees to look into it."], "correct": 1, "tag": "", "sol": "Best (b): it surfaces the gap transparently, states the limits of your own evidence and proposes a way to verify it, leaving the decision with the DC. Runner-up (c) takes the evidence seriously but over-claims: a 12-village sample is not proof, and quietly swapping official data is not your call. (a) suppresses relevant evidence and (d) makes accountability depend on an informal promise. Competency: integrity, evidence and public accountability."}, {"kind": "mcq", "text": "At a gram sabha, a sarpanch angrily alleges that his village was left out of the road-repair list because of bias. The list was prepared by a scoring formula you helped design. Several villagers are recording the exchange on their phones. What is the <b>MOST</b> appropriate action?", "opts": ["Tell him firmly that the list follows objective criteria and cannot be changed, so the matter is closed.", "Assure him that his village will be added to the next list, so that the meeting can proceed calmly.", "Ask him to raise the matter in the BDPO's office later, since a gram sabha is not the right forum for one village's individual complaint.", "Acknowledge his concern, explain briefly how villages were scored, and offer to go through his village's scores with him and the JE."], "correct": 3, "tag": "", "sol": "Best (d): it calms the situation by listening, explains the basis openly in front of citizens, and offers a concrete way to check the scores. Runner-up (c) avoids a public argument but looks dismissive on camera and leaves the allegation of bias unanswered. (a) is confrontational even if correct, and (b) is a promise you have no authority to make. Competency: stakeholder management and communication."}, {"kind": "mcq", "text": "You are helping run a block-level camp for disability certificates. Turnout is low, and you notice that very few women and elderly persons from the distant villages have come. Anganwadi workers say many eligible people cannot travel to the block headquarters on their own. What is the <b>MOST</b> appropriate action?", "opts": ["Use ANM and anganwadi lists to identify eligible persons village-wise, and hold the next camps at cluster level with transport arranged.", "Extend the block camp by two more days and announce it widely through local newspapers, cable channels, village announcements and the district's social media handles.", "Report that demand in the block is lower than estimated, so that camp resources can be shifted to blocks with better turnout.", "Ask the medical board to accept applications by post, so that people can apply without having to attend the camp at all."], "correct": 0, "tag": "", "sol": "Best (a): the barrier is access, not awareness, so taking the camp closer and arranging transport, using frontline workers' lists, reaches those being left out. Runner-up (b) adds publicity and days but people who cannot travel still cannot come. (c) reads exclusion as low demand, and (d) cannot work because certification needs an in-person assessment. Competency: citizen orientation and inclusion."}, {"kind": "mcq", "text": "It is Monday morning. The DC wants a two-page note on anganwadi infrastructure gaps by 5 pm today for a call with the state. A BDPO wants help cleaning his dashboard data before next week's review. A CM Window grievance marked to you is due in three days, and a local college has invited you to give a talk this afternoon. What is the <b>MOST</b> appropriate action?", "opts": ["Start with the dashboard clean-up, since data quality underpins every other review in the district.", "Split the day evenly across all four tasks, so that none of them falls behind schedule.", "Finish the DC's note first, block time tomorrow for the grievance, fix a slot with the BDPO, and politely reschedule the talk.", "Ask the DC to extend the note's deadline by a day, so that the citizen's grievance, which affects a real person, can be resolved first."], "correct": 2, "tag": "", "sol": "Best (c): it ranks tasks by urgency and importance: the same-day note for the state call first, then the grievance well within its deadline, with the other two scheduled rather than dropped. Runner-up (d) sounds citizen-friendly, but the grievance has three days in hand while the note has a hard deadline today. (a) and (b) ignore the deadlines. Competency: ownership, prioritisation and execution."}, {"kind": "mcq", "text": "You designed an online form for weekly reporting by anganwadi supervisors. After three weeks, only 35% submit on time. Supervisors tell you the network in their areas is weak and the form takes too long. The DC asks you for an update. What is the <b>MOST</b> appropriate action?", "opts": ["Request the DC to issue a circular making the form compulsory for all supervisors, with written explanations sought from those who default.", "Continue unchanged for another month, since any new tool takes time to be adopted and early numbers are often low.", "Meet a few supervisors, cut the form to essential fields, add an offline option, and report the revised plan and lessons to the DC.", "Go back to the earlier paper registers, since the online form has clearly not worked in this district's conditions."], "correct": 2, "tag": "", "sol": "Best (c): it treats the low compliance as feedback on the design, fixes the real causes, and reports the lessons honestly. Runner-up (a) may raise numbers briefly but punishes users for a design problem, and the weak network remains. (b) ignores clear feedback and (d) gives up rather than adapting. Competency: adaptability, resilience and learning."}, {"kind": "mcq", "text": "Two members of the district team, an MIS consultant and a programme officer, have been clashing over who should present the scheme data at the monthly review. Their friction is now slowing down the team's work, and both have complained to you separately. What is the <b>MOST</b> appropriate action?", "opts": ["Raise the matter at the next review meeting with the DC, so that their roles are fixed in front of everyone.", "Talk to each of them separately to understand their concerns before suggesting any division of work.", "Propose a split in which each presents the part of the analysis they own, and agree on it together.", "Bring both together informally to agree on a shared timeline and on who signs off the final numbers before each review."], "correct": 0, "tag": "", "sol": "Least appropriate (a): airing a peer conflict in the DC's review embarrasses both colleagues, hardens positions and skips the steps the team can take itself. (b), (c) and (d) are sensible: understanding each side, then agreeing roles and sign-off together. (d) may look too informal, but an informal joint conversation is often the quickest way to settle a role dispute. Competency: teamwork and conflict management."}, {"kind": "mcq", "text": "Many grievances about delayed old-age pensions reach the DC's office, and each one is being fixed individually. Going through 200 such cases, you find that about 60% involve a mismatch between the date of birth in the family database and in the bank or Aadhaar records. What is the <b>MOST</b> appropriate action?", "opts": ["Set a target for officials to clear all pending pension grievances within seven days, with daily monitoring by the DC's office.", "Recommend that applications be accepted only after documents are verified in person at the block office.", "Ask bank branches to fast-track payments for the complainants whose cases have already been flagged.", "Share the pattern, propose a one-time correction drive and a check at data entry, and track whether new grievances fall."], "correct": 3, "tag": "", "sol": "Best (d): it uses the case data to find the root cause, fixes it for everyone (not only those who complained), prevents new errors at entry, and measures the result. Runner-up (a) clears the backlog but treats symptoms, so the same mismatch will keep creating new grievances. (b) adds a burden on all applicants and (c) helps only those who complained. Competency: systems thinking and innovation."}, {"kind": "mcq", "text": "You are inspecting a school building under construction. You notice that the concrete curing is clearly inadequate. It is getting dark and the last bus has left, and the contractor offers to drop you back to the district headquarters in his car. What is the <b>MOST</b> appropriate action?", "opts": ["Accept the lift, since it is only a practical courtesy, and record your observations on the work honestly anyway.", "Decline politely, arrange your return through the office or another means, and record the curing problem as you found it.", "Accept the lift since refusing may seem rude, but inform your supervisor the next morning so that it is formally on record.", "Decline the lift, and hold back the curing issue for now so that it does not look like a personal reaction."], "correct": 1, "tag": "", "sol": "Best (b): accepting a favour from a party whose work you are assessing creates a conflict of interest, even if your report stays honest; declining and reporting faithfully protects both. Runner-up (c) shows openness, but telling someone afterwards does not remove the obligation already created or how it looks. (a) gives the same perception problem, and (d) suppresses a genuine finding. Competency: integrity and public accountability."}, {"kind": "mcq", "text": "A local journalist calls you, asking why the dialysis unit at the district hospital has been non-functional for two weeks. He says his story will run tonight. You know some of the facts from a review meeting, but you are not an authorised spokesperson. What is the <b>MOST</b> appropriate action?", "opts": ["Politely say you are not authorised to speak to the media, and at once brief the DC's office and the DIPRO with the facts you have.", "Share the facts you know off the record, so that the story is at least accurate without quoting you.", "Decline to comment and end the call, since dealing with the media is outside an associate's role.", "Give a short statement that the unit will be restored soon, to reassure patients who read the story."], "correct": 0, "tag": "", "sol": "Best (a): it respects the authorised channel and also ensures the administration can give an accurate, timely response before the story runs. Runner-up (c) is correct about not speaking, but it lets a known issue reach the press without alerting those who must respond. (b) breaches the channel, and (d) makes an unverified promise. Competency: stakeholder management and communication."}, {"kind": "mcq", "text": "An elderly widow comes to the DC's office in distress. Her pension stopped because the family database wrongly adds the income of her son, who lives separately. The staff told her to apply online for a correction, but she has no smartphone and nobody to help her. What is the <b>MOST</b> appropriate action?", "opts": ["Give her the helpline number and a printed note listing the steps and documents, so that a neighbour or relative can apply online for her.", "Ask her to come back with her son, since the correction will need his details and his consent as well.", "Help her file the correction that day through the designated centre or operator, note her case, and follow up until the pension resumes.", "Forward her case to the DC with a recommendation that the pension be released while the correction is pending."], "correct": 2, "tag": "", "sol": "Best (c): it removes the barrier she actually faces, uses the proper channel for the correction, and owns the outcome through follow-up. Runner-up (a) gives correct information but leaves the burden on a citizen who has already said she cannot use it. (b) adds another trip, and (d) asks for an exception rather than fixing the record. Competency: citizen orientation and inclusion."}, {"kind": "mcq", "text": "You promised the DC a village-wise analysis of crop-residue burning hotspots by Friday. On Wednesday you learn that the latest satellite fire data from the agriculture department will only arrive on Saturday. What is the <b>MOST</b> appropriate action?", "opts": ["Wait for the complete data and submit on Monday instead, since a partial analysis could mislead the DC on where to deploy teams.", "Inform the DC now, submit what is possible by Friday with the gaps marked, and send an update once the data arrives.", "Fill the gap with last year's figures for the missing period, so that the analysis is complete by Friday.", "Write to the agriculture department's head that their delay is holding up the DC's review."], "correct": 1, "tag": "", "sol": "Best (b): flagging the problem early and delivering a clearly labelled partial analysis keeps the commitment honest and useful. Runner-up (a) protects quality but misses the deadline without warning; the DC may have planned around Friday. (c) presents old data as current, and (d) shifts blame instead of solving the problem. Competency: ownership, prioritisation and execution."}, {"kind": "mcq", "text": "In a district meeting, a senior officer sharply criticises your proposal for a new grievance-tracking sheet as 'impractical', in front of other officers. You feel demoralised, and you also suspect that some of his objections are valid. What is the <b>MOST</b> appropriate action?", "opts": ["Withdraw the proposal, since pushing it further could damage your working relationship with the senior officer.", "Point out in the meeting that his own department has the highest pendency, which is why the sheet is needed.", "Try the sheet quietly in one block anyway, and present the results at a later meeting so that real evidence, not opinion, settles the question.", "Ask for a short follow-up with the officer to understand his objections, revise the design, and pilot it with his agreement."], "correct": 3, "tag": "", "sol": "Best (d): it separates the criticism from the person, treats it as learning, and builds the buy-in that implementation will need. Runner-up (c) shows initiative, but working around a senior stakeholder loses his support and may make the results look like a challenge. (a) gives up too easily, and (b) turns a design debate into a confrontation. Competency: adaptability, resilience and learning."}, {"kind": "mcq", "text": "You and a fellow associate prepared a district education report together, sharing the work equally. In a review meeting, the DC praises you alone for the 'excellent report', assuming it was your work. Your colleague is not present. What is the <b>MOST</b> appropriate action?", "opts": ["Mention in the meeting itself that the analysis was a joint effort with your colleague.", "Later, send the DC a short note acknowledging your colleague's contribution to the report.", "Tell your colleague about the praise, and make sure both names appear on the next version.", "Say nothing, since correcting a senior in a meeting may seem awkward and credit evens out over time."], "correct": 3, "tag": "", "sol": "Least appropriate (d): staying silent lets credit be wrongly given and erodes trust within the team. (a), (b) and (c) all give fair credit; (a) may feel awkward in a meeting, but a brief mention is courteous and accurate. Competency: teamwork and conflict management."}, {"kind": "mcq", "text": "A few villages in a block have low institutional deliveries. A colleague proposes building a mobile app to track pregnant women. Your data show that smartphone access among these women is low, while ASHAs already keep due-lists in their registers. What is the <b>MOST</b> appropriate action?", "opts": ["Pilot an ASHA-led due-list with call or SMS reminders in two villages, measure the change in deliveries, and then decide on scaling.", "Develop the app anyway, since smartphone use is rising and a digital tool will be ready for the future.", "Commission a detailed district-wide survey on the causes of home deliveries before trying any intervention, so that the response is fully evidence-based.", "Roll out the reminder system in all villages of the district at once, so that no woman is left out."], "correct": 0, "tag": "", "sol": "Best (a): it builds on the existing system (ASHAs), fits the users' reality, and tests on a small scale with a measurable outcome before scaling. Runner-up (c) values evidence, but a long survey delays action when a cheap, testable idea is available. (b) ignores the access data, and (d) scales without knowing whether it works. Competency: systems thinking and innovation."}, {"kind": "mcq", "text": "You realise that a figure in last week's report to the DC, which has since been shared with the state, was wrong. Because of a formula error in your spreadsheet, the number of beneficiaries was overstated by about 8%. Nobody has noticed so far. What is the <b>MOST</b> appropriate action?", "opts": ["Correct it quietly in next month's report, so that the series becomes accurate from now on.", "Wait to see whether anyone queries the number, and explain the error then if it comes up.", "Inform the DC promptly with the corrected figure and the cause, and add a cross-check step to your process.", "Tell your fellow associates so that the team learns from the mistake, and correct the number in the shared master file."], "correct": 2, "tag": "", "sol": "Best (c): owning the error openly lets the DC correct what the state has received, and the process fix stops it from happening again. Runner-up (a) fixes the future numbers but leaves a wrong figure on record with the state without anyone being told. (b) hides the error, and (d) informs peers but not the person accountable for the report. Competency: integrity and public accountability."}, {"kind": "mcq", "text": "You are building a district dashboard for the DC. The Civil Surgeon's office is unwilling to share block-level health data, saying the data are confidential and the request means extra work for already stretched staff. What is the <b>MOST</b> appropriate action?", "opts": ["Request the DC to issue an order directing the health department to share all the data within a week.", "Meet the Civil Surgeon's team, show how the dashboard helps them, and agree on aggregate, non-personal fields in a simple monthly format.", "Build the dashboard from publicly available data, so that the health department does not need to be involved at all.", "Send a formal letter listing the data needed and a deadline, with a copy to the DC to ensure compliance."], "correct": 1, "tag": "", "sol": "Best (b): it answers both concerns (confidentiality through aggregate data, workload through a simple format) and gives the department a reason to own the dashboard. Runner-up (a) may get the data, but forced and unwilling reporting usually means poor-quality, delayed data. (c) leaves out key data, and (d) is just a softer version of an order. Competency: stakeholder management and communication."}, {"kind": "mcq", "text": "You are organising awareness meetings on an urban housing scheme. The meetings are held at 11 am in the municipal office. You notice that daily-wage workers and most women from the slum settlements, the main target group, are not attending. What is the <b>MOST</b> appropriate action?", "opts": ["Upload the meeting recording and FAQs to the municipal website and social media for those who could not attend.", "Ask the ward councillors to pass the information on to the residents who did not attend the meetings.", "Hold short evening sessions inside the settlements, with women's self-help group members helping to bring people in.", "Distribute printed pamphlets about the scheme door to door in the settlements, so that the information reaches every household."], "correct": 2, "tag": "", "sol": "Best (c): it changes the time and place to suit the people being left out and keeps it two-way, so they can ask about eligibility and documents. Runner-up (d) spreads information but is one-way and does not help people with limited literacy or with specific questions. (a) assumes digital access, and (b) depends on second-hand messages. Competency: citizen orientation and inclusion."}, {"kind": "mcq", "text": "The DC has asked you to lead the arrangements for a district grievance camp in five days. About twelve departments must send officers with their records, and you have no formal authority over any of them. What is the <b>MOST</b> appropriate action?", "opts": ["Send a circular to all departments with the date and venue, asking them to attend with their records.", "Focus first on publicity, since the camp's success depends mainly on how many citizens attend.", "Request the DC to name a senior officer as coordinator, since you lack authority over the departments.", "Make a checklist with owners and deadlines, confirm nodal officers by phone, pre-register grievances, and review readiness daily."], "correct": 3, "tag": "", "sol": "Best (d): it turns the instruction into a plan with named owners and daily follow-up, and pre-registration lets departments come prepared, so the camp can actually resolve cases. Runner-up (a) is a necessary first step, but a circular alone rarely ensures that the right officers come prepared. (b) neglects readiness, and (c) hands back a task you were asked to lead. Competency: ownership, prioritisation and execution."}, {"kind": "mcq", "text": "Midway through your work on school education, heavy rains flood several villages. The DC asks you to support flood-relief coordination for the next three weeks, an area in which you have no experience. What is the <b>MOST</b> appropriate action?", "opts": ["Keep most of your time on the education work, since the flood duty is temporary and others can handle it.", "Quickly learn the relief procedures from the revenue staff, and take up whatever tasks are assigned to you.", "Hand over your pending education tasks with a short status note, so that they do not stall.", "Set up a simple tracker for relief camps and supplies, so that gaps are visible to the DC every day."], "correct": 0, "tag": "", "sol": "Least appropriate (a): it resists a legitimate change in priorities during an emergency and puts your plans above an urgent public need. (b), (c) and (d) show quick learning, a responsible handover and useful contribution. (c) may look like a distraction, but it keeps earlier commitments from being dropped. Competency: adaptability, resilience and learning."}, {"kind": "mcq", "text": "In a block review, the BDPO and the Executive Engineer (Panchayati Raj) blame each other for delays in building community centres. The meeting turns tense, and the DC asks you to sort out the issue before the next review. What is the <b>MOST</b> appropriate action?", "opts": ["Report to the DC which officer is mainly at fault, based on the file notings and dates, so that responsibility is clearly fixed.", "Map each stalled work step by step with both officers, find where each delay occurred, and agree on owners and dates.", "Meet each officer separately and urge them to cooperate more closely in the interest of the district.", "Suggest that the DC give the work to a single agency, so that there is no confusion over who is responsible."], "correct": 1, "tag": "", "sol": "Best (b): it moves the discussion from blame to facts, and gives each pending step a clear owner and date, which is what unblocks the work. Runner-up (a) brings accountability, but deciding who is at fault does not restart the stalled works and makes both officers defensive. (c) is too vague, and (d) is a structural change beyond what the problem needs. Competency: teamwork and conflict management."}]}];
/* ================= build slide lists ================= */
var SLIDES = {}; SECTIONS.forEach(function(sec){ SLIDES[sec.id]=sec.slides; });
var TAB_DEFS = SECTIONS.map(function(sec){ return {id:sec.id, label:sec.label, sub:sec.sub}; });

/* ================= state ================= */
function blankItem(slide){
  if(slide.kind==='mcq'||slide.kind==='ar'){
    return {status:'unanswered', attempts:0, choice:undefined};
  }
  return {status:'unanswered', curStep:0, stepStates: slide.flat.map(function(){ return {status:'unanswered', attempts:0, inputs:{}}; })};
}
function defaultState(){
  var s={tabs:{}};
  TAB_DEFS.forEach(function(td){
    s.tabs[td.id] = { idx:0, maxReached:0, items: SLIDES[td.id].map(function(sl){ return blankItem(sl); }) };
  });
  return s;
}
var appState = {mode:null, learning:null, quiz:null};
var state = null;      // alias for appState[appState.mode]
var MODE = null;
var activeTab=TAB_DEFS[0].id;

function setMode(m){
  appState.mode = m;
  if(!appState[m]) appState[m] = defaultState();
  state = appState[m];
  MODE = m;
}
/* ================= student accounts (saved on this device) ================= */
var SHEET_KEY='sopaan-cmp1';
var ACC_KEY='sopaan-students-v1';
var storageOK=true;
var MEM={};
function lsGet(k){ var r=null; try{ r=localStorage.getItem(k); }catch(e){ storageOK=false; }
  if(r===null||r===undefined) r=MEM[k]||null; try{ return r?JSON.parse(r):null; }catch(e){ return null; } }
function lsSet(k,v){ var j=JSON.stringify(v); MEM[k]=j; try{ localStorage.setItem(k,j); return true; }catch(e){ storageOK=false; return false; } }
try{ localStorage.setItem('sopaan-probe','1'); localStorage.removeItem('sopaan-probe'); }catch(e){ storageOK=false; }
function hashPin(pin,salt){ var h=2166136261, str=salt+'|'+pin; for(var i=0;i<str.length;i++){ h^=str.charCodeAt(i); h=Math.imul(h,16777619)>>>0; } return h.toString(36); }
function accKey(name,roll){ return (name.trim().toLowerCase().replace(/\s+/g,' ')+'#'+roll.trim().toLowerCase()); }
function accounts(){ return lsGet(ACC_KEY)||{students:{}}; }
var student=null; // {key,name,roll}
var records=[];   // finished-tab history for this student on this sheet
function progKey(){ return SHEET_KEY+'::'+student.key; }

function loadState(){
  appState = {mode:null, learning:null, quiz:null}; records=[]; activeTab=TAB_DEFS[0].id;
  var saved=lsGet(progKey());
  if(!saved) return;
  try{
    ['learning','quiz'].forEach(function(m){
      if(saved[m] && saved[m].tabs){
        var fresh = defaultState();
        TAB_DEFS.forEach(function(td){
          if(saved[m].tabs[td.id] && saved[m].tabs[td.id].items && saved[m].tabs[td.id].items.length===SLIDES[td.id].length){
            fresh.tabs[td.id] = saved[m].tabs[td.id];
          }
        });
        appState[m] = fresh;
      }
    });
    if(saved.mode==='learning' || saved.mode==='quiz') appState.mode = saved.mode;
    if(saved.activeTab && TAB_DEFS.some(function(t){ return t.id===saved.activeTab; })) activeTab = saved.activeTab;
    if(Array.isArray(saved.records)) records = saved.records;
  }catch(e){}
}
function saveState(){
  if(!student) return;
  lsSet(progKey(), {mode:appState.mode, learning:appState.learning, quiz:appState.quiz, activeTab:activeTab, records:records, updated:Date.now()});
  var acc=accounts(); if(acc.students[student.key]){ acc.students[student.key].last=Date.now(); lsSet(ACC_KEY,acc); }
}
function addRecord(mode, tabId, correct, revealed, skipped, total){
  records.unshift({at:Date.now(), mode:mode, tab:tabId, correct:correct, revealed:revealed, skipped:skipped, total:total});
  if(records.length>60) records.length=60;
  saveState();
}
function fmtDate(ms){ try{ return new Date(ms).toLocaleString(undefined,{day:'numeric',month:'short',hour:'2-digit',minute:'2-digit'}); }catch(e){ return ''; } }

function renderWho(){
  var el=document.getElementById('whoBar');
  if(!student){ el.hidden=true; el.innerHTML=''; return; }
  el.hidden=false;
  el.innerHTML='Signed in as <b>'+esc(student.name)+'</b> · Roll '+esc(student.roll)+
    ' <button id="btnRecord">My record</button> <button id="btnSignOut">Sign out</button>';
  document.getElementById('btnRecord').addEventListener('click', renderRecord);
  document.getElementById('btnSignOut').addEventListener('click', signOut);
}
function signOut(){
  saveState(); student=null; state=null; MODE=null;
  var acc=accounts(); delete acc.current; lsSet(ACC_KEY,acc);
  document.getElementById('modePill').hidden=true;
  renderWho(); renderLogin();
}
function signIn(key){
  var acc=accounts(); var st=acc.students[key]; if(!st) return;
  student={key:key, name:st.name, roll:st.roll};
  acc.current=key; st.last=Date.now(); lsSet(ACC_KEY,acc);
  loadState(); renderWho();
  if(appState.mode==='learning' || appState.mode==='quiz'){
    setMode(appState.mode); document.getElementById('modePill').hidden=false; updateModePill();
    showChrome(true); buildTabbar(); renderSlide();
    showToast('Welcome back, '+st.name.split(' ')[0]+'. Picking up where you left off.');
  } else {
    renderModePicker();
  }
}
function renderLogin(msg){
  showChrome(false);
  var acc=accounts(); var keys=Object.keys(acc.students).sort(function(a,b){ return (acc.students[b].last||0)-(acc.students[a].last||0); });
  var h='<div class="login-card"><h2>Student sign-in</h2>'+
    '<p class="lead">Sign in to save your answers, see your record and continue where you left off next time.</p>';
  if(!storageOK) h+='<div class="login-err">This browser is blocking saved data (for example, a private window). You can still practise, but progress will not be kept after you close the page.</div>';
  if(msg) h+='<div class="login-err">'+esc(msg)+'</div>';
  if(keys.length){
    h+='<div class="known"><span class="known-label">Continue as</span>';
    keys.slice(0,6).forEach(function(k){ var st=acc.students[k];
      h+='<button class="known-btn" data-k="'+esc(k)+'"><span>'+esc(st.name)+' <small>· Roll '+esc(st.roll)+'</small></span><small>'+(st.last?'Last active '+fmtDate(st.last):'')+'</small></button>'; });
    h+='</div>';
  }
  h+='<form id="loginForm" novalidate>'+
    '<div class="fld"><label for="lgName">Full name</label><input id="lgName" autocomplete="name" required></div>'+
    '<div class="fld-row"><div class="fld"><label for="lgRoll">Roll no.</label><input id="lgRoll" required></div>'+
    '<div class="fld"><label for="lgPin">4-digit PIN</label><input id="lgPin" type="password" inputmode="numeric" maxlength="4" autocomplete="off" required></div></div>'+
    '<button class="btn btn-primary" type="submit" style="width:100%;">Sign in</button>'+
    '<p class="login-note">New here? Enter your name, roll no. and a PIN you will remember, and your profile is created. Progress is saved on this device, so use the same device and browser to continue.</p>'+
    '</form></div>';
  var wrap=document.getElementById('wrap'); wrap.innerHTML=h;
  wrap.querySelectorAll('.known-btn').forEach(function(b){
    b.addEventListener('click', function(){
      var st=accounts().students[b.dataset.k];
      document.getElementById('lgName').value=st.name; document.getElementById('lgRoll').value=st.roll;
      document.getElementById('lgPin').focus();
    });
  });
  document.getElementById('loginForm').addEventListener('submit', function(e){
    e.preventDefault();
    var name=document.getElementById('lgName').value.trim(), roll=document.getElementById('lgRoll').value.trim(), pin=document.getElementById('lgPin').value.trim();
    if(!name||!roll){ renderLoginErr('Enter your name and roll no.'); return; }
    if(!/^\d{4}$/.test(pin)){ renderLoginErr('Your PIN must be exactly 4 digits.'); return; }
    var k=accKey(name,roll); var acc=accounts();
    if(acc.students[k]){
      if(acc.students[k].pin!==hashPin(pin,k)){ renderLoginErr('That PIN does not match this name and roll no. Try again.'); return; }
    } else {
      acc.students[k]={name:name.replace(/\s+/g,' '), roll:roll, pin:hashPin(pin,k), created:Date.now()};
      lsSet(ACC_KEY,acc);
    }
    signIn(k);
  });
}
function renderLoginErr(m){
  var n=document.getElementById('lgName').value, r=document.getElementById('lgRoll').value;
  renderLogin(m); document.getElementById('lgName').value=n; document.getElementById('lgRoll').value=r; document.getElementById('lgPin').focus();
}
function tabSummary(m){
  var st=appState[m]; if(!st) return null;
  return TAB_DEFS.map(function(td){
    var items=st.tabs[td.id].items, n=items.length;
    var c=items.filter(function(i){return i.status==='correct';}).length;
    var done=items.filter(function(i){return i.status!=='unanswered';}).length;
    return {label:td.label, n:n, done:done, correct:c};
  });
}
function renderRecord(){
  showChrome(false);
  var tabLabel=function(id){ var t=TAB_DEFS.find(function(x){return x.id===id;}); return t?t.label:id; };
  var h='<div class="rec-card"><h2>'+esc(student.name)+'’s record</h2><p class="rec-empty" style="margin:0 0 12px;">Roll '+esc(student.roll)+' · CMGGA 2026 · Mock Paper 1</p>';
  ['learning','quiz'].forEach(function(m){
    var sum=tabSummary(m);
    h+='<h3>'+(m==='learning'?'📘 Learning Sheet':'📝 Quiz Mode')+'</h3>';
    if(!sum){ h+='<p class="rec-empty">Not started yet.</p>'; return; }
    h+='<div class="rec-table-wrap"><table class="rec-table"><thead><tr><th>Section</th><th>Progress</th><th>Correct first time</th></tr></thead><tbody>';
    sum.forEach(function(r){ var pct=Math.round(r.done/r.n*100);
      h+='<tr><td>'+r.label+'</td><td><span class="rec-bar"><i style="width:'+pct+'%"></i></span>'+r.done+' / '+r.n+'</td><td>'+(m==='quiz'?'—':r.correct+' / '+r.n)+'</td></tr>'; });
    h+='</tbody></table></div>';
  });
  h+='</div><div class="rec-card"><h3>Finished sections</h3>';
  if(!records.length){ h+='<p class="rec-empty">No sections finished yet. Each time you finish a tab, your score is recorded here.</p>'; }
  else {
    h+='<div class="rec-table-wrap"><table class="rec-table"><thead><tr><th>When</th><th>Mode</th><th>Section</th><th>Score</th></tr></thead><tbody>';
    records.forEach(function(r){ h+='<tr><td>'+fmtDate(r.at)+'</td><td>'+(r.mode==='quiz'?'Quiz':'Learning')+'</td><td>'+tabLabel(r.tab)+'</td><td>'+r.correct+' / '+r.total+(r.mode==='learning'?' <span class="rec-empty">('+r.revealed+' revealed, '+r.skipped+' skipped)</span>':'')+'</td></tr>'; });
    h+='</tbody></table></div>';
  }
  h+='</div><button class="btn btn-primary" id="btnBack">'+(MODE?'Back to practice':'Choose a mode')+'</button>';
  document.getElementById('wrap').innerHTML=h;
  document.getElementById('btnBack').addEventListener('click', function(){
    if(MODE){ showChrome(true); buildTabbar(); renderSlide(); } else renderModePicker();
  });
  window.scrollTo({top:0});
}

/* ================= tab bar ================= */
function buildTabbar(){
  var el=document.getElementById('tabbar');
  el.innerHTML = '<button class="tab-btn'+(activeTab==='theory'?' active':'')+'" data-tab="theory">Theory<span class="tab-count">notes</span></button>' + TAB_DEFS.map(function(t){
    return '<button class="tab-btn'+(t.id===activeTab?' active':'')+'" data-tab="'+t.id+'">'+t.label+'<span class="tab-count">'+SLIDES[t.id].length+'</span></button>';
  }).join('') + '<button class="tab-btn'+(activeTab==='report'?' active':'')+'" data-tab="report">📊 Report<span class="tab-count">pie</span></button>';
  el.querySelectorAll('.tab-btn').forEach(function(btn){
    btn.addEventListener('click', function(){ activeTab=btn.dataset.tab; buildTabbar(); renderSlide(); window.scrollTo({top:0,behavior:'smooth'}); });
  });
}

/* ================= rendering ================= */
function canProceed(item){ return item.status==='correct'||item.status==='revealed'||item.status==='skipped'; }

function renderSlide(){
  if(!state.tabs[activeTab]){ activeTab=TAB_DEFS[0].id; }
  var ts = state.tabs[activeTab];
  var slides = SLIDES[activeTab];
  if(ts.idx>=slides.length||ts.idx<0) ts.idx=0;
  var idx = ts.idx;
  var slide = slides[idx];
  var item = ts.items[idx];

  var tdef=TAB_DEFS.find(function(t){return t.id===activeTab;});
  document.getElementById('spLabel').textContent = tdef.label+' · Question '+(idx+1)+' of '+slides.length;
  document.getElementById('secSub').textContent = tdef.label+' — '+tdef.sub;
  document.getElementById('spFill').style.width = Math.round(((idx)/(Math.max(slides.length-1,1)))*100)+'%';

  var h='<div class="qcard">';
  if(slide.kind==='mcq' || slide.kind==='ar'){
    h += renderChoiceBody(slide, item, idx);
  } else {
    h += renderBlankBody(slide, item, idx);
  }
  h += '<div class="feedback" id="feedbackBox"></div>';
  if(MODE==='learning' && (item.status==='correct'||item.status==='revealed')) h += solutionHTML(slide);
  h += '</div>';

  document.getElementById('wrap').innerHTML = h;
  wireSlideEvents(slide, item, idx);
  restoreFeedback(item);
  renderNavbar(item);
  updateFab();
  saveState();
}

function solutionHTML(slide){
  if(!slide.sol) return '';
  return '<div class="solution"><div class="sol-h">Solution</div>'+slide.sol.split('\n').map(function(l){ return '<div class="sol-line">'+fr(esc(l))+'</div>'; }).join('')+'</div>';
}
var LETTERS=['a','b','c','d','e','f'];
function chosenHTML(slide,item){
  var opts = slide.kind==='mcq' ? slide.opts : AR_OPTIONS;
  if(item.choice===undefined) return '';
  var ok=item.choice===slide.correct;
  var h='<div class="chosen '+(ok?'ok':'bad')+'"><b>Your answer:</b> ('+LETTERS[item.choice]+') '+fr(esc(opts[item.choice]))+(ok?' ✓':' ✗')+'</div>';
  if(!ok) h+='<div class="chosen ok"><b>Correct answer:</b> ('+LETTERS[slide.correct]+') '+fr(esc(opts[slide.correct]))+'</div>';
  return h;
}
function renderChoiceBody(slide, item, idx){
  var h='<div class="qhead"><div class="qnum">'+(idx+1)+'</div>';
  if(slide.kind==='mcq'){
    h += '<div class="qtext">'+fr(esc(slide.text))+(slide.tag?'<span class="qtag">'+esc(slide.tag)+'</span>':'')+'</div>';
  } else {
    h += '<div class="qtext"><span class="qtag" style="margin-left:0;margin-right:6px;">A / R</span>Assertion (A): '+fr(esc(slide.a))+'<br>Reason (R): '+fr(esc(slide.r))+(slide.tag?'<span class="qtag">'+esc(slide.tag)+'</span>':'')+'</div>';
  }
  h += '</div>';
  if(slide.fig) h += '<div class="fig">'+slide.fig+'</div>';
  var opts = slide.kind==='mcq' ? slide.opts : AR_OPTIONS;
  if(MODE==='quiz') h += '<div class="quiz-hint">Quiz mode — pick an option. The correct answer is revealed once you finish this tab.</div>';
  var locked = MODE==='learning' && (item.status==='correct' || item.status==='revealed');
  h += '<div class="options">';
  opts.forEach(function(opt,i){
    var cls='opt';
    if(locked){
      if(i===slide.correct) cls+=' is-correct';
      else if(item.choice===i) cls+=' is-wrong';
      cls+=' locked';
    }
    if(item.choice===i) cls+=' is-chosen';
    h += '<label class="'+cls+'"><input type="radio" name="choice" value="'+i+'" '+(item.choice===i?'checked':'')+' '+(locked?'disabled':'')+'> <span class="opt-l">('+LETTERS[i]+')</span> <span class="opt-t">'+fr(esc(opt))+'</span>'+(item.choice===i?'<span class="opt-tag">'+(locked?(i===slide.correct?'Your answer ✓':'Your answer ✗'):'Selected')+'</span>':'')+'</label>';
  });
  h += '</div>';
  if(locked) h += chosenHTML(slide,item);
  return h;
}

function renderBlankBody(slide, item, idx){
  var h='<div class="qhead"><div class="qnum">'+(idx+1)+'</div><div class="qtext">';
  if(slide.kind==='case'){ h += '<b>'+esc(slide.title)+'.</b> '+esc(slide.body); }
  else { var pp=fr(esc(slide.p)).split('\n'); h += pp[0]+pp.slice(1).map(function(x){return '<span class="datline">'+x+'</span>';}).join(''); }
  h += (slide.tag?'<span class="qtag">'+esc(slide.tag)+'</span>':'')+'</div>';
  if(slide.marks) h += '<div class="marks-pill">'+slide.marks+'</div>';
  h += '</div>';
  if(slide.fig) h += '<div class="fig">'+slide.fig+'</div>';

  var total = slide.flat.length;
  var hasExpr = slide.flat.some(function(s){ return s.expr===true; });
  var hasFrac = slide.flat.some(function(s){ return ['fv','fe','fl','fm','fi','flist'].indexOf(s.expr)>=0; });
  var blankCount=0; slide.flat.forEach(function(s){ blankCount+=Object.keys(s.a).length; });

  if(MODE==='quiz'){
    h += '<div class="step-badge">'+blankCount+' blank'+(blankCount===1?'':'s')+' in this question</div>';
    h += '<div class="quiz-hint">Quiz mode — fill in what you can. Correct answers are revealed once you finish this tab.</div>';
    if(hasFrac) h += '<div class="quiz-hint">Type fractions like <b>3/4</b> and mixed numbers like <b>2 3/4</b> (whole number, space, fraction).</div>';
    if(hasExpr) h += '<div class="quiz-hint">Type answers like <b>2x-5</b>, <b>x^2-4</b> or <b>3+2i</b>. Use ^ for powers, | | for absolute value and pi for π. Any equivalent form is accepted.</div>';
    h += '<div class="steps">';
    for(var qi=0; qi<total; qi++){
      var qstep = slide.flat[qi];
      var qss = item.stepStates[qi];
      if(qstep.partLabel) h += '<div class="subpart-label">'+esc(qstep.partLabel)+'</div>';
      if(qstep.orDivider) h += '<div class="or-divider">OR</div>';
      var qline = fr(qstep.t);
      Object.keys(qstep.a).forEach(function(bkey){
        var val = qss.inputs[bkey]||'';
        var inp='<input class="blank-input'+(['fv','fe','fl','fm','fi','dec'].indexOf(qstep.expr)>=0?' fr':(qstep.expr==='flist'||qstep.expr==='dlist'||qstep.expr==='glist')?' wide':qstep.expr===true?' expr':(qstep.expr==='words'||qstep.expr==='list'||qstep.expr==='expanded'||qstep.expr==='set'||qstep.expr==='primes'||qstep.expr==='trans'||qstep.expr==='rot'?' wide':''))+'" data-step="'+qi+'" data-bkey="'+bkey+'" value="'+esc(val)+'">';
        qline = qline.replace('__'+bkey+'__', inp);
      });
      if(qstep.fig) h += '<div class="fig">'+qstep.fig+'</div>';
      h += '<div class="step-line">'+qline+'</div>';
    }
    h += '</div>';
    return h;
  }

  if(hasFrac) h += '<div class="quiz-hint">Type fractions like <b>3/4</b> and mixed numbers like <b>2 3/4</b> (whole number, space, fraction).</div>';
  if(hasExpr) h += '<div class="quiz-hint">Type answers like <b>2x-5</b>, <b>x^2-4</b> or <b>3+2i</b>. Use ^ for powers, | | for absolute value and pi for π. Any equivalent form is accepted.</div>';
  var locked = item.status==='correct' || item.status==='revealed';
  var upto = locked ? total-1 : item.curStep;
  h += '<div class="step-badge">Step '+(Math.min(item.curStep,total-1)+1)+' of '+total+'</div>';
  h += '<div class="steps">';
  for(var i=0;i<=upto;i++){
    var step = slide.flat[i];
    var ss = item.stepStates[i];
    if(step.partLabel) h += '<div class="subpart-label">'+esc(step.partLabel)+'</div>';
    if(step.orDivider) h += '<div class="or-divider">OR</div>';
    var resolved = ss.status==='correct' || ss.status==='revealed';
    var line = fr(step.t);
    Object.keys(step.a).forEach(function(bkey){
      var fs = ss.inputs['fs_'+bkey];
      var cls = fs==='correct'?'is-correct':(fs==='wrong'?'is-wrong':'');
      var val = ss.inputs[bkey]||'';
      var dis = resolved ? 'disabled':'';
      var inp='<input class="blank-input '+cls+(['fv','fe','fl','fm','fi','dec'].indexOf(step.expr)>=0?' fr':(step.expr==='flist'||step.expr==='dlist'||step.expr==='glist')?' wide':step.expr===true?' expr':(step.expr==='words'||step.expr==='list'||step.expr==='expanded'||step.expr==='set'||step.expr==='primes'||step.expr==='trans'||step.expr==='rot'?' wide':''))+'" data-step="'+i+'" data-bkey="'+bkey+'" value="'+esc(val)+'" '+dis+'>';
      line = line.replace('__'+bkey+'__', inp);
    });
    if(step.fig) h += '<div class="fig">'+step.fig+'</div>';
    h += '<div class="step-line'+(resolved?' resolved':'')+'">'+line+'</div>';
    if(ss.status==='revealed'){
      var reveals=[];
      Object.keys(step.a).forEach(function(bkey){ reveals.push(bkey+' = '+esc(step.a[bkey])); });
      h += '<div class="reveal-note">correct: '+reveals.join(', ')+'</div>';
    }
  }
  h += '</div>';
  return h;
}

var __flash=null;
function restoreFeedback(item){
  var fb=document.getElementById('feedbackBox'); if(!fb) return;
  if(__flash){ fb.className='feedback show '+__flash.c; fb.innerHTML=__flash.h; __flash=null; return; }
  if(MODE==='quiz'){ fb.className='feedback'; fb.innerHTML=''; return; }
  if(item.status==='correct'){ fb.className='feedback show ok'; fb.innerHTML='<b>All done — correct!</b>'; }
  else if(item.status==='revealed'){ fb.className='feedback show reveal'; fb.innerHTML='<b>Answer revealed above.</b> Move on whenever you’re ready.'; }
  else if(item.status==='skipped'){ fb.className='feedback show retry'; fb.innerHTML='Skipped — you can answer it now and press <b>Check</b>, or come back later from the Question Palette.'; }
  else { fb.className='feedback'; fb.innerHTML=''; }
}

function slideIsAnswered(slide,item){
  if(slide.kind==='mcq'||slide.kind==='ar') return item.choice!==undefined;
  return item.stepStates.some(function(ss){ return Object.keys(ss.inputs).some(function(k){ return k.indexOf('fs_')!==0 && ss.inputs[k] && String(ss.inputs[k]).trim()!==''; }); });
}
function renderNavbar(item){
  var ts = state.tabs[activeTab];
  var slides = SLIDES[activeTab];
  var slide = slides[ts.idx];
  var isLast = ts.idx === slides.length-1;
  var h='';
  h += '<button class="btn" id="btnPrev" '+(ts.idx===0?'disabled':'')+'>&larr; Previous</button>';

  if(MODE==='quiz'){
    h += '<button class="btn" id="btnSkip">Skip</button>';
    h += '<span class="spacer"></span>';
    h += '<button class="btn btn-primary" id="btnNext">'+(isLast?'Finish':'Next →')+'</button>';
  } else {
    h += '<button class="btn" id="btnSkip" '+(item.status!=='unanswered'?'disabled':'')+'>Skip</button>';
    h += '<span class="spacer"></span>';
    h += '<button class="btn btn-primary" id="btnCheck" '+((item.status!=='unanswered'&&item.status!=='skipped')?'disabled':'')+'>Check</button>';
    h += '<button class="btn btn-primary" id="btnNext" '+(canProceed(item)?'':'disabled')+'>'+(isLast?'Finish':'Next →')+'</button>';
  }
  document.getElementById('navbarInner').innerHTML = h;

  document.getElementById('btnPrev').addEventListener('click', function(){ if(ts.idx>0){ ts.idx--; renderSlide(); } });

  if(MODE==='quiz'){
    document.getElementById('btnSkip').addEventListener('click', function(){
      item.status='skipped';
      advanceQuiz(ts, slides);
    });
    document.getElementById('btnNext').addEventListener('click', function(){
      item.status = slideIsAnswered(slide,item) ? 'answered' : 'unanswered';
      advanceQuiz(ts, slides);
    });
  } else {
    document.getElementById('btnSkip').addEventListener('click', function(){
      if(item.status==='unanswered'){ item.status='skipped'; renderSlide(); }
    });
    document.getElementById('btnNext').addEventListener('click', function(){
      if(!canProceed(item)) return;
      if(ts.idx < slides.length-1){ ts.idx++; ts.maxReached=Math.max(ts.maxReached, ts.idx); renderSlide(); }
      else { renderFinished(); }
    });
    document.getElementById('btnCheck').addEventListener('click', function(){ handleCheck(); });
  }
}
function advanceQuiz(ts, slides){
  if(ts.idx < slides.length-1){ ts.idx++; ts.maxReached=Math.max(ts.maxReached, ts.idx); renderSlide(); }
  else { renderFinished(); }
}

function wireSlideEvents(slide, item, idx){
  document.querySelectorAll('input[type="radio"][name="choice"]').forEach(function(r){
    r.addEventListener('change', function(){ item.choice=parseInt(r.value,10); saveState();
      document.querySelectorAll('.opt').forEach(function(l){ l.classList.remove('is-chosen'); var t=l.querySelector('.opt-tag'); if(t) t.remove(); });
      var lab=r.closest('.opt'); lab.classList.add('is-chosen'); var tg=document.createElement('span'); tg.className='opt-tag'; tg.textContent='Selected'; lab.appendChild(tg); });
  });
  document.querySelectorAll('.blank-input').forEach(function(inp){
    inp.addEventListener('input', function(){
      var si=parseInt(inp.dataset.step,10), bk=inp.dataset.bkey;
      item.stepStates[si].inputs[bk]=inp.value;
      saveState();
    });
  });
}

function handleCheck(){
  var ts = state.tabs[activeTab];
  var slide = SLIDES[activeTab][ts.idx];
  var item = ts.items[ts.idx];
  if(item.status==='skipped') item.status='unanswered';
  var fb = document.getElementById('feedbackBox');

  if(slide.kind==='mcq' || slide.kind==='ar'){
    if(item.choice===undefined){ fb.className='feedback show err'; fb.innerHTML='Please choose an option first.'; return; }
    var ok = item.choice===slide.correct;
    if(ok){
      item.status='correct'; playSuccess();
      fb.className='feedback show ok'; fb.innerHTML='<b>Correct!</b>';
    } else {
      item.attempts=(item.attempts||0)+1;
      if(item.attempts>=2){ item.status='revealed'; playReveal(); }
      else { playWrong(); fb.className='feedback show retry'; fb.innerHTML='<b>Not quite — try again</b> (attempt 1 of 2) <span class="attempts-dots"><span class="used"></span><span></span></span>'; __flash={c:'retry',h:'<b>Not quite — try again</b> (attempt 1 of 2) <span class="attempts-dots"><span class="used"></span><span></span></span>'}; }
    }
    renderSlide();
    return;
  }

  // blank / case
  var step = slide.flat[item.curStep];
  var ss = item.stepStates[item.curStep];
  var blanks = Object.keys(step.a);
  var missing = blanks.some(function(k){ return !ss.inputs[k] || String(ss.inputs[k]).trim()===''; });
  if(missing){ fb.className='feedback show err'; fb.innerHTML='Fill in every blank in this step before checking.'; return; }

  var allGood=true;
  blanks.forEach(function(k){
    var good=answerMatches(ss.inputs[k], step.a[k], step.accept, step.expr);
    ss.inputs['fs_'+k]=good?'correct':'wrong';
    if(!good) allGood=false;
  });

  if(allGood){
    ss.status='correct'; playSuccess();
    advanceStepOrFinish(item, slide);
  } else {
    ss.attempts=(ss.attempts||0)+1;
    if(ss.attempts>=2){
      ss.status='revealed'; playReveal();
      advanceStepOrFinish(item, slide);
    } else {
      playWrong();
      fb.className='feedback show retry';
      fb.innerHTML='<b>Not quite — try again</b> (attempt 1 of 2) <span class="attempts-dots"><span class="used"></span><span></span></span>'; __flash={c:'retry',h:'<b>Not quite — try again</b> (attempt 1 of 2) <span class="attempts-dots"><span class="used"></span><span></span></span>'};
      renderSlide();
      return;
    }
  }
  renderSlide();
}

function advanceStepOrFinish(item, slide){
  var total = slide.flat.length;
  var hasExpr = slide.flat.some(function(s){ return s.expr===true; });
  var hasFrac = slide.flat.some(function(s){ return ['fv','fe','fl','fm','fi','flist'].indexOf(s.expr)>=0; });
  if(item.curStep < total-1){
    item.curStep++;
  } else {
    var anyRevealed = item.stepStates.some(function(ss){ return ss.status==='revealed'; });
    item.status = anyRevealed ? 'revealed' : 'correct';
  }
}

/* ================= palette ================= */
var overlay=document.getElementById('overlay');
function statusOf(tabId,i){
  var ts=state.tabs[tabId];
  if(i>ts.maxReached) return 'locked';
  if(i===ts.idx) return 'current';
  return ts.items[i].status==='unanswered' ? 'locked' : ts.items[i].status;
}
function buildPalette(){
  var slides=SLIDES[activeTab];
  document.getElementById('paletteTitle').textContent = TAB_DEFS.find(function(t){return t.id===activeTab;}).label+' · Question palette';
  var body=document.getElementById('paletteBody');
  var html='';
  for(var i=0;i<slides.length;i++){
    html += '<div class="chip" data-status="'+statusOf(activeTab,i)+'" data-idx="'+i+'">'+(i+1)+'</div>';
  }
  body.innerHTML = html;
  body.querySelectorAll('.chip').forEach(function(chip){
    chip.addEventListener('click', function(){
      var i=parseInt(chip.dataset.idx,10);
      var ts=state.tabs[activeTab];
      if(i>ts.maxReached){ showToast('Finish the earlier questions to unlock this one.'); return; }
      ts.idx=i; closePalette(); renderSlide();
    });
  });
}
function openPalette(){ buildPalette(); overlay.classList.add('show'); }
function closePalette(){ overlay.classList.remove('show'); }
var toastTimer;
function showToast(msg){
  var t=document.getElementById('toast'); t.textContent=msg; t.classList.add('show');
  clearTimeout(toastTimer); toastTimer=setTimeout(function(){ t.classList.remove('show'); },2200);
}
document.getElementById('paletteFab').addEventListener('click', openPalette);
document.getElementById('paletteClose').addEventListener('click', closePalette);
overlay.addEventListener('click', function(e){ if(e.target===overlay) closePalette(); });

function updateFab(){
  var slides=SLIDES[activeTab];
  var done=state.tabs[activeTab].items.filter(function(it){ return it.status==='correct'||it.status==='revealed'||it.status==='skipped'; }).length;
  document.getElementById('fabBadge').textContent = done+'/'+slides.length;
}

/* ================= overall progress + finish ================= */
function updateChapterProgress(){
  var total=0, done=0;
  TAB_DEFS.forEach(function(td){
    state.tabs[td.id].items.forEach(function(it){
      total++;
      if(it.status==='correct'||it.status==='revealed'||it.status==='skipped') done++;
    });
  });
  var pct = total>0 ? Math.round((done/total)*100) : 0;
  document.getElementById('cpFill').style.width=pct+'%';
  document.getElementById('cpLabel').textContent=pct+'% complete';
}
function isSlideCorrect(tabId,i){
  var slide=SLIDES[tabId][i], item=state.tabs[tabId].items[i];
  if(slide.kind==='mcq'||slide.kind==='ar') return item.choice===slide.correct;
  return slide.flat.every(function(step,si){
    var ss=item.stepStates[si];
    return Object.keys(step.a).every(function(k){ return answerMatches(ss.inputs[k], step.a[k], step.accept, step.expr); });
  });
}
function isSlideAttempted(tabId,i){
  var slide=SLIDES[tabId][i], item=state.tabs[tabId].items[i];
  if(slide.kind==='mcq'||slide.kind==='ar') return item.choice!==undefined;
  return slide.flat.some(function(step,si){
    var ss=item.stepStates[si];
    return Object.keys(step.a).some(function(k){ return ss.inputs[k] && String(ss.inputs[k]).trim()!==''; });
  });
}
function slideLabel(slide){
  var t = slide.kind==='case' ? slide.title : (slide.kind==='ar' ? slide.a : (slide.p||slide.text||''));
  t = String(t);
  return t.length>90 ? t.slice(0,90)+'…' : t;
}
function slideAnswerText(slide, item, correctSide){
  if(slide.kind==='mcq'||slide.kind==='ar'){
    var opts = slide.kind==='mcq' ? slide.opts : AR_OPTIONS;
    if(correctSide) return '('+LETTERS[slide.correct]+') '+opts[slide.correct];
    return item.choice!==undefined ? '('+LETTERS[item.choice]+') '+opts[item.choice] : '— not attempted —';
  }
  return slide.flat.map(function(step,si){
    var ss=item.stepStates[si];
    return Object.keys(step.a).map(function(k){
      return correctSide ? step.a[k] : (ss.inputs[k] || '—');
    }).join(', ');
  }).join('  |  ');
}

function renderFinished(){
  if(MODE==='quiz'){ renderQuizResults(); return; }
  var ts=state.tabs[activeTab];
  var correct=ts.items.filter(function(i){return i.status==='correct';}).length;
  var revealed=ts.items.filter(function(i){return i.status==='revealed';}).length;
  var skipped=ts.items.filter(function(i){return i.status==='skipped';}).length;
  var h='<div class="qcard done-card"><div class="big">✨</div><h2>Tab complete</h2>';
  h+='<p style="color:var(--ink-soft);font-size:14px;">You worked through all '+ts.items.length+' questions in this tab.</p>';
  if(!ts.recorded){ ts.recorded=true; addRecord('learning', activeTab, correct, revealed, skipped, ts.items.length); }
  h+='<div class="score-pills">'+
     '<span class="score-pill" style="background:var(--success-soft);color:var(--success);">'+correct+' correct</span>'+
     '<span class="score-pill" style="background:var(--danger-soft);color:var(--danger);">'+revealed+' revealed</span>'+
     '<span class="score-pill" style="background:var(--gold-soft);color:var(--retry-text);">'+skipped+' skipped</span></div>'+
     '<button class="btn btn-primary" id="btnReview">Review from question 1</button></div>';
  document.getElementById('wrap').innerHTML=h;
  document.getElementById('navbarInner').innerHTML='';
  document.getElementById('btnReview').addEventListener('click', function(){ ts.idx=0; ts.recorded=false; renderSlide(); });
  updateChapterProgress(); saveState();
}

function renderQuizResults(){
  var ts=state.tabs[activeTab];
  var slides=SLIDES[activeTab];
  var correctCount=0, attemptedCount=0;
  var rowsHtml = slides.map(function(slide,i){
    var item=ts.items[i];
    var ok=isSlideCorrect(activeTab,i);
    var att=isSlideAttempted(activeTab,i);
    if(ok) correctCount++;
    if(att) attemptedCount++;
    var tagCls = ok?'ok':(att?'bad':'na');
    var tagText = ok?'Correct':(att?'Incorrect':'Not attempted');
    var row='<div class="review-row">';
    row+='<span class="review-tag '+tagCls+'">Q'+(i+1)+' · '+tagText+'</span>';
    row+='<div class="review-q">'+fr(esc(slideLabel(slide)))+'</div>';
    row+='<div class="review-ans"><b>Your answer:</b> '+fr(esc(slideAnswerText(slide,item,false)))+'</div>';
    if(!ok) row+='<div class="review-ans" style="color:var(--success);"><b>Correct answer:</b> '+fr(esc(slideAnswerText(slide,item,true)))+'</div>';
    if(slide.sol) row+='<details class="rev-sol"><summary>Show solution</summary>'+solutionHTML(slide)+'</details>';
    row+='</div>';
    return row;
  }).join('');

  addRecord('quiz', activeTab, correctCount, 0, 0, slides.length);
  var h='<div class="qcard done-card" style="text-align:left;">';
  h+='<div style="text-align:center;"><div class="big">🏁</div><h2>Quiz complete</h2>';
  h+='<p style="color:var(--ink-soft);font-size:14px;">'+correctCount+' / '+slides.length+' correct · '+attemptedCount+' attempted</p></div>';
  h+='<div style="margin-top:16px;">'+rowsHtml+'</div>';
  h+='<div style="text-align:center;margin-top:6px;"><button class="btn btn-primary" id="btnReview">Review from question 1</button></div>';
  h+='</div>';
  document.getElementById('wrap').innerHTML=h;
  document.getElementById('navbarInner').innerHTML='';
  document.getElementById('btnReview').addEventListener('click', function(){ ts.idx=0; renderSlide(); });
  playSuccess();
  updateChapterProgress(); saveState();
}

/* ================= mode picker ================= */
function updateModePill(){
  var btn=document.getElementById('modePill');
  if(!btn) return;
  btn.textContent = MODE==='quiz' ? '📝 Quiz Mode · switch' : '📘 Learning Sheet · switch';
}
function showChrome(show){
  document.querySelector('.tabbar').style.display = show?'':'none';
  document.querySelector('.slide-progress').style.display = show?'':'none';
  document.querySelector('.navbar').style.display = show?'':'none';
  document.getElementById('paletteFab').style.display = show?'':'none';
}
function renderModePicker(){
  showChrome(false);
  var wrap=document.getElementById('wrap');
  wrap.innerHTML =
    '<div class="mode-pick">'+
      '<div class="mode-card" data-pick="learning"><div class="mode-icon">📘</div><h3>Learning Sheet</h3>'+
      '<p>Work through each question step by step with instant feedback — two tries, then the correct value is revealed right there so you can keep moving.</p></div>'+
      '<div class="mode-card" data-pick="quiz"><div class="mode-icon">📝</div><h3>Quiz Mode</h3>'+
      '<p>Attempt every question with no hints along the way. Your score and the full answer key are shown together once you finish the tab — just like the real exam.</p></div>'+
    '</div>';
  wrap.querySelectorAll('[data-pick]').forEach(function(card){
    card.addEventListener('click', function(){
      setMode(card.dataset.pick); activeTab='theory';
      document.getElementById('modePill').hidden=false;
      updateModePill();
      showChrome(true);
      buildTabbar();
      renderSlide();
    });
  });
}
document.getElementById('modePill').addEventListener('click', function(){
  if(!appState.mode){ return; }
  setMode(appState.mode==='quiz' ? 'learning' : 'quiz');
  updateModePill();
  showChrome(true);
  buildTabbar();
  renderSlide();
});

/* ================= boot ================= */
var _origRenderSlide = renderSlide;
renderSlide = function(){ _origRenderSlide(); updateChapterProgress(); updateModePill(); };


/* ================= theory tab ================= */
function renderTheory(){
  var wrap=document.getElementById('wrap');
  wrap.innerHTML='<div class="theory">'+fr(THEORY)+'</div>';
  document.querySelector('.slide-progress').style.display='none';
  document.querySelector('.navbar').style.display='none';
  document.getElementById('paletteFab').style.display='none';
  document.getElementById('secSub').textContent='Theory — notes, key ideas and worked examples';
  wrap.querySelectorAll('[data-go]').forEach(function(b){ b.addEventListener('click',function(){ activeTab=b.dataset.go; buildTabbar(); renderSlide(); window.scrollTo({top:0,behavior:'smooth'}); }); });
  wrap.querySelectorAll('[data-jump]').forEach(function(b){ b.addEventListener('click',function(){ var t=document.getElementById(b.dataset.jump); if(t) t.scrollIntoView({behavior:'smooth',block:'start'}); }); });
}
var _rsTheory = renderSlide;
renderSlide = function(){
  if(activeTab==='theory'){ renderTheory(); buildTabbar(); updateChapterProgress(); updateModePill(); saveState(); return; }
  document.querySelector('.slide-progress').style.display='';
  document.querySelector('.navbar').style.display='';
  document.getElementById('paletteFab').style.display='';
  _rsTheory();
};


/* ================= MYP criterion report ================= */
var CRIT_COL={A:'var(--accent-text)',B:'var(--gold)',C:'#8A6FC4',D:'#2F9AA0'};
function critStats(){
  return REPORT.map(function(r){
    var tabId=r[0], slides=SLIDES[tabId], ts=state&&state.tabs[tabId];
    var c=0,w=0,n=0;
    slides.forEach(function(sl,i){
      if(!ts||!ts.items[i]){ n++; return; }
      var it=ts.items[i];
      if(MODE==='learning'){
        if(it.status==='correct') c++; else if(it.status==='revealed') w++; else n++;
      } else {
        if(isSlideCorrect(tabId,i)) c++; else if(isSlideAttempted(tabId,i)) w++; else n++;
      }
    });
    var tot=slides.length, pct=tot?Math.round(c/tot*100):0;
    var lvl=Math.round(c/Math.max(tot,1)*8);
    return {tab:tabId,letter:r[1],name:r[2],c:c,w:w,n:n,tot:tot,pct:pct,lvl:lvl};
  });
}
function arcPath(cx,cy,r,a0,a1){
  if(a1-a0>=Math.PI*2-1e-6){ return 'M'+(cx-r)+','+cy+' a'+r+','+r+' 0 1,0 '+(2*r)+',0 a'+r+','+r+' 0 1,0 '+(-2*r)+',0 Z'; }
  var x0=cx+r*Math.sin(a0), y0=cy-r*Math.cos(a0), x1=cx+r*Math.sin(a1), y1=cy-r*Math.cos(a1);
  return 'M'+cx+','+cy+' L'+x0.toFixed(2)+','+y0.toFixed(2)+' A'+r+','+r+' 0 '+((a1-a0)>Math.PI?1:0)+',1 '+x1.toFixed(2)+','+y1.toFixed(2)+' Z';
}
function pieSVG(parts,size,hole,center,sub){
  var tot=parts.reduce(function(s,p){return s+p.v;},0), cx=size/2, cy=size/2, r=size/2-4, a=0, h='';
  if(!tot){ h+='<circle cx="'+cx+'" cy="'+cy+'" r="'+r+'" style="fill:var(--paper-2);stroke:var(--rule)"/>'; }
  parts.forEach(function(p){ if(!p.v) return; var b=a+p.v/tot*Math.PI*2; h+='<path d="'+arcPath(cx,cy,r,a,b)+'" style="fill:'+p.col+';stroke:var(--card);stroke-width:2"><title>'+esc(p.label)+': '+p.v+'</title></path>'; a=b; });
  if(hole) h+='<circle cx="'+cx+'" cy="'+cy+'" r="'+(r*hole)+'" style="fill:var(--card)"/>';
  if(center) h+='<text x="'+cx+'" y="'+(cy-(sub?4:0))+'" text-anchor="middle" dominant-baseline="middle" style="fill:var(--ink);font:700 '+(size>150?22:15)+'px Fraunces,serif">'+center+'</text>';
  if(sub) h+='<text x="'+cx+'" y="'+(cy+16)+'" text-anchor="middle" style="fill:var(--ink-soft);font:600 11px \'Source Sans 3\',sans-serif">'+sub+'</text>';
  return '<svg viewBox="0 0 '+size+' '+size+'" width="'+size+'" height="'+size+'" role="img">'+h+'</svg>';
}
function band(l){ return l===0?'0':(l<=2?'1–2':(l<=4?'3–4':(l<=6?'5–6':'7–8'))); }
function renderReport(){
  var st=critStats(), totC=0, totQ=0;
  st.forEach(function(s){ totC+=s.c; totQ+=s.tot; });
  var h='<div class="theory">';
  h+='<section class="note"><h2>Chapter test report</h2><p class="lt">'+(MODE==='quiz'?'<b>Quiz mode</b> results: answers are marked when you finish each test tab.':'<b>Learning mode</b> results: a question counts as correct only if you got it without the answer being revealed. Switch to Quiz mode for an exam-style score.')+'</p>';
  h+='<div class="rep-top"><div class="rep-pie">'+pieSVG(st.map(function(s){return {v:s.c,col:CRIT_COL[s.letter],label:'Criterion '+s.letter};}),200,0.55,totC+'/'+totQ,'correct')+'</div>';
  h+='<div class="rep-legend"><div class="rep-cap">Marks earned, by criterion</div>'+st.map(function(s){ return '<div class="rep-li"><span class="sw" style="background:'+CRIT_COL[s.letter]+'"></span><b>'+s.letter+'</b>&nbsp;'+esc(s.name)+'<span class="rep-n">'+s.c+' / '+s.tot+'</span></div>'; }).join('')+'</div></div></section>';
  h+='<div class="rep-grid">'+st.map(function(s){
    return '<div class="rep-card"><div class="rep-h"><span class="crit" style="background:'+CRIT_COL[s.letter]+'">'+s.letter+'</span>'+esc(s.name)+'</div>'+
      '<div class="rep-row">'+pieSVG([{v:s.c,col:'var(--success)',label:'Correct'},{v:s.w,col:'var(--danger)',label:'Incorrect'},{v:s.n,col:'var(--locked)',label:'Not attempted'}],120,0.5,s.pct+'%')+
      '<div class="rep-stats"><div><span class="sw" style="background:var(--success)"></span>Correct <b>'+s.c+'</b></div><div><span class="sw" style="background:var(--danger)"></span>Incorrect <b>'+s.w+'</b></div><div><span class="sw" style="background:var(--locked)"></span>Not attempted <b>'+s.n+'</b></div>'+
      '<div class="rep-lvl">Indicative level <b>'+s.lvl+'</b> / 8 <span>(band '+band(s.lvl)+')</span></div></div></div>'+
      '<button class="hub-btn" data-go="'+s.tab+'">Open Test '+s.letter+' →</button></div>';
  }).join('')+'</div>';
  h+='<p class="rep-note">Indicative level = fraction of questions correct × 8, rounded. It is a practice guide only; your teacher awards the real MYP criterion levels.</p></div>';
  var wrap=document.getElementById('wrap'); wrap.innerHTML=h;
  document.querySelector('.slide-progress').style.display='none';
  document.querySelector('.navbar').style.display='none';
  document.getElementById('paletteFab').style.display='none';
  document.getElementById('secSub').textContent='Report — chapter test results by MYP criterion';
  wrap.querySelectorAll('[data-go]').forEach(function(b){ b.addEventListener('click',function(){ activeTab=b.dataset.go; buildTabbar(); renderSlide(); window.scrollTo({top:0,behavior:'smooth'}); }); });
}
var _rsReport = renderSlide;
renderSlide = function(){
  if(activeTab==='report'){ renderReport(); buildTabbar(); updateChapterProgress(); updateModePill(); saveState(); return; }
  _rsReport();
};


/* ================= skipped-question return ================= */
function firstSkippedIdx(ts){
  for(var i=0;i<ts.items.length;i++){
    var it=ts.items[i];
    if(MODE==='quiz'){ if(!isSlideAttempted(activeTab,i)) return i; }
    else if(it.status==='skipped'||it.status==='unanswered') return i;
  }
  return -1;
}
function skippedList(ts){
  var out=[]; for(var i=0;i<ts.items.length;i++){ var it=ts.items[i];
    if(MODE==='quiz' ? !isSlideAttempted(activeTab,i) : (it.status==='skipped'||it.status==='unanswered')) out.push(i); }
  return out;
}
function renderSkipGate(ts){
  var list=skippedList(ts);
  var h='<div class="qcard done-card"><div class="big">⏭️</div><h2>You skipped '+list.length+' question'+(list.length>1?'s':'')+'</h2>'+
    '<p style="color:var(--ink-soft);font-size:14px;">Answer them now, or submit the tab as it is. Answers are marked only when you submit.</p>'+
    '<div class="skip-chips">'+list.map(function(i){ return '<button class="chip skip-go" data-i="'+i+'">Q'+(i+1)+'</button>'; }).join('')+'</div>'+
    '<div class="skip-btns"><button class="btn btn-primary" id="btnGoSkipped">Answer skipped questions</button><button class="btn" id="btnSubmitAnyway">Submit anyway</button></div></div>';
  document.getElementById('wrap').innerHTML=h;
  document.getElementById('navbarInner').innerHTML='';
  var go=function(i){ ts.idx=i; ts.maxReached=Math.max(ts.maxReached,i); renderSlide(); window.scrollTo({top:0,behavior:'smooth'}); };
  document.getElementById('btnGoSkipped').addEventListener('click',function(){ go(list[0]); });
  document.querySelectorAll('.skip-go').forEach(function(b){ b.addEventListener('click',function(){ go(parseInt(b.dataset.i,10)); }); });
  document.getElementById('btnSubmitAnyway').addEventListener('click',function(){ ts.submitOK=true; renderFinished(); ts.submitOK=false; });
  saveState();
}
var _rfSkip = renderFinished;
renderFinished = function(){
  var ts=state.tabs[activeTab];
  if(MODE==='quiz' && !ts.submitOK && skippedList(ts).length){ renderSkipGate(ts); return; }
  _rfSkip();
  if(MODE==='learning'){
    var list=skippedList(ts);
    if(list.length){
      var card=document.querySelector('.done-card');
      if(card){ var d=document.createElement('div'); d.className='skip-btns';
        d.innerHTML='<button class="btn btn-primary" id="btnGoSkipped">Attempt skipped questions ('+list.length+')</button>';
        card.appendChild(d);
        document.getElementById('btnGoSkipped').addEventListener('click',function(){ ts.idx=list[0]; ts.recorded=false; renderSlide(); window.scrollTo({top:0,behavior:'smooth'}); }); }
    }
  }
};


/* ================= approx answers (physics: within 1%) ================= */
var _amTools = answerMatches;
answerMatches = function(input,answer,accept,expr){
  if(expr==='approx'){
    var n1=parseNum(input); if(n1===null) return false;
    return [answer].concat(accept||[]).some(function(a){ var n2=parseNum(a); if(n2===null) return false; return Math.abs(n1-n2) <= Math.max(0.011*Math.abs(n2), 1e-9); });
  }
  return _amTools(input,answer,accept,expr);
};

/* ================= palette: every question already reached can be opened ================= */
statusOf = function(tabId,i){
  var ts=state.tabs[tabId];
  if(i>ts.maxReached) return 'locked';
  if(i===ts.idx) return 'current';
  var s=ts.items[i].status;
  if(s==='unanswered') return 'skipped';
  return s;
};

/* ================= on-screen keyboard ================= */
var KB={on:true, page:'num', target:null};
try{ var kbp=localStorage.getItem('sopaan-kb-pref'); if(kbp==='off') KB.on=false; }catch(e){}
function kbSave(){ try{ localStorage.setItem('sopaan-kb-pref', KB.on?'on':'off'); }catch(e){} }
var KEYS_NUM=[['7','8','9','(',')'],['4','5','6','−','/'],['1','2','3','.',','],['0',':','%','°','⌫'],['abc','←','→','Clear','Done']];
var KEYS_FRAC=[['7','8','9','/'],['4','5','6','−'],['1','2','3','space'],['0',',','⌫','Clear'],['abc','←','→','Done']];
var KEYS_ALG=[['7','8','9','x','y','n'],['4','5','6','+','−','a'],['1','2','3','×','÷','b'],['0','.','(',')','^','²'],['/','π','|','t','⌫','Clear'],['abc','←','→','Done']];
function kbLayoutFor(inp){ try{ var ts=state.tabs[activeTab], sl=SLIDES[activeTab][ts.idx], stp=sl.flat[parseInt(inp.dataset.step,10)]; var m=stp.expr, key=String(stp.a[inp.dataset.bkey]||'');
  if(m==='words'||m==='glist'||m==='angle') return 'abc'; if(m===true||m==='pow'||m==='primes') return 'alg';
  if(['fv','fe','fl','fm','fi','flist'].indexOf(m)>=0) return 'frac'; if(m==='dec'||m==='approx'||m==='dlist'||m==='set'||m==='coord'||m==='list'||m==='time') return 'num';
  if(/^[\-−]?\d+ \d+\/\d+$/.test(key)||/^[\-−]?\d+\/\d+$/.test(key)) return 'frac'; if(/[a-df-z]/i.test(key.replace(/pi/gi,''))) return /\d/.test(key)?'alg':'abc'; return 'num'; }catch(e){ return 'num'; } }
var KEYS_CALC=[['7','8','9','x','(',')'],['4','5','6','+','−','^'],['1','2','3','×','/','²'],['0','.','e','eˣ','√','ln'],['sin','cos','tan','t','⌫','Clear'],['sec','csc','cot','π','θ','∛'],['abc','←','→','Done']];
var KEYS_ABC=[['q','w','e','r','t','y','u','i','o','p'],['a','s','d','f','g','h','j','k','l','-'],['z','x','c','v','b','n','m',',',':','/'],['123','space','←','→','⌫','Done']];
function kbBuild(){
  var el=document.getElementById('vkb'); if(!el){ el=document.createElement('div'); el.id='vkb'; el.className='vkb'; document.body.appendChild(el);
    el.addEventListener('pointerdown',function(e){ var b=e.target.closest('button[data-k]'); e.preventDefault(); if(b) kbPress(b.dataset.k); });
    el.addEventListener('mousedown',function(e){ e.preventDefault(); }); }
  var rows={num:KEYS_NUM,frac:KEYS_FRAC,alg:KEYS_ALG,abc:KEYS_ABC,calc:KEYS_CALC}[KB.page]||KEYS_NUM;
  el.innerHTML='<div class="vkb-top"><span>⌨️ Keyboard</span><button data-k="device" class="vkb-link">Use device keyboard</button></div>'+
    rows.map(function(r){ return '<div class="vkb-row">'+r.map(function(k){
      var cls='vkb-k'+(/^(abc|123|Done|Clear|⌫|←|→|space)$/.test(k)?' fn':'')+(k==='Done'?' done':'');
      return '<button type="button" class="'+cls+'" data-k="'+k+'">'+(k==='space'?'space':k)+'</button>'; }).join('')+'</div>'; }).join('');
  return el;
}
function kbShow(inp){ KB.target=inp; KB.home=kbLayoutFor(inp); KB.page=KB.home; if(!KB.on) return; var cp=document.getElementById('calcPanel'); if(cp&&cp.classList.contains('show')) return; var el=kbBuild(); var nb=document.querySelector('.navbar'); el.style.bottom=(nb?nb.getBoundingClientRect().height:0)+'px'; el.classList.add('show'); document.body.classList.add('kb-open'); setTimeout(function(){ var r=inp.getBoundingClientRect(), top=el.getBoundingClientRect().top; if(r.bottom>top-12) window.scrollBy({top:r.bottom-top+60,behavior:'smooth'}); else if(r.top<60) window.scrollBy({top:r.top-80,behavior:'smooth'}); },30); }
function kbHide(){ var el=document.getElementById('vkb'); if(el) el.classList.remove('show'); document.body.classList.remove('kb-open'); }
function kbInsert(s){
  var t=KB.target; if(!t||t.disabled) return;
  var a=t.selectionStart==null?t.value.length:t.selectionStart, b=t.selectionEnd==null?a:t.selectionEnd;
  t.value=t.value.slice(0,a)+s+t.value.slice(b); var p=a+s.length; try{ t.setSelectionRange(p,p); }catch(e){}
  t.dispatchEvent(new Event('input',{bubbles:true}));
}
function kbPress(k){
  var t=KB.target; if(k==='device'){ KB.on=false; kbSave(); kbHide(); document.querySelectorAll('.blank-input').forEach(function(i){ i.removeAttribute('inputmode'); }); if(t){ t.blur(); setTimeout(function(){ t.focus(); },50); } showToast('Device keyboard on. Tap ⌨️ on any blank to bring the on-screen keyboard back.'); return; }
  if(k==='Done'){ kbHide(); if(t) t.blur(); return; }
  if(k==='abc'||k==='123'){ KB.page=(k==='abc')?'abc':(KB.home&&KB.home!=='abc'?KB.home:'num'); kbBuild(); return; }
  if(!t) return;
  if(k==='⌫'){ var a=t.selectionStart, b=t.selectionEnd; if(a===b&&a>0){ t.value=t.value.slice(0,a-1)+t.value.slice(b); try{t.setSelectionRange(a-1,a-1);}catch(e){} } else { t.value=t.value.slice(0,a)+t.value.slice(b); try{t.setSelectionRange(a,a);}catch(e){} } t.dispatchEvent(new Event('input',{bubbles:true})); return; }
  if(k==='Clear'){ t.value=''; t.dispatchEvent(new Event('input',{bubbles:true})); return; }
  if(k==='←'||k==='→'){ var p=(t.selectionStart||0)+(k==='←'?-1:1); p=Math.max(0,Math.min(t.value.length,p)); try{t.setSelectionRange(p,p);}catch(e){} return; }
  var map={'−':'-','space':' '}; kbInsert(map[k]!==undefined?map[k]:k);
}
function kbWire(){
  document.querySelectorAll('.blank-input').forEach(function(inp){
    if(inp.dataset.kb) return; inp.dataset.kb='1';
    if(KB.on) inp.setAttribute('inputmode','none');
    inp.addEventListener('focus',function(){ kbShow(inp); });
    var btn=document.createElement('button'); btn.type='button'; btn.className='kb-toggle'; btn.title='On-screen keyboard'; btn.textContent='⌨️'; btn.tabIndex=-1;
    btn.addEventListener('mousedown',function(e){ e.preventDefault(); });
    btn.addEventListener('click',function(){ KB.on=true; kbSave(); document.querySelectorAll('.blank-input').forEach(function(i){ i.setAttribute('inputmode','none'); }); inp.focus(); kbShow(inp); });
    if(!inp.disabled) inp.insertAdjacentElement('afterend',btn);
  });
}
document.addEventListener('focusout',function(e){ setTimeout(function(){ var a=document.activeElement; if(!a||!a.classList||!a.classList.contains('blank-input')){ if(!document.querySelector('#vkb:hover')) kbHide(); } },120); });

/* ================= calculator ================= */
var CALC={expr:'', ans:0};
function calcEval(src){
  var s=String(src).replace(/×/g,'*').replace(/÷/g,'/').replace(/−/g,'-').replace(/π/g,'(PI)').replace(/Ans/g,'('+CALC.ans+')').replace(/\^/g,'**').replace(/√\(/g,'sqrt(').replace(/²/g,'**2').replace(/E/g,'*10**');
  s=s.replace(/(^|[(*\/+\-,])-/g,'$1(-1)*');
  if(/[^0-9+\-*/().,a-z A-Z]/.test(s)) throw 0;
  var ok=s.replace(/sin|cos|tan|asin|acos|atan|sqrt|log|ln|PI|abs/g,''); if(/[a-zA-Z]/.test(ok)) throw 0;
  var f=new Function('sin','cos','tan','asin','acos','atan','sqrt','log','ln','PI','abs','return ('+s+');');
  var d=Math.PI/180;
  var v=f(function(x){return Math.sin(x*d);},function(x){return Math.cos(x*d);},function(x){return Math.tan(x*d);},
    function(x){return Math.asin(x)/d;},function(x){return Math.acos(x)/d;},function(x){return Math.atan(x)/d;},Math.sqrt,Math.log10,Math.log,Math.PI,Math.abs);
  if(typeof v!=='number'||!isFinite(v)) throw 0; return v;
}
function fmtNum(v){ if(Math.abs(v)>=1e10||(Math.abs(v)<1e-6&&v!==0)) return v.toExponential(6).replace(/\.?0+e/,'e'); return String(parseFloat(v.toPrecision(10))); }
var CKEYS=[['sin(','cos(','tan(','√(','^','²'],['asin(','acos(','atan(','(',')','π'],['7','8','9','÷','⌫','AC'],['4','5','6','×','E','Ans'],['1','2','3','−','(−)','Insert'],['0','.','=','+']];
function openCalc(){
  var p=document.getElementById('calcPanel');
  if(!p){ p=document.createElement('div'); p.id='calcPanel'; p.className='tool-panel calc';
    p.innerHTML='<div class="tp-head"><b>🧮 Calculator</b><span class="tp-note">degrees · tap a blank, then Insert</span><button class="tp-x" data-c="close">✕</button></div>'+
      '<div class="calc-disp"><div class="calc-expr" id="calcExpr"></div><div class="calc-res" id="calcRes">0</div></div>'+
      '<div class="calc-keys">'+CKEYS.map(function(r){ return r.map(function(k){ return '<button type="button" data-c="'+k+'" class="'+(k==='='?'eq':(/^(AC|⌫|Insert)$/.test(k)?'fn':''))+'">'+({'sin(':'sin','cos(':'cos','tan(':'tan','asin(':'sin⁻¹','acos(':'cos⁻¹','atan(':'tan⁻¹','√(':'√'}[k]||k)+'</button>'; }).join(''); }).join('')+'</div>';
    document.body.appendChild(p);
    p.addEventListener('mousedown',function(e){ if(e.target.closest('button')) e.preventDefault(); });
    p.addEventListener('click',function(e){ var b=e.target.closest('button[data-c]'); if(!b) return; calcKey(b.dataset.c); });
  }
  kbHide(); var nb=document.querySelector('.navbar'); p.style.bottom=((nb?nb.getBoundingClientRect().height:0)+8)+'px'; p.classList.add('show'); document.body.classList.add('calc-open'); calcShow();
}
function calcShow(res){ document.getElementById('calcExpr').textContent=CALC.expr||' '; if(res!==undefined) document.getElementById('calcRes').textContent=res; }
function calcKey(k){
  if(k==='close'){ document.getElementById('calcPanel').classList.remove('show'); document.body.classList.remove('calc-open'); return; }
  if(k==='AC'){ CALC.expr=''; calcShow('0'); return; }
  if(k==='⌫'){ CALC.expr=CALC.expr.replace(/(asin\(|acos\(|atan\(|sin\(|cos\(|tan\(|√\(|Ans|.)$/,''); calcShow(); return; }
  if(k==='='){ try{ var v=calcEval(CALC.expr); CALC.ans=v; calcShow(fmtNum(v)); }catch(e){ calcShow('Error'); } return; }
  if(k==='(−)'){ CALC.expr+='−'; calcShow(); return; }
  if(k==='Insert'){ var r=document.getElementById('calcRes').textContent; if(KB.target && !KB.target.disabled && r!=='Error'){ KB.target.value=r; KB.target.dispatchEvent(new Event('input',{bubbles:true})); showToast('Inserted '+r+' into the blank.'); } else showToast('Tap a blank first, then press Insert.'); return; }
  CALC.expr+=k; calcShow();
}

/* ================= Desmos ================= */
var DESMOS_KEY='dcb31709b452b1cf9dc26972add0fda6', desmosCalc=null, desmosLoading=false;
function openDesmos(exprs){
  var p=document.getElementById('desmosPanel');
  if(!p){ p=document.createElement('div'); p.id='desmosPanel'; p.className='tool-panel desmos';
    p.innerHTML='<div class="tp-head"><b>📈 Desmos graphing calculator</b><button class="tp-x" id="desmosReset">Reset graph</button><button class="tp-x" id="desmosClose">✕</button></div><div id="desmosBox"><div class="desmos-msg">Loading Desmos…</div></div>';
    document.body.appendChild(p);
    document.getElementById('desmosClose').addEventListener('click',function(){ p.classList.remove('show'); });
    document.getElementById('desmosReset').addEventListener('click',function(){ if(desmosCalc) desmosSet(p._exprs||[]); });
  }
  p._exprs=exprs||[]; p.classList.add('show');
  if(window.Desmos){ desmosInit(); desmosSet(p._exprs); return; }
  if(desmosLoading) return; desmosLoading=true;
  var sc=document.createElement('script'); sc.src='https://www.desmos.com/api/v1.9/calculator.js?apiKey='+DESMOS_KEY;
  sc.onload=function(){ desmosInit(); desmosSet(p._exprs); };
  sc.onerror=function(){ desmosLoading=false; document.getElementById('desmosBox').innerHTML='<div class="desmos-msg">Desmos needs an internet connection. <a href="https://www.desmos.com/calculator" target="_blank" rel="noopener">Open Desmos in a new tab</a>.</div>'; };
  document.head.appendChild(sc);
}
function desmosInit(){ if(desmosCalc) return; var box=document.getElementById('desmosBox'); box.innerHTML=''; desmosCalc=Desmos.GraphingCalculator(box,{expressionsCollapsed:false,settingsMenu:false,border:false,degreeMode:true}); }
function desmosSet(exprs){ if(!desmosCalc) return; desmosCalc.setBlank(); (exprs||[]).forEach(function(e,i){ if(typeof e==='string') desmosCalc.setExpression({id:'e'+i,latex:e}); else desmosCalc.setExpression(Object.assign({id:'e'+i},e)); }); }

/* ================= toolbar on each question ================= */
var _rsTools = renderSlide;
renderSlide = function(){
  _rsTools();
  kbHide();
  if(activeTab==='theory'||activeTab==='report') return;
  var ts=state.tabs[activeTab]; if(!ts) return;
  var slide=SLIDES[activeTab][ts.idx], card=document.querySelector('#wrap .qcard');
  if(card && slide && slide.tools && slide.tools.length && !card.querySelector('.tool-bar')){
    var bar=document.createElement('div'); bar.className='tool-bar';
    bar.innerHTML=(slide.tools.indexOf('calc')>=0?'<button type="button" class="tool-btn" data-t="calc">🧮 Calculator</button>':'')+
                  (slide.tools.indexOf('desmos')>=0?'<button type="button" class="tool-btn" data-t="desmos">📈 Desmos graph</button>':'');
    card.insertBefore(bar, card.firstChild);
    bar.addEventListener('click',function(e){ var b=e.target.closest('[data-t]'); if(!b) return; if(b.dataset.t==='calc') openCalc(); else openDesmos(slide.desmos||[]); });
  }
  kbWire();
};



/* ================= signed fractions in text: {−3/4}, {3/−4}, {−2 1/3}, {p/q} ================= */
fr = function(s){ return String(s).replace(/&lt;(\/?)(b|sup|sub|i)>/g,'<$1$2>')
  .replace(/\{([−-]?\d+) (\d+)\/(\d+)\}/g,'<span class="mx">$1<span class="fq"><span>$2</span><span>$3</span></span></span>')
  .replace(/\{([−-]?[A-Za-z0-9]+)\/([−-]?[A-Za-z0-9]+)\}/g,'<span class="fq"><span>$1</span><span>$2</span></span>'); };
/* ================= BMA badge → main page of this sheet (theory hub) ================= */
(function(){
  var c=document.querySelector('.brand .crest'); if(!c) return;
  var a=document.createElement('button'); a.type='button'; a.className='crest crest-home'; a.title='Back to the main page (theory notes)'; a.setAttribute('aria-label','Main page');
  a.innerHTML='<img src="data:image/png;base64,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" alt="Brain and Mind"><span class="crest-h">⌂</span>'; c.parentNode.replaceChild(a,c);
  a.addEventListener('click',function(){
    if(!student||!MODE){ window.scrollTo({top:0,behavior:'smooth'}); return; }
    if(typeof kbHide==='function') kbHide(); if(typeof SP!=='undefined'&&SP.on) spToggle(false);
    var cp=document.getElementById('calcPanel'); if(cp) cp.classList.remove('show'); document.body.classList.remove('calc-open');
    activeTab = (typeof THEORY!=='undefined') ? 'theory' : TAB_DEFS[0].id;
    buildTabbar(); renderSlide(); window.scrollTo({top:0,behavior:'smooth'});
  });
})();

/* ================= session clock: starts at sign-in and keeps running ================= */
var CLK={t0:null};
(function(){
  var row=document.querySelector('.brand .brand-row'); if(!row) return;
  var d=document.createElement('div'); d.className='bmasw off'; d.id='swBox'; d.title='Time since you signed in';
  d.innerHTML='<span class="bmasw-ic">⏱</span><span class="bmasw-t" id="swT">00:00</span>';
  row.appendChild(d); setInterval(swTick,1000);
})();
function swFmt(s){ s=Math.floor(s||0); var h=Math.floor(s/3600), m=Math.floor(s%3600/60), x=s%60; return (h?h+':'+String(m).padStart(2,'0'):String(m).padStart(2,'0'))+':'+String(x).padStart(2,'0'); }
function swTick(){
  var box=document.getElementById('swBox'); if(!box) return;
  if(student && !CLK.t0) CLK.t0=Date.now();
  if(!student) CLK.t0=null;
  box.classList.toggle('off',!CLK.t0);
  document.getElementById('swT').textContent = CLK.t0 ? swFmt((Date.now()-CLK.t0)/1000) : '00:00';
}
function swTab(){ try{ if(!state||!state.tabs||activeTab==='theory'||activeTab==='report') return null; return state.tabs[activeTab]||null; }catch(e){ return null; } }
var _rsSW = renderSlide;
renderSlide = function(){ _rsSW(); swTick(); };
var _rfSW = renderFinished;
renderFinished = function(){ _rfSW(); var done=document.querySelector('#wrap .done-card'); if(CLK.t0 && done && !done.querySelector('.bmasw-done')){ var p=document.createElement('p'); p.className='bmasw-done'; p.textContent='⏱ Time since sign-in: '+swFmt((Date.now()-CLK.t0)/1000); var h2=done.querySelector('h2'); if(h2) h2.insertAdjacentElement('afterend',p); else done.appendChild(p); } };

/* ================= scratchpad (Khan-style, 4 pens) ================= */
var SP={on:false, draw:true, color:'ink', size:3, erase:false, store:{}, key:null, cv:null, ctx:null, down:false, last:null};
var SP_COL={ink:null, blue:'#2563EB', red:'#DC2626', green:'#16A34A'};
function spInk(){ return getComputedStyle(document.documentElement).getPropertyValue('--ink').trim()||'#211E1A'; }
function spKey(){ var ts=swTab(); return ts ? (MODE+'|'+activeTab+'|'+ts.idx) : null; }
function spBuild(){
  if(SP.cv) return;
  var cv=document.createElement('canvas'); cv.id='spCanvas'; cv.className='sp-canvas'; document.body.appendChild(cv);
  var bar=document.createElement('div'); bar.id='spBar'; bar.className='sp-bar';
  bar.innerHTML='<span class="sp-lbl">✏️ Scratchpad</span>'+
    ['ink','blue','red','green'].map(function(c){ return '<button type="button" class="sp-pen" data-c="'+c+'" title="'+(c==='ink'?'black':c)+' pen"><i style="background:'+(c==='ink'?'var(--ink)':SP_COL[c])+'"></i></button>'; }).join('')+
    '<button type="button" class="sp-tool" data-t="erase" title="Eraser">🧽</button><button type="button" class="sp-tool" data-t="size" title="Pen size">●</button><button type="button" class="sp-tool" data-t="scroll" title="Pause drawing to scroll or answer">✋</button>'+
    '<button type="button" class="sp-tool" data-t="clear" title="Clear page">🗑</button><button type="button" class="sp-tool" data-t="close" title="Close scratchpad">✕</button>';
  document.body.appendChild(bar);
  bar.addEventListener('click',function(e){ var b=e.target.closest('button'); if(!b) return;
    if(b.dataset.c){ SP.color=b.dataset.c; SP.erase=false; SP.draw=true; }
    else if(b.dataset.t==='erase'){ SP.erase=true; SP.draw=true; }
    else if(b.dataset.t==='size'){ SP.size = SP.size===3?6:(SP.size===6?1.5:3); b.textContent = SP.size===6?'⬤':(SP.size===1.5?'·':'●'); }
    else if(b.dataset.t==='scroll'){ SP.draw=!SP.draw; }
    else if(b.dataset.t==='clear'){ spClear(); }
    else if(b.dataset.t==='close'){ spToggle(false); return; }
    spUI(); });
  SP.cv=cv; SP.ctx=cv.getContext('2d');
  cv.addEventListener('pointerdown',function(e){ if(!SP.draw) return; e.preventDefault(); cv.setPointerCapture(e.pointerId); SP.down=true; SP.last=spPt(e); spDot(SP.last); });
  cv.addEventListener('pointermove',function(e){ if(!SP.down) return; e.preventDefault(); var p=spPt(e); spLine(SP.last,p); SP.last=p; });
  var up=function(){ if(SP.down){ SP.down=false; spSave(); } };
  cv.addEventListener('pointerup',up); cv.addEventListener('pointercancel',up); cv.addEventListener('pointerleave',up);
  window.addEventListener('resize',function(){ if(SP.on) spFit(true); });
}
function spPt(e){ var r=SP.cv.getBoundingClientRect(); return {x:e.clientX-r.left, y:e.clientY-r.top}; }
function spStyle(){ var c=SP.ctx; c.lineCap='round'; c.lineJoin='round'; c.globalCompositeOperation=SP.erase?'destination-out':'source-over'; c.strokeStyle=c.fillStyle=(SP.color==='ink'?spInk():SP_COL[SP.color]); c.lineWidth=SP.erase?22:SP.size; }
function spDot(p){ spStyle(); var c=SP.ctx; c.beginPath(); c.arc(p.x,p.y,(SP.erase?11:SP.size/2),0,Math.PI*2); c.fill(); }
function spLine(a,b){ spStyle(); var c=SP.ctx; c.beginPath(); c.moveTo(a.x,a.y); c.lineTo(b.x,b.y); c.stroke(); }
function spSave(){ if(SP.key&&SP.cv){ try{ SP.store[SP.key]=SP.cv.toDataURL(); }catch(e){} } }
function spClear(){ if(!SP.ctx) return; SP.ctx.save(); SP.ctx.setTransform(1,0,0,1,0,0); SP.ctx.clearRect(0,0,SP.cv.width,SP.cv.height); SP.ctx.restore(); if(SP.key) delete SP.store[SP.key]; }
function spFit(keep){
  var wrap=document.getElementById('wrap'); if(!wrap||!SP.cv) return;
  var r=wrap.getBoundingClientRect(), top=r.top+window.scrollY, h=Math.max(wrap.scrollHeight, window.innerHeight-r.top)+40, w=document.documentElement.clientWidth;
  var old=keep&&SP.key?SP.store[SP.key]:null, dpr=window.devicePixelRatio||1;
  SP.cv.style.top=top+'px'; SP.cv.style.left='0px'; SP.cv.style.width=w+'px'; SP.cv.style.height=h+'px';
  SP.cv.width=Math.round(w*dpr); SP.cv.height=Math.round(h*dpr); SP.ctx.setTransform(dpr,0,0,dpr,0,0);
  if(old){ var im=new Image(); im.onload=function(){ SP.ctx.save(); SP.ctx.setTransform(1,0,0,1,0,0); SP.ctx.drawImage(im,0,0); SP.ctx.restore(); }; im.src=old; }
}
function spLoad(){ spSave(); SP.key=spKey(); spFit(false); var d=SP.key&&SP.store[SP.key]; if(d){ var im=new Image(); im.onload=function(){ SP.ctx.save(); SP.ctx.setTransform(1,0,0,1,0,0); SP.ctx.drawImage(im,0,0); SP.ctx.restore(); }; im.src=d; } }
function spUI(){
  var bar=document.getElementById('spBar'); if(!bar) return;
  bar.querySelectorAll('.sp-pen').forEach(function(b){ b.classList.toggle('on', !SP.erase && SP.draw && b.dataset.c===SP.color); });
  bar.querySelector('[data-t=erase]').classList.toggle('on', SP.erase && SP.draw);
  bar.querySelector('[data-t=scroll]').classList.toggle('on', !SP.draw);
  SP.cv.classList.toggle('passive', !SP.draw);
  var fb=document.getElementById('spFab'); if(fb) fb.classList.toggle('on',SP.on);
}
function spToggle(on){
  spBuild(); SP.on=(on===undefined)?!SP.on:on;
  document.body.classList.toggle('sp-open',SP.on); SP.cv.style.display=SP.on?'block':'none'; document.getElementById('spBar').style.display=SP.on?'flex':'none';
  if(SP.on){ SP.draw=true; SP.erase=false; spLoad(); if(typeof kbHide==='function') kbHide(); } else { spSave(); }
  spUI();
}
(function(){ var f=document.createElement('button'); f.type='button'; f.id='spFab'; f.className='sp-fab'; f.innerHTML='✏️ <span>Scratchpad</span>'; f.title='Open a scratchpad to write your working'; f.addEventListener('click',function(){ spToggle(); }); document.body.appendChild(f); })();
var _rsSP = renderSlide;
renderSlide = function(){ _rsSP(); var fab=document.getElementById('spFab'); var q=!!swTab(); if(fab) fab.style.display=q?'':'none'; if(!q && SP.on) spToggle(false); if(SP.on) setTimeout(spLoad,30); };


/* ================= v4: attempt classification ================= */
function v4Class(item){
  if(!item) return 'un';
  if(item.status==='skipped') return 'sk';
  if(item.status==='unanswered') return 'un';
  if(item.stepStates){ // step question
    if(item.status!=='correct' && item.status!=='revealed') return 'un';
    if(item.status==='revealed' || item.stepStates.some(function(s){return s.status==='revealed';})) return 'w';
    return item.stepStates.some(function(s){return (s.attempts||0)>0;}) ? 'c2' : 'c1';
  }
  if(item.status==='revealed') return 'w';
  if(item.status==='correct') return (item.attempts||0)>0 ? 'c2' : 'c1';
  if(item.status==='wrong'||item.status==='incorrect') return 'w';
  return 'un';
}
function v4Counts(items){ var c={n:items.length,c1:0,c2:0,w:0,sk:0,un:0}; items.forEach(function(it){ c[v4Class(it)]++; }); return c; }

/* ================= v4: My record with attempt columns ================= */
renderRecord = function(){
  showChrome(false);
  var tabLabel=function(id){ var t=TAB_DEFS.find(function(x){return x.id===id;}); return t?t.label:id; };
  var title=(document.querySelector('.chapter-title')||{}).textContent||'';
  var h='<div class="rec-card"><h2>'+esc(student.name)+'’s record</h2><p class="rec-empty" style="margin:0 0 12px;">Roll '+esc(student.roll)+(title?' · '+esc(title):'')+'</p>';
  var st=appState.learning;
  h+='<h3>📘 Learning Sheet — attempts</h3><p class="v4leg"><b>1st ✓</b> correct on the first attempt · <b>2nd ✓</b> correct on the second attempt · <b>Wrong</b> still wrong after two attempts (answer revealed) · <b>Skip</b> skipped<span class="v4left"> · <b>Left</b> not done yet</span></p>';
  if(!st){ h+='<p class="rec-empty">Not started yet.</p>'; }
  else {
    var T={n:0,c1:0,c2:0,w:0,sk:0,un:0};
    h+='<div class="rec-table-wrap"><table class="rec-table v4rec"><thead><tr><th>Sheet</th><th>Qs</th><th>1st ✓</th><th>2nd ✓</th><th>Wrong</th><th>Skip</th><th class="v4left">Left</th></tr></thead><tbody>';
    TAB_DEFS.forEach(function(td){ var tt=st.tabs[td.id]; if(!tt||!tt.items||!tt.items.length) return; var c=v4Counts(tt.items);
      ['n','c1','c2','w','sk','un'].forEach(function(k){ T[k]+=c[k]; });
      h+='<tr><td>'+td.label+'</td><td>'+c.n+'</td><td class="v4g">'+c.c1+'</td><td class="v4o">'+c.c2+'</td><td class="v4r">'+c.w+'</td><td>'+c.sk+'</td><td class="v4left">'+c.un+'</td></tr>'; });
    h+='<tr class="v4tot"><td>Total</td><td>'+T.n+'</td><td class="v4g">'+T.c1+'</td><td class="v4o">'+T.c2+'</td><td class="v4r">'+T.w+'</td><td>'+T.sk+'</td><td class="v4left">'+T.un+'</td></tr>';
    h+='</tbody></table></div>';
    var doneN=T.c1+T.c2+T.w; if(doneN){ h+='<p class="v4sum">Of '+doneN+' questions answered: <b>'+Math.round(T.c1/doneN*100)+'%</b> right first time, <b>'+Math.round(T.c2/doneN*100)+'%</b> right on the second try, <b>'+Math.round(T.w/doneN*100)+'%</b> still wrong after two tries.</p>'; }
  }
  var q=appState.quiz;
  h+='<h3>📝 Quiz Mode</h3>';
  if(!q){ h+='<p class="rec-empty">Not started yet.</p>'; }
  else {
    h+='<div class="rec-table-wrap"><table class="rec-table v4rec"><thead><tr><th>Sheet</th><th>Qs</th><th>Status</th><th>Correct</th><th>Wrong</th></tr></thead><tbody>';
    TAB_DEFS.forEach(function(td){ var tt=q.tabs[td.id]; if(!tt||!tt.items||!tt.items.length) return; var n=tt.items.length, cor=0, att=0;
      tt.items.forEach(function(it){ if(it.status!=='unanswered'||it.choice!==undefined) att++; });
      var rec=records.filter(function(r){ return r.mode==='quiz'&&r.tab===td.id; })[0];
      if(rec){ cor=rec.correct; att=Math.max(att,rec.total); }
      h+='<tr><td>'+td.label+'</td><td>'+n+'</td><td>'+(rec?'Finished':att+' / '+n)+'</td><td class="v4g">'+(rec?cor:'—')+'</td><td class="v4r">'+(rec?(rec.total-cor):'—')+'</td></tr>'; });
    h+='</tbody></table></div>';
  }
  h+='</div><div class="rec-card"><h3>Finished sheets (latest first)</h3>';
  if(!records.length){ h+='<p class="rec-empty">No sheets finished yet. Each time you finish a sheet, your score is recorded here.</p>'; }
  else {
    h+='<div class="rec-table-wrap"><table class="rec-table v4rec"><thead><tr><th>When</th><th>Mode</th><th>Sheet</th><th>Score</th><th>1st ✓</th><th>2nd ✓</th><th>Wrong</th></tr></thead><tbody>';
    records.forEach(function(r){ h+='<tr><td>'+fmtDate(r.at)+'</td><td>'+(r.mode==='quiz'?'Quiz':'Learning')+'</td><td>'+tabLabel(r.tab)+'</td><td>'+r.correct+' / '+r.total+'</td><td>'+(r.c1!=null?r.c1:'—')+'</td><td>'+(r.c2!=null?r.c2:'—')+'</td><td>'+(r.w!=null?r.w:(r.mode==='quiz'?r.total-r.correct:'—'))+'</td></tr>'; });
    h+='</tbody></table></div>';
  }
  h+='</div><button class="btn btn-primary" id="btnBack">'+(MODE?'Back to practice':'Choose a mode')+'</button>';
  document.getElementById('wrap').innerHTML=h;
  document.getElementById('btnBack').addEventListener('click', function(){ if(MODE){ showChrome(true); buildTabbar(); renderSlide(); } else renderModePicker(); });
  window.scrollTo({top:0});
};
var _v4add = addRecord;
addRecord = function(mode, tabId, correct, revealed, skipped, total){
  _v4add(mode, tabId, correct, revealed, skipped, total);
  try{ if(mode==='learning'&&records[0]){ var c=v4Counts(state.tabs[tabId].items); records[0].c1=c.c1; records[0].c2=c.c2; records[0].w=c.w; saveState(); } }catch(e){}
};

/* ================= v4: celebration ================= */
function v4Cracker(){
  var ctx=ensureAudio(); if(!ctx) return; try{ if(ctx.state==='suspended') ctx.resume(); }catch(e){}
  var now=ctx.currentTime;
  function pop(t, vol, dur, hp){
    var len=Math.floor(ctx.sampleRate*dur), buf=ctx.createBuffer(1,len,ctx.sampleRate), d=buf.getChannelData(0);
    for(var i=0;i<len;i++){ d[i]=(Math.random()*2-1)*Math.pow(1-i/len,3); }
    var src=ctx.createBufferSource(); src.buffer=buf;
    var f=ctx.createBiquadFilter(); f.type='highpass'; f.frequency.value=hp;
    var g=ctx.createGain(); g.gain.setValueAtTime(vol,t); g.gain.exponentialRampToValueAtTime(0.001,t+dur);
    src.connect(f); f.connect(g); g.connect(ctx.destination); src.start(t); src.stop(t+dur+0.02);
  }
  pop(now,0.9,0.35,300);                                   // big bang
  for(var k=0;k<14;k++){ pop(now+0.35+Math.random()*1.3, 0.25+Math.random()*0.35, 0.05+Math.random()*0.08, 1500+Math.random()*2500); } // crackles
  [523.25,659.25,783.99,1046.5].forEach(function(fq,i){ var o=ctx.createOscillator(), g=ctx.createGain(); o.type='triangle'; o.frequency.value=fq;
    var t=now+0.15+i*0.12; g.gain.setValueAtTime(0.0001,t); g.gain.exponentialRampToValueAtTime(0.18,t+0.03); g.gain.exponentialRampToValueAtTime(0.001,t+0.5);
    o.connect(g); g.connect(ctx.destination); o.start(t); o.stop(t+0.55); });
}
function v4Confetti(){
  var cv=document.createElement('canvas'); cv.className='v4conf'; document.body.appendChild(cv);
  var W=cv.width=window.innerWidth*(window.devicePixelRatio||1), H=cv.height=window.innerHeight*(window.devicePixelRatio||1), s=(window.devicePixelRatio||1);
  var ctx=cv.getContext('2d'), cols=['#e8b13a','#d9534f','#2e86de','#27ae60','#9b59b6','#f39c12','#1abc9c','#ff6b9a'], P=[];
  function burst(x,y,n){ for(var i=0;i<n;i++){ var a=Math.random()*Math.PI*2, v=(4+Math.random()*9)*s;
    P.push({x:x,y:y,vx:Math.cos(a)*v,vy:Math.sin(a)*v-6*s,w:(6+Math.random()*7)*s,h:(4+Math.random()*5)*s,r:Math.random()*6,vr:(Math.random()-.5)*.4,c:cols[i%cols.length],life:0,flyer:Math.random()<.25}); } }
  burst(W*0.2,H*0.35,90); burst(W*0.8,H*0.35,90); setTimeout(function(){ burst(W*0.5,H*0.25,120); },380); setTimeout(function(){ burst(W*0.35,H*0.3,70); burst(W*0.65,H*0.3,70); },800);
  var t0=performance.now();
  (function frame(t){
    ctx.clearRect(0,0,W,H);
    P.forEach(function(p){ p.vy+=0.22*s; p.vx*=0.985; p.vy*=0.985; p.x+=p.vx; p.y+=p.vy; p.r+=p.vr; p.life++;
      ctx.save(); ctx.translate(p.x,p.y); ctx.rotate(p.r); ctx.fillStyle=p.c;
      if(p.flyer){ ctx.fillRect(-p.w*1.4,-1.5*s,p.w*2.8,3*s); } else { ctx.fillRect(-p.w/2,-p.h/2,p.w,p.h*Math.abs(Math.cos(p.life/6))); }
      ctx.restore(); });
    if(t-t0<4200) requestAnimationFrame(frame); else cv.remove();
  })(t0);
}
function v4NextTab(){
  var i=TAB_DEFS.findIndex(function(t){return t.id===activeTab;});
  for(var j=i+1;j<TAB_DEFS.length;j++){ var id=TAB_DEFS[j].id; if(id!=='theory' && SLIDES[id] && SLIDES[id].length) return TAB_DEFS[j]; }
  return null;
}
function v4Celebrate(){
  var done=document.querySelector('#wrap .done-card'); if(!done || done.dataset.v4) return; done.dataset.v4='1';
  var ts=state.tabs[activeTab], c=v4Counts(ts.items), n=ts.items.length;
  var first=(student&&student.name)?String(student.name).split(' ')[0]:'';
  var pct=MODE==='quiz'?null:Math.round((c.c1+c.c2)/Math.max(n,1)*100);
  var msg = pct===null ? 'You finished this sheet!' : (pct>=90?'Outstanding work!':pct>=75?'Excellent effort!':pct>=50?'Well done — keep going!':'Great persistence — every try makes you stronger!');
  var banner=document.createElement('div'); banner.className='v4ban';
  banner.innerHTML='<div class="v4trophy">🏆</div><div class="v4h">Congratulations'+(first?', '+esc(first):'')+'!</div><div class="v4m">'+msg+'</div>'+
    (MODE==='quiz'?'':'<div class="v4pills"><span class="v4p g">✅ '+c.c1+' first attempt</span><span class="v4p o">🔁 '+c.c2+' second attempt</span><span class="v4p r">❌ '+c.w+' finally wrong</span>'+(c.sk?'<span class="v4p s">⏭ '+c.sk+' skipped</span>':'')+'</div>');
  done.insertBefore(banner, done.firstChild);
  var nx=v4NextTab(), wrapB=document.createElement('div'); wrapB.className='v4next';
  if(nx){ wrapB.innerHTML='<button class="btn btn-primary v4go" id="v4Next">Next sheet: '+nx.label+' →</button>'; }
  else if(SLIDES.report!==undefined || TAB_DEFS.some(function(t){return t.id==='report';})){ wrapB.innerHTML='<button class="btn btn-primary v4go" id="v4Next">📊 View my report →</button>'; }
  else { wrapB.innerHTML='<button class="btn btn-primary v4go" id="v4Next">⌂ Back to the home page</button>'; }
  banner.appendChild(wrapB);
  document.getElementById('v4Next').addEventListener('click',function(){
    var t=nx?nx.id:(TAB_DEFS.some(function(x){return x.id==='report';})?'report':(TAB_DEFS[0]&&TAB_DEFS[0].id));
    activeTab=t; showChrome(true); buildTabbar(); renderSlide(); window.scrollTo({top:0,behavior:'smooth'}); });
  setTimeout(function(){ var r=banner.getBoundingClientRect(); window.scrollBy({top:r.top-110,behavior:'smooth'}); },60);
  v4Confetti(); v4Cracker();
}
var _v4rf = renderFinished;
renderFinished = function(){ _v4rf.apply(this,arguments); try{ v4Celebrate(); }catch(e){ console.log('v4',e); } };


/* ================= v5: inequality plotters ================= */
var PLT={};
function pFrac(s){ s=String(s).trim().replace(/−/g,'-'); if(/^[-+]?∞$|^[-+]?inf$/i.test(s)) return s.charAt(0)==='-'?-Infinity:Infinity;
  var m=s.match(/^([-+]?\d*\.?\d+)\s*\/\s*(\d*\.?\d+)$/); if(m) return parseFloat(m[1])/parseFloat(m[2]); var v=parseFloat(s); return isNaN(v)?null:v; }
function fmtN(v){ if(v===Infinity) return '∞'; if(v===-Infinity) return '−∞'; var r=Math.round(v*1000)/1000; var s=String(r); for(var d=2;d<=12;d++){ var n=Math.round(v*d); if(Math.abs(n/d-v)<1e-9 && Math.abs(n)%d!==0){ s=n+'/'+d; break; } } return s.replace('-','−'); }
/* ---- intervals ---- */
function ivParse(s){ s=String(s||'').trim(); if(!s) return null; if(/^(∅|\{\s*\}|none|empty)$/i.test(s)) return [];
  if(/^(ℝ|R|all real( numbers)?)$/i.test(s)) return [{a:-Infinity,ai:false,b:Infinity,bi:false}];
  var parts=s.split(/\s*(?:∪|U|u|or)\s*/), out=[];
  for(var i=0;i<parts.length;i++){ var m=parts[i].match(/^([\[(])\s*([^,]+?)\s*,\s*([^\])]+?)\s*([\])])$/); if(!m) return null;
    var a=pFrac(m[2]), b=pFrac(m[3]); if(a===null||b===null) return null; out.push({a:a,ai:m[1]==='['&&isFinite(a),b:b,bi:m[4]===']'&&isFinite(b)}); }
  return ivNorm(out); }
function ivNorm(L){ L=L.filter(function(t){ return t.a<t.b||(t.a===t.b&&t.ai&&t.bi); }).sort(function(p,q){ return p.a-q.a||((q.ai?1:0)-(p.ai?1:0)); });
  var o=[]; L.forEach(function(t){ var l=o[o.length-1];
    if(l && (t.a<l.b || (Math.abs(t.a-l.b)<1e-9 && (l.bi||t.ai)))){ if(t.b>l.b||(Math.abs(t.b-l.b)<1e-9&&t.bi)){ l.b=t.b; l.bi=t.bi; } }
    else o.push({a:t.a,ai:t.ai,b:t.b,bi:t.bi}); }); return o; }
function ivEq(x,y){ var A=ivParse(x),B=ivParse(y); if(!A||!B||A.length!==B.length) return false;
  for(var i=0;i<A.length;i++){ var p=A[i],q=B[i]; if(Math.abs(p.a-q.a)>1e-6&&!(p.a===q.a)) return false; if(Math.abs(p.b-q.b)>1e-6&&!(p.b===q.b)) return false; if(p.ai!==q.ai||p.bi!==q.bi) return false; } return true; }
function ivFmt(L){ if(!L.length) return '∅'; return L.map(function(t){ return (t.ai?'[':'(')+fmtN(t.a)+', '+fmtN(t.b)+(t.bi?']':')'); }).join(' ∪ '); }
/* ---- half-planes ---- */
function linParse(side){ side=String(side).replace(/\s+/g,'').replace(/−/g,'-').replace(/\*/g,''); if(!side) side='0';
  if(!/^[-+]/.test(side)) side='+'+side; var re=/([-+])(\(?\d*\.?\d*(?:\/\d*\.?\d+)?\)?)([xy]?)/g, m, r={x:0,y:0,c:0}, used=0;
  while((m=re.exec(side))!==null){ if(m[0]==='') { re.lastIndex++; continue; } used+=m[0].length; var co=m[2].replace(/[()]/g,''); var v=co===''?1:pFrac(co); if(v===null) return null; if(m[1]==='-') v=-v; if(m[3]) r[m[3]]+=v; else { if(co==='') return null; r.c+=v; } }
  if(used!==side.length) return null; return r; }
function hpParse(s){ s=String(s).replace(/<=/g,'≤').replace(/>=/g,'≥'); var m=s.match(/^(.*?)(≤|≥|<|>)(.*)$/); if(!m) return null;
  var L=linParse(m[1]), R=linParse(m[3]); if(!L||!R) return null; var a=L.x-R.x, b=L.y-R.y, c=R.c-L.c, op=m[2];
  if(Math.abs(a)<1e-12&&Math.abs(b)<1e-12) return null; var n=Math.sqrt(a*a+b*b), sg=(Math.abs(a)>1e-12? (a>0?1:-1):(b>0?1:-1));
  a=a/n*sg; b=b/n*sg; c=c/n*sg; if(sg<0) op={'≤':'≥','≥':'≤','<':'>','>':'<'}[op]; return {a:a,b:b,c:c,op:op}; }
function hpList(s){ s=String(s||'').trim(); if(!s) return null; var parts=s.split(/\s*(?:;|,|\band\b)\s*/).filter(Boolean), o=[]; for(var i=0;i<parts.length;i++){ var h=hpParse(parts[i]); if(!h) return null; o.push(h);} return o; }
function hpEq(x,y){ var A=hpList(x),B=hpList(y); if(!A||!B||A.length!==B.length) return false; var used=B.map(function(){return false;});
  return A.every(function(p){ for(var j=0;j<B.length;j++){ var q=B[j]; if(!used[j]&&p.op===q.op&&Math.abs(p.a-q.a)<1e-6&&Math.abs(p.b-q.b)<1e-6&&Math.abs(p.c-q.c)<1e-6){ used[j]=true; return true; } } return false; }); }
function gcd(a,b){ a=Math.abs(a);b=Math.abs(b); while(b){ var t=a%b;a=b;b=t;} return a; }
function hpFmtInt(a,b,c,op){ var g=gcd(gcd(a,b),c)||1; a/=g;b/=g;c/=g; if(a<0||(a===0&&b<0)){ a=-a;b=-b;c=-c; op=({'≤':'≥','≥':'≤','<':'>','>':'<'}[op]||op); }
  function term(k,v,first){ if(!k) return ''; var s=(k<0?(first?'−':' − '):(first?'':' + ')); var m=Math.abs(k); return s+(m===1?'':m)+v; }
  var lhs=term(a,'x',true); lhs+=term(b,'y',lhs===''); return lhs+' '+op+' '+String(c).replace('-','−'); }
/* ---- answer checking ---- */
(function(){ var _am=answerMatches; answerMatches=function(input,answer,accept,expr){
  if(expr==='plot1'||expr==='plot2'){ if(input===undefined||input===null||String(input).trim()==='') return false; var f=expr==='plot1'?ivEq:hpEq;
    return [answer].concat(accept||[]).some(function(a){ return f(input,a); }); }
  return _am.apply(this,arguments); }; })();
/* ---- SVG helpers ---- */
function sv(tag,attrs){ return '<'+tag+' '+Object.keys(attrs).map(function(k){return k+'="'+attrs[k]+'"';}).join(' ')+'/>'; }
/* ---- number-line widget ---- */
function nlEncode(st){ var P=st.pts.slice().sort(function(p,q){return p.v-q.v;}), n=P.length, R=[];
  for(var i=0;i<=n;i++){ R.push({a:i===0?-Infinity:P[i-1].v, b:i===n?Infinity:P[i].v, on:!!st.sh[i]}); }
  var L=[]; R.forEach(function(r,i){ if(r.on) L.push({a:r.a,ai:i>0&&P[i-1].closed,b:r.b,bi:i<n&&P[i].closed}); });
  P.forEach(function(p,i){ if(p.closed && !st.sh[i] && !st.sh[i+1]) L.push({a:p.v,ai:true,b:p.v,bi:true}); });
  var out=[]; L.forEach(function(t){ out.push(t); }); return ivFmt(ivNorm(out)); }
function nlDraw(w){ var st=w._st, lo=st.lo, hi=st.hi, W=340, H=78, x0=22, x1=W-22, y=40, X=function(v){ return x0+(v-lo)/(hi-lo)*(x1-x0); };
  var P=st.pts.slice().sort(function(p,q){return p.v-q.v;}), n=P.length, h='';
  var col='var(--accent-text)';
  for(var i=0;i<=n;i++){ if(!st.sh[i]) continue; var a=i===0?x0-14:X(P[i-1].v), b=i===n?x1+14:X(P[i].v);
    h+=sv('line',{x1:a,y1:y,x2:b,y2:y,style:'stroke:'+col+';stroke-width:7;stroke-linecap:round;opacity:.85'});
    if(i===0) h+='<polygon points="'+(x0-18)+','+y+' '+(x0-6)+','+(y-8)+' '+(x0-6)+','+(y+8)+'" style="fill:'+col+'"/>';
    if(i===n) h+='<polygon points="'+(x1+18)+','+y+' '+(x1+6)+','+(y-8)+' '+(x1+6)+','+(y+8)+'" style="fill:'+col+'"/>'; }
  h=sv('line',{x1:x0-16,y1:y,x2:x1+16,y2:y,style:'stroke:var(--ink);stroke-width:1.6'})+h;
  var every=Math.max(1,Math.ceil((hi-lo)/14));
  for(var v=Math.ceil(lo/st.step)*st.step; v<=hi+1e-9; v+=st.step){ var big=Math.abs(v-Math.round(v))<1e-9; var xx=X(v);
    h+=sv('line',{x1:xx,y1:y-(big?8:4),x2:xx,y2:y+(big?8:4),style:'stroke:var(--ink);stroke-width:'+(big?1.4:1)});
    if(big && Math.round(v)%every===0) h+='<text x="'+xx+'" y="'+(y+24)+'" text-anchor="middle" style="font:13px sans-serif;fill:var(--ink)">'+String(Math.round(v)).replace('-','−')+'</text>'; }
  P.forEach(function(p){ h+=sv('circle',{cx:X(p.v),cy:y,r:7,style:'stroke:'+col+';stroke-width:2.5;fill:'+(p.closed?col:'var(--card)')}); });
  if(st.key){ var K=ivParse(st.key)||[]; K.forEach(function(t){ var a=isFinite(t.a)?X(t.a):x0-14, b=isFinite(t.b)?X(t.b):x1+14;
      h+=sv('line',{x1:a,y1:y-17,x2:b,y2:y-17,style:'stroke:var(--success);stroke-width:5;stroke-linecap:round'});
      if(isFinite(t.a)) h+=sv('circle',{cx:a,cy:y-17,r:5,style:'stroke:var(--success);stroke-width:2;fill:'+(t.ai?'var(--success)':'var(--card)')});
      if(isFinite(t.b)) h+=sv('circle',{cx:b,cy:y-17,r:5,style:'stroke:var(--success);stroke-width:2;fill:'+(t.bi?'var(--success)':'var(--card)')}); }); }
  w.querySelector('.plw-svg').innerHTML='<svg viewBox="0 0 '+W+' '+H+'" style="width:100%;max-width:520px;touch-action:manipulation">'+h+'</svg>';
  w._X=X; w._x0=x0; w._x1=x1; w._W=W; }
function nlTap(w,ev){ var st=w._st; if(st.ro) return; var svg=w.querySelector('svg'), r=svg.getBoundingClientRect(), px=(ev.clientX-r.left)*w._W/r.width;
  var v=st.lo+(px-w._x0)/(w._x1-w._x0)*(st.hi-st.lo), sv_=Math.round(v/st.step)*st.step;
  var near=Math.abs(sv_-v)<st.step*0.28 && sv_>=st.lo-1e-9 && sv_<=st.hi+1e-9;
  if(near){ var idx=-1; st.pts.forEach(function(p,i){ if(Math.abs(p.v-sv_)<1e-9) idx=i; });
    if(idx<0){ st.pts.push({v:Math.round(sv_*1e6)/1e6,closed:true}); st.sh={}; } else if(st.pts[idx].closed){ st.pts[idx].closed=false; } else { st.pts.splice(idx,1); st.sh={}; } }
  else { var P=st.pts.slice().sort(function(p,q){return p.v-q.v;}), i=0; while(i<P.length && P[i].v<v) i++; st.sh[i]=!st.sh[i]; }
  plwSave(w); }
/* ---- grid widget ---- */
function clipPoly(poly,a,b,c,ge){ var out=[], f=function(p){ var s=a*p[0]+b*p[1]-c; return ge? s>=-1e-9 : s<=1e-9; };
  for(var i=0;i<poly.length;i++){ var P=poly[i], Q=poly[(i+1)%poly.length], fp=f(P), fq=f(Q);
    if(fp) out.push(P); if(fp!==fq){ var sp=a*P[0]+b*P[1]-c, sq=a*Q[0]+b*Q[1]-c, t=sp/(sp-sq); out.push([P[0]+t*(Q[0]-P[0]),P[1]+t*(Q[1]-P[1])]); } } return out; }
function grLines(st){ return st.lines.map(function(L){ var a=L.p2[1]-L.p1[1], b=L.p1[0]-L.p2[0], c=a*L.p1[0]+b*L.p1[1]; return {a:a,b:b,c:c,L:L}; }); }
function grEncode(st){ var o=[]; var bad=false; grLines(st).forEach(function(q){ if(!q.L.side){ bad=true; return; } var s=q.a*q.L.side[0]+q.b*q.L.side[1]-q.c; if(Math.abs(s)<1e-9){ bad=true; return; }
    var op=s<0?(q.L.solid?'≤':'<'):(q.L.solid?'≥':'>'); o.push(hpFmtInt(q.a,q.b,q.c,op)); }); return (bad||!o.length)?'':o.join('; '); }
function grDraw(w){ var st=w._st, lo=st.lo, hi=st.hi, W=340, pad=18, S=(W-2*pad)/(hi-lo), X=function(x){return pad+(x-lo)*S;}, Y=function(y){return W-pad-(y-lo)*S;}, h='';
  var box=[[lo,lo],[hi,lo],[hi,hi],[lo,hi]], every=Math.max(1,Math.ceil((hi-lo)/12));
  for(var g=lo; g<=hi; g++){ var ax=(g===0); h+=sv('line',{x1:X(g),y1:Y(lo),x2:X(g),y2:Y(hi),style:'stroke:'+(ax?'var(--ink)':'var(--rule)')+';stroke-width:'+(ax?1.6:1)});
    h+=sv('line',{x1:X(lo),y1:Y(g),x2:X(hi),y2:Y(g),style:'stroke:'+(ax?'var(--ink)':'var(--rule)')+';stroke-width:'+(ax?1.6:1)});
    if(g!==0 && g%every===0 && lo<=0 && hi>=0){ h+='<text x="'+X(g)+'" y="'+(Y(0)+13)+'" text-anchor="middle" style="font:10px sans-serif;fill:var(--ink-soft)">'+String(g).replace('-','−')+'</text>';
      h+='<text x="'+(X(0)-4)+'" y="'+(Y(g)+3)+'" text-anchor="end" style="font:10px sans-serif;fill:var(--ink-soft)">'+String(g).replace('-','−')+'</text>'; } }
  if(lo<=0&&hi>=0){ h+='<text x="'+(X(hi)-2)+'" y="'+(Y(0)-5)+'" text-anchor="end" style="font:italic 13px serif;fill:var(--ink)">x</text><text x="'+(X(0)+6)+'" y="'+(Y(hi)+12)+'" style="font:italic 13px serif;fill:var(--ink)">y</text>'; }
  var Ls=grLines(st), inter=box.slice(), anySide=false, cols=['#2e86de','#e67e22','#8e44ad','#16a085','#c0392b'];
  Ls.forEach(function(q,i){ if(!q.L.side) return; anySide=true; var s=q.a*q.L.side[0]+q.b*q.L.side[1]-q.c, ge=s>0; var pl=clipPoly(box,q.a,q.b,q.c,ge); inter=clipPoly(inter,q.a,q.b,q.c,ge);
    if(pl.length>2) h+='<polygon points="'+pl.map(function(p){return X(p[0])+','+Y(p[1]);}).join(' ')+'" style="fill:'+cols[i%5]+';opacity:.13"/>'; });
  if(anySide && Ls.length>1 && inter.length>2) h+='<polygon points="'+inter.map(function(p){return X(p[0])+','+Y(p[1]);}).join(' ')+'" style="fill:var(--accent-text);opacity:.28"/>';
  if(st.key){ var K=hpList(st.key)||[], kin=box.slice(); K.forEach(function(k){ var ge=(k.op==='≥'||k.op==='>'); kin=clipPoly(kin,k.a,k.b,k.c,ge); });
    if(kin.length>2) h+='<polygon points="'+kin.map(function(p){return X(p[0])+','+Y(p[1]);}).join(' ')+'" style="fill:none;stroke:var(--success);stroke-width:3;stroke-dasharray:2 3"/>'; }
  Ls.forEach(function(q,i){ var seg=clipLine(q.a,q.b,q.c,lo,hi); if(!seg) return;
    h+=sv('line',{x1:X(seg[0][0]),y1:Y(seg[0][1]),x2:X(seg[1][0]),y2:Y(seg[1][1]),style:'stroke:'+cols[i%5]+';stroke-width:'+(i===st.sel?3.4:2.6)+(q.L.solid?'':';stroke-dasharray:8 6')});
    [q.L.p1,q.L.p2].forEach(function(p){ h+=sv('circle',{cx:X(p[0]),cy:Y(p[1]),r:4.5,style:'fill:'+cols[i%5]}); });
    if(q.L.side) h+='<text x="'+X(q.L.side[0])+'" y="'+(Y(q.L.side[1])+5)+'" text-anchor="middle" style="font:bold 15px sans-serif;fill:'+cols[i%5]+'">✓</text>'; });
  if(st.pend) h+=sv('circle',{cx:X(st.pend[0]),cy:Y(st.pend[1]),r:6,style:'fill:none;stroke:var(--danger);stroke-width:2.5'});
  w.querySelector('.plw-svg').innerHTML='<svg viewBox="0 0 '+W+' '+W+'" style="width:100%;max-width:460px;touch-action:manipulation">'+h+'</svg>';
  w._inv=function(px,py){ return [lo+(px-pad)/S, lo+(W-pad-py)/S]; }; w._W=W;
  var list=w.querySelector('.plw-list'); list.innerHTML=st.lines.map(function(L,i){ var q=Ls[i]; var eq=hpFmtInt(q.a,q.b,q.c,'=').replace(' = ',' = ');
    return '<div class="plw-row'+(i===st.sel?' sel':'')+'" data-i="'+i+'"><span class="plw-sw" style="background:'+cols[i%5]+'"></span><span class="plw-eq">'+eq+'</span>'+
      (st.ro?'':'<button type="button" data-a="style">'+(L.solid?'━ solid (≤, ≥)':'┅ dashed (<, >)')+'</button><button type="button" data-a="side">'+(L.side?'🎨 change side':'🎨 shade a side')+'</button><button type="button" data-a="del" aria-label="Delete line">✕</button>')+'</div>'; }).join('');
  var msg=w.querySelector('.plw-msg'); msg.textContent= st.ro?'':(st.pend?'Tap a second grid point on the line.':(st.mode==='side'?'Tap a point in the region you want to keep (not on the line).':(st.lines.length?'Tap two grid points to draw another boundary line, or adjust a line below.':'Tap two grid points to draw the boundary line.'))); }
function clipLine(a,b,c,lo,hi){ var P=[]; if(Math.abs(b)>1e-12){ [lo,hi].forEach(function(x){ var y=(c-a*x)/b; if(y>=lo-1e-9&&y<=hi+1e-9) P.push([x,y]); }); }
  if(Math.abs(a)>1e-12){ [lo,hi].forEach(function(y){ var x=(c-b*y)/a; if(x>=lo-1e-9&&x<=hi+1e-9) P.push([x,y]); }); }
  if(P.length<2) return null; var best=[P[0],P[1]], d=0; for(var i=0;i<P.length;i++) for(var j=i+1;j<P.length;j++){ var dd=Math.hypot(P[i][0]-P[j][0],P[i][1]-P[j][1]); if(dd>d){ d=dd; best=[P[i],P[j]]; } } return best; }
function grTap(w,ev){ var st=w._st; if(st.ro) return; var svg=w.querySelector('svg'), r=svg.getBoundingClientRect(); var p=w._inv((ev.clientX-r.left)*w._W/r.width,(ev.clientY-r.top)*w._W/r.width);
  if(st.mode==='side' && st.sel>=0 && st.lines[st.sel]){ var L=st.lines[st.sel]; var a=L.p2[1]-L.p1[1], b=L.p1[0]-L.p2[0], c=a*L.p1[0]+b*L.p1[1]; if(Math.abs(a*p[0]+b*p[1]-c)/Math.hypot(a,b)<0.15){ return; } L.side=[Math.round(p[0]*100)/100,Math.round(p[1]*100)/100]; st.mode='draw'; plwSave(w); return; }
  var g=[Math.round(p[0]),Math.round(p[1])]; if(g[0]<st.lo||g[0]>st.hi||g[1]<st.lo||g[1]>st.hi) return;
  if(!st.pend){ st.pend=g; grDraw(w); return; } if(g[0]===st.pend[0]&&g[1]===st.pend[1]){ st.pend=null; grDraw(w); return; }
  st.lines.push({p1:st.pend,p2:g,solid:true,side:null}); st.pend=null; st.sel=st.lines.length-1; st.mode='side'; plwSave(w); }
/* ---- wiring ---- */
function plwSave(w){ var st=w._st, enc; if(st.kind==='1d'){ enc=nlEncode(st); nlDraw(w); } else { enc=grEncode(st); grDraw(w); }
  var inp=w._inp; if(inp && !inp.disabled){ inp.value=enc; inp.dispatchEvent(new Event('input',{bubbles:true})); }
  try{ PLT[w._key]=JSON.stringify({pts:st.pts,sh:st.sh,lines:st.lines}); }catch(e){}
  var sm=w.querySelector('.plw-sum'); if(sm) sm.innerHTML= enc? 'Your graph shows: <b>'+esc(enc)+'</b>' : (st.kind==='2d'&&st.lines.length?'Shade a side for every line to finish.':''); }
function plwInit(){ document.querySelectorAll('.plotw').forEach(function(w){ if(w._st) return;
  var figd=w.closest('.fig'), line=figd&&figd.nextElementSibling, inp=line&&line.querySelector('.blank-input'); w._inp=inp||null;
  if(inp){ inp.setAttribute('tabindex','-1'); inp.setAttribute('inputmode','none'); inp.style.cssText='position:absolute;opacity:0;width:1px;height:1px;padding:0;border:0;pointer-events:none;'; }
  var kind=w.dataset.kind, st={kind:kind,lo:parseFloat(w.dataset.lo),hi:parseFloat(w.dataset.hi),step:parseFloat(w.dataset.step||'1'),pts:[],sh:{},lines:[],pend:null,sel:-1,mode:'draw',ro:!!(inp&&inp.disabled),key:null};
  w._st=st; w._key=MODE+'|'+activeTab+'|'+state.tabs[activeTab].idx+'|'+(inp?inp.dataset.step:'')+'|'+(w.dataset.id||'');
  var saved=PLT[w._key]; if(saved){ try{ var o=JSON.parse(saved); st.pts=o.pts||[]; st.sh=o.sh||{}; st.lines=o.lines||[]; }catch(e){} }
  else if(inp && inp.value){ if(kind==='1d'){ (ivParse(inp.value)||[]).forEach(function(t){ /* rebuild from value */ var i0=st.pts.length;
        if(isFinite(t.a)) st.pts.push({v:t.a,closed:t.ai}); if(isFinite(t.b)&&t.b!==t.a) st.pts.push({v:t.b,closed:t.bi}); });
      var P=st.pts.slice().sort(function(p,q){return p.v-q.v;}); st.pts=P; var L=ivParse(inp.value)||[]; for(var i=0;i<=P.length;i++){ var m=(i===0?(P.length?P[0].v-1:0):(i===P.length?P[i-1].v+1:(P[i-1].v+P[i].v)/2)); st.sh[i]=L.some(function(t){ return m>t.a&&m<t.b; }); } } }
  if(st.ro && inp && w.dataset.key){ var ok=(kind==='1d'?ivEq:hpEq)(inp.value,w.dataset.key); if(!ok) st.key=w.dataset.key; }
  if(MODE==='quiz') st.key=null;
  w.innerHTML='<div class="plw-svg"></div>'+(kind==='2d'?'<div class="plw-list"></div><div class="plw-msg"></div>':'<div class="plw-msg">'+(st.ro?'':'Tap a number to place an endpoint (tap again: ● closed → ○ open → remove). Tap a part of the line to shade it.')+'</div>')+
    (st.ro?'':'<div class="plw-tools"><button type="button" data-a="undo">↩ Undo</button><button type="button" data-a="clear">🗑 Clear</button></div>')+'<div class="plw-sum"></div>'+(st.key?'<div class="plw-key">Correct graph shown in <b style="color:var(--success)">green</b>: '+esc(w.dataset.key)+'</div>':'');
  w._hist=[];
  w.addEventListener('click',function(ev){ var b=ev.target.closest('button[data-a]'); if(!b) return; ev.preventDefault(); var a=b.dataset.a;
    if(a==='clear'){ st.pts=[]; st.sh={}; st.lines=[]; st.pend=null; st.sel=-1; st.mode='draw'; plwSave(w); return; }
    if(a==='undo'){ if(kind==='1d'){ st.pts.pop(); st.sh={}; } else { if(st.pend) st.pend=null; else st.lines.pop(); st.sel=st.lines.length-1; st.mode='draw'; } plwSave(w); return; }
    var row=b.closest('.plw-row'); if(!row) return; var i=parseInt(row.dataset.i,10); st.sel=i;
    if(a==='style'){ st.lines[i].solid=!st.lines[i].solid; plwSave(w); }
    if(a==='side'){ st.mode='side'; grDraw(w); }
    if(a==='del'){ st.lines.splice(i,1); st.sel=st.lines.length-1; st.mode='draw'; plwSave(w); } });
  w.querySelector('.plw-svg').addEventListener('click',function(ev){ if(kind==='1d') nlTap(w,ev); else grTap(w,ev); });
  if(kind==='1d') nlDraw(w); else grDraw(w); plwSave0(w); }); }
function plwSave0(w){ var st=w._st, enc=st.kind==='1d'?nlEncode(st):grEncode(st); var sm=w.querySelector('.plw-sum'); if(sm&&enc&&(st.pts.length||st.lines.length)) sm.innerHTML='Your graph shows: <b>'+esc(enc)+'</b>'; }
(function(){ var _rs=renderSlide; renderSlide=function(){ _rs.apply(this,arguments); try{ if(document.querySelector('#wrap .plotw')){ plwInit();
  var sl=SLIDES[activeTab][state.tabs[activeTab].idx]; if(sl&&sl.flat&&sl.flat.every(function(s){ return !s.expr||s.expr==='plot1'||s.expr==='plot2'; })) document.querySelectorAll('#wrap .quiz-hint').forEach(function(q){ if(/Type expressions/.test(q.textContent)) q.remove(); }); } }catch(e){ console.log('plot',e); } }; })();


/* ================= v6: helpers ================= */
function v6Correct(tab,i){ var it=state.tabs[tab].items[i]; if(MODE==='quiz'){ try{ return isSlideCorrect(tab,i); }catch(e){ return false; } } var c=v4Class(it); return c==='c1'||c==='c2'; }
function v6Stats(tab){ var ts=state.tabs[tab]; if(!ts||!ts.items) return null; var sl=SLIDES[tab]||[], o={n:ts.items.length,ans:0,ok:0,c1:0,c2:0,w:0,sk:0,wrong:[],byKind:{mcq:[0,0],step:[0,0],plot:[0,0]},stepFail:{first:0,mid:0,last:0}};
  ts.items.forEach(function(it,i){ var s=sl[i]||{}, kind=s.kind==='mcq'||s.kind==='ar'?'mcq':((s.flat||[]).some(function(f){return f.expr==='plot1'||f.expr==='plot2';})?'plot':'step');
    if(MODE==='quiz'){ var att=false; try{ att=isSlideAttempted(tab,i); }catch(e){} if(!att) return; o.ans++; var ok=v6Correct(tab,i); if(ok) o.ok++; else o.wrong.push(i); o.byKind[kind][0]++; if(ok) o.byKind[kind][1]++; return; }
    var c=v4Class(it); if(c==='un') return; if(c==='sk'){ o.sk++; return; } o.ans++; o.byKind[kind][0]++;
    if(c==='c1'){ o.c1++; o.ok++; o.byKind[kind][1]++; } else if(c==='c2'){ o.c2++; o.ok++; o.byKind[kind][1]++; } else { o.w++; o.wrong.push(i); }
    if(it.stepStates&&it.stepStates.length>1){ var L=it.stepStates.length; it.stepStates.forEach(function(ss,k){ if(ss.status==='revealed'||(ss.attempts||0)>0){ if(k===0) o.stepFail.first++; else if(k===L-1) o.stepFail.last++; else o.stepFail.mid++; } }); } });
  o.acc=o.ans?Math.round(o.ok/o.ans*100):null; o.first=o.ans?Math.round(o.c1/o.ans*100):null; return o; }
function v6Qtabs(){ return TAB_DEFS.filter(function(t){ return SLIDES[t.id]&&SLIDES[t.id].length; }); }

/* ================= v6: accuracy meter ================= */
(function(){ var sp=document.querySelector('.slide-progress'); if(!sp) return; var m=document.createElement('div'); m.id='accMeter'; m.className='accm'; sp.parentNode.insertBefore(m, sp.nextSibling); })();
function v6Gauge(p){ var r=26, cx=32, cy=32, a=Math.PI*(1-(p||0)/100), x=cx+r*Math.cos(a), y=cy-r*Math.sin(a), col=p===null?'var(--rule)':(p>=75?'var(--success)':p>=50?'var(--gold)':'var(--danger)');
  return '<svg viewBox="0 0 64 38" class="accg"><path d="M6 32 A26 26 0 0 1 58 32" style="fill:none;stroke:var(--rule);stroke-width:7;stroke-linecap:round"/>'+(p?'<path d="M6 32 A26 26 0 0 1 '+x.toFixed(1)+' '+y.toFixed(1)+'" style="fill:none;stroke:'+col+';stroke-width:7;stroke-linecap:round"/>':'')+
    '<line x1="32" y1="32" x2="'+(cx+20*Math.cos(a)).toFixed(1)+'" y2="'+(cy-20*Math.sin(a)).toFixed(1)+'" style="stroke:var(--ink);stroke-width:2.5;stroke-linecap:round"/><circle cx="32" cy="32" r="3.5" style="fill:var(--ink)"/></svg>'; }
function v6Meter(){ var m=document.getElementById('accMeter'); if(!m) return; var tab=activeTab, sl=SLIDES[tab];
  if(!MODE||!sl||!sl.length||!state.tabs[tab]){ m.style.display='none'; return; } m.style.display='';
  var o=v6Stats(tab); var all={ans:0,ok:0}; v6Qtabs().forEach(function(t){ var s=v6Stats(t.id); if(s){ all.ans+=s.ans; all.ok+=s.ok; } });
  var chap=all.ans?Math.round(all.ok/all.ans*100):null;
  if(MODE==='quiz'){ m.innerHTML=v6Gauge(null)+'<div class="acct"><b>🎯 Accuracy</b><span>Quiz mode: answered '+o.ans+' of '+o.n+' — your accuracy appears when you finish this sheet.</span></div>'; return; }
  var p=o.acc, lab=p===null?'—':p+'%', col=p===null?'':(p>=75?'g':p>=50?'o':'r');
  m.innerHTML=v6Gauge(p)+'<div class="acct"><b>🎯 Accuracy <span class="accp '+col+'">'+lab+'</span></b><span>'+(o.ans?o.ok+' of '+o.ans+' right · '+o.c1+' on the first try':'Answer a question to start the meter')+(chap!==null?' · Chapter '+chap+'%':'')+'</span></div>'; }
(function(){ var _rs=renderSlide; renderSlide=function(){ _rs.apply(this,arguments); try{ v6Meter(); }catch(e){} }; })();
(function(){ var _sc=showChrome; showChrome=function(show){ _sc(show); var m=document.getElementById('accMeter'); if(m&&!show) m.style.display='none'; }; })();

/* ================= v6: observations on the finished card ================= */
function v6NoteFor(tab){ var b=null, sec=null; try{ var tmp=document.createElement('div'); tmp.innerHTML=(typeof THEORY!=='undefined'?THEORY:''); b=tmp.querySelector('section [data-go="'+tab+'"]'); }catch(e){}
  if(b) sec=b.closest('section'); return sec&&sec.id?sec.id:null; }
function v6Observe(){ var done=document.querySelector('#wrap .done-card'); if(!done||done.dataset.v6) return; done.dataset.v6='1';
  var tab=activeTab, o=v6Stats(tab); if(!o||!o.ans) return; var first=(student&&student.name)?String(student.name).split(' ')[0]:'You';
  var tdef=TAB_DEFS.find(function(t){return t.id===tab;})||{label:''}, acc=o.acc, lvl, lvlc;
  if(acc>=90){ lvl='Excellent understanding — this topic is mastered'; lvlc='g'; } else if(acc>=75){ lvl='Strong understanding — just a few points to polish'; lvlc='g'; } else if(acc>=50){ lvl='Developing understanding — the basics are in place'; lvlc='o'; } else { lvl='Building understanding — a little more practice will make it click'; lvlc='r'; }
  var pos=[], grow=[], rev=[];
  // positive diagnostic remarks
  if(MODE!=='quiz' && o.first>=70) pos.push('Your first-try accuracy of <b>'+o.first+'%</b> shows you understood the method before checking.');
  if(MODE!=='quiz' && o.c2>0) pos.push('You corrected <b>'+o.c2+'</b> answer'+(o.c2>1?'s':'')+' on the second try — spotting and fixing your own mistakes is a great habit.');
  var K={mcq:'multiple-choice reasoning',step:'step-by-step working',plot:'plotting graphs'}, best=null, worst=null;
  Object.keys(o.byKind).forEach(function(k){ var v=o.byKind[k]; if(v[0]<2) return; var r=v[1]/v[0]; if(!best||r>best.r) best={k:k,r:r}; if(!worst||r<worst.r) worst={k:k,r:r}; });
  if(best && best.r>=0.6) pos.push('A real strength: <b>'+K[best.k]+'</b> ('+Math.round(best.r*100)+'% correct).');
  if(o.sk===0 && o.ans===o.n) pos.push('You attempted every question in the sheet — excellent persistence.');
  if(acc>=90) pos.push('You are ready to move on to the next sheet with confidence.');
  if(!pos.length) pos.push('You finished the whole sheet, '+esc(first)+' — finishing is the first step to mastering it. Every question you worked through added to your understanding.');
  // growth areas
  if(worst && best && worst.k!==best.k && worst.r<0.6) grow.push('Practise more <b>'+K[worst.k]+'</b> ('+Math.round(worst.r*100)+'% correct so far).');
  var sf=o.stepFail, tot=sf.first+sf.mid+sf.last; if(MODE!=='quiz' && tot>=2){ var mx=Math.max(sf.first,sf.mid,sf.last);
    if(mx===sf.first) grow.push('Most slips happened in the <b>first step</b> — re-read the question and set up the method carefully before calculating.');
    else if(mx===sf.last) grow.push('Most slips happened in the <b>final step</b> — the method was right; check the last simplification or rounding.');
    else grow.push('Most slips happened in the <b>middle steps</b> — write each line of working fully and check signs and arithmetic.'); }
  if(o.wrong.length) grow.push('Have another look at '+(o.wrong.length>1?'these questions':'this question')+': '+o.wrong.slice(0,10).map(function(i){ return '<button type="button" class="v6q" data-q="'+i+'">Q'+(i+1)+'</button>'; }).join(' ')+(o.wrong.length>10?' …':''));
  if(o.sk) grow.push('Come back to the <b>'+o.sk+'</b> skipped question'+(o.sk>1?'s':'')+' when you are ready.');
  // review suggestions
  var nid=v6NoteFor(tab); if(acc<75 && nid) rev.push('<button type="button" class="v6r" data-n="'+nid+'">📖 Re-read the notes for '+esc(tdef.label)+'</button>');
  var tabs=v6Qtabs(), ci=tabs.findIndex(function(t){return t.id===tab;}), weakPrev=[];
  for(var j=0;j<ci;j++){ var t=tabs[j]; if(/^Assessment|Test|Report/i.test(t.label)) continue; var s=v6Stats(t.id); if(s&&s.ans&&s.acc<60) weakPrev.push({t:t,a:s.acc}); else if(acc<60 && j===ci-1 && (!s||!s.ans)) weakPrev.push({t:t,a:null}); }
  weakPrev.slice(-3).forEach(function(w){ rev.push('<button type="button" class="v6t" data-t="'+w.t.id+'">🔁 Review '+esc(w.t.label)+(w.a!==null?' (you scored '+w.a+'%)':' (not attempted yet)')+'</button>'); });
  var revTxt = rev.length? '<div class="v6sub">Suggested review</div><div class="v6btns">'+rev.join('')+'</div>' : '<div class="v6sub">Suggested review</div><p class="v6p">'+(acc>=75?'No earlier topics need review — you are ready for the next sheet.':'Re-try the questions above, then move on.')+'</p>';
  var box=document.createElement('div'); box.className='v6obs';
  box.innerHTML='<div class="v6h">📝 Teacher’s observations</div><div class="v6lvl '+lvlc+'">'+lvl+' · <b>'+acc+'%</b> accuracy</div>'+
    '<div class="v6sub">What went well</div><ul class="v6ul">'+pos.map(function(x){return '<li>'+x+'</li>';}).join('')+'</ul>'+
    (grow.length?'<div class="v6sub">Next steps</div><ul class="v6ul">'+grow.map(function(x){return '<li>'+x+'</li>';}).join('')+'</ul>':'')+revTxt;
  var ban=done.querySelector('.v4ban'); if(ban&&ban.nextSibling) done.insertBefore(box, ban.nextSibling); else done.appendChild(box);
  box.addEventListener('click',function(ev){ var b=ev.target.closest('button'); if(!b) return;
    if(b.dataset.q!==undefined){ var ts=state.tabs[tab]; ts.idx=parseInt(b.dataset.q,10); ts.recorded=false; showChrome(true); buildTabbar(); renderSlide(); window.scrollTo({top:0,behavior:'smooth'}); }
    else if(b.dataset.t){ activeTab=b.dataset.t; showChrome(true); buildTabbar(); renderSlide(); window.scrollTo({top:0,behavior:'smooth'}); }
    else if(b.dataset.n){ var th=TAB_DEFS.find(function(t){return t.id==='theory';}); if(th){ activeTab='theory'; showChrome(true); buildTabbar(); renderSlide(); setTimeout(function(){ var el=document.getElementById(b.dataset.n); if(el) el.scrollIntoView({behavior:'smooth',block:'start'}); },80); } } });
  try{ if(records[0]&&records[0].tab===tab){ records[0].obs=lvl.split(' — ')[0]; saveState(); } }catch(e){}
}
(function(){ var _rf=renderFinished; renderFinished=function(){ _rf.apply(this,arguments); try{ v6Observe(); }catch(e){ console.log('v6',e); } }; })();

/* ================= v6: whiteboard ================= */
var WB={on:false,pages:[[]],pg:0,tool:'pen',color:'#1f2937',size:4,bg:'grid',redo:[],cur:null,cv:null,ctx:null,w0:0};
var WB_COLS=['#1f2937','#2563eb','#dc2626','#16a34a','#ea580c','#9333ea','#db2777','#ffffff'];
function wbKey(){ try{ return 'sopaan-wb::'+document.title+'::'+(student?student.name+'#'+student.roll:'')+'::'+MODE+'|'+activeTab+'|'+((state.tabs[activeTab]||{}).idx||0); }catch(e){ return 'sopaan-wb'; } }
function wbLoad(){ WB.pages=[[]]; WB.pg=0; WB.redo=[]; WB.w0=0; try{ var s=localStorage.getItem(wbKey()); if(s){ var o=JSON.parse(s); if(o&&o.pages){ WB.pages=o.pages; WB.pg=Math.min(o.pg||0,WB.pages.length-1); WB.bg=o.bg||'grid'; WB.w0=o.w0||0; } } }catch(e){} }
function wbStore(){ try{ localStorage.setItem(wbKey(), JSON.stringify({pages:WB.pages,pg:WB.pg,bg:WB.bg,w0:WB.w0})); }catch(e){} }
function wbBuild(){ if(document.getElementById('wbOv')) return; var d=document.createElement('div'); d.id='wbOv'; d.className='wbov';
  var tools=[['pen','✏️','Pen'],['hl','🖍️','Highlighter'],['er','🧽','Eraser'],['line','／','Line'],['arrow','➚','Arrow'],['rect','▭','Rectangle'],['ell','◯','Circle'],['text','T','Text']];
  d.innerHTML='<div class="wbbar"><button type="button" data-a="close" class="wbx" title="Close">✕ Close</button><span class="wbsep"></span>'+tools.map(function(t){ return '<button type="button" class="wbt" data-tool="'+t[0]+'" title="'+t[2]+'">'+t[1]+'</button>'; }).join('')+
    '<span class="wbsep"></span>'+WB_COLS.map(function(c){ return '<button type="button" class="wbc" data-col="'+c+'" style="background:'+c+'" title="Colour"></button>'; }).join('')+
    '<span class="wbsep"></span><input type="range" min="1" max="24" value="4" class="wbsz" title="Size"><span class="wbsep"></span>'+
    '<button type="button" data-a="undo" title="Undo">↶</button><button type="button" data-a="redo" title="Redo">↷</button><button type="button" data-a="bg" title="Background">▦</button><button type="button" data-a="clear" title="Clear page">🗑</button>'+
    '<span class="wbsep"></span><button type="button" data-a="prev" title="Previous page">◀</button><span class="wbpg"></span><button type="button" data-a="next" title="Next / new page">▶</button>'+
    '<span class="wbsep"></span><button type="button" data-a="save" title="Save as picture">💾</button></div><div class="wbbody"><div class="wbq"><div class="wbqh"><b>📌 Question</b><button type="button" class="wbqt">Hide question</button></div><div class="wbqc"></div></div><canvas class="wbcv"></canvas></div>';
  document.body.appendChild(d); d.querySelector('.wbqt').addEventListener('click',function(){ var q=d.querySelector('.wbq'); q.classList.toggle('min'); this.textContent=q.classList.contains('min')?'Show question':'Hide question'; setTimeout(function(){ wbSize(); wbDraw(); },20); });
  WB.cv=d.querySelector('canvas.wbcv'); WB.ctx=WB.cv.getContext('2d');
  d.querySelector('.wbbar').addEventListener('click',function(ev){ var b=ev.target.closest('button'); if(!b) return;
    if(b.dataset.tool){ WB.tool=b.dataset.tool; wbUI(); return; } if(b.dataset.col){ WB.color=b.dataset.col; wbUI(); return; }
    var a=b.dataset.a, P=WB.pages[WB.pg];
    if(a==='undo'&&P.length){ WB.redo.push(P.pop()); } else if(a==='redo'&&WB.redo.length){ P.push(WB.redo.pop()); } else if(a==='clear'&&P.length){ WB.pages[WB.pg]=[]; WB.redo=[]; }
    else if(a==='bg'){ WB.bg={grid:'lines',lines:'plain',plain:'grid'}[WB.bg]; } else if(a==='prev'&&WB.pg>0){ WB.pg--; WB.redo=[]; } else if(a==='next'){ WB.pg++; if(WB.pg>=WB.pages.length) WB.pages.push([]); WB.redo=[]; }
    else if(a==='save'){ try{ var l=document.createElement('a'); l.download='whiteboard-page-'+(WB.pg+1)+'.png'; l.href=wbExport(); l.click(); }catch(e){} }
    else if(a==='close'){ wbToggle(false); return; }
    wbStore(); wbDraw(); wbUI(); });
  d.querySelector('.wbsz').addEventListener('input',function(){ WB.size=parseInt(this.value,10); });
  var cv=WB.cv; cv.addEventListener('pointerdown',wbDown); cv.addEventListener('pointermove',wbMove); cv.addEventListener('pointerup',wbUp); cv.addEventListener('pointercancel',wbUp);
  window.addEventListener('resize',function(){ if(WB.on){ wbSize(); wbDraw(); } }); }
function wbUI(){ var d=document.getElementById('wbOv'); if(!d) return; d.querySelectorAll('.wbt').forEach(function(b){ b.classList.toggle('on',b.dataset.tool===WB.tool); }); d.querySelectorAll('.wbc').forEach(function(b){ b.classList.toggle('on',b.dataset.col===WB.color); }); d.querySelector('.wbpg').textContent=(WB.pg+1)+' / '+WB.pages.length; }
function wbSize(){ var cv=WB.cv, r=cv.getBoundingClientRect(), dpr=window.devicePixelRatio||1; cv.width=Math.round(r.width*dpr); cv.height=Math.round(r.height*dpr); WB.ctx.setTransform(dpr,0,0,dpr,0,0); if(!WB.w0) WB.w0=r.width; WB.sc=r.width/WB.w0; }
function wbP(e){ var r=WB.cv.getBoundingClientRect(); return [(e.clientX-r.left)/WB.sc,(e.clientY-r.top)/WB.sc]; }
function wbDown(e){ e.preventDefault(); var p=wbP(e);
  if(WB.tool==='text'){ wbText(p); return; } WB.cv.setPointerCapture(e.pointerId);
  WB.cur={t:WB.tool,c:WB.color,s:WB.tool==='hl'?Math.max(12,WB.size*3):(WB.tool==='er'?Math.max(18,WB.size*4):WB.size),pts:[p],a:p,b:p}; }
function wbMove(e){ if(!WB.cur) return; var p=wbP(e); if(WB.cur.t==='pen'||WB.cur.t==='hl'||WB.cur.t==='er') WB.cur.pts.push(p); else WB.cur.b=p; wbDraw(); }
function wbUp(){ if(!WB.cur) return; WB.pages[WB.pg].push(WB.cur); WB.cur=null; WB.redo=[]; wbStore(); wbDraw(); }
function wbText(p){ var d=document.getElementById('wbOv'), r=WB.cv.getBoundingClientRect(); var inp=document.createElement('input'); inp.className='wbin'; inp.placeholder='Type, then Enter';
  inp.style.left=(r.left+p[0]*WB.sc)+'px'; inp.style.top=(r.top+p[1]*WB.sc-14)+'px'; inp.style.color=WB.color; d.appendChild(inp); inp.focus(); setTimeout(function(){ inp.focus(); },60);
  var fin=function(){ if(inp._d) return; inp._d=1; var v=inp.value.trim(); inp.remove(); if(v){ WB.pages[WB.pg].push({t:'text',c:WB.color,s:Math.max(24,WB.size*5),a:p,str:v}); WB.redo=[]; wbStore(); wbDraw(); } };
  inp.addEventListener('keydown',function(ev){ if(ev.key==='Enter') fin(); if(ev.key==='Escape'){ inp.value=''; fin(); } }); setTimeout(function(){ inp.addEventListener('blur',fin); },300); }
function wbShape(c,o){ var k=WB.sc; c.save(); c.lineCap='round'; c.lineJoin='round'; c.strokeStyle=c.fillStyle=o.c; c.lineWidth=o.s*k; c.globalAlpha=o.t==='hl'?0.35:1; c.globalCompositeOperation=o.t==='er'?'destination-out':'source-over';
  if(o.t==='pen'||o.t==='hl'||o.t==='er'){ c.beginPath(); o.pts.forEach(function(p,i){ if(i) c.lineTo(p[0]*k,p[1]*k); else c.moveTo(p[0]*k,p[1]*k); }); if(o.pts.length===1) c.lineTo(o.pts[0][0]*k+0.1,o.pts[0][1]*k); c.stroke(); }
  else if(o.t==='line'||o.t==='arrow'){ c.beginPath(); c.moveTo(o.a[0]*k,o.a[1]*k); c.lineTo(o.b[0]*k,o.b[1]*k); c.stroke(); if(o.t==='arrow'){ var an=Math.atan2(o.b[1]-o.a[1],o.b[0]-o.a[0]), h=(10+o.s*2)*k; c.beginPath(); c.moveTo(o.b[0]*k,o.b[1]*k); c.lineTo(o.b[0]*k-h*Math.cos(an-0.45),o.b[1]*k-h*Math.sin(an-0.45)); c.lineTo(o.b[0]*k-h*Math.cos(an+0.45),o.b[1]*k-h*Math.sin(an+0.45)); c.closePath(); c.fill(); } }
  else if(o.t==='rect'){ c.strokeRect(o.a[0]*k,o.a[1]*k,(o.b[0]-o.a[0])*k,(o.b[1]-o.a[1])*k); }
  else if(o.t==='ell'){ c.beginPath(); c.ellipse((o.a[0]+o.b[0])/2*k,(o.a[1]+o.b[1])/2*k,Math.abs(o.b[0]-o.a[0])/2*k,Math.abs(o.b[1]-o.a[1])/2*k,0,0,Math.PI*2); c.stroke(); }
  else if(o.t==='text'){ c.font=(o.s*k)+'px "Source Sans 3",sans-serif'; c.textBaseline='middle'; c.fillText(o.str,o.a[0]*k,o.a[1]*k); }
  c.restore(); }
function wbBg(c,W,H,bg){ c.fillStyle='#ffffff'; c.fillRect(0,0,W,H); if(bg==='plain') return; c.strokeStyle=bg==='grid'?'#e5e7eb':'#dbeafe'; c.lineWidth=1; var g=28*WB.sc; c.beginPath(); for(var y=g;y<H;y+=g){ c.moveTo(0,y); c.lineTo(W,y); } if(bg==='grid') for(var x=g;x<W;x+=g){ c.moveTo(x,0); c.lineTo(x,H); } c.stroke(); }
function wbDraw(){ var c=WB.ctx, r=WB.cv.getBoundingClientRect(), W=r.width, H=r.height; c.clearRect(0,0,W,H);
  var ink=document.createElement('canvas'), dpr=window.devicePixelRatio||1; ink.width=WB.cv.width; ink.height=WB.cv.height; var ic=ink.getContext('2d'); ic.setTransform(dpr,0,0,dpr,0,0);
  WB.pages[WB.pg].concat(WB.cur?[WB.cur]:[]).forEach(function(o){ wbShape(ic,o); });
  wbBg(c,W,H,WB.bg); c.save(); c.setTransform(1,0,0,1,0,0); c.drawImage(ink,0,0); c.restore(); }
function wbExport(){ return WB.cv.toDataURL('image/png'); }
function wbFillQ(){ var d=document.getElementById('wbOv'); if(!d) return; var box=d.querySelector('.wbq'), c=d.querySelector('.wbqc'), q=document.querySelector('#wrap .qcard');
  if(!q){ box.style.display='none'; return; } box.style.display='';
  var cl=q.cloneNode(true); cl.removeAttribute('id'); cl.querySelectorAll('[id]').forEach(function(e){ e.removeAttribute('id'); });
  cl.querySelectorAll('input,button,select,textarea').forEach(function(e){ e.setAttribute('tabindex','-1'); e.disabled=true; });
  cl.querySelectorAll('.feedback,.step-badge,.quiz-hint,.plw-tools,.plw-msg').forEach(function(e){ e.remove(); });
  cl.querySelectorAll('canvas').forEach(function(e){ e.remove(); });
  c.innerHTML=''; c.appendChild(cl); var tdef=(TAB_DEFS.find(function(t){return t.id===activeTab;})||{}).label||''; var h=d.querySelector('.wbqh b'); if(h) h.textContent='📌 '+tdef+' · Question '+(((state.tabs[activeTab]||{}).idx||0)+1); }
function wbToggle(on){ WB.on=(on===undefined)?!WB.on:on; wbBuild(); var d=document.getElementById('wbOv'); d.classList.toggle('show',WB.on); document.body.classList.toggle('wb-open',WB.on);
  if(WB.on){ wbLoad(); wbFillQ(); setTimeout(function(){ wbSize(); wbDraw(); wbUI(); },30); } }
(function(){ var f=document.createElement('button'); f.type='button'; f.id='wbFab'; f.className='wb-fab'; f.innerHTML='🧑‍🏫 <span>Whiteboard</span>'; f.title='Open the whiteboard'; f.addEventListener('click',function(){ wbToggle(true); }); document.body.appendChild(f); })();
(function(){ var _rs=renderSlide; renderSlide=function(){ _rs.apply(this,arguments); var f=document.getElementById('wbFab'); if(f) f.style.display=MODE?'':'none'; }; })();


/* ================= v7: scatter-graph plotter ================= */
var SCT={};
function scPts(s){ s=String(s||'').trim(); if(!s) return []; return s.split(/\s*;\s*/).filter(Boolean).map(function(p){ var a=p.replace(/[()]/g,'').split(/\s*,\s*/); return [parseFloat(a[0]),parseFloat(a[1])]; }).filter(function(p){ return isFinite(p[0])&&isFinite(p[1]); }); }
function scEqPts(inp,key,tolx,toly){ var A=scPts(inp),B=scPts(key); if(!A.length||A.length!==B.length) return false; var used=B.map(function(){return false;});
  return A.every(function(p){ for(var j=0;j<B.length;j++){ if(!used[j]&&Math.abs(p[0]-B[j][0])<=tolx+1e-9&&Math.abs(p[1]-B[j][1])<=toly+1e-9){ used[j]=true; return true; } } return false; }); }
function scLine(s){ var m=String(s||'').match(/^line:\(([^,]+),([^)]+)\)-\(([^,]+),([^)]+)\)/); if(!m) return null; var x1=+m[1],y1=+m[2],x2=+m[3],y2=+m[4]; if(Math.abs(x2-x1)<1e-9) return null; var k=(y2-y1)/(x2-x1); return {m:k,c:y1-k*x1}; }
(function(){ var _am=answerMatches; answerMatches=function(input,answer,accept,expr){
  if(expr==='spts'||expr==='slbf'){ if(input===undefined||input===null||String(input).trim()==='') return false;
    var meta=String((accept&&accept[0])||''); var mm=meta.match(/tol:([\d.]+),([\d.]+)/), tx=mm?+mm[1]:0.5, ty=mm?+mm[2]:0.5;
    if(expr==='spts') return scEqPts(input,answer,tx,ty);
    if(String(input).trim()===String(answer).trim()) return true;
    var L=scLine(input), k=String(answer).split(','), m=+k[0], c=+k[1], tol=+k[2], xa=+k[3], xb=+k[4]; if(!L) return false;
    return [xa,xb].every(function(x){ return Math.abs((L.m*x+L.c)-(m*x+c))<=tol; }); }
  return _am.apply(this,arguments); }; })();
function scDraw(w){ var st=w._st, W=360, H=300, L=52, R=14, T=14, B=44, X=function(x){ return L+(x-st.xlo)/(st.xhi-st.xlo)*(W-L-R); }, Y=function(y){ return H-B-(y-st.ylo)/(st.yhi-st.ylo)*(H-T-B); }, h='';
  function line(x1,y1,x2,y2,sty){ return '<line x1="'+x1.toFixed(1)+'" y1="'+y1.toFixed(1)+'" x2="'+x2.toFixed(1)+'" y2="'+y2.toFixed(1)+'" style="'+sty+'"/>'; }
  var fmt=function(v){ var a=Math.abs(v); return (a>=10000? (v/1000)+'k' : String(Math.round(v*100)/100)).replace('-','−'); };
  if(st.xminor) for(var x=st.xlo;x<=st.xhi+1e-9;x+=st.xminor) h+=line(X(x),Y(st.ylo),X(x),Y(st.yhi),'stroke:var(--rule);stroke-width:.6');
  if(st.yminor) for(var y=st.ylo;y<=st.yhi+1e-9;y+=st.yminor) h+=line(X(st.xlo),Y(y),X(st.xhi),Y(y),'stroke:var(--rule);stroke-width:.6');
  for(var x2=st.xlo;x2<=st.xhi+1e-9;x2+=st.xstep){ h+=line(X(x2),Y(st.ylo),X(x2),Y(st.yhi),'stroke:var(--rule);stroke-width:1.2'); h+='<text x="'+X(x2).toFixed(1)+'" y="'+(H-B+15)+'" text-anchor="middle" style="font:11px sans-serif;fill:var(--ink-soft)">'+fmt(x2)+'</text>'; }
  for(var y2=st.ylo;y2<=st.yhi+1e-9;y2+=st.ystep){ h+=line(X(st.xlo),Y(y2),X(st.xhi),Y(y2),'stroke:var(--rule);stroke-width:1.2'); h+='<text x="'+(L-5)+'" y="'+(Y(y2)+4).toFixed(1)+'" text-anchor="end" style="font:11px sans-serif;fill:var(--ink-soft)">'+fmt(y2)+'</text>'; }
  h+=line(X(st.xlo),Y(st.ylo),X(st.xhi),Y(st.ylo),'stroke:var(--ink);stroke-width:1.6')+line(X(st.xlo),Y(st.ylo),X(st.xlo),Y(st.yhi),'stroke:var(--ink);stroke-width:1.6');
  h+='<text x="'+((L+W-R)/2)+'" y="'+(H-6)+'" text-anchor="middle" style="font:600 12.5px sans-serif;fill:var(--ink)">'+esc(st.xlab)+'</text>';
  h+='<text transform="translate(13,'+((T+H-B)/2)+') rotate(-90)" text-anchor="middle" style="font:600 12.5px sans-serif;fill:var(--ink)">'+esc(st.ylab)+'</text>';
  if(st.line){ var a=st.line, xs=[st.xlo,st.xhi].map(function(x){ return [x,a[0]*x+a[1]]; }); h+='<g clip-path="url(#scclip'+w._n+')">'+line(X(xs[0][0]),Y(xs[0][1]),X(xs[1][0]),Y(xs[1][1]),'stroke:var(--accent-text);stroke-width:2')+'</g>'; }
  function cross(px,py,col,sz){ return line(px-sz,py-sz,px+sz,py+sz,'stroke:'+col+';stroke-width:2.4')+line(px-sz,py+sz,px+sz,py-sz,'stroke:'+col+';stroke-width:2.4'); }
  st.fixed.forEach(function(p){ h+=cross(X(p[0]),Y(p[1]),'var(--ink)',4.5); });
  if(st.key){ if(st.mode==='spts') scPts(st.key).forEach(function(p){ h+='<circle cx="'+X(p[0]).toFixed(1)+'" cy="'+Y(p[1]).toFixed(1)+'" r="8" style="fill:none;stroke:var(--success);stroke-width:2.5"/>'; });
    else { var k=st.key.split(',').map(Number); h+='<g clip-path="url(#scclip'+w._n+')">'+line(X(k[3]),Y(k[0]*k[3]+k[1]),X(k[4]),Y(k[0]*k[4]+k[1]),'stroke:var(--success);stroke-width:3;stroke-dasharray:6 5')+'</g>'; } }
  st.pts.forEach(function(p){ h+=cross(X(p[0]),Y(p[1]),'var(--danger)',6); });
  if(st.mode==='slbf'){ if(st.lp.length===2){ var P=st.lp, k2=(P[1][1]-P[0][1])/(P[1][0]-P[0][0]||1e-9), c2=P[0][1]-k2*P[0][0];
      var ya=k2*st.xlo+c2, yb=k2*st.xhi+c2; h+='<g clip-path="url(#scclip'+w._n+')">'+line(X(st.xlo),Y(ya),X(st.xhi),Y(yb),'stroke:var(--danger);stroke-width:2.6')+'</g>'; }
    st.lp.forEach(function(p){ h+='<circle cx="'+X(p[0]).toFixed(1)+'" cy="'+Y(p[1]).toFixed(1)+'" r="5" style="fill:var(--danger)"/>'; }); }
  w.querySelector('.scw-svg').innerHTML='<svg viewBox="0 0 '+W+' '+H+'" style="width:100%;max-width:520px;touch-action:manipulation;overflow:hidden"><clipPath id="scclip'+w._n+'"><rect x="'+L+'" y="'+T+'" width="'+(W-L-R)+'" height="'+(H-T-B)+'"/></clipPath>'+h+'</svg>';
  w._inv=function(px,py){ return [st.xlo+(px-L)/(W-L-R)*(st.xhi-st.xlo), st.ylo+(H-B-py)/(H-T-B)*(st.yhi-st.ylo)]; }; w._W=W; w._H=H; }
function scEnc(st){ if(st.mode==='spts') return st.pts.map(function(p){ return p[0]+','+p[1]; }).join('; ');
  if(st.lp.length<2) return ''; return 'line:('+st.lp[0][0]+','+st.lp[0][1]+')-('+st.lp[1][0]+','+st.lp[1][1]+')'; }
function scSave(w){ var st=w._st, enc=scEnc(st); scDraw(w); var inp=w._inp; if(inp&&!inp.disabled){ inp.value=enc; inp.dispatchEvent(new Event('input',{bubbles:true})); }
  try{ SCT[w._key]=JSON.stringify({pts:st.pts,lp:st.lp}); }catch(e){}
  var sm=w.querySelector('.scw-sum'); if(sm) sm.innerHTML= st.mode==='spts' ? (st.pts.length?'Points plotted: <b>'+st.pts.length+'</b>':'') : (st.lp.length===2?'Line drawn — tap ↩ Undo to move it.':(st.lp.length?'Tap a second point on your line.':'')); }
function scTap(w,ev){ var st=w._st; if(st.ro) return; var svg=w.querySelector('svg'), r=svg.getBoundingClientRect(), p=w._inv((ev.clientX-r.left)*w._W/r.width,(ev.clientY-r.top)*w._H/r.height);
  if(p[0]<st.xlo||p[0]>st.xhi||p[1]<st.ylo||p[1]>st.yhi) return;
  var q=[Math.round(p[0]/st.xsnap)*st.xsnap, Math.round(p[1]/st.ysnap)*st.ysnap]; q=[+q[0].toFixed(6),+q[1].toFixed(6)];
  if(st.mode==='spts'){ var i=st.pts.findIndex(function(a){ return Math.abs(a[0]-q[0])<1e-9&&Math.abs(a[1]-q[1])<1e-9; }); if(i>=0) st.pts.splice(i,1); else st.pts.push(q); }
  else { if(st.lp.length>=2) st.lp=[]; if(!(st.lp.length===1&&Math.abs(st.lp[0][0]-q[0])<1e-9)) st.lp.push(q); }
  scSave(w); }
var SCN=0;
function scInit(){ document.querySelectorAll('.scatw').forEach(function(w){ if(w._st) return; w._n=++SCN;
  var figd=w.closest('.fig'), line=figd&&figd.nextElementSibling, inp=(w.dataset.mode&&line)?line.querySelector('.blank-input'):null; w._inp=inp||null;
  if(inp){ inp.setAttribute('tabindex','-1'); inp.setAttribute('inputmode','none'); inp.style.cssText='position:absolute;opacity:0;width:1px;height:1px;padding:0;border:0;pointer-events:none;'; }
  var D=w.dataset, num=function(k,d){ var v=parseFloat(D[k]); return isFinite(v)?v:d; };
  var st={mode:D.mode||'',xlo:num('xlo',0),xhi:num('xhi',10),xstep:num('xstep',1),xminor:num('xminor',0),ylo:num('ylo',0),yhi:num('yhi',10),ystep:num('ystep',1),yminor:num('yminor',0),
    xsnap:num('xsnap',num('xminor',0)||num('xstep',1)),ysnap:num('ysnap',num('yminor',0)||num('ystep',1)),xlab:D.xlab||'',ylab:D.ylab||'',fixed:scPts(D.pts),line:D.line?D.line.split(',').map(Number):null,pts:[],lp:[],ro:!!(inp&&inp.disabled),key:null};
  w._st=st; w._key=MODE+'|'+activeTab+'|'+state.tabs[activeTab].idx+'|'+(inp?inp.dataset.step:'')+'|'+(D.id||'');
  var sv=SCT[w._key]; if(sv){ try{ var o=JSON.parse(sv); st.pts=o.pts||[]; st.lp=o.lp||[]; }catch(e){} }
  else if(inp&&inp.value){ if(st.mode==='spts') st.pts=scPts(inp.value); else { var m=inp.value.match(/^line:\(([^,]+),([^)]+)\)-\(([^,]+),([^)]+)\)/); if(m) st.lp=[[+m[1],+m[2]],[+m[3],+m[4]]]; } }
  if(st.ro && inp && D.key && MODE!=='quiz'){ if(!answerMatches(inp.value,D.key,D.meta?[D.meta]:[],st.mode)) st.key=D.key; }
  var tip=st.mode==='spts'?'Tap the grid to plot each point (tap a point again to remove it).':(st.mode==='slbf'?'Tap two points to draw your line of best fit (tap again to start over).':'');
  w.innerHTML='<div class="scw-svg"></div>'+(st.mode&&!st.ro?'<div class="plw-msg">'+tip+'</div><div class="plw-tools"><button type="button" data-a="undo">↩ Undo</button><button type="button" data-a="clear">🗑 Clear</button></div>':'')+'<div class="scw-sum"></div>'+(st.key?'<div class="plw-key">Correct answer shown in <b style="color:var(--success)">green</b>.</div>':'');
  w.addEventListener('click',function(ev){ var b=ev.target.closest('button[data-a]'); if(!b) return; ev.preventDefault(); if(b.dataset.a==='clear'){ st.pts=[]; st.lp=[]; } else { if(st.mode==='spts') st.pts.pop(); else st.lp.pop(); } scSave(w); });
  if(st.mode) w.querySelector('.scw-svg').addEventListener('click',function(ev){ scTap(w,ev); });
  scDraw(w); var sm=w.querySelector('.scw-sum'); if(sm&&st.mode==='spts'&&st.pts.length) sm.innerHTML='Points plotted: <b>'+st.pts.length+'</b>'; }); }
(function(){ var _rs=renderSlide; renderSlide=function(){ _rs.apply(this,arguments); try{ if(document.querySelector('#wrap .scatw')){ scInit();
  var sl=SLIDES[activeTab][state.tabs[activeTab].idx]; if(sl&&sl.flat&&sl.flat.every(function(s){ return !s.expr||s.expr==='spts'||s.expr==='slbf'||s.expr==='plot1'||s.expr==='plot2'; })) document.querySelectorAll('#wrap .quiz-hint').forEach(function(q){ if(/Type expressions/.test(q.textContent)) q.remove(); }); } }catch(e){ console.log('scat',e); } }; })();


/* ================= calculus answer mode ================= */
function calcCompile(src){
  var s=String(src).replace(/\s+/g,'').replace(/[×∗·]/g,'*').replace(/÷/g,'/').replace(/[−–—]/g,'-')
    .replace(/²/g,'^(2)').replace(/³/g,'^(3)').replace(/π/g,'#').replace(/θ/g,'q').replace(/eˣ/g,'e^x');
  if(s.indexOf('=')>=0) s=s.slice(s.lastIndexOf('=')+1);
  var FN=['sqrt','cbrt','abs','ln','log','exp','sin','cos','tan','sec','csc','cot','pi'];
  var i=0,toks=[];
  while(i<s.length){
    var ch=s[i];
    if(/[0-9.]/.test(ch)){ var j=i; while(j<s.length&&/[0-9.]/.test(s[j])) j++; toks.push({k:'n',v:parseFloat(s.slice(i,j))}); i=j; continue; }
    if(ch==='√'){ toks.push({k:'f',v:'sqrt'}); i++; continue; }
    if(ch==='∛'){ toks.push({k:'f',v:'cbrt'}); i++; continue; }
    if(/[a-zA-Z#]/.test(ch)){
      var hit=null; for(var q=0;q<FN.length;q++){ if(s.substr(i,FN[q].length).toLowerCase()===FN[q]){ hit=FN[q]; break; } }
      if(hit==='pi'){ toks.push({k:'v',v:'#'}); i+=2; continue; }
      if(hit){ toks.push({k:'f',v:hit}); i+=hit.length; continue; }
      toks.push({k:'v',v:ch}); i++; continue; }
    if('+-*/^()|'.indexOf(ch)>=0){ toks.push({k:ch}); i++; continue; }
    return null;
  }
  // absolute value bars -> abs( )
  var t2=[],open=false; for(var a=0;a<toks.length;a++){ var tk=toks[a]; if(tk.k==='|'){ if(!open){ t2.push({k:'f',v:'abs'}); t2.push({k:'('}); open=true; } else { t2.push({k:')'}); open=false; } } else t2.push(tk); }
  toks=t2;
  var out=[];
  for(var t=0;t<toks.length;t++){ var A=toks[t], B=out[out.length-1];
    if(B&&(B.k==='n'||B.k==='v'||B.k===')')&&(A.k==='n'||A.k==='v'||A.k==='('||A.k==='f')) out.push({k:'&'});
    out.push(A); }
  var p=0; function pk(){ return out[p]; }
  var F={sqrt:Math.sqrt,cbrt:Math.cbrt,ln:Math.log,log:function(x){return Math.log(x)/Math.LN10;},exp:Math.exp,sin:Math.sin,cos:Math.cos,tan:Math.tan,
    sec:function(x){return 1/Math.cos(x);},csc:function(x){return 1/Math.sin(x);},cot:function(x){return 1/Math.tan(x);},abs:Math.abs};
  function E(){ var n=T(); while(pk()&&(pk().k==='+'||pk().k==='-')){ var o=out[p++].k,r=T(); n=(function(l,r,o){return function(e){return o==='+'?l(e)+r(e):l(e)-r(e);};})(n,r,o);} return n; }
  function T(){ var n=I(); while(pk()&&(pk().k==='*'||pk().k==='/')){ var o=out[p++].k,r=I(); n=(function(l,r,o){return function(e){return o==='*'?l(e)*r(e):l(e)/r(e);};})(n,r,o);} return n; }
  function I(){ var n=U(); while(pk()&&pk().k==='&'){ p++; var r=P(); n=(function(l,r){return function(e){return l(e)*r(e);};})(n,r);} return n; }
  function U(){ if(pk()&&pk().k==='-'){ p++; var u=U(); return function(e){return -u(e);}; } if(pk()&&pk().k==='+'){ p++; return U(); } return P(); }
  function P(){ var b=Aa(); if(pk()&&pk().k==='^'){ p++; var x=U(); return function(e){return Math.pow(b(e),x(e));}; } return b; }
  function Aa(){ var t=out[p++]; if(!t) throw 0;
    if(t.k==='n') return function(){return t.v;};
    if(t.k==='v'){ if(t.v==='#') return function(){return Math.PI;}; if(t.v==='e') return function(){return Math.E;}; return function(e){return e[t.v];}; }
    if(t.k==='('){ var n=E(); if(!pk()||pk().k!==')') throw 0; p++; return n; }
    if(t.k==='f'){ var fn=F[t.v]; var ex=null;
      if(pk()&&pk().k==='^'){ p++; ex=Aa(); if(pk()&&pk().k==='&') p++; }            // sin^2(x)
      var arg; if(pk()&&pk().k==='('){ p++; arg=E(); if(!pk()||pk().k!==')') throw 0; p++; } else { arg=P(); while(pk()&&pk().k==='&'&&out[p+1]&&(out[p+1].k==='n'||(out[p+1].k==='v'&&out[p+1].v!=='e'))){ p++; var nx=P(); arg=(function(l,r){return function(e){return l(e)*r(e);};})(arg,nx); } }
      return ex? function(e){ return Math.pow(fn(arg(e)),ex(e)); } : function(e){ return fn(arg(e)); }; }
    throw 0; }
  try{ var f=E(); if(p!==out.length) return null; return f; }catch(e){ return null; }
}
function calcEqual(input,answer){
  var f=calcCompile(input), g=calcCompile(answer); if(!f||!g) return false;
  var hits=0;
  for(var trial=0;trial<14;trial++){
    var env={}; 'abcdfghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'.split('').forEach(function(c){ env[c]=0.35+Math.random()*2.3; });
    var x=f(env), y=g(env); if(!isFinite(x)||!isFinite(y)) continue;
    if(Math.abs(x-y)>1e-6*Math.max(1,Math.abs(x),Math.abs(y))) return false; hits++;
  }
  return hits>=4;
}
(function(){
  var _am=answerMatches;
  answerMatches=function(input,answer,accept,expr){
    if(expr==='expanded'){ if(input===undefined||input===null||String(input).trim()==='') return false; if(/[()\[\]]/.test(String(input))) return false; return _am.call(this,input,answer,accept,true); }
    if(expr==='calc'){ if(input===undefined||input===null||String(input).trim()==='') return false;
      if(calcEqual(input,answer)) return true; return (accept||[]).some(function(a){ return calcEqual(input,a); }); }
    return _am.apply(this,arguments); };
  var _kl=kbLayoutFor;
  kbLayoutFor=function(inp){ try{ var ts=state.tabs[activeTab], sl=SLIDES[activeTab][ts.idx], stp=sl.flat[parseInt(inp.dataset.step,10)]; if(stp.expr==='calc') return 'calc'; }catch(e){} return _kl(inp); };
  var _kp=kbPress;
  kbPress=function(k){ var m={'eˣ':'e^(','√':'√(','ln':'ln(','sin':'sin(','cos':'cos(','tan':'tan(','sec':'sec(','csc':'csc(','cot':'cot(','∛':'∛('}; if(KB.page==='calc'&&m[k]){ kbInsert(m[k]); return; } return _kp(k); };
})();


/* ================= v5: interactive plotting ================= */
var GP={};
function gpNum(s){ s=String(s).trim().replace(/[−–]/g,'-'); var m=s.match(/^(-?\d+(?:\.\d+)?)\/(\d+(?:\.\d+)?)$/); if(m) return parseFloat(m[1])/parseFloat(m[2]); var m2=s.match(/^(-?)(\d+) (\d+)\/(\d+)$/); if(m2) return (m2[1]?-1:1)*(+m2[2]+m2[3]/m2[4]); var v=parseFloat(s); return isFinite(v)&&/^-?\d*\.?\d+$/.test(s)?v:NaN; }
function gpIneq(src){ // -> {f:function(x,y), op:'<'|'<='|'>'|'>=', a,b,c} with f = lhs-rhs
  var s=String(src).replace(/≤/g,'<=').replace(/≥/g,'>=').replace(/\s+/g,'').replace(/−/g,'-');
  var m=s.match(/^(.*?)(<=|>=|<|>)(.*)$/); if(!m) return null;
  var L=calcCompile(m[1]), R=calcCompile(m[3]); if(!L||!R) return null;
  var f=function(x,y){ return L({x:x,y:y})-R({x:x,y:y}); };
  var d=f(0,0), a=f(1,0)-d, b=f(0,1)-d; return {f:f,op:m[2],a:a,b:b,c:-d,src:src};
}
function gpOpTxt(op){ return {'<':'<','<=':'≤','>':'>','>=':'≥'}[op]; }
function gpSat(I,x,y){ var v=I.f(x,y); if(I.op==='<') return v<-1e-9; if(I.op==='<=') return v<=1e-9; if(I.op==='>') return v>1e-9; return v>=-1e-9; }
function gpParseG(v){ var m=String(v||'').match(/^G:(-?[\d.]+),(-?[\d.]+);(-?[\d.]+),(-?[\d.]+);([sd]);(-?[\d.]+),(-?[\d.]+)$/); if(!m) return null;
  return {p:[[+m[1],+m[2]],[+m[3],+m[4]]], solid:m[5]==='s', sh:[+m[6],+m[7]]}; }
function gpParseN(v){ var m=String(v||'').match(/^N:([^;]+);([^;]+);([LRBO])$/); if(!m) return null;
  var vs=m[1].split(',').map(gpNum), cs=m[2].split(','); if(vs.some(isNaN)) return null; return {v:vs, c:cs.map(function(c){return c==='c';}), mode:m[3]}; }
function gpOpt(accept,pre){ var r=null; (accept||[]).forEach(function(a){ if(String(a).indexOf(pre)===0) r=String(a).slice(pre.length); }); return r; }
function gpCheckG(input,answer,accept){
  var I=gpIneq(gpOpt(accept,'INEQ:')||''), S=gpParseG(input); if(!I||!S) return false;
  var p=S.p; if(Math.abs(p[0][0]-p[1][0])<1e-9&&Math.abs(p[0][1]-p[1][1])<1e-9) return false;
  var tol=1e-7*Math.max(1,Math.abs(I.a),Math.abs(I.b),Math.abs(I.c));
  if(Math.abs(I.f(p[0][0],p[0][1]))>tol||Math.abs(I.f(p[1][0],p[1][1]))>tol) return false;
  var strict=(I.op==='<'||I.op==='>'); if(S.solid===strict) return false;
  if(Math.abs(I.f(S.sh[0],S.sh[1]))<tol) return false;
  return gpSat(I,S.sh[0],S.sh[1]);
}
function gpCheckN(input,answer){
  var S=gpParseN(input), K=gpParseN(answer); if(!S||!K) return false;
  if(S.mode!==K.mode||S.v.length!==K.v.length) return false;
  var sv=S.v.slice(), sc=S.c.slice(); if(sv.length===2&&sv[0]>sv[1]){ sv.reverse(); sc.reverse(); }
  for(var i=0;i<sv.length;i++){ if(Math.abs(sv[i]-K.v[i])>1e-6||sc[i]!==K.c[i]) return false; }
  return true;
}
function gpHumanG(v){ var S=gpParseG(v); if(!S) return v||'—'; return 'boundary through ('+S.p[0]+') and ('+S.p[1]+'), '+(S.solid?'solid':'dashed')+', shaded on the side of ('+S.sh+')'; }
function gpHumanN(v){ var S=gpParseN(v); if(!S) return v||'—'; var d=function(i){ return (S.c[i]?'closed':'open')+' dot at '+S.v[i]; };
  if(S.mode==='L') return d(0)+', shaded to the left'; if(S.mode==='R') return d(0)+', shaded to the right';
  return d(0)+' and '+d(1)+', shaded '+(S.mode==='B'?'between them':'outside them'); }
(function(){
  var _am=answerMatches;
  answerMatches=function(input,answer,accept,expr){
    if(expr==='gplot') return gpCheckG(input,answer,accept);
    if(expr==='nplot') return gpCheckN(input,answer);
    return _am.apply(this,arguments); };
  var _sat=slideAnswerText;
  slideAnswerText=function(slide,item,correctSide){
    if(slide.kind!=='blank'||!slide.flat.some(function(s){return s.expr==='gplot'||s.expr==='nplot';})) return _sat.apply(this,arguments);
    return slide.flat.map(function(step,si){ var ss=item.stepStates[si];
      return Object.keys(step.a).map(function(k){
        if(step.expr==='gplot') return correctSide ? 'the graph of '+(gpOpt(step.accept,'INEQ:')||'').replace(/<=/g,'≤').replace(/>=/g,'≥') : gpHumanG(ss.inputs[k]);
        if(step.expr==='nplot') return correctSide ? gpHumanN(step.a[k])+((gpOpt(step.accept,'INEQ:'))?' ('+gpOpt(step.accept,'INEQ:').replace(/<=/g,'≤').replace(/>=/g,'≥')+')':'') : gpHumanN(ss.inputs[k]);
        return correctSide ? step.a[k] : (ss.inputs[k] || '—'); }).join(', '); }).join('  |  ');
  };
  var _rs=renderSlide;
  renderSlide=function(){ _rs.apply(this,arguments); try{ gpEnhance(); grInitAll(); }catch(e){ console.log('gp',e); } };
})();
function gpStep(inp){ try{ var ts=state.tabs[activeTab], sl=SLIDES[activeTab][ts.idx]; return sl.flat[parseInt(inp.dataset.step,10)]; }catch(e){ return null; } }
function gpEnhance(){
  document.querySelectorAll('.blank-input').forEach(function(inp){
    var st=gpStep(inp); if(!st||(st.expr!=='gplot'&&st.expr!=='nplot')||inp.dataset.gp) return; inp.dataset.gp='1';
    inp.classList.add('gp-hidden'); inp.setAttribute('tabindex','-1'); inp.setAttribute('aria-hidden','true');
    var box=document.createElement('div'); box.className='gp-box';
    var line=inp.closest('.step-line'); (line||inp.parentNode).appendChild(box);
    var ts=state.tabs[activeTab], item=ts.items[ts.idx], ss=item.stepStates?item.stepStates[parseInt(inp.dataset.step,10)]:null;
    var done=inp.disabled, revealed=ss&&ss.status==='revealed';
    if(st.expr==='gplot') gpBuildG(box,inp,st,done,revealed); else gpBuildN(box,inp,st,done,revealed);
    var rn=line&&line.nextElementSibling; if(rn&&rn.classList.contains('reveal-note')){ var iq=gpOpt(st.accept,'INEQ:'); rn.textContent='Correct graph'+(iq?' of '+iq.replace(/<=/g,'≤').replace(/>=/g,'≥'):'')+' shown in green.'; }
  });
}
function gpKey(inp){ return (MODE||'')+'|'+activeTab+'|'+state.tabs[activeTab].idx+'|'+inp.dataset.step; }
function gpSet(inp,v){ inp.value=v; inp.dispatchEvent(new Event('input',{bubbles:true})); }
/* ---------- coordinate-plane widget ---------- */
function gpRange(st,def){ var r=gpOpt(st.accept,'R:'); if(!r) return def; var a=r.split(',').map(Number); return a.length>=2&&a.every(isFinite)?a:def; }
function gpClipHalf(poly,a,b,c,keepPos){ // keep points with s*(a x + b y - c) >= 0
  var s=keepPos?1:-1, out=[]; for(var i=0;i<poly.length;i++){ var P=poly[i], Q=poly[(i+1)%poly.length];
    var fp=s*(a*P[0]+b*P[1]-c), fq=s*(a*Q[0]+b*Q[1]-c);
    if(fp>=0) out.push(P); if((fp>=0)!==(fq>=0)){ var t=fp/(fp-fq); out.push([P[0]+t*(Q[0]-P[0]),P[1]+t*(Q[1]-P[1])]); } } return out; }
function gpBuildG(box,inp,st,done,revealed){
  var R=gpRange(st,[-8,8,-8,8]), x0=R[0],x1=R[1],y0=R[2],y1=R[3], W=320, H=Math.round(320*(y1-y0)/(x1-x0)), pad=0;
  var X=function(x){ return (x-x0)/(x1-x0)*W; }, Y=function(y){ return H-(y-y0)/(y1-y0)*H; };
  var S=gpParseG(inp.value)||{p:[],solid:true,sh:null}; if(!gpParseG(inp.value)){ if(GP[gpKey(inp)]) S=JSON.parse(JSON.stringify(GP[gpKey(inp)])); }
  var I=gpIneq(gpOpt(st.accept,'INEQ:')||'');
  box.innerHTML='<div class="gp-help">'+(done?'Your graph':'① Tap two grid points on the boundary line · ② choose Solid or Dashed · ③ tap the side to shade')+'</div>'+
    '<svg class="gp-svg" viewBox="-14 -14 '+(W+28)+' '+(H+28)+'" style="max-width:100%;touch-action:manipulation"></svg>'+
    (done?'':'<div class="gp-tools"><button type="button" data-k="s" class="gp-b">━ Solid (≤, ≥)</button><button type="button" data-k="d" class="gp-b">┅ Dashed (&lt;, &gt;)</button><button type="button" data-k="u" class="gp-b">↶ Undo</button><button type="button" data-k="c" class="gp-b">Clear</button></div>')+
    '<div class="gp-stat"></div>';
  var svg=box.querySelector('svg'), stat=box.querySelector('.gp-stat');
  function lineSeg(a,b,c){ // endpoints of a x + b y = c inside box
    var pts=[], add=function(x,y){ if(x>=x0-1e-9&&x<=x1+1e-9&&y>=y0-1e-9&&y<=y1+1e-9&&!pts.some(function(p){return Math.abs(p[0]-x)<1e-9&&Math.abs(p[1]-y)<1e-9;})) pts.push([x,y]); };
    if(Math.abs(b)>1e-12){ add(x0,(c-a*x0)/b); add(x1,(c-a*x1)/b); } if(Math.abs(a)>1e-12){ add((c-b*y0)/a,y0); add((c-b*y1)/a,y1); } return pts.slice(0,2); }
  function region(a,b,c,keepPos,fill){ var poly=gpClipHalf([[x0,y0],[x1,y0],[x1,y1],[x0,y1]],a,b,c,keepPos); if(poly.length<3) return '';
    return '<polygon points="'+poly.map(function(p){return X(p[0]).toFixed(1)+','+Y(p[1]).toFixed(1);}).join(' ')+'" style="fill:'+fill+';opacity:.28"/>'; }
  function draw(){
    var h='', i;
    for(i=Math.ceil(x0);i<=x1;i++) h+='<line x1="'+X(i)+'" y1="0" x2="'+X(i)+'" y2="'+H+'" style="stroke:var(--rule);stroke-width:'+(i===0?0:1)+'"/>';
    for(i=Math.ceil(y0);i<=y1;i++) h+='<line x1="0" y1="'+Y(i)+'" x2="'+W+'" y2="'+Y(i)+'" style="stroke:var(--rule);stroke-width:'+(i===0?0:1)+'"/>';
    if(x0<0&&x1>0) h+='<line x1="'+X(0)+'" y1="0" x2="'+X(0)+'" y2="'+H+'" style="stroke:var(--ink);stroke-width:1.6"/>';
    if(y0<0&&y1>0) h+='<line x1="0" y1="'+Y(0)+'" x2="'+W+'" y2="'+Y(0)+'" style="stroke:var(--ink);stroke-width:1.6"/>';
    var step=(x1-x0)>12?2:1; for(i=Math.ceil(x0);i<=x1;i++) if(i!==0&&i%step===0) h+='<text x="'+X(i)+'" y="'+(Y(0)+13)+'" text-anchor="middle" style="font:10px sans-serif;fill:var(--ink-soft)">'+String(i).replace('-','−')+'</text>';
    for(i=Math.ceil(y0);i<=y1;i++) if(i!==0&&i%step===0) h+='<text x="'+(X(0)-5)+'" y="'+(Y(i)+3.5)+'" text-anchor="end" style="font:10px sans-serif;fill:var(--ink-soft)">'+String(i).replace('-','−')+'</text>';
    h+='<text x="'+(W+4)+'" y="'+(Y(0)-4)+'" style="font:italic 12px serif;fill:var(--ink)">x</text><text x="'+(X(0)+5)+'" y="-3" style="font:italic 12px serif;fill:var(--ink)">y</text>';
    if(S.p.length===2){ var P=S.p, a=P[1][1]-P[0][1], b=P[0][0]-P[1][0], c=a*P[0][0]+b*P[0][1];
      if(Math.abs(a)>1e-12||Math.abs(b)>1e-12){
        if(S.sh){ var keep=(a*S.sh[0]+b*S.sh[1]-c)>0; h+=region(a,b,c,keep,'var(--accent-text)'); }
        var sg2=lineSeg(a,b,c); if(sg2.length===2) h+='<line x1="'+X(sg2[0][0])+'" y1="'+Y(sg2[0][1])+'" x2="'+X(sg2[1][0])+'" y2="'+Y(sg2[1][1])+'" style="stroke:var(--accent-text);stroke-width:2.6;'+(S.solid?'':'stroke-dasharray:8 6')+'"/>'; } }
    if((done||revealed)&&revealed&&I){ // correct answer in green
      var keepPos=I.op==='>'||I.op==='>='; h+=region(I.a,I.b,I.c,keepPos,'var(--success)'); var sg=lineSeg(I.a,I.b,I.c);
      if(sg.length===2) h+='<line x1="'+X(sg[0][0])+'" y1="'+Y(sg[0][1])+'" x2="'+X(sg[1][0])+'" y2="'+Y(sg[1][1])+'" style="stroke:var(--success);stroke-width:3;'+((I.op==='<'||I.op==='>')?'stroke-dasharray:8 6':'')+'"/>'; }
    S.p.forEach(function(p){ h+='<circle cx="'+X(p[0])+'" cy="'+Y(p[1])+'" r="5.5" style="fill:var(--danger)"/>'; });
    if(S.sh) h+='<text x="'+X(S.sh[0])+'" y="'+(Y(S.sh[1])+5)+'" text-anchor="middle" style="font:700 15px sans-serif;fill:var(--accent-text)">✚</text>';
    h+='<rect x="0" y="0" width="'+W+'" height="'+H+'" style="fill:transparent;stroke:var(--ink-soft);stroke-width:1" class="gp-hit"/>';
    svg.innerHTML=h;
    var msg = S.p.length<2 ? 'Point '+(S.p.length+1)+' of 2: tap a grid point on the boundary line.' : (!S.sh ? 'Line: '+(S.solid?'solid':'dashed')+'. Now tap a point on the side to shade.' : 'Boundary through ('+S.p[0]+') and ('+S.p[1]+'), '+(S.solid?'solid':'dashed')+', shaded side marked ✚. Press Check.');
    if(!done) stat.textContent=msg; else stat.textContent=S.p.length===2&&S.sh?gpHumanG(inp.value):'';
  }
  function save(){ GP[gpKey(inp)]=JSON.parse(JSON.stringify(S)); if(S.p.length===2&&S.sh) gpSet(inp,'G:'+S.p[0]+';'+S.p[1]+';'+(S.solid?'s':'d')+';'+S.sh); else gpSet(inp,''); }
  if(!done){
    svg.addEventListener('click',function(e){ var r=svg.getBoundingClientRect(), vb=svg.viewBox.baseVal, sx=(e.clientX-r.left)/r.width*vb.width+vb.x, sy=(e.clientY-r.top)/r.height*vb.height+vb.y;
      var x=x0+sx/W*(x1-x0), y=y0+(H-sy)/H*(y1-y0); if(x<x0-0.3||x>x1+0.3||y<y0-0.3||y>y1+0.3) return;
      if(S.p.length<2){ var gx=Math.round(x), gy=Math.round(y); if(S.p.length===1&&S.p[0][0]===gx&&S.p[0][1]===gy) return; S.p.push([gx,gy]); S.sh=null; }
      else { S.sh=[Math.round(x*2)/2,Math.round(y*2)/2]; var a=S.p[1][1]-S.p[0][1], b=S.p[0][0]-S.p[1][0], c=a*S.p[0][0]+b*S.p[0][1]; if(Math.abs(a*S.sh[0]+b*S.sh[1]-c)<1e-9){ S.sh=[Math.round(x*4)/4,Math.round(y*4)/4]; if(Math.abs(a*S.sh[0]+b*S.sh[1]-c)<1e-9) S.sh=null; } }
      save(); draw(); });
    box.querySelectorAll('.gp-b').forEach(function(b){ b.addEventListener('click',function(){ var k=b.dataset.k;
      if(k==='s') S.solid=true; else if(k==='d') S.solid=false; else if(k==='c'){ S={p:[],solid:S.solid,sh:null}; } else if(k==='u'){ if(S.sh) S.sh=null; else S.p.pop(); }
      box.querySelectorAll('.gp-b[data-k=s],.gp-b[data-k=d]').forEach(function(x){ x.classList.toggle('on',(x.dataset.k==='s')===S.solid); });
      save(); draw(); }); });
    box.querySelectorAll('.gp-b[data-k=s],.gp-b[data-k=d]').forEach(function(x){ x.classList.toggle('on',(x.dataset.k==='s')===S.solid); });
  }
  draw();
}
/* ---------- number-line widget ---------- */
function gpBuildN(box,inp,st,done,revealed){
  var R=gpRange(st,[-8,8]), lo=R[0], hi=R[1], W=320, H=70, X=function(v){ return 14+(v-lo)/(hi-lo)*(W-28); };
  var S=gpParseN(inp.value)||{v:[],c:[],mode:''}; var draft={v:['',''],c:['c','c'],n:1,mode:''};
  if(gpParseN(inp.value)){ var T=gpParseN(inp.value); draft.n=T.v.length; draft.v=[String(T.v[0]),T.v[1]!==undefined?String(T.v[1]):'']; draft.c=[T.c[0]?'c':'o',T.c[1]?'c':'o']; draft.mode=T.mode; }
  else { if(GP[gpKey(inp)]) draft=JSON.parse(JSON.stringify(GP[gpKey(inp)])); }
  var K=gpParseN(st.a[Object.keys(st.a)[0]]);
  box.innerHTML='<div class="gp-help">'+(done?'Your number line':'Choose 1 or 2 endpoints, type each value, pick open ○ / closed ● dots and the shading')+'</div>'+
    '<svg class="gp-svg" viewBox="0 0 '+W+' '+H+'" style="max-width:100%"></svg>'+
    (done?'':'<div class="gp-tools gp-n">'+
      '<span class="gp-lab">Endpoints:</span><button type="button" class="gp-b" data-n="1">1</button><button type="button" class="gp-b" data-n="2">2</button><br>'+
      '<span class="gp-lab">A =</span><input class="gp-in" data-i="0" inputmode="decimal" placeholder="value"><button type="button" class="gp-b" data-ci="0" data-c="o">○ open</button><button type="button" class="gp-b" data-ci="0" data-c="c">● closed</button><br>'+
      '<span class="gp-row2"><span class="gp-lab">B =</span><input class="gp-in" data-i="1" inputmode="decimal" placeholder="value"><button type="button" class="gp-b" data-ci="1" data-c="o">○ open</button><button type="button" class="gp-b" data-ci="1" data-c="c">● closed</button><br></span>'+
      '<span class="gp-lab">Shade:</span><span class="gp-sh1"><button type="button" class="gp-b" data-m="L">← left</button><button type="button" class="gp-b" data-m="R">right →</button></span><span class="gp-sh2"><button type="button" class="gp-b" data-m="B">between</button><button type="button" class="gp-b" data-m="O">outside</button></span></div>')+
    '<div class="gp-stat"></div>';
  var svg=box.querySelector('svg'), stat=box.querySelector('.gp-stat');
  function seg(a,b,col,y){ return '<line x1="'+X(a)+'" y1="'+y+'" x2="'+X(b)+'" y2="'+y+'" style="stroke:'+col+';stroke-width:5;stroke-linecap:round;opacity:.85"/>'; }
  function arrowTo(v,dir,col,y){ var e=dir<0?lo:hi; return seg(v,e,col,y)+'<path d="M'+X(e)+' '+y+' l'+(dir<0?8:-8)+' -6 v12 z" style="fill:'+col+'"/>'; }
  function dot(v,closed,col,y){ return '<circle cx="'+X(v)+'" cy="'+y+'" r="6" style="fill:'+(closed?col:'var(--card)')+';stroke:'+col+';stroke-width:2.4"/>'; }
  function paint(T,col,y){ if(!T) return ''; var h='', v=T.v.slice(), c=T.c.slice(); if(v.length===2&&v[0]>v[1]){ v.reverse(); c.reverse(); }
    if(T.mode==='L') h+=arrowTo(v[0],-1,col,y); else if(T.mode==='R') h+=arrowTo(v[0],1,col,y); else if(T.mode==='B') h+=seg(v[0],v[1],col,y); else if(T.mode==='O') h+=arrowTo(v[0],-1,col,y)+arrowTo(v[1],1,col,y);
    v.forEach(function(x,i){ h+=dot(x,c[i],col,y); }); return h; }
  function cur(){ var vs=draft.v.slice(0,draft.n).map(gpNum); if(vs.some(isNaN)||!draft.mode) return null; if(draft.n===1&&'LR'.indexOf(draft.mode)<0) return null; if(draft.n===2&&'BO'.indexOf(draft.mode)<0) return null;
    return {v:vs,c:draft.c.slice(0,draft.n).map(function(x){return x==='c';}),mode:draft.mode}; }
  function draw(){
    var h='<line x1="6" y1="40" x2="'+(W-6)+'" y2="40" style="stroke:var(--ink);stroke-width:1.6"/><path d="M'+(W-6)+' 40 l-8 -5 v10z M6 40 l8 -5 v10z" style="fill:var(--ink)"/>';
    var step=(hi-lo)>16?2:1; for(var i=Math.ceil(lo);i<=hi;i++){ h+='<line x1="'+X(i)+'" y1="35" x2="'+X(i)+'" y2="45" style="stroke:var(--ink);stroke-width:1"/>'; if(i%step===0) h+='<text x="'+X(i)+'" y="60" text-anchor="middle" style="font:11px sans-serif;fill:var(--ink-soft)">'+String(i).replace('-','−')+'</text>'; }
    if(revealed&&K) h+=paint(K,'var(--success)',22);
    var T=done?gpParseN(inp.value):cur(); h+=paint(T,'var(--accent-text)',40); svg.innerHTML=h;
    if(!done){ box.querySelectorAll('.gp-b[data-n]').forEach(function(b){ b.classList.toggle('on',+b.dataset.n===draft.n); });
      box.querySelector('.gp-row2').style.display=draft.n===2?'':'none'; box.querySelector('.gp-sh1').style.display=draft.n===1?'':'none'; box.querySelector('.gp-sh2').style.display=draft.n===2?'':'none';
      box.querySelectorAll('.gp-b[data-ci]').forEach(function(b){ b.classList.toggle('on',draft.c[+b.dataset.ci]===b.dataset.c); });
      box.querySelectorAll('.gp-b[data-m]').forEach(function(b){ b.classList.toggle('on',draft.mode===b.dataset.m); });
      stat.textContent = T ? gpHumanN('N:'+T.v.join(',')+';'+T.c.map(function(x){return x?'c':'o';}).join(',')+';'+T.mode)+'. Press Check.' : 'Fill in the endpoint value(s) and choose the shading.'; }
    else stat.textContent = T?gpHumanN(inp.value):'';
  }
  function save(){ GP[gpKey(inp)]=JSON.parse(JSON.stringify(draft)); var T=cur(); gpSet(inp, T? 'N:'+draft.v.slice(0,draft.n).map(function(s){return String(s).trim().replace(/[−–]/g,'-');}).join(',')+';'+draft.c.slice(0,draft.n).join(',')+';'+draft.mode : ''); }
  if(!done){
    box.querySelectorAll('.gp-in').forEach(function(f){ f.value=draft.v[+f.dataset.i]||''; f.addEventListener('input',function(){ draft.v[+f.dataset.i]=f.value; save(); draw(); }); });
    box.querySelectorAll('.gp-b').forEach(function(b){ b.addEventListener('click',function(){
      if(b.dataset.n){ draft.n=+b.dataset.n; draft.mode=''; } if(b.dataset.ci) draft.c[+b.dataset.ci]=b.dataset.c; if(b.dataset.m) draft.mode=b.dataset.m; save(); draw(); }); });
  }
  draw();
}
/* ---------- inequality grapher (explore tool) ---------- */
function grInitAll(root){ (root||document).querySelectorAll('.ineq-grapher:not([data-ok])').forEach(grInit); }
function grInit(el){
  el.dataset.ok='1'; var init=el.dataset.init||'y >= 2x - 1; x + y < 6';
  el.innerHTML='<div class="gr-head">📈 Inequality grapher</div><div class="gr-row"><input class="gr-in" value="'+esc(init)+'" aria-label="inequalities"><button type="button" class="gp-b gr-go">Plot</button></div>'+
    '<div class="gr-hint">Type one or more inequalities in x and y, separated by ; (e.g. 2x + 3y ≤ 6; x ≥ 0; y ≥ 0). The region that satisfies all of them is shaded; solid lines for ≤ ≥, dashed for &lt; &gt;.</div>'+
    '<canvas class="gr-cv" width="640" height="640"></canvas><div class="gr-msg"></div>';
  var cv=el.querySelector('canvas'), inp=el.querySelector('.gr-in'), msg=el.querySelector('.gr-msg');
  function plot(){
    var ctx=cv.getContext('2d'), W=cv.width, H=cv.height, x0=-10,x1=10,y0=-10,y1=10, cs=getComputedStyle(document.documentElement);
    var ink=cs.getPropertyValue('--ink').trim()||'#222', rule=cs.getPropertyValue('--rule').trim()||'#ddd', acc=cs.getPropertyValue('--accent-text').trim()||'#1F3B6B', card=cs.getPropertyValue('--card').trim()||'#fff';
    var parts=inp.value.split(/[;,]/).map(function(s){return s.trim();}).filter(Boolean), Is=[];
    for(var i=0;i<parts.length;i++){ var I=gpIneq(parts[i]); if(!I){ msg.textContent='Could not read “'+parts[i]+'”. Use x, y, numbers, + − × /, ^ and one of < > ≤ ≥ (or <= >=).'; return; } Is.push(I); }
    msg.textContent=Is.length?'Shaded: points satisfying '+parts.map(function(p){return p.replace(/<=/g,'≤').replace(/>=/g,'≥');}).join(' and ')+'.':'';
    var X=function(x){return (x-x0)/(x1-x0)*W;}, Y=function(y){return H-(y-y0)/(y1-y0)*H;};
    ctx.fillStyle=card; ctx.fillRect(0,0,W,H);
    var cell=4; ctx.fillStyle=acc; ctx.globalAlpha=0.28;
    for(var px=0;px<W;px+=cell) for(var py=0;py<H;py+=cell){ var x=x0+(px+cell/2)/W*(x1-x0), y=y1-(py+cell/2)/H*(y1-y0); if(Is.length&&Is.every(function(I){return gpSat(I,x,y);})) ctx.fillRect(px,py,cell,cell); }
    ctx.globalAlpha=1; ctx.strokeStyle=rule; ctx.lineWidth=1;
    for(var g=x0;g<=x1;g++){ ctx.beginPath(); ctx.moveTo(X(g),0); ctx.lineTo(X(g),H); ctx.stroke(); ctx.beginPath(); ctx.moveTo(0,Y(g)); ctx.lineTo(W,Y(g)); ctx.stroke(); }
    ctx.strokeStyle=ink; ctx.lineWidth=2; ctx.beginPath(); ctx.moveTo(X(0),0); ctx.lineTo(X(0),H); ctx.moveTo(0,Y(0)); ctx.lineTo(W,Y(0)); ctx.stroke();
    ctx.fillStyle=ink; ctx.font='20px sans-serif'; ctx.textAlign='center'; for(g=x0+2;g<=x1-1;g+=2){ if(g) { ctx.fillText(String(g),X(g),Y(0)+22); ctx.fillText(String(g),X(0)-16,Y(g)+7); } }
    Is.forEach(function(I){ // boundary f = 0 by sampling sign changes
      var strict=(I.op==='<'||I.op==='>'), n=320; ctx.fillStyle=acc;
      for(var i=0;i<n;i++) for(var j=0;j<n;j++){ var xa=x0+i/n*(x1-x0), ya=y0+j/n*(y1-y0), d=(x1-x0)/n;
        var f00=I.f(xa,ya), f10=I.f(xa+d,ya), f01=I.f(xa,ya+d);
        if((f00>0)!==(f10>0)||(f00>0)!==(f01>0)||Math.abs(f00)<1e-12){ if(strict&&((i+j)%14>6)) continue; ctx.fillRect(X(xa)-1.6,Y(ya)-1.6,3.2,3.2); } } });
  }
  el.querySelector('.gr-go').addEventListener('click',plot); inp.addEventListener('keydown',function(e){ if(e.key==='Enter') plot(); });
  plot();
}


/* ================= exam: negative marking ================= */
CRIT_COL.E='#C0392B';
var NEG=0.33;
function exNet(c,w){ return Math.round((c-NEG*w)*100)/100; }
(function(){ var _rr=renderReport; renderReport=function(){ _rr(); try{
  var st=critStats(), C=0,W=0,N=0,T=0; st.forEach(function(s){ C+=s.c; W+=s.w; N+=s.n; T+=s.tot; });
  var wrap=document.getElementById('wrap'); var h2=wrap.querySelector('section.note h2'); if(h2) h2.textContent='Mock paper report';
  wrap.querySelectorAll('.rep-lvl,.rep-note').forEach(function(e){ e.remove(); });
  wrap.querySelectorAll('.rep-cap').forEach(function(e){ e.textContent='Marks earned, by part'; });
  wrap.querySelectorAll('button[data-go]').forEach(function(b){ b.textContent=b.textContent.replace('Open Test','Open Part'); });
  wrap.querySelectorAll('.rep-card').forEach(function(card,i){ var s=st[i]; if(!s) return; var d=document.createElement('div'); d.className='ex-net'; d.innerHTML='Net score <b>'+exNet(s.c,s.w)+'</b> / '+s.tot+' <span>(+'+s.c+' − 0.33 × '+s.w+')</span>'; var b=card.querySelector('button'); card.insertBefore(d,b); });
  var att=C+W, net=exNet(C,W), acc=att?Math.round(C/att*100):0;
  var box=document.createElement('div'); box.className='ex-sum';
  box.innerHTML='<div class="ex-big">'+net+'<span> / '+T+'</span></div><div class="ex-lab">Score with negative marking (+1 correct, −0.33 wrong, 0 unattempted)</div>'+
    '<div class="ex-row"><span>✅ Correct <b>'+C+'</b></span><span>❌ Wrong <b>'+W+'</b> (−'+Math.round(NEG*W*100)/100+')</span><span>⏭ Unattempted <b>'+N+'</b></span><span>🎯 Accuracy of attempted <b>'+acc+'%</b></span></div>'+
    '<div class="ex-tip">'+(att&&acc<60?'Your accuracy is below 60% — with negative marking, skip questions where you can’t eliminate at least two options.':(att?'Good accuracy — with this accuracy, attempting more questions will raise your net score.':'Take each part in Quiz mode, then come back here for your score.'))+'</div>';
  var sec=wrap.querySelector('section.note'); if(sec){ var top=sec.querySelector('.rep-top'); sec.insertBefore(box, top); }
 }catch(e){ console.log('exam',e); } }; })();
(function(){ var _rq=renderQuizResults; renderQuizResults=function(){ _rq.apply(this,arguments); try{ var ts=state.tabs[activeTab], sl=SLIDES[activeTab], c=0,w=0;
  sl.forEach(function(s,i){ if(isSlideCorrect(activeTab,i)) c++; else if(isSlideAttempted(activeTab,i)) w++; });
  var done=document.querySelector('#wrap .done-card'); if(!done) return; var p=document.createElement('div'); p.className='ex-sum ex-small';
  p.innerHTML='<div class="ex-big">'+exNet(c,w)+'<span> / '+sl.length+'</span></div><div class="ex-lab">Net score for this part (+'+c+' − 0.33 × '+w+')</div>'; done.insertBefore(p, done.querySelector('div[style*="margin-top:16px"]')||null); }catch(e){} }; })();

renderLogin();
})();
</script>
</body>
</html>
