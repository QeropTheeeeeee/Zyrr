<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>💎 ZyroYonk Premium Keys</title>
<style>
  *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

  :root {
    --bg: #0a0a12;
    --bg2: #111120;
    --bg3: #181828;
    --border: rgba(124,58,237,0.22);
    --text: #e8e8f8;
    --muted: #5858a0;
    --accent: #7c3aed;
    --accent-light: #a78bfa;
    --success: #22c55e;
    --gold: #f59e0b;
  }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'Segoe UI', system-ui, sans-serif;
    min-height: 100vh;
    overflow-x: hidden;
  }

  #bubbleCanvas { position:fixed; inset:0; z-index:0; pointer-events:none; }

  /* ========== CAPTCHA OVERLAY ========== */
  .captcha-overlay {
    position:fixed;
    inset:0;
    z-index:1000;
    background:rgba(10,10,18,.98);
    backdrop-filter:blur(20px);
    display:flex;
    align-items:center;
    justify-content:center;
    transition:opacity .5s, visibility .5s;
  }

  .captcha-overlay.hidden {
    opacity:0;
    visibility:hidden;
    pointer-events:none;
  }

  .captcha-container {
    max-width:450px;
    width:90%;
    padding:2.5rem 2rem;
    background:linear-gradient(135deg,rgba(17,17,32,.95) 0%,rgba(20,20,45,.95) 100%);
    border:2px solid rgba(124,58,237,.5);
    border-radius:28px;
    box-shadow:0 0 80px rgba(124,58,237,.3),inset 0 0 30px rgba(124,58,237,.05);
    text-align:center;
    animation:captchaPop .4s ease;
  }

  @keyframes captchaPop {
    from { transform:scale(.9); opacity:0; }
    to { transform:scale(1); opacity:1; }
  }

  .captcha-icon {
    font-size:4rem;
    margin-bottom:1rem;
  }

  .captcha-title {
    font-size:1.8rem;
    font-weight:900;
    margin-bottom:.5rem;
    background:linear-gradient(140deg,#f0ecff 0%,#c4b5fd 50%,#818cf8 100%);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
    background-clip:text;
  }

  .captcha-desc {
    font-size:14px;
    color:var(--muted);
    margin-bottom:2rem;
  }

  .captcha-box {
    background:rgba(0,0,0,.3);
    border:1.5px solid rgba(124,58,237,.3);
    border-radius:16px;
    padding:1.5rem;
    margin-bottom:1.5rem;
  }

  .captcha-question {
    display:flex;
    align-items:center;
    justify-content:center;
    gap:10px;
    margin-bottom:1.2rem;
  }

  .captcha-emoji {
    font-size:2.5rem;
  }

  .captcha-text {
    font-size:1.5rem;
    font-weight:700;
    color:#e8e8f8;
    letter-spacing:2px;
  }

  .captcha-input {
    width:100%;
    padding:14px 18px;
    background:rgba(24,24,40,.9);
    border:2px solid rgba(124,58,237,.4);
    border-radius:12px;
    color:#fff;
    font-size:16px;
    text-align:center;
    outline:none;
    transition:all .2s;
  }

  .captcha-input:focus {
    border-color:#7c3aed;
    box-shadow:0 0 20px rgba(124,58,237,.3);
  }

  .captcha-input::placeholder {
    color:var(--muted);
    font-size:14px;
  }

  .captcha-error {
    color:#f87171;
    font-size:12px;
    margin-top:8px;
    min-height:18px;
  }

  .captcha-btn {
    width:100%;
    padding:14px;
    background:linear-gradient(135deg,#7c3aed,#4f46e5);
    border:none;
    border-radius:12px;
    color:#fff;
    font-size:15px;
    font-weight:700;
    cursor:pointer;
    transition:all .2s;
    box-shadow:0 4px 22px rgba(124,58,237,.48);
  }

  .captcha-btn:hover {
    box-shadow:0 7px 32px rgba(124,58,237,.7);
    transform:translateY(-1px);
  }

  .captcha-btn:disabled {
    opacity:.5;
    cursor:not-allowed;
    transform:none;
    box-shadow:none;
  }

  .captcha-refresh {
    display:flex;
    align-items:center;
    justify-content:center;
    gap:5px;
    margin-top:15px;
    color:var(--muted);
    font-size:13px;
    cursor:pointer;
    transition:color .2s;
  }

  .captcha-refresh:hover {
    color:#a78bfa;
  }

  .security-badge {
    display:flex;
    align-items:center;
    justify-content:center;
    gap:8px;
    margin-top:20px;
    padding-top:15px;
    border-top:1px solid rgba(255,255,255,.05);
    color:var(--muted);
    font-size:11px;
  }

  /* NAV */
  nav {
    position:sticky; top:0; z-index:200;
    background:rgba(10,10,18,.93);
    backdrop-filter:blur(18px);
    border-bottom:1px solid var(--border);
    padding:0 2rem;
    display:flex; align-items:center; justify-content:space-between;
    height:56px;
  }
  .nav-logo {
    font-size:17px; font-weight:800;
    background:linear-gradient(130deg,#c4b5fd,#818cf8,#60a5fa);
    -webkit-background-clip:text; -webkit-text-fill-color:transparent;
    background-clip:text; text-decoration:none; letter-spacing:-.5px;
  }
  .nav-links { display:flex; align-items:center; gap:4px; list-style:none; }
  .nav-links a {
    color:#9090c0; text-decoration:none; font-size:13px;
    padding:6px 13px; border-radius:8px;
    border:1px solid transparent; transition:all .18s;
  }
  .nav-links a:hover { color:#e0e0f8; background:rgba(124,58,237,.13); border-color:var(--border); }
  .status-a { display:flex; align-items:center; gap:6px; color:#22c55e !important; font-size:12px; font-weight:600; }
  .dot { width:7px; height:7px; border-radius:50%; background:#22c55e; box-shadow:0 0 8px #22c55e; animation:blink 2s infinite; }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:.35} }
  .discord-a { background:#5865F2 !important; color:#fff !important; -webkit-text-fill-color:#fff !important; font-weight:700 !important; border-color:#5865F2 !important; }
  .discord-a:hover { background:#4752c4 !important; border-color:#4752c4 !important; }

  /* MAIN */
  main {
    position:relative; z-index:1;
    display:flex; flex-direction:column; align-items:center;
    padding:4rem 1.5rem 5rem; gap:2.2rem;
  }

  .badge {
    display:inline-flex; align-items:center; gap:9px;
    background:rgba(124,58,237,.16);
    border:1.5px solid rgba(124,58,237,.44);
    border-radius:999px; padding:9px 26px;
    font-size:12px; font-weight:800; color:#c4b5fd;
    letter-spacing:2px; text-transform:uppercase;
    box-shadow:0 0 24px rgba(124,58,237,.2),inset 0 0 14px rgba(124,58,237,.07);
  }

  h1 {
    font-size:clamp(2.3rem,6vw,3.6rem); font-weight:900; text-align:center;
    background:linear-gradient(140deg,#f0ecff 0%,#c4b5fd 38%,#818cf8 72%,#60a5fa 100%);
    -webkit-background-clip:text; -webkit-text-fill-color:transparent; background-clip:text;
    line-height:1.1; letter-spacing:-1.5px;
  }
  .sub { font-size:15px; color:var(--muted); text-align:center; max-width:500px; }

  /* ========== SUPPORTED GAMES SECTION ========== */
  .games-section {
    width:100%; 
    max-width:900px;
    margin-top:0.5rem;
    margin-bottom:0.5rem;
  }

  .games-header {
    display:flex;
    align-items:center;
    justify-content:center;
    gap:12px;
    margin-bottom:1.8rem;
  }

  .games-title {
    font-size:1.8rem; 
    font-weight:800; 
    text-align:center;
    background:linear-gradient(140deg,#f0ecff 0%,#c4b5fd 40%,#818cf8 70%,#60a5fa 100%);
    -webkit-background-clip:text; 
    -webkit-text-fill-color:transparent;
    background-clip:text;
  }

  .games-count {
    background:rgba(124,58,237,.2);
    border:1px solid rgba(124,58,237,.4);
    color:#c4b5fd;
    font-size:14px;
    font-weight:700;
    padding:4px 12px;
    border-radius:999px;
  }

  .games-grid {
    display:flex;
    flex-direction:column;
    gap:0.85rem;
  }

  .game-item {
    background:linear-gradient(135deg,rgba(17,17,32,.95) 0%,rgba(20,20,45,.9) 100%);
    border:1.5px solid var(--border);
    border-radius:18px;
    overflow:hidden;
    backdrop-filter:blur(12px);
    transition:all .3s cubic-bezier(0.4, 0, 0.2, 1);
    box-shadow:0 4px 20px rgba(0,0,0,.3);
    position:relative;
  }

  .game-item:hover {
    border-color:rgba(124,58,237,.6);
    box-shadow:0 8px 30px rgba(124,58,237,.2),0 0 0 1px rgba(124,58,237,.1) inset;
  }

  .game-item.expanded {
    border-color:rgba(124,58,237,.7);
    box-shadow:0 12px 40px rgba(124,58,237,.25),0 0 30px rgba(124,58,237,.1) inset;
  }

  .game-header {
    display:flex;
    align-items:center;
    gap:16px;
    padding:1.1rem 1.4rem;
    cursor:pointer;
    user-select:none;
    position:relative;
    transition:all .2s;
  }

  .game-header::before {
    content:'';
    position:absolute;
    left:0;
    top:0;
    bottom:0;
    width:4px;
    background:linear-gradient(180deg,#7c3aed,#a78bfa,#7c3aed);
    opacity:0;
    transition:opacity .3s;
  }

  .game-item:hover .game-header::before,
  .game-item.expanded .game-header::before {
    opacity:1;
  }

  .game-thumbnail {
    width:60px;
    height:60px;
    border-radius:14px;
    background:linear-gradient(135deg,rgba(124,58,237,.2),rgba(79,70,229,.1));
    border:2px solid rgba(124,58,237,.4);
    flex-shrink:0;
    overflow:hidden;
    position:relative;
    box-shadow:0 4px 15px rgba(0,0,0,.3);
  }

  .game-item:hover .game-thumbnail {
    border-color:rgba(124,58,237,.7);
    box-shadow:0 0 20px rgba(124,58,237,.3);
  }

  .game-thumbnail img {
    width:100%;
    height:100%;
    object-fit:cover;
  }

  .game-thumbnail::after {
    content:'';
    position:absolute;
    inset:0;
    background:linear-gradient(135deg,transparent 50%,rgba(124,58,237,.1) 100%);
    pointer-events:none;
  }

  .game-info {
    flex:1;
  }

  .game-name-row {
    display:flex;
    align-items:center;
    gap:8px;
    margin-bottom:4px;
    flex-wrap:wrap;
  }

  .game-name {
    font-size:17px; 
    font-weight:800;
    background:linear-gradient(135deg,#fff,#e0d5ff);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
    background-clip:text;
  }

  .status-badges {
    display:flex;
    align-items:center;
    gap:5px;
    flex-wrap:wrap;
  }

  .status-badge {
    display:inline-flex;
    align-items:center;
    gap:4px;
    padding:3px 10px;
    border-radius:999px;
    font-size:9px;
    font-weight:800;
    letter-spacing:.5px;
    text-transform:uppercase;
  }

  .status-dot {
    width:6px;
    height:6px;
    border-radius:50%;
  }

  .status-badge.supported {
    background:rgba(34,197,94,.12);
    border:1px solid rgba(34,197,94,.4);
    color:#4ade80;
  }
  .status-badge.supported .status-dot {
    background:#22c55e;
    box-shadow:0 0 8px #22c55e;
  }

  .status-badge.new-script {
    background:rgba(59,130,246,.12);
    border:1px solid rgba(59,130,246,.4);
    color:#60a5fa;
  }
  .status-badge.new-script .status-dot {
    background:#3b82f6;
    box-shadow:0 0 8px #3b82f6;
    animation:blink 1.5s infinite;
  }

  .status-badge.updated {
    background:rgba(34,197,94,.12);
    border:1px solid rgba(34,197,94,.4);
    color:#4ade80;
  }
  .status-badge.updated .status-dot {
    background:#22c55e;
    box-shadow:0 0 8px #22c55e;
    animation:blink 1.5s infinite;
  }

  .status-badge.not-functioning {
    background:rgba(239,68,68,.12);
    border:1px solid rgba(239,68,68,.4);
    color:#f87171;
  }
  .status-badge.not-functioning .status-dot {
    background:#ef4444;
    box-shadow:0 0 8px #ef4444;
  }

  .game-creator {
    font-size:12px;
    color:var(--muted);
    display:flex;
    align-items:center;
    gap:4px;
  }

  .game-creator::before {
    content:'👤';
    font-size:10px;
    opacity:.7;
  }

  .dropdown-indicator {
    display:flex;
    align-items:center;
    justify-content:center;
    width:32px;
    height:32px;
    border-radius:10px;
    background:rgba(124,58,237,.1);
    border:1px solid rgba(124,58,237,.25);
    color:var(--accent-light);
    transition:all .3s;
  }

  .game-item:hover .dropdown-indicator {
    background:rgba(124,58,237,.2);
    border-color:rgba(124,58,237,.5);
  }

  .dropdown-arrow {
    font-size:16px;
    transition:transform .4s cubic-bezier(0.34, 1.56, 0.64, 1);
  }

  .game-item.expanded .dropdown-arrow {
    transform:rotate(180deg);
  }

  .game-item.expanded .dropdown-indicator {
    background:rgba(124,58,237,.25);
    border-color:rgba(124,58,237,.6);
    box-shadow:0 0 15px rgba(124,58,237,.3);
  }

  .game-description {
    max-height:0;
    overflow:hidden;
    transition:max-height .5s cubic-bezier(0.4, 0, 0.2, 1);
    background:linear-gradient(180deg,rgba(10,10,20,.5) 0%,rgba(5,5,15,.3) 100%);
    border-top:1px solid transparent;
  }

  .game-item.expanded .game-description {
    max-height:600px;
    border-top-color:rgba(124,58,237,.3);
  }

  .desc-content {
    padding:1.5rem 1.8rem;
  }

  .feature-sections {
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:1.5rem;
    margin-bottom:1.2rem;
  }

  @media(max-width:600px){
    .feature-sections {
      grid-template-columns:1fr;
      gap:1rem;
    }
  }

  .feature-section {
    background:rgba(0,0,0,.2);
    border-radius:16px;
    padding:1.2rem 1.3rem;
    border:1px solid rgba(255,255,255,.05);
  }

  .feature-title {
    font-size:15px;
    font-weight:800;
    margin-bottom:1rem;
    display:flex;
    align-items:center;
    gap:8px;
    padding-bottom:0.7rem;
    border-bottom:1.5px solid rgba(255,255,255,.08);
  }

  .free-title {
    color:#60a5fa;
  }

  .free-title .title-icon {
    background:rgba(59,130,246,.15);
    border:1px solid rgba(59,130,246,.3);
  }

  .premium-title {
    background:linear-gradient(135deg,#c4b5fd,#a78bfa);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
    background-clip:text;
  }

  .premium-title .title-icon {
    background:rgba(124,58,237,.2);
    border:1px solid rgba(124,58,237,.4);
  }

  .title-icon {
    width:28px;
    height:28px;
    border-radius:8px;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:14px;
  }

  .feature-list {
    list-style:none;
    display:grid;
    gap:0.5rem;
  }

  .feature-list li {
    font-size:12px;
    color:#c0c0e0;
    display:flex;
    align-items:center;
    gap:8px;
    padding:4px 0;
    transition:all .2s;
  }

  .feature-list li:hover {
    color:#e0e0ff;
    transform:translateX(3px);
  }

  .feature-icon {
    width:18px;
    height:18px;
    border-radius:5px;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:10px;
    font-weight:800;
  }

  .free-icon {
    background:rgba(59,130,246,.12);
    border:1px solid rgba(59,130,246,.3);
    color:#60a5fa;
  }

  .premium-icon {
    background:rgba(124,58,237,.15);
    border:1px solid rgba(124,58,237,.35);
    color:#a78bfa;
  }

  .game-footer {
    display:flex;
    align-items:center;
    justify-content:flex-start;
    margin-top:1rem;
    padding-top:1rem;
    border-top:1px solid rgba(255,255,255,.06);
  }

  .game-link {
    display:inline-flex;
    align-items:center;
    gap:8px;
    padding:9px 18px;
    background:linear-gradient(135deg,rgba(124,58,237,.2),rgba(79,70,229,.1));
    border:1.5px solid rgba(124,58,237,.4);
    border-radius:10px;
    color:#c4b5fd;
    text-decoration:none;
    font-size:12px;
    font-weight:700;
    transition:all .25s;
  }

  .game-link:hover {
    background:linear-gradient(135deg,rgba(124,58,237,.3),rgba(79,70,229,.2));
    border-color:rgba(124,58,237,.7);
    box-shadow:0 0 20px rgba(124,58,237,.3);
    transform:scale(1.02);
  }

  /* PRICING GRID */
  .pricing-grid {
    display:grid; 
    grid-template-columns:repeat(auto-fit,minmax(170px,1fr));
    gap:1rem; 
    width:100%; 
    max-width:1100px;
    margin-top:0.5rem;
  }

  .price-card {
    background:rgba(17,17,32,.82); 
    border:1px solid var(--border);
    border-radius:20px; 
    padding:1.5rem 1.2rem;
    position:relative; 
    overflow:hidden; 
    backdrop-filter:blur(12px);
    transition:all .25s;
    text-align:center;
  }

  .price-card::before {
    content:''; position:absolute; inset:0;
    background:linear-gradient(135deg,rgba(124,58,237,.05) 0%,transparent 60%);
    border-radius:20px; pointer-events:none;
  }

  .price-card:hover { 
    border-color:rgba(124,58,237,.55); 
    transform:translateY(-5px); 
    box-shadow:0 14px 42px rgba(124,58,237,.22); 
  }

  .price-card.popular {
    border-color:rgba(124,58,237,.6);
    background:linear-gradient(150deg,rgba(124,58,237,.12) 0%,rgba(17,17,32,.9) 55%);
  }

  .price-card.lifetime {
    border-color:rgba(245,158,11,.5);
    background:linear-gradient(150deg,rgba(245,158,11,.08) 0%,rgba(17,17,32,.9) 55%);
  }

  .popular-tag {
    position:absolute; top:12px; right:12px;
    background:rgba(124,58,237,.25); border:1px solid rgba(124,58,237,.45);
    color:#c4b5fd; font-size:9px; font-weight:800; letter-spacing:.8px;
    text-transform:uppercase; padding:3px 8px; border-radius:999px;
  }

  .lifetime-tag {
    position:absolute; top:12px; right:12px;
    background:rgba(245,158,11,.2); border:1px solid rgba(245,158,11,.4);
    color:#fbbf24; font-size:9px; font-weight:800; letter-spacing:.8px;
    text-transform:uppercase; padding:3px 8px; border-radius:999px;
  }

  .card-icon {
    width:50px; height:50px; border-radius:14px;
    display:flex; align-items:center; justify-content:center;
    font-size:22px; margin:0 auto 1rem;
    background:rgba(124,58,237,.15); border:1px solid rgba(124,58,237,.24);
  }

  .card-title { 
    font-size:18px; font-weight:800; color:#e8e8f8; 
    margin-bottom:4px; 
  }

  .card-desc { 
    font-size:11px; color:var(--muted); 
    margin-bottom:1rem; 
  }

  .price-row { 
    display:flex; align-items:baseline; justify-content:center; 
    gap:4px; margin-bottom:1rem; 
  }

  .price-num { 
    font-size:2rem; font-weight:900; 
    background:linear-gradient(135deg,#e8e8f8,#c4b5fd);
    -webkit-background-clip:text; -webkit-text-fill-color:transparent;
    background-clip:text;
  }

  .price-unit { 
    font-size:11px; color:var(--muted); 
  }

  .save-badge {
    background:rgba(34,197,94,.12); border:1px solid rgba(34,197,94,.25);
    color:#4ade80; font-size:10px; font-weight:700;
    padding:2px 8px; border-radius:999px;
    display:inline-block; margin-bottom:0.8rem;
  }

  .feat-list { 
    list-style:none; 
    display:flex; 
    flex-direction:column; 
    gap:6px; 
    margin-bottom:1.2rem;
    text-align:left;
  }

  .feat-list li { 
    font-size:11px; color:#b0b0d0; 
    display:flex; align-items:center; gap:6px; 
  }

  .chk {
    width:16px; height:16px; border-radius:50%; flex-shrink:0;
    background:rgba(34,197,94,.12); border:1px solid rgba(34,197,94,.28);
    color:#22c55e; font-size:9px; font-weight:800;
    display:flex; align-items:center; justify-content:center;
  }

  /* BUTTONS */
  .btn {
    display:flex; align-items:center; justify-content:center; gap:8px;
    width:100%; padding:11px; border-radius:10px; border:none;
    cursor:pointer; font-size:13px; font-weight:700;
    text-decoration:none; transition:all .2s; font-family:inherit;
  }

  .btn-p {
    background:linear-gradient(135deg,#7c3aed,#4f46e5);
    color:#fff; box-shadow:0 4px 22px rgba(124,58,237,.48);
  }

  .btn-p:hover { 
    box-shadow:0 7px 32px rgba(124,58,237,.7); 
    transform:translateY(-1px); filter:brightness(1.08); 
  }

  .btn-lifetime {
    background:linear-gradient(135deg,#f59e0b,#d97706);
    color:#fff; box-shadow:0 4px 22px rgba(245,158,11,.4);
  }

  .btn-lifetime:hover {
    box-shadow:0 7px 32px rgba(245,158,11,.6);
    transform:translateY(-1px); filter:brightness(1.08);
  }

  /* STATUS BOX */
  .sbox {
    width:100%; max-width:680px;
    background:rgba(17,17,32,.82); border:1px solid var(--border);
    border-radius:22px; padding:1.65rem; backdrop-filter:blur(12px);
    margin-top:0.5rem;
  }

  .shead { display:flex; align-items:center; gap:12px; margin-bottom:1.2rem; }
  .sicon {
    width:40px; height:40px; border-radius:11px;
    background:rgba(124,58,237,.14); border:1px solid rgba(124,58,237,.22);
    display:flex; align-items:center; justify-content:center; font-size:18px;
  }

  .stitle { font-size:15px; font-weight:800; color:#e8e8f8; }
  .ssub   { font-size:12px; color:var(--muted); }

  .apill {
    margin-left:auto; display:flex; align-items:center; gap:6px;
    background:rgba(34,197,94,.12); border:1px solid rgba(34,197,94,.28);
    color:#22c55e; font-size:12px; font-weight:700;
    padding:5px 14px; border-radius:999px;
  }

  .adot { 
    width:7px; height:7px; background:#22c55e; border-radius:50%; 
    box-shadow:0 0 7px #22c55e; animation:blink 2s infinite; 
  }

  .mgrid {
    display:grid; grid-template-columns:repeat(auto-fill,minmax(145px,1fr));
    gap:10px; margin-bottom:1.2rem;
  }

  .mcell {
    background:rgba(24,24,40,.9); border:1px solid rgba(255,255,255,.055);
    border-radius:11px; padding:13px 14px;
  }

  .mlabel { 
    font-size:10px; font-weight:700; letter-spacing:.8px; 
    text-transform:uppercase; color:var(--muted); margin-bottom:5px; 
  }

  .mval { font-size:14px; font-weight:700; color:#d0d0f0; }

  footer {
    position:relative; z-index:1; text-align:center;
    padding:2rem; font-size:12px; color:rgba(100,100,160,.4);
    border-top:1px solid rgba(255,255,255,.04);
    margin-top:2rem;
  }

  @media(max-width:700px){
    nav{padding:0 1rem;}
    .nav-links a{padding:5px 9px;font-size:12px;}
    main{padding:2.5rem 1rem;}
    .pricing-grid{grid-template-columns:repeat(2,1fr);}
  }

  @media(max-width:450px){
    .pricing-grid{grid-template-columns:1fr;}
  }
</style>
</head>
<body>

<canvas id="bubbleCanvas"></canvas>

<!-- CAPTCHA OVERLAY -->
<div class="captcha-overlay" id="captchaOverlay">
  <div class="captcha-container">
    <div class="captcha-icon">🔐</div>
    <div class="captcha-title">Verify to Continue</div>
    <div class="captcha-desc">Complete the captcha to access ZyroYonk Premium</div>
    
    <div class="captcha-box">
      <div class="captcha-question">
        <span class="captcha-emoji" id="captchaEmoji">🔢</span>
        <span class="captcha-text" id="captchaQuestion">5 + 3 = ?</span>
      </div>
      <input type="text" class="captcha-input" id="captchaInput" placeholder="Enter answer..." autocomplete="off">
      <div class="captcha-error" id="captchaError"></div>
    </div>
    
    <button class="captcha-btn" id="captchaBtn" onclick="verifyCaptcha()">✅ Verify & Unlock</button>
    
    <div class="captcha-refresh" onclick="refreshCaptcha()">
      <span>🔄</span>
      <span>New Captcha</span>
    </div>
    
    <div class="security-badge">
      <span>🛡️</span>
      <span>Secured by ZyroYonk • Protection Active</span>
    </div>
  </div>
</div>

<nav>
  <a class="nav-logo" href="#">ZyroYonk</a>
  <ul class="nav-links">
    <li><a href="#">Premium</a></li>
    <li><a href="#games">Games</a></li>
    <li><a href="#" class="status-a"><span class="dot"></span> Status : Active</a></li>
    <li><a href="https://discord.com/invite/pfgHhKnzyu" target="_blank" class="discord-a">💬 Discord</a></li>
  </ul>
</nav>

<main>
  <div class="badge">💎 Premium Access Only</div>
  <h1>ZyroYonk Premium</h1>
  <p class="sub">Choose your premium plan — No checkpoints, instant access, full features</p>

  <!-- SUPPORTED GAMES SECTION -->
  <div class="games-section" id="games">
    <div class="games-header">
      <h2 class="games-title">🎮 Supported Games</h2>
      <span class="games-count">6 Games</span>
    </div>
    <div class="games-grid" id="gamesContainer">
      <!-- Games will be loaded dynamically -->
    </div>
  </div>

  <!-- PRICING CARDS -->
  <div class="pricing-grid">
    
    <!-- 3 Days -->
    <div class="price-card">
      <div class="card-icon">⚡</div>
      <div class="card-title">3 Days</div>
      <div class="card-desc">Quick access pass</div>
      <div class="price-row">
        <span class="price-num">149</span>
        <span class="price-unit">Robux</span>
      </div>
      <ul class="feat-list">
        <li><span class="chk">✓</span> 3 Days access</li>
        <li><span class="chk">✓</span> No checkpoint</li>
        <li><span class="chk">✓</span> All features</li>
        <li><span class="chk">✓</span> Support included</li>
      </ul>
      <a class="btn btn-p" href="https://discord.com/invite/pfgHhKnzyu" target="_blank">🔓 Get Access</a>
    </div>

    <!-- 15 Days -->
    <div class="price-card popular">
      <div class="popular-tag">🔥 POPULAR</div>
      <div class="card-icon">⭐</div>
      <div class="card-title">15 Days</div>
      <div class="card-desc">Best value for short term</div>
      <div class="price-row">
        <span class="price-num">399</span>
        <span class="price-unit">Robux</span>
      </div>
      <div class="save-badge">💰 Save 34%</div>
      <ul class="feat-list">
        <li><span class="chk">✓</span> 15 Days access</li>
        <li><span class="chk">✓</span> No checkpoint</li>
        <li><span class="chk">✓</span> Priority support</li>
        <li><span class="chk">✓</span> All premium features</li>
      </ul>
      <a class="btn btn-p" href="https://discord.com/invite/pfgHhKnzyu" target="_blank">🔓 Get Access</a>
    </div>

    <!-- 30 Days -->
    <div class="price-card">
      <div class="card-icon">👑</div>
      <div class="card-title">30 Days</div>
      <div class="card-desc">Monthly premium</div>
      <div class="price-row">
        <span class="price-num">699</span>
        <span class="price-unit">Robux</span>
      </div>
      <div class="save-badge">💰 Save 42%</div>
      <ul class="feat-list">
        <li><span class="chk">✓</span> 30 Days access</li>
        <li><span class="chk">✓</span> No checkpoint</li>
        <li><span class="chk">✓</span> Priority support</li>
        <li><span class="chk">✓</span> Early updates</li>
        <li><span class="chk">✓</span> All premium features</li>
      </ul>
      <a class="btn btn-p" href="https://discord.com/invite/pfgHhKnzyu" target="_blank">🔓 Get Access</a>
    </div>

    <!-- 60 Days -->
    <div class="price-card">
      <div class="card-icon">💪</div>
      <div class="card-title">60 Days</div>
      <div class="card-desc">2 Month access</div>
      <div class="price-row">
        <span class="price-num">1,199</span>
        <span class="price-unit">Robux</span>
      </div>
      <div class="save-badge">💰 Save 50%</div>
      <ul class="feat-list">
        <li><span class="chk">✓</span> 60 Days access</li>
        <li><span class="chk">✓</span> No checkpoint</li>
        <li><span class="chk">✓</span> VIP support</li>
        <li><span class="chk">✓</span> Early updates</li>
        <li><span class="chk">✓</span> Beta features</li>
        <li><span class="chk">✓</span> All premium features</li>
      </ul>
      <a class="btn btn-p" href="https://discord.com/invite/pfgHhKnzyu" target="_blank">🔓 Get Access</a>
    </div>

    <!-- 90 Days -->
    <div class="price-card popular">
      <div class="popular-tag">💎 ELITE</div>
      <div class="card-icon">🏆</div>
      <div class="card-title">90 Days</div>
      <div class="card-desc">3 Month elite access</div>
      <div class="price-row">
        <span class="price-num">1,599</span>
        <span class="price-unit">Robux</span>
      </div>
      <div class="save-badge">💰 Save 55%</div>
      <ul class="feat-list">
        <li><span class="chk">✓</span> 90 Days access</li>
        <li><span class="chk">✓</span> No checkpoint</li>
        <li><span class="chk">✓</span> Elite support</li>
        <li><span class="chk">✓</span> Early updates</li>
        <li><span class="chk">✓</span> Beta features</li>
        <li><span class="chk">✓</span> Custom requests</li>
        <li><span class="chk">✓</span> All premium features</li>
      </ul>
      <a class="btn btn-p" href="https://discord.com/invite/pfgHhKnzyu" target="_blank">🔓 Get Access</a>
    </div>

    <!-- Lifetime -->
    <div class="price-card lifetime">
      <div class="lifetime-tag">🌟 FOREVER</div>
      <div class="card-icon">♾️</div>
      <div class="card-title">Lifetime</div>
      <div class="card-desc">One-time payment</div>
      <div class="price-row">
        <span class="price-num">2,999</span>
        <span class="price-unit">Robux</span>
      </div>
      <div class="save-badge" style="background:rgba(245,158,11,.15);border-color:rgba(245,158,11,.3);color:#fbbf24;">💰 Best Value</div>
      <ul class="feat-list">
        <li><span class="chk">✓</span> Lifetime access</li>
        <li><span class="chk">✓</span> Never expires</li>
        <li><span class="chk">✓</span> Lifetime support</li>
        <li><span class="chk">✓</span> All updates forever</li>
        <li><span class="chk">✓</span> Beta features first</li>
        <li><span class="chk">✓</span> Custom script requests</li>
        <li><span class="chk">✓</span> Everything included</li>
      </ul>
      <a class="btn btn-lifetime" href="https://discord.com/invite/pfgHhKnzyu" target="_blank">🌟 Get Lifetime</a>
    </div>

  </div>

  <!-- STATUS BOX -->
  <div class="sbox">
    <div class="shead">
      <div class="sicon">💎</div>
      <div>
        <div class="stitle">Premium System Status</div>
        <div class="ssub">All plans include instant access</div>
      </div>
      <div class="apill"><span class="adot"></span> Active</div>
    </div>
    <div class="mgrid">
      <div class="mcell"><div class="mlabel">🔐 No Checkpoints</div><div class="mval">Instant Access</div></div>
      <div class="mcell"><div class="mlabel">⚡ Updates</div><div class="mval">Weekly</div></div>
      <div class="mcell"><div class="mlabel">💬 Support</div><div class="mval">24/7 Discord</div></div>
      <div class="mcell"><div class="mlabel">🎮 Features</div><div class="mval">Full Premium</div></div>
    </div>
    <a class="btn btn-p" href="https://discord.com/invite/pfgHhKnzyu" target="_blank" style="text-decoration:none;">💬 Join Discord to Purchase</a>
  </div>

</main>

<footer>
  &copy; 2026 ZyroYonk Premium — All rights reserved<br>
  <span style="color:rgba(124,58,237,.5);">Supported Games Updated Weekly</span>
</footer>

<script>
/* ────────── CAPTCHA SYSTEM ────────── */
let currentAnswer = 0;
let captchaVerified = false;

// Check if already verified in this session
if (sessionStorage.getItem('zyroyonk_verified') === 'true') {
  document.getElementById('captchaOverlay').classList.add('hidden');
  captchaVerified = true;
}

function generateCaptcha() {
  const operations = [
    { emoji: '➕', text: '+', func: (a,b) => a + b },
    { emoji: '➖', text: '-', func: (a,b) => a - b },
    { emoji: '✖️', text: '×', func: (a,b) => a * b }
  ];
  
  const op = operations[Math.floor(Math.random() * operations.length)];
  let num1, num2;
  
  if (op.text === '×') {
    num1 = Math.floor(Math.random() * 5) + 2;
    num2 = Math.floor(Math.random() * 5) + 2;
  } else if (op.text === '-') {
    num1 = Math.floor(Math.random() * 8) + 3;
    num2 = Math.floor(Math.random() * num1) + 1;
  } else {
    num1 = Math.floor(Math.random() * 7) + 2;
    num2 = Math.floor(Math.random() * 7) + 2;
  }
  
  currentAnswer = op.func(num1, num2);
  
  document.getElementById('captchaEmoji').textContent = op.emoji;
  document.getElementById('captchaQuestion').textContent = `${num1} ${op.text} ${num2} = ?`;
  document.getElementById('captchaInput').value = '';
  document.getElementById('captchaError').textContent = '';
}

function refreshCaptcha() {
  generateCaptcha();
  document.getElementById('captchaInput').focus();
}

function verifyCaptcha() {
  if (captchaVerified) return;
  
  const input = document.getElementById('captchaInput');
  const error = document.getElementById('captchaError');
  const userAnswer = parseInt(input.value);
  
  if (isNaN(userAnswer)) {
    error.textContent = '❌ Please enter a number';
    input.style.borderColor = '#ef4444';
    return;
  }
  
  if (userAnswer === currentAnswer) {
    // Success!
    captchaVerified = true;
    sessionStorage.setItem('zyroyonk_verified', 'true');
    
    // Hide overlay with animation
    const overlay = document.getElementById('captchaOverlay');
    overlay.classList.add('hidden');
    
    // Play success effect
    input.style.borderColor = '#22c55e';
  } else {
    error.textContent = '❌ Incorrect answer, try again';
    input.style.borderColor = '#ef4444';
    input.value = '';
    input.focus();
    
    // 20% chance to refresh captcha on wrong answer
    if (Math.random() < 0.2) {
      setTimeout(() => generateCaptcha(), 500);
    }
  }
}

// Enter key to submit
document.getElementById('captchaInput').addEventListener('keydown', (e) => {
  if (e.key === 'Enter') {
    verifyCaptcha();
  }
});

// Reset border color on input
document.getElementById('captchaInput').addEventListener('input', () => {
  document.getElementById('captchaInput').style.borderColor = '';
});

// Generate first captcha
generateCaptcha();

/* ────────── BUBBLE BG ────────── */
const canvas = document.getElementById('bubbleCanvas');
const ctx = canvas.getContext('2d');
let W, H, bubbles = [];
const COLORS = ['rgba(124,58,237,','rgba(99,102,241,','rgba(59,130,246,','rgba(139,92,246,','rgba(79,70,229,','rgba(245,158,11,'];

function resize(){ W=canvas.width=window.innerWidth; H=canvas.height=window.innerHeight; }

function mkBubble(){
  const r = 18 + Math.random()*80;
  return {
    x: Math.random()*W, y: H + r + Math.random()*H, r,
    speedY: .25+Math.random()*.6, speedX: -.18+Math.random()*.36,
    wobble: Math.random()*Math.PI*2, wobbleSpeed: .008+Math.random()*.02,
    wobbleAmp: 12+Math.random()*36,
    alpha: .06+Math.random()*.16,
    color: COLORS[Math.floor(Math.random()*COLORS.length)],
    pulse: Math.random()*Math.PI*2, pulseSpeed: .01+Math.random()*.025,
  };
}

function initBubbles(){
  bubbles=[];
  for(let i=0;i<28;i++){ const b=mkBubble(); b.y=Math.random()*H; bubbles.push(b); }
}

function drawBubble(b){
  const pr = b.r*(1+.04*Math.sin(b.pulse));
  const g = ctx.createRadialGradient(b.x,b.y,0,b.x,b.y,pr*1.6);
  g.addColorStop(0,  b.color+(b.alpha*.55)+')');
  g.addColorStop(.5, b.color+(b.alpha*.22)+')');
  g.addColorStop(1,  b.color+'0)');
  ctx.beginPath(); ctx.arc(b.x,b.y,pr*1.6,0,Math.PI*2); ctx.fillStyle=g; ctx.fill();
  ctx.beginPath(); ctx.arc(b.x,b.y,pr,0,Math.PI*2);
  ctx.strokeStyle=b.color+(b.alpha*1.8)+')'; ctx.lineWidth=1.2; ctx.stroke();
  ctx.beginPath(); ctx.arc(b.x-pr*.28,b.y-pr*.3,pr*.28,0,Math.PI*2);
  ctx.fillStyle='rgba(255,255,255,'+(b.alpha*.55)+')'; ctx.fill();
}

function tick(){
  ctx.clearRect(0,0,W,H);
  bubbles.forEach((b,i)=>{
    b.wobble+=b.wobbleSpeed; b.pulse+=b.pulseSpeed;
    b.x+=b.speedX+Math.sin(b.wobble)*.4; b.y-=b.speedY;
    drawBubble(b);
    if(b.y+b.r < -50) bubbles[i]=mkBubble();
  });
  requestAnimationFrame(tick);
}
resize(); initBubbles(); tick();
window.addEventListener('resize',()=>{ resize(); initBubbles(); });

/* ────────── GAMES DATA ────────── */
const games = [
  {
    id: '90158090737937',
    name: '🥦 +1 Fat To Fit',
    creator: 'Boar Community',
    url: 'https://www.roblox.com/games/90158090737937/1-Fat-To-Fit',
    status: 'supported',
    freeFeatures: ['Auto Farm', 'Auto Teleport', 'Auto Rebirth', 'Auto Collect', 'Auto Eat', 'Fast Walk'],
    premiumFeatures: ['Instant Take All', 'Auto Upgrade', 'Fast Mode', 'Skip Animation', 'VIP Commands', 'Unlock All Areas']
  },
  {
    id: '13772394625',
    name: '⚔️ Blade Ball',
    creator: 'Wiggity',
    url: 'https://www.roblox.com/games/13772394625/Blade-Ball',
    status: 'updated',
    freeFeatures: ['Auto Parry', 'Auto Block', 'ESP Players', 'Ball Trajectory', 'Player Radar'],
    premiumFeatures: ['Instant Win', 'God Mode', 'Teleport to Ball', 'Auto Clicker', 'Speed Boost', 'Unlock All Swords']
  },
  {
    id: '142823291',
    name: '🔪 Murder Mystery 2',
    creator: 'Nikilis',
    url: 'https://www.roblox.com/games/142823291/Murder-Mystery-2',
    status: 'supported',
    freeFeatures: ['ESP Murderer', 'Auto Collect Coins', 'Player Radar', 'Gun ESP', 'Item ESP'],
    premiumFeatures: ['Instant Kill', 'God Mode', 'Teleport to Murderer', 'Auto Shoot', 'Infinite Ammo', 'Unlock All Knives']
  },
  {
    id: '87324404788780',
    name: '🐾 Pet Simulator 99',
    creator: 'BIG Games',
    url: 'https://www.roblox.com/games/87324404788780/Pet-Simulator-99',
    status: 'new-script',
    freeFeatures: ['Auto Farm', 'Auto Hatch', 'Auto Collect', 'Auto Rebirth', 'Auto Open Eggs'],
    premiumFeatures: ['Instant Take All', 'Mega Farm', 'Auto Upgrade', 'Fast Hatch', 'VIP Zone Access', 'Infinite Coins']
  },
  {
    id: '16732694052',
    name: '🎣 Fisch',
    creator: 'Fisching',
    url: 'https://www.roblox.com/games/16732694052/Fisch',
    status: 'not-functioning',
    freeFeatures: ['Auto Fish', 'Auto Shake', 'Fish ESP', 'Auto Sell', 'Weather Predict'],
    premiumFeatures: ['Instant Catch', 'Perfect Catch', 'Rare Fish Only', 'Auto Bait', 'Speed Fish', 'Unlock All Rods']
  },
  {
    id: '13576792216',
    name: '⚽ Blue Lock Rivals',
    creator: 'BL Rivals',
    url: 'https://www.roblox.com/games/13576792216/Blue-Lock-Rivals',
    status: 'supported',
    freeFeatures: ['Auto Dribble', 'Auto Shoot', 'Player ESP', 'Ball Tracker', 'Stamina ESP'],
    premiumFeatures: ['Instant Goal', 'Speed Boost', 'Perfect Pass', 'Stamina Hack', 'Unlock All Skills', 'Teleport to Ball']
  }
];

const CUSTOM_IMAGE = 'https://i.pinimg.com/736x/37/3a/b3/373ab3e072178f47dcb7fdafaddb6854.jpg';

function getStatusBadge(status) {
  const badges = {
    'supported': { text: '✅ Supported', class: 'supported' },
    'new-script': { text: '🆕 New Script', class: 'new-script' },
    'updated': { text: '🔄 Updated', class: 'updated' },
    'not-functioning': { text: '⚠️ Not Functioning', class: 'not-functioning' }
  };
  return badges[status] || badges['supported'];
}

function loadGames() {
  const container = document.getElementById('gamesContainer');
  container.innerHTML = '';
  
  games.forEach((game) => {
    const gameItem = document.createElement('div');
    gameItem.className = 'game-item';
    
    const statusBadge = getStatusBadge(game.status);
    
    gameItem.innerHTML = `
      <div class="game-header" onclick="this.parentElement.classList.toggle('expanded')">
        <div class="game-thumbnail">
          <img src="${CUSTOM_IMAGE}" alt="${game.name}" onerror="this.src='${CUSTOM_IMAGE}'">
        </div>
        <div class="game-info">
          <div class="game-name-row">
            <span class="game-name">${game.name}</span>
            <div class="status-badges">
              <span class="status-badge supported">
                <span class="status-dot"></span>
                ✅ Supported
              </span>
              ${game.status !== 'supported' ? `
                <span class="status-badge ${statusBadge.class}">
                  <span class="status-dot"></span>
                  ${statusBadge.text}
                </span>
              ` : ''}
            </div>
          </div>
          <div class="game-creator">${game.creator}</div>
        </div>
        <div class="dropdown-indicator">
          <span class="dropdown-arrow">▼</span>
        </div>
      </div>
      <div class="game-description">
        <div class="desc-content">
          <div class="feature-sections">
            <div class="feature-section">
              <div class="feature-title free-title">
                <span class="title-icon">🆓</span>
                <span>FreeMium User</span>
              </div>
              <ul class="feature-list">
                ${game.freeFeatures.map(f => `
                  <li>
                    <span class="feature-icon free-icon">[+]</span>
                    ${f}
                  </li>
                `).join('')}
              </ul>
            </div>
            <div class="feature-section">
              <div class="feature-title premium-title">
                <span class="title-icon">💎</span>
                <span>Premium User</span>
              </div>
              <ul class="feature-list">
                ${game.premiumFeatures.map(f => `
                  <li>
                    <span class="feature-icon premium-icon">[+]</span>
                    ${f}
                  </li>
                `).join('')}
              </ul>
            </div>
          </div>
          <div class="game-footer">
            <a class="game-link" href="${game.url}" target="_blank">
              🎮 Play ${game.name.split(' ').slice(1).join(' ')} →
            </a>
          </div>
        </div>
      </div>
    `;
    
    container.appendChild(gameItem);
  });
}

loadGames();
</script>
</body>
</html>
