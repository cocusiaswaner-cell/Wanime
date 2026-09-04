<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1, user-scalable=no">
<meta http-equiv="Content-Security-Policy" content="default-src 'self' 'unsafe-inline' data: https://fonts.googleapis.com https://fonts.gstatic.com; img-src 'self' data:; script-src 'self' 'unsafe-inline';">
<title>Wanime — Streaming Anime</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#0a0c10; --surface:#12151c; --surface-2:#181c25; --surface-3:#1f2430;
    --border:#242a37; --text:#f2f3f6; --text-dim:#8d95a6; --text-faint:#5b6274;
    --brand:#22d6ac; --brand-dim:#12503f; --amber:#f3b444; --link:#5b9dff; --danger:#ef5468;
    --radius-s:10px; --radius-m:16px; --radius-l:22px;
  }
  html[data-theme="light"]{
    --bg:#f4f5f7; --surface:#ffffff; --surface-2:#eef0f3; --surface-3:#e4e7ec;
    --border:#dde1e7; --text:#12151c; --text-dim:#5b6274; --text-faint:#8d95a6; --brand-dim:#d3f7ee;
  }
  *{box-sizing:border-box;-webkit-tap-highlight-color:transparent;}
  html,body{margin:0;padding:0;height:100%;}
  body{background:var(--bg);color:var(--text);font-family:'Inter',-apple-system,sans-serif;
    display:flex;justify-content:center;min-height:100vh;transition:background .25s ease,color .25s ease;}
  h1,h2,h3,.brand-font{font-family:'Space Grotesk',sans-serif;}
  ::selection{background:var(--brand);color:#04140f;}
  button,input,textarea,select{font-family:inherit;}
  a{color:var(--link);text-decoration:none;}
  .hidden{display:none !important;}
  ::-webkit-scrollbar{width:0;height:0;}

  .app-frame{width:100%;max-width:430px;min-height:100vh;background:var(--bg);position:relative;
    display:flex;flex-direction:column;border-left:1px solid var(--border);border-right:1px solid var(--border);overflow-x:hidden;}

  /* TOPBAR */
  #topbar{position:sticky;top:0;z-index:30;background:linear-gradient(180deg,var(--bg) 70%,transparent);backdrop-filter:blur(10px);padding:14px 16px 10px;}
  .brand-row{display:flex;align-items:center;justify-content:space-between;margin-bottom:12px;}
  .brand{display:flex;align-items:center;gap:8px;font-weight:700;font-size:20px;letter-spacing:-0.02em;}
  .brand .mark{width:26px;height:26px;border-radius:8px;background:linear-gradient(135deg,var(--brand),#0f8f72);
    display:flex;align-items:center;justify-content:center;color:#05140f;font-weight:700;font-size:14px;font-family:'Space Grotesk',sans-serif;}
  .topbar-actions{display:flex;gap:8px;align-items:center;}
  .icon-btn{width:36px;height:36px;border-radius:50%;background:var(--surface-2);border:1px solid var(--border);
    display:flex;align-items:center;justify-content:center;color:var(--text-dim);cursor:pointer;flex-shrink:0;}
  .icon-btn:active{transform:scale(.93);}
  .admin-pill{display:flex;align-items:center;gap:5px;background:var(--brand-dim);border:1px solid var(--brand);color:var(--brand);
    font-size:10.5px;font-weight:700;padding:6px 10px;border-radius:20px;cursor:pointer;white-space:nowrap;}

  .search-bar{display:flex;align-items:center;gap:10px;background:var(--surface-2);border:1px solid var(--border);
    border-radius:14px;padding:11px 14px;cursor:text;}
  .search-bar svg{flex-shrink:0;color:var(--text-faint);}
  .search-bar span{color:var(--text-faint);font-size:14.5px;}

  /* VIEWS */
  main.view{display:none;padding:4px 16px 100px;flex:1;animation:fade .2s ease;}
  main.view.active{display:block;}
  @keyframes fade{from{opacity:0;transform:translateY(4px);}to{opacity:1;transform:translateY(0);}}

  .section{margin-top:22px;}
  .section-head{display:flex;align-items:baseline;justify-content:space-between;margin-bottom:12px;}
  .section-head h2{font-size:18px;margin:0;font-weight:600;}
  .section-head h2 b{color:var(--brand);font-weight:700;}
  .section-head a.see-all{font-size:13px;color:var(--link);font-weight:500;white-space:nowrap;cursor:pointer;}

  .hscroll{display:flex;gap:12px;overflow-x:auto;scroll-snap-type:x proximity;padding-bottom:4px;margin:0 -16px;padding-left:16px;padding-right:16px;}
  .hscroll::-webkit-scrollbar{display:none;}
  .rank-grid{display:grid;grid-template-columns:1.15fr 1fr;gap:12px;}
  .rank-col{display:flex;flex-direction:column;gap:12px;}
  .catalog-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:12px;}

  .card{position:relative;flex-shrink:0;background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-m);overflow:hidden;scroll-snap-align:start;}
  .card-thumb{position:relative;aspect-ratio:2/3;width:100%;
    background:repeating-linear-gradient(135deg,var(--surface-3) 0 2px,var(--surface-2) 2px 14px);
    display:flex;align-items:center;justify-content:center;overflow:hidden;}
  .card-thumb img{width:100%;height:100%;object-fit:cover;position:relative;z-index:0;}
  .card-thumb::after{content:"";position:absolute;inset:0;background:linear-gradient(180deg,transparent 45%,rgba(0,0,0,.75) 100%);}
  .placeholder-glyph{color:var(--text-faint);z-index:1;opacity:.55;}
  .badge{position:absolute;top:8px;left:8px;z-index:2;background:var(--surface);color:var(--text);font-size:11px;font-weight:700;padding:3px 8px;border-radius:7px;border:1px solid var(--border);}
  .badge.rank{background:var(--amber);color:#241a02;border:none;}
  .badge.soon{background:rgba(0,0,0,.55);color:#fff;border:1px dashed rgba(255,255,255,.35);backdrop-filter:blur(2px);}
  .badge.status{background:rgba(0,0,0,.55);color:#fff;border:none;backdrop-filter:blur(2px);}
  .rating{position:absolute;top:8px;right:8px;z-index:2;display:flex;align-items:center;gap:3px;background:rgba(0,0,0,.55);backdrop-filter:blur(2px);padding:3px 7px;border-radius:7px;font-size:11.5px;font-weight:600;color:var(--amber);}
  .card-body{padding:9px 10px 11px;}
  .card-eps{font-size:11px;position:absolute;bottom:8px;left:8px;z-index:2;font-weight:600;color:#e7e9ee;}
  .card-title{font-size:12.5px;font-weight:600;line-height:1.3;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;min-height:32px;}
  .card-sub{font-size:10.5px;color:var(--text-faint);margin-top:3px;}
  .card-admin-actions{display:flex;gap:6px;padding:0 10px 10px;}
  .mini-btn{flex:1;padding:7px 0;border-radius:8px;border:1px solid var(--border);background:var(--surface-2);color:var(--text-dim);font-size:11px;font-weight:700;cursor:pointer;text-align:center;}
  .mini-btn.danger{color:var(--danger);border-color:rgba(239,84,104,.35);}
  .mini-btn:active{transform:scale(.96);}

  .chip-row{display:flex;gap:8px;overflow-x:auto;margin:0 -16px;padding:0 16px 4px;}
  .chip-row::-webkit-scrollbar{display:none;}
  .chip{flex-shrink:0;padding:8px 14px;border-radius:999px;background:var(--surface-2);border:1px solid var(--border);font-size:12.5px;font-weight:500;color:var(--text-dim);cursor:pointer;white-space:nowrap;}
  .chip.active{background:var(--brand);border-color:var(--brand);color:#04140f;font-weight:700;}
  .chip:active{transform:scale(.96);}

  .genre-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:9px;}
  .genre-tile{padding:13px 8px;text-align:center;border-radius:14px;background:var(--surface);border:1px solid var(--border);font-size:12.5px;font-weight:600;color:var(--text-dim);cursor:pointer;}
  .genre-tile.selected{background:var(--brand);color:#04140f;border-color:var(--brand);}
  .genre-tile:active{transform:scale(.97);}

  .empty-state{border:1.5px dashed var(--border);border-radius:var(--radius-l);padding:34px 20px;text-align:center;color:var(--text-dim);}
  .empty-state .eg{font-size:30px;margin-bottom:10px;}
  .empty-state h3{margin:0 0 6px;font-size:15px;color:var(--text);}
  .empty-state p{margin:0;font-size:12.5px;line-height:1.5;color:var(--text-faint);max-width:280px;margin:0 auto;}
  .empty-state .cta{margin-top:16px;display:inline-block;background:var(--brand);color:#04140f;font-weight:700;font-size:13px;padding:10px 20px;border-radius:12px;border:none;cursor:pointer;}
  .empty-mini{flex-shrink:0;width:118px;aspect-ratio:2/3;border-radius:var(--radius-m);border:1.5px dashed var(--border);
    display:flex;flex-direction:column;align-items:center;justify-content:center;gap:6px;color:var(--text-faint);background:var(--surface);}
  .empty-mini span{font-size:10px;font-weight:600;text-align:center;padding:0 8px;}

  .banner{border-radius:var(--radius-l);padding:20px;position:relative;overflow:hidden;background:linear-gradient(120deg,var(--brand-dim),var(--surface-2) 70%);border:1px solid var(--border);margin-top:18px;}
  .banner h3{margin:0 0 6px;font-size:15.5px;}
  .banner p{margin:0 0 12px;font-size:12px;color:var(--text-dim);max-width:230px;line-height:1.5;}
  .banner button{background:var(--text);color:var(--bg);border:none;padding:9px 16px;border-radius:11px;font-weight:700;font-size:12.5px;cursor:pointer;}

  .day-tabs{display:flex;gap:6px;overflow-x:auto;margin:0 -16px 16px;padding:0 16px;}
  .day-tabs::-webkit-scrollbar{display:none;}
  .day-tab{flex-shrink:0;padding:9px 14px;border-radius:12px;background:var(--surface-2);border:1px solid var(--border);font-size:12.5px;font-weight:600;color:var(--text-dim);cursor:pointer;}
  .day-tab.active{background:var(--text);color:var(--bg);border-color:var(--text);}

  .profile-card{display:flex;align-items:center;gap:13px;padding:16px;background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-l);margin-top:6px;cursor:pointer;}
  .avatar{width:52px;height:52px;border-radius:50%;flex-shrink:0;background:linear-gradient(135deg,var(--brand),#0f8f72);
    display:flex;align-items:center;justify-content:center;font-weight:700;font-size:20px;color:#04140f;font-family:'Space Grotesk',sans-serif;}
  .profile-card .name{font-weight:700;font-size:15.5px;}
  .profile-card .role{font-size:11px;color:var(--brand);font-weight:700;margin-top:2px;display:inline-flex;align-items:center;gap:4px;}
  .profile-card .role.admin{color:var(--amber);}
  .menu-group{margin-top:20px;}
  .menu-label{font-size:11.5px;text-transform:uppercase;letter-spacing:.06em;color:var(--text-faint);font-weight:700;margin:0 0 8px 4px;}
  .menu-item{display:flex;align-items:center;gap:12px;padding:13px 4px;border-bottom:1px solid var(--border);cursor:pointer;}
  .menu-item:last-child{border-bottom:none;}
  .menu-item .m-icon{width:34px;height:34px;border-radius:10px;background:var(--surface-2);display:flex;align-items:center;justify-content:center;color:var(--text-dim);flex-shrink:0;}
  .menu-item .m-text{flex:1;min-width:0;}
  .menu-item .m-title{font-size:13.5px;font-weight:600;}
  .menu-item .m-sub{font-size:11px;color:var(--text-faint);margin-top:1px;}
  .menu-item .chev{color:var(--text-faint);flex-shrink:0;}

  .toggle{width:42px;height:25px;border-radius:20px;background:var(--surface-3);position:relative;cursor:pointer;flex-shrink:0;border:1px solid var(--border);transition:.2s;}
  .toggle::after{content:"";position:absolute;width:19px;height:19px;border-radius:50%;background:var(--text-faint);top:2px;left:2px;transition:.2s;}
  .toggle.on{background:var(--brand);border-color:var(--brand);}
  .toggle.on::after{transform:translateX(17px);background:#04140f;}

  .notice{display:flex;gap:10px;background:var(--surface-2);border:1px solid var(--border);border-radius:14px;padding:13px;margin-top:18px;}
  .notice svg{flex-shrink:0;color:var(--amber);margin-top:1px;}
  .notice p{margin:0;font-size:11.5px;line-height:1.55;color:var(--text-dim);}
  .notice b{color:var(--text);}
  .notice.brand svg{color:var(--brand);}

  #bottom-nav{position:sticky;bottom:0;z-index:30;display:flex;justify-content:space-around;align-items:center;background:var(--surface);border-top:1px solid var(--border);padding:9px 4px calc(9px + env(safe-area-inset-bottom));}
  .nav-btn{display:flex;flex-direction:column;align-items:center;gap:3px;background:none;border:none;color:var(--text-faint);cursor:pointer;padding:4px 10px;border-radius:12px;font-size:10px;font-weight:600;}
  .nav-btn.active{color:var(--brand);}
  .nav-btn.active .nb-pill{background:var(--brand-dim);}
  .nb-pill{padding:4px 14px;border-radius:10px;}
  .nb-pill svg{display:block;}

  #search-overlay{position:fixed;inset:0;z-index:100;background:var(--bg);display:none;flex-direction:column;max-width:430px;margin:0 auto;left:0;right:0;}
  #search-overlay.open{display:flex;}
  .search-top{display:flex;align-items:center;gap:10px;padding:14px 16px;border-bottom:1px solid var(--border);}
  .search-top .search-bar{flex:1;}
  .search-top input{background:none;border:none;outline:none;color:var(--text);font-size:14.5px;width:100%;}
  .search-top input::placeholder{color:var(--text-faint);}
  .search-cancel{font-size:13.5px;color:var(--link);font-weight:600;background:none;border:none;cursor:pointer;flex-shrink:0;}
  .search-body{padding:16px;overflow-y:auto;flex:1;}
  .tag-row{display:flex;flex-wrap:wrap;gap:8px;margin-top:10px;}

  .sheet-backdrop{position:fixed;inset:0;background:rgba(4,6,10,.6);z-index:150;display:none;max-width:430px;margin:0 auto;}
  .sheet-backdrop.open{display:block;}
  .sheet{position:absolute;left:0;right:0;bottom:0;background:var(--surface);border-radius:22px 22px 0 0;border:1px solid var(--border);border-bottom:none;
    padding:10px 18px calc(22px + env(safe-area-inset-bottom));max-height:86vh;overflow-y:auto;animation:slideup .22s ease;}
  @keyframes slideup{from{transform:translateY(30px);opacity:.4;}to{transform:translateY(0);opacity:1;}}
  .sheet .handle{width:38px;height:4px;background:var(--border);border-radius:3px;margin:6px auto 16px;}
  .sheet-head{display:flex;align-items:flex-start;justify-content:space-between;gap:10px;}
  .sheet h3{margin:0 0 4px;font-size:16.5px;}
  .sheet .sheet-sub{font-size:12px;color:var(--text-faint);margin-bottom:16px;}
  .sheet-close{width:30px;height:30px;border-radius:50%;background:var(--surface-2);border:1px solid var(--border);color:var(--text-dim);display:flex;align-items:center;justify-content:center;cursor:pointer;flex-shrink:0;}

  .setting-row{display:flex;align-items:center;justify-content:space-between;padding:12px 0;border-bottom:1px solid var(--border);gap:10px;}
  .setting-row:last-child{border-bottom:none;}
  .setting-row .s-title{font-size:13.5px;font-weight:600;}
  .setting-row .s-sub{font-size:11px;color:var(--text-faint);margin-top:2px;}

  .device-row{display:flex;align-items:center;gap:11px;padding:11px 0;border-bottom:1px solid var(--border);}
  .device-row:last-child{border-bottom:none;}
  .device-row .d-icon{width:32px;height:32px;border-radius:9px;background:var(--surface-2);display:flex;align-items:center;justify-content:center;color:var(--text-dim);}
  .device-row .d-title{font-size:13px;font-weight:600;}
  .device-row .d-sub{font-size:10.5px;color:var(--text-faint);margin-top:1px;}
  .device-row .d-dot{width:7px;height:7px;border-radius:50%;background:var(--brand);margin-left:auto;flex-shrink:0;}

  .field{margin-bottom:14px;}
  .field label{display:block;font-size:12px;font-weight:700;color:var(--text-dim);margin-bottom:6px;}
  .field input[type=text], .field input[type=password], .field input[type=number], .field textarea, .field select{
    width:100%;background:var(--surface-2);border:1px solid var(--border);border-radius:11px;padding:11px 13px;color:var(--text);font-size:13.5px;outline:none;}
  .field input:focus, .field textarea:focus, .field select:focus{border-color:var(--brand);}
  .field textarea{resize:vertical;min-height:70px;}
  .field .hint{font-size:10.5px;color:var(--text-faint);margin-top:5px;}
  .field .err{font-size:11.5px;color:var(--danger);margin-top:6px;display:none;}
  .field .err.show{display:block;}
  .genre-select-row{display:flex;flex-wrap:wrap;gap:7px;}
  .file-btn{display:flex;align-items:center;gap:8px;background:var(--surface-2);border:1px dashed var(--border);border-radius:11px;padding:12px;font-size:12.5px;color:var(--text-dim);cursor:pointer;}
  .file-preview{width:56px;height:56px;border-radius:10px;object-fit:cover;flex-shrink:0;background:var(--surface-3);}

  .btn-primary{width:100%;background:var(--brand);color:#04140f;border:none;padding:13px;border-radius:12px;font-weight:700;font-size:14px;cursor:pointer;margin-top:6px;}
  .btn-primary:active{transform:scale(.98);}
  .btn-secondary{width:100%;background:var(--surface-3);color:var(--text);border:none;padding:13px;border-radius:12px;font-weight:700;font-size:13.5px;cursor:pointer;margin-top:10px;}

  .admin-row{display:flex;align-items:center;gap:10px;padding:10px 0;border-bottom:1px solid var(--border);}
  .admin-row:last-child{border-bottom:none;}
  .admin-thumb{width:44px;height:58px;border-radius:8px;object-fit:cover;background:var(--surface-2);flex-shrink:0;}
  .admin-row .a-title{font-size:13px;font-weight:700;}
  .admin-row .a-sub{font-size:10.5px;color:var(--text-faint);margin-top:2px;}
  .admin-row .a-actions{display:flex;gap:6px;margin-left:auto;flex-shrink:0;}
  .icon-mini{width:30px;height:30px;border-radius:9px;background:var(--surface-2);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;color:var(--text-dim);cursor:pointer;}
  .icon-mini.danger{color:var(--danger);}

  #toast-wrap{position:fixed;bottom:86px;left:0;right:0;display:flex;flex-direction:column;align-items:center;gap:8px;z-index:200;max-width:430px;margin:0 auto;pointer-events:none;}
  .toast{background:var(--text);color:var(--bg);font-size:12.5px;font-weight:600;padding:10px 18px;border-radius:12px;box-shadow:0 8px 24px rgba(0,0,0,.35);animation:toastIn .18s ease,toastOut .25s ease 2.4s forwards;text-align:center;}
  @keyframes toastIn{from{transform:translateY(10px);opacity:0;}to{transform:translateY(0);opacity:1;}}
  @keyframes toastOut{to{opacity:0;transform:translateY(6px);}}
</style>
</head>
<body>
<div class="app-frame" id="app-frame">

  <header id="topbar">
    <div class="brand-row">
      <div class="brand"><span class="mark">W</span>anime</div>
      <div class="topbar-actions">
        <div class="admin-pill hidden" id="admin-pill">
          <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.4"><path d="M12 2v20M2 12h20"/></svg>
          Kelola
        </div>
        <button class="icon-btn" id="btn-theme" aria-label="Ganti tema">
          <svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 12.8A9 9 0 1 1 11.2 3a7 7 0 0 0 9.8 9.8Z"/></svg>
        </button>
      </div>
    </div>
    <div class="search-bar" id="open-search">
      <svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="7"/><path d="m21 21-4.3-4.3"/></svg>
      <span>Cari anime, genre, atau studio…</span>
    </div>
  </header>

  <!-- ================= HOME ================= -->
  <main class="view active" id="view-home">
    <div class="section">
      <div class="section-head"><h2>Anime <b>Trending</b></h2><a class="see-all" data-nav="explore">Lihat semua ›</a></div>
      <div class="rank-grid" id="rank-grid"></div>
    </div>
    <div class="section">
      <div class="section-head"><h2>Jelajahi Genre</h2><a class="see-all" data-nav="explore">Semua genre ›</a></div>
      <div class="chip-row" id="home-genre-chips"></div>
    </div>
    <div class="section">
      <div class="section-head"><h2>Update Terbaru</h2><a class="see-all" data-nav="jadwal">Jadwal rilis ›</a></div>
      <div class="hscroll" id="row-update"></div>
    </div>
    <div class="section">
      <div class="section-head"><h2>Rekomendasi Aksi</h2></div>
      <div class="hscroll" id="row-action"></div>
    </div>
    <div class="section">
      <div class="section-head"><h2>Anime Tamat</h2></div>
      <div class="hscroll" id="row-completed"></div>
    </div>
    <div class="banner">
      <h3>Katalog baru dimulai dari sini</h3>
      <p>Wanime baru diluncurkan — koleksi akan bertambah secara berkala. Aktifkan notifikasi agar tidak ketinggalan judul pertama.</p>
      <button id="btn-notify">Aktifkan notifikasi</button>
    </div>
  </main>

  <!-- ================= EXPLORE / GENRE ================= -->
  <main class="view" id="view-explore">
    <div class="section" style="margin-top:14px;">
      <div class="section-head"><h2>Semua <b>Genre</b></h2></div>
      <div class="genre-grid" id="genre-grid"></div>
    </div>
    <div class="section" id="genre-result-section">
      <div class="section-head"><h2 id="genre-result-title">Pilih genre</h2></div>
      <div id="genre-result-body">
        <div class="empty-state">
          <div class="eg">🎬</div>
          <h3>Ketuk salah satu genre</h3>
          <p>Pilih genre di atas untuk melihat daftar anime pada kategori tersebut.</p>
        </div>
      </div>
    </div>
  </main>

  <!-- ================= JADWAL ================= -->
  <main class="view" id="view-jadwal">
    <div class="section" style="margin-top:14px;">
      <div class="section-head"><h2>Jadwal <b>Rilis</b></h2></div>
      <div class="day-tabs" id="day-tabs"></div>
      <div class="empty-state">
        <div class="eg">🗓️</div>
        <h3 id="jadwal-title">Belum ada jadwal hari ini</h3>
        <p>Jadwal tayang mingguan akan muncul di sini begitu judul pertama Wanime dirilis.</p>
      </div>
    </div>
  </main>

  <!-- ================= RIWAYAT / KOLEKSI ================= -->
  <main class="view" id="view-riwayat">
    <div class="section" style="margin-top:14px;">
      <div class="section-head"><h2>Terakhir <b>Ditonton</b></h2></div>
      <div class="empty-state">
        <div class="eg">🕓</div>
        <h3>Riwayat kamu masih kosong</h3>
        <p>Anime yang kamu tonton akan otomatis tersimpan di sini.</p>
        <button class="cta" data-nav="explore">Jelajahi anime</button>
      </div>
    </div>
    <div class="section">
      <div class="section-head"><h2>Koleksi Saya</h2></div>
      <div class="empty-state">
        <div class="eg">🔖</div>
        <h3>Belum ada yang disimpan</h3>
        <p>Ketuk ikon bookmark pada judul untuk menyimpannya ke koleksi.</p>
      </div>
    </div>
  </main>

  <!-- ================= PROFIL ================= -->
  <main class="view" id="view-profil">

    <!-- state: belum masuk -->
    <div id="profil-guest" style="margin-top:14px;">
      <div class="empty-state">
        <div class="eg">👤</div>
        <h3>Kamu belum masuk</h3>
        <p>Masuk untuk mengakses pengaturan akun, keamanan, dan riwayat tontonanmu.</p>
        <button class="cta" id="btn-open-login">Masuk</button>
      </div>
      <div class="menu-group">
        <div class="menu-label">Lainnya</div>
        <div class="menu-item" data-sheet="sheet-theme">
          <div class="m-icon"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 12.8A9 9 0 1 1 11.2 3a7 7 0 0 0 9.8 9.8Z"/></svg></div>
          <div class="m-text"><div class="m-title">Tampilan</div><div class="m-sub">Tema gelap / terang</div></div>
          <svg class="chev" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 6 6 6-6 6"/></svg>
        </div>
        <div class="menu-item" data-sheet="sheet-about">
          <div class="m-icon"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="9"/><path d="M12 16v-4M12 8h.01"/></svg></div>
          <div class="m-text"><div class="m-title">Tentang Wanime</div><div class="m-sub">Versi 1.1.0</div></div>
          <svg class="chev" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 6 6 6-6 6"/></svg>
        </div>
      </div>
    </div>

    <!-- state: sudah masuk -->
    <div id="profil-user" class="hidden">
      <div class="profile-card" id="profile-card-btn" style="margin-top:14px;">
        <div class="avatar" id="profile-avatar">A</div>
        <div style="flex:1;min-width:0;">
          <div class="name" id="profile-name">Pengguna</div>
          <div class="role" id="profile-role">
            <svg width="11" height="11" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2 4 5v6c0 5 3.4 9.4 8 11 4.6-1.6 8-6 8-11V5l-8-3Z"/></svg>
            PENGGUNA
          </div>
        </div>
        <svg class="chev" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 6 6 6-6 6"/></svg>
      </div>

      <div class="menu-group" id="admin-menu-group" class="hidden">
        <div class="menu-label">Administrator</div>
        <div class="menu-item" id="menu-manage-content">
          <div class="m-icon" style="color:var(--amber);"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2v20M2 12h20"/></svg></div>
          <div class="m-text"><div class="m-title">Kelola konten</div><div class="m-sub" id="catalog-count-sub">0 anime dalam katalog</div></div>
          <svg class="chev" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 6 6 6-6 6"/></svg>
        </div>
      </div>

      <div class="menu-group">
        <div class="menu-label">Akun</div>
        <div class="menu-item" data-sheet="sheet-account">
          <div class="m-icon"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="8" r="4"/><path d="M4 21c0-4 3.6-7 8-7s8 3 8 7"/></svg></div>
          <div class="m-text"><div class="m-title">Pengaturan akun</div><div class="m-sub">Profil, preferensi tontonan</div></div>
          <svg class="chev" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 6 6 6-6 6"/></svg>
        </div>
        <div class="menu-item" data-sheet="sheet-security">
          <div class="m-icon"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2 4 5v6c0 5 3.4 9.4 8 11 4.6-1.6 8-6 8-11V5l-8-3Z"/></svg></div>
          <div class="m-text"><div class="m-title">Keamanan &amp; privasi</div><div class="m-sub">Verifikasi 2 langkah, perangkat aktif</div></div>
          <svg class="chev" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 6 6 6-6 6"/></svg>
        </div>
        <div class="menu-item" data-sheet="sheet-theme">
          <div class="m-icon"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 12.8A9 9 0 1 1 11.2 3a7 7 0 0 0 9.8 9.8Z"/></svg></div>
          <div class="m-text"><div class="m-title">Tampilan</div><div class="m-sub">Tema gelap / terang</div></div>
          <svg class="chev" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 6 6 6-6 6"/></svg>
        </div>
      </div>

      <div class="menu-group">
        <div class="menu-label">Lainnya</div>
        <div class="menu-item" data-sheet="sheet-about">
          <div class="m-icon"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="9"/><path d="M12 16v-4M12 8h.01"/></svg></div>
          <div class="m-text"><div class="m-title">Tentang Wanime</div><div class="m-sub">Versi 1.1.0</div></div>
          <svg class="chev" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 6 6 6-6 6"/></svg>
        </div>
        <div class="menu-item" id="btn-logout">
          <div class="m-icon" style="color:var(--danger);"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h4M16 17l5-5-5-5M21 12H9"/></svg></div>
          <div class="m-text"><div class="m-title" style="color:var(--danger);">Keluar akun</div></div>
        </div>
      </div>

      <div class="notice">
        <svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 9v4M12 17h.01M10.3 3.9 2 18a1.7 1.7 0 0 0 1.5 2.5h17a1.7 1.7 0 0 0 1.5-2.5L13.7 3.9a1.7 1.7 0 0 0-3.4 0Z"/></svg>
        <p id="content-notice"><b>Penambahan konten dibatasi.</b> Hanya administrator resmi Wanime yang dapat menambahkan atau mengubah judul di katalog.</p>
      </div>
    </div>
  </main>

  <nav id="bottom-nav">
    <button class="nav-btn active" data-view="home">
      <span class="nb-pill"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m3 11 9-8 9 8"/><path d="M5 10v10h14V10"/></svg></span>Beranda
    </button>
    <button class="nav-btn" data-view="jadwal">
      <span class="nb-pill"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="5" width="18" height="16" rx="2"/><path d="M3 10h18M8 3v4M16 3v4"/></svg></span>Jadwal
    </button>
    <button class="nav-btn" data-view="explore">
      <span class="nb-pill"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2v2M12 20v2M2 12h2M20 12h2M4.9 4.9l1.4 1.4M17.7 17.7l1.4 1.4M4.9 19.1l1.4-1.4M17.7 6.3l1.4-1.4"/><circle cx="12" cy="12" r="4"/></svg></span>Genre
    </button>
    <button class="nav-btn" data-view="riwayat">
      <span class="nb-pill"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3 3"/></svg></span>Riwayat
    </button>
    <button class="nav-btn" data-view="profil">
      <span class="nb-pill"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="8" r="4"/><path d="M4 21c0-4 3.6-7 8-7s8 3 8 7"/></svg></span>Profil
    </button>
  </nav>

  <!-- ================= SEARCH OVERLAY ================= -->
  <div id="search-overlay">
    <div class="search-top">
      <div class="search-bar" style="flex:1;">
        <svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="7"/><path d="m21 21-4.3-4.3"/></svg>
        <input id="search-input" type="text" maxlength="60" placeholder="Cari anime di sini" autocomplete="off">
      </div>
      <button class="search-cancel" id="close-search">Batal</button>
    </div>
    <div class="search-body"><div id="search-result"></div></div>
  </div>

  <!-- ================= SHEETS ================= -->
  <div class="sheet-backdrop" id="sheet-backdrop">

    <div class="sheet hidden" id="sheet-login">
      <div class="handle"></div>
      <div class="sheet-head"><div><h3>Masuk ke Wanime</h3><div class="sheet-sub">Gunakan akun kamu untuk melanjutkan.</div></div><div class="sheet-close" data-close>✕</div></div>
      <form id="login-form">
        <div class="field">
          <label>Nama pengguna</label>
          <input type="text" id="login-user" maxlength="40" placeholder="cth. akunku" autocomplete="off" required>
        </div>
        <div class="field">
          <label>Kata sandi</label>
          <input type="password" id="login-pass" maxlength="60" placeholder="Kata sandi" required>
          <div class="err" id="login-err">Nama pengguna dan kata sandi wajib diisi.</div>
        </div>
        <button type="submit" class="btn-primary">Masuk</button>
        <div class="field" style="margin-top:14px;margin-bottom:0;">
          <div class="hint">Login pada demo ini disimulasikan di sisi klien (tanpa server) dan akan tereset saat halaman dimuat ulang. Masuk dengan kredensial administrator akan membuka akses "Kelola konten".</div>
        </div>
      </form>
    </div>

    <div class="sheet hidden" id="sheet-security">
      <div class="handle"></div>
      <div class="sheet-head"><div><h3>Keamanan &amp; privasi</h3><div class="sheet-sub">Kelola proteksi akses akun Wanime kamu.</div></div><div class="sheet-close" data-close>✕</div></div>
      <div class="setting-row"><div><div class="s-title">Verifikasi 2 langkah</div><div class="s-sub">Kode tambahan saat login perangkat baru</div></div><div class="toggle on" data-toggle data-msg-on="Verifikasi 2 langkah diaktifkan" data-msg-off="Verifikasi 2 langkah dinonaktifkan"></div></div>
      <div class="setting-row"><div><div class="s-title">Kunci layar streaming</div><div class="s-sub">Cegah tangkapan layar pada pemutar</div></div><div class="toggle on" data-toggle data-msg-on="Kunci layar diaktifkan" data-msg-off="Kunci layar dinonaktifkan"></div></div>
      <div class="setting-row"><div><div class="s-title">Notifikasi login baru</div><div class="s-sub">Peringatan e-mail untuk perangkat asing</div></div><div class="toggle" data-toggle data-msg-on="Notifikasi login diaktifkan" data-msg-off="Notifikasi login dinonaktifkan"></div></div>
      <div class="menu-label" style="margin-top:18px;">Perangkat aktif</div>
      <div class="device-row">
        <div class="d-icon"><svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="2" width="14" height="20" rx="2"/><path d="M12 18h.01"/></svg></div>
        <div><div class="d-title">Perangkat ini</div><div class="d-sub">Aktif sekarang · Indonesia</div></div>
        <div class="d-dot"></div>
      </div>
      <button class="btn-secondary" id="btn-signout-others">Keluar dari semua perangkat lain</button>
    </div>

    <div class="sheet hidden" id="sheet-account">
      <div class="handle"></div>
      <div class="sheet-head"><div><h3>Pengaturan akun</h3><div class="sheet-sub">Preferensi dasar untuk pengalaman menontonmu.</div></div><div class="sheet-close" data-close>✕</div></div>
      <div class="setting-row"><div><div class="s-title">Putar otomatis episode</div><div class="s-sub">Lanjut ke episode berikutnya</div></div><div class="toggle on" data-toggle data-msg-on="Putar otomatis diaktifkan" data-msg-off="Putar otomatis dinonaktifkan"></div></div>
      <div class="setting-row"><div><div class="s-title">Skip intro otomatis</div></div><div class="toggle" data-toggle data-msg-on="Skip intro diaktifkan" data-msg-off="Skip intro dinonaktifkan"></div></div>
      <div class="setting-row"><div><div class="s-title">Simpan riwayat tontonan</div></div><div class="toggle on" data-toggle data-msg-on="Riwayat akan disimpan" data-msg-off="Riwayat tidak akan disimpan"></div></div>
      <div class="setting-row" id="row-subtitle-lang" style="cursor:pointer;">
        <div><div class="s-title">Bahasa subtitle</div><div class="s-sub" id="subtitle-lang-val">Indonesia</div></div>
        <svg class="chev" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m9 6 6 6-6 6"/></svg>
      </div>
    </div>

    <div class="sheet hidden" id="sheet-theme">
      <div class="handle"></div>
      <div class="sheet-head"><div><h3>Tampilan</h3><div class="sheet-sub">Pilih mode tampilan yang nyaman untukmu.</div></div><div class="sheet-close" data-close>✕</div></div>
      <div class="setting-row"><div><div class="s-title">Mode gelap</div><div class="s-sub">Direkomendasikan untuk menonton malam hari</div></div><div class="toggle on" id="toggle-dark"></div></div>
    </div>

    <div class="sheet hidden" id="sheet-about">
      <div class="handle"></div>
      <div class="sheet-head"><div><h3>Tentang Wanime</h3><div class="sheet-sub">Wanime v1.1.0</div></div><div class="sheet-close" data-close>✕</div></div>
      <p style="font-size:12.5px;color:var(--text-dim);line-height:1.6;">Wanime adalah platform streaming anime. Katalog diisi secara bertahap oleh administrator melalui panel "Kelola konten". Pengguna umum tidak dapat menambah maupun mengubah judul.</p>
    </div>

    <!-- ADMIN: daftar konten -->
    <div class="sheet hidden" id="sheet-manage">
      <div class="handle"></div>
      <div class="sheet-head"><div><h3>Kelola konten</h3><div class="sheet-sub" id="manage-sub">0 anime dalam katalog</div></div><div class="sheet-close" data-close>✕</div></div>
      <button class="btn-primary" id="btn-add-anime">+ Tambah anime baru</button>
      <div style="margin-top:16px;" id="manage-list"></div>
    </div>

    <!-- ADMIN: form tambah/edit -->
    <div class="sheet hidden" id="sheet-form">
      <div class="handle"></div>
      <div class="sheet-head"><div><h3 id="form-title">Tambah anime</h3><div class="sheet-sub">Data ini hanya tersimpan selama sesi berjalan.</div></div><div class="sheet-close" data-close>✕</div></div>
      <form id="anime-form">
        <div class="field">
          <label>Poster (opsional)</label>
          <label class="file-btn" id="file-btn-label">
            <img id="file-preview" class="file-preview hidden" alt="">
            <span id="file-btn-text">Ketuk untuk unggah gambar poster</span>
          </label>
          <input type="file" id="poster-input" accept="image/*" class="hidden">
        </div>
        <div class="field">
          <label>Judul anime *</label>
          <input type="text" id="f-title" maxlength="80" placeholder="cth. Petualangan Awan Senja" required>
          <div class="err" id="f-title-err">Judul wajib diisi.</div>
        </div>
        <div class="field">
          <label>Sinopsis</label>
          <textarea id="f-synopsis" maxlength="400" placeholder="Ringkasan singkat cerita…"></textarea>
        </div>
        <div class="field" style="display:flex;gap:10px;">
          <div style="flex:1;">
            <label>Jumlah episode</label>
            <input type="number" id="f-episodes" min="0" max="9999" placeholder="12">
          </div>
          <div style="flex:1;">
            <label>Rating (0–10)</label>
            <input type="number" id="f-rating" min="0" max="10" step="0.01" placeholder="7.50">
          </div>
        </div>
        <div class="field">
          <label>Status tayang</label>
          <select id="f-status">
            <option value="Ongoing">Ongoing</option>
            <option value="Tamat">Tamat</option>
          </select>
        </div>
        <div class="field">
          <label>Genre * (pilih minimal satu)</label>
          <div class="genre-select-row" id="form-genre-row"></div>
          <div class="err" id="f-genre-err">Pilih minimal satu genre.</div>
        </div>
        <button type="submit" class="btn-primary" id="btn-save-anime">Simpan anime</button>
      </form>
    </div>

  </div>
</div>

<div id="toast-wrap"></div>

<script>
(function(){
  "use strict";

  /* =========================================================
     STATE
  ========================================================= */
  var GENRES = ["Movie","Action","Adventure","Comedy","Demons","Drama","Ecchi","Fantasy","Game","Harem",
    "Historical","Horror","Josei","Magic","Martial Arts","Mecha","Military","Music","Mystery","Psychological",
    "Parody","Police","Romance","Samurai","School","Sci-Fi","Seinen","Shoujo","Shoujo Ai","Shounen",
    "Slice of Life","Sports","Space","Super Power","Supernatural","Thriller","Vampire"];
  var DAYS = ["Senin","Selasa","Rabu","Kamis","Jumat","Sabtu","Minggu"];

  // Katalog tersimpan hanya di memori (sesi berjalan) — bukan localStorage, sesuai batasan artifact.
  var CATALOG = [];
  var nextId = 1;

  // Kredensial admin demo. CATATAN PENTING: ini hanya untuk simulasi front-end.
  // Pada aplikasi produksi sungguhan, verifikasi admin WAJIB dilakukan di server,
  // bukan dicocokkan di kode klien seperti ini.
  var ADMIN_USER = "admin";
  var ADMIN_PASS = "wanime-admin";

  var state = { loggedIn:false, isAdmin:false, username:"", selectedGenre:null, editingId:null, posterData:null, formGenres:[] };

  /* =========================================================
     UTIL
  ========================================================= */
  function escapeHTML(str){
    return String(str).replace(/[&<>"']/g, function(c){ return {"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]; });
  }
  function debounce(fn, ms){ var t; return function(){ var a=arguments,ctx=this; clearTimeout(t); t=setTimeout(function(){fn.apply(ctx,a);}, ms); }; }
  if(!window.CSS) window.CSS = {};
  if(!window.CSS.escape){ window.CSS.escape = function(s){ return String(s).replace(/[^a-zA-Z0-9_\-]/g, "\\$&"); }; }

  function toast(msg){
    var wrap = document.getElementById("toast-wrap");
    var el = document.createElement("div");
    el.className = "toast";
    el.textContent = msg;
    wrap.appendChild(el);
    setTimeout(function(){ el.remove(); }, 2700);
  }

  document.addEventListener("contextmenu", function(e){
    if(e.target.closest(".card-thumb") || e.target.closest(".empty-mini")){ e.preventDefault(); toast("Konten dilindungi hak cipta"); }
  });
  document.addEventListener("dragstart", function(e){
    if(e.target.closest(".card") || e.target.closest(".empty-mini")) e.preventDefault();
  });

  /* =========================================================
     CARD RENDERING
  ========================================================= */
  function cardThumbInner(item){
    if(item && item.poster){
      return '<img src="'+item.poster+'" alt="'+escapeHTML(item.title)+'">';
    }
    return '<svg class="placeholder-glyph" width="30" height="30" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><rect x="3" y="4" width="18" height="14" rx="2"/><path d="m3 9 5-5M8 18l5-5m6-5-5 5"/></svg>';
  }

  function renderCard(item, opts){
    opts = opts || {};
    var rankBadge = opts.rank ? '<span class="badge rank">#'+opts.rank+'</span>' : "";
    var ratingHtml = (item.rating!=null && item.rating!=="") ? '<div class="rating">★ '+escapeHTML(item.rating)+'</div>' : "";
    var epsHtml = item.episodes ? '<div class="card-eps">Eps '+escapeHTML(item.episodes)+'</div>' : "";
    var statusHtml = !opts.rank ? '<span class="badge status">'+escapeHTML(item.status||"Ongoing")+'</span>' : "";
    var adminActions = "";
    if(state.isAdmin && opts.adminActions){
      adminActions = '<div class="card-admin-actions">'
        + '<button type="button" class="mini-btn" data-edit="'+item.id+'">Edit</button>'
        + '<button type="button" class="mini-btn danger" data-delete="'+item.id+'">Hapus</button>'
        + '</div>';
    }
    return '<div class="card">'
      + '<div class="card-thumb">' + rankBadge + statusHtml + ratingHtml + epsHtml + cardThumbInner(item) + '</div>'
      + '<div class="card-body"><div class="card-title">'+escapeHTML(item.title)+'</div>'
      + '<div class="card-sub">'+escapeHTML((item.genres||[]).slice(0,2).join(", ") || "—")+'</div></div>'
      + adminActions
      + '</div>';
  }

  function emptyMini(label){
    return '<div class="empty-mini"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><rect x="3" y="4" width="18" height="14" rx="2"/><path d="m3 9 5-5M8 18l5-5m6-5-5 5"/></svg><span>'+escapeHTML(label)+'</span></div>';
  }

  function bindCardAdminEvents(container){
    if(!state.isAdmin) return;
    container.querySelectorAll("[data-edit]").forEach(function(btn){
      btn.addEventListener("click", function(e){ e.stopPropagation(); openAnimeForm(btn.dataset.edit); });
    });
    container.querySelectorAll("[data-delete]").forEach(function(btn){
      btn.addEventListener("click", function(e){ e.stopPropagation(); deleteAnime(btn.dataset.delete); });
    });
  }

  /* =========================================================
     RENDER: HOME
  ========================================================= */
  function renderHome(){
    // Rank grid (top 3 by rating)
    var ranked = CATALOG.slice().sort(function(a,b){ return (parseFloat(b.rating)||0) - (parseFloat(a.rating)||0); }).slice(0,3);
    var rankGrid = document.getElementById("rank-grid");
    if(ranked.length === 0){
      rankGrid.innerHTML =
        '<div class="card"><div class="card-thumb"><span class="badge rank">#1</span><span class="badge soon" style="left:auto;right:8px;">Segera</span>'
        + '<svg class="placeholder-glyph" width="34" height="34" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><rect x="3" y="4" width="18" height="14" rx="2"/><path d="m3 9 5-5M8 18l5-5m6-5-5 5"/></svg></div>'
        + '<div class="card-body"><div class="card-title">Slot #1 kosong</div><div class="card-sub">Menunggu rilis pertama</div></div></div>'
        + '<div class="rank-col">'
        + '<div class="card" style="display:flex;flex-direction:row;"><div class="card-thumb" style="width:92px;aspect-ratio:1/1;flex-shrink:0;"><span class="badge rank">#2</span></div><div class="card-body" style="display:flex;flex-direction:column;justify-content:center;"><div class="card-title">Slot #2 kosong</div><div class="card-sub">Belum ada judul</div></div></div>'
        + '<div class="card" style="display:flex;flex-direction:row;"><div class="card-thumb" style="width:92px;aspect-ratio:1/1;flex-shrink:0;"><span class="badge rank">#3</span></div><div class="card-body" style="display:flex;flex-direction:column;justify-content:center;"><div class="card-title">Slot #3 kosong</div><div class="card-sub">Belum ada judul</div></div></div>'
        + '</div>';
    } else {
      var html = renderCard(ranked[0], {rank:1});
      html += '<div class="rank-col">';
      for(var i=1;i<3;i++){
        if(ranked[i]) html += renderCard(ranked[i], {rank:i+1});
        else html += '<div class="card" style="display:flex;flex-direction:row;"><div class="card-thumb" style="width:92px;aspect-ratio:1/1;flex-shrink:0;"><span class="badge rank">#'+(i+1)+'</span></div><div class="card-body" style="display:flex;flex-direction:column;justify-content:center;"><div class="card-title">Slot kosong</div><div class="card-sub">Belum ada judul</div></div></div>';
      }
      html += '</div>';
      rankGrid.innerHTML = html;
      bindCardAdminEvents(rankGrid);
    }

    renderRow("row-update", CATALOG.slice().sort(function(a,b){return b.id-a.id;}).slice(0,8));
    renderRow("row-action", CATALOG.filter(function(a){return (a.genres||[]).indexOf("Action")>-1;}));
    renderRow("row-completed", CATALOG.filter(function(a){return a.status==="Tamat";}));
  }

  function renderRow(containerId, list){
    var el = document.getElementById(containerId);
    if(!el) return;
    if(list.length === 0){
      var h = "";
      for(var i=0;i<4;i++) h += emptyMini("Segera hadir");
      el.innerHTML = h;
      return;
    }
    el.innerHTML = list.map(function(item){ return renderCard(item, {adminActions:true}); }).join("");
    bindCardAdminEvents(el);
  }

  /* =========================================================
     RENDER: EXPLORE / GENRE
  ========================================================= */
  var homeChips = document.getElementById("home-genre-chips");
  var genreGrid = document.getElementById("genre-grid");

  GENRES.forEach(function(g){
    var c1 = document.createElement("div");
    c1.className = "chip"; c1.textContent = g;
    c1.addEventListener("click", function(){ goExplore(g); });
    homeChips.appendChild(c1);

    var tile = document.createElement("div");
    tile.className = "genre-tile"; tile.textContent = g;
    tile.dataset.genre = g;
    tile.addEventListener("click", function(){ selectGenre(this.dataset.genre); });
    genreGrid.appendChild(tile);
  });

  function selectGenre(g){
    state.selectedGenre = g;
    document.querySelectorAll(".genre-tile").forEach(function(t){ t.classList.toggle("selected", t.dataset.genre===g); });
    document.getElementById("genre-result-title").textContent = g;
    var body = document.getElementById("genre-result-body");
    var items = CATALOG.filter(function(a){ return (a.genres||[]).indexOf(g) > -1; });
    if(items.length === 0){
      body.innerHTML = '<div class="empty-state"><div class="eg">🎬</div><h3>Belum ada anime di genre ini</h3><p>Konten akan ditambahkan oleh administrator secara bertahap. Cek kembali nanti.</p></div>';
    } else {
      body.innerHTML = '<div class="catalog-grid">' + items.map(function(item){ return renderCard(item, {adminActions:true}); }).join("") + '</div>';
      bindCardAdminEvents(body);
    }
  }
  function goExplore(g){ showView("explore"); selectGenre(g); document.getElementById("genre-result-section").scrollIntoView({behavior:"smooth", block:"nearest"}); }

  /* =========================================================
     JADWAL
  ========================================================= */
  var dayTabs = document.getElementById("day-tabs");
  var todayIdx = (new Date().getDay() + 6) % 7;
  DAYS.forEach(function(d, i){
    var b = document.createElement("div");
    b.className = "day-tab" + (i===todayIdx ? " active" : "");
    b.textContent = d;
    b.addEventListener("click", function(){
      dayTabs.querySelectorAll(".day-tab").forEach(function(x){x.classList.remove("active");});
      b.classList.add("active");
      document.getElementById("jadwal-title").textContent = "Belum ada jadwal di hari " + d;
    });
    dayTabs.appendChild(b);
  });
  document.getElementById("jadwal-title").textContent = "Belum ada jadwal di hari " + DAYS[todayIdx];

  /* =========================================================
     NAVIGASI
  ========================================================= */
  var views = ["home","explore","jadwal","riwayat","profil"];
  function showView(name){
    views.forEach(function(v){ document.getElementById("view-"+v).classList.toggle("active", v===name); });
    document.querySelectorAll(".nav-btn").forEach(function(b){ b.classList.toggle("active", b.dataset.view===name); });
    window.scrollTo({top:0});
  }
  document.querySelectorAll(".nav-btn").forEach(function(b){ b.addEventListener("click", function(){ showView(b.dataset.view); }); });
  document.querySelectorAll("[data-nav]").forEach(function(el){ el.addEventListener("click", function(){ showView(el.dataset.nav); }); });

  /* =========================================================
     SEARCH
  ========================================================= */
  var overlay = document.getElementById("search-overlay");
  var searchInput = document.getElementById("search-input");
  var resultBox = document.getElementById("search-result");
  document.getElementById("open-search").addEventListener("click", function(){
    overlay.classList.add("open"); searchInput.value=""; renderSearchDefault(); setTimeout(function(){searchInput.focus();}, 50);
  });
  document.getElementById("close-search").addEventListener("click", function(){ overlay.classList.remove("open"); });

  function renderSearchDefault(){
    var recent = CATALOG.slice().sort(function(a,b){return b.id-a.id;}).slice(0,4);
    var html = "";
    if(recent.length){
      html += '<div class="menu-label">Baru ditambahkan</div><div class="catalog-grid" id="search-recent"></div>';
    }
    html += '<div class="menu-label" style="margin-top:'+(recent.length?"18px":"0")+';">Genre populer</div><div class="tag-row" id="search-genre-tags"></div>';
    resultBox.innerHTML = html;
    if(recent.length){
      var rec = document.getElementById("search-recent");
      rec.innerHTML = recent.map(function(item){ return renderCard(item, {}); }).join("");
    }
    var tagRow = document.getElementById("search-genre-tags");
    GENRES.slice(0,12).forEach(function(g){
      var c = document.createElement("div");
      c.className = "chip"; c.textContent = g;
      c.addEventListener("click", function(){ overlay.classList.remove("open"); goExplore(g); });
      tagRow.appendChild(c);
    });
  }

  var doSearch = debounce(function(){
    var raw = searchInput.value;
    var safeQuery = raw.replace(/[^a-zA-Z0-9\u00C0-\u024F \-]/g, "").trim().slice(0, 60);
    if(!safeQuery){ renderSearchDefault(); return; }
    var q = safeQuery.toLowerCase();
    var titleMatches = CATALOG.filter(function(a){ return a.title.toLowerCase().indexOf(q) > -1; });
    var matchedGenres = GENRES.filter(function(g){ return g.toLowerCase().indexOf(q) === 0; });

    if(titleMatches.length){
      resultBox.innerHTML = '<div class="menu-label">Hasil untuk "'+escapeHTML(safeQuery)+'"</div><div class="catalog-grid" id="search-title-results"></div>';
      document.getElementById("search-title-results").innerHTML = titleMatches.map(function(item){ return renderCard(item, {}); }).join("");
      return;
    }
    var html = '<div class="empty-state" style="padding:26px 16px;"><div class="eg">🔍</div><h3>Tidak ada hasil untuk "'+escapeHTML(safeQuery)+'"</h3><p>Coba jelajahi berdasarkan genre di bawah ini.</p></div>';
    if(matchedGenres.length) html += '<div class="menu-label" style="margin-top:16px;">Genre serupa</div><div class="tag-row" id="search-match-tags"></div>';
    resultBox.innerHTML = html;
    if(matchedGenres.length){
      var box = document.getElementById("search-match-tags");
      matchedGenres.forEach(function(g){
        var c = document.createElement("div");
        c.className = "chip"; c.textContent = g;
        c.addEventListener("click", function(){ overlay.classList.remove("open"); goExplore(g); });
        box.appendChild(c);
      });
    }
  }, 250);
  searchInput.addEventListener("input", doSearch);

  /* =========================================================
     SHEETS (buka / tutup)
  ========================================================= */
  var backdrop = document.getElementById("sheet-backdrop");
  function openSheet(id){
    document.querySelectorAll(".sheet").forEach(function(s){ s.classList.add("hidden"); });
    document.getElementById(id).classList.remove("hidden");
    backdrop.classList.add("open");
  }
  function closeSheets(){ backdrop.classList.remove("open"); }
  document.querySelectorAll("[data-sheet]").forEach(function(item){
    item.addEventListener("click", function(){ openSheet(item.dataset.sheet); });
  });
  document.querySelectorAll("[data-close]").forEach(function(btn){ btn.addEventListener("click", closeSheets); });
  backdrop.addEventListener("click", function(e){ if(e.target === backdrop) closeSheets(); });

  /* generic toggles (kecuali toggle tema, ditangani terpisah) */
  document.querySelectorAll("[data-toggle]").forEach(function(t){
    t.addEventListener("click", function(){
      t.classList.toggle("on");
      var msg = t.classList.contains("on") ? t.dataset.msgOn : t.dataset.msgOff;
      if(msg) toast(msg);
    });
  });

  /* =========================================================
     TEMA (perbaikan bug double-handler)
  ========================================================= */
  function applyTheme(light){
    document.documentElement.setAttribute("data-theme", light ? "light" : "dark");
    document.getElementById("toggle-dark").classList.toggle("on", !light);
  }
  document.getElementById("btn-theme").addEventListener("click", function(){
    var isLight = document.documentElement.getAttribute("data-theme") === "light";
    applyTheme(!isLight);
    toast(isLight ? "Mode gelap diaktifkan" : "Mode terang diaktifkan");
  });
  document.getElementById("toggle-dark").addEventListener("click", function(){
    var darkNow = this.classList.contains("on");
    applyTheme(darkNow); // jika sedang gelap (on) -> pindah ke terang; else -> ke gelap
    toast(darkNow ? "Mode terang diaktifkan" : "Mode gelap diaktifkan");
  });

  document.getElementById("row-subtitle-lang").addEventListener("click", function(){
    var el = document.getElementById("subtitle-lang-val");
    el.textContent = el.textContent === "Indonesia" ? "English" : "Indonesia";
    toast("Bahasa subtitle diganti ke " + el.textContent);
  });

  document.getElementById("btn-signout-others").addEventListener("click", function(){
    toast("Berhasil keluar dari semua perangkat lain");
  });

  document.getElementById("btn-notify").addEventListener("click", function(){
    toast("Notifikasi diaktifkan — kamu akan diberi tahu saat judul pertama rilis");
  });

  /* =========================================================
     LOGIN / LOGOUT
  ========================================================= */
  var profilGuest = document.getElementById("profil-guest");
  var profilUser = document.getElementById("profil-user");
  var adminMenuGroup = document.getElementById("admin-menu-group");
  var adminPill = document.getElementById("admin-pill");

  function renderProfil(){
    profilGuest.classList.toggle("hidden", state.loggedIn);
    profilUser.classList.toggle("hidden", !state.loggedIn);
    adminPill.classList.toggle("hidden", !state.isAdmin);
    if(!state.loggedIn) return;
    document.getElementById("profile-avatar").textContent = state.username.charAt(0).toUpperCase();
    document.getElementById("profile-name").textContent = state.username;
    var roleEl = document.getElementById("profile-role");
    if(state.isAdmin){
      roleEl.classList.add("admin");
      roleEl.innerHTML = '<svg width="11" height="11" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2 4 5v6c0 5 3.4 9.4 8 11 4.6-1.6 8-6 8-11V5l-8-3Z"/></svg> ADMINISTRATOR';
    } else {
      roleEl.classList.remove("admin");
      roleEl.innerHTML = '<svg width="11" height="11" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2 4 5v6c0 5 3.4 9.4 8 11 4.6-1.6 8-6 8-11V5l-8-3Z"/></svg> PENGGUNA TERVERIFIKASI';
    }
    adminMenuGroup.classList.toggle("hidden", !state.isAdmin);
    document.getElementById("catalog-count-sub").textContent = CATALOG.length + " anime dalam katalog";
    document.getElementById("content-notice").innerHTML = state.isAdmin
      ? '<b>Kamu masuk sebagai administrator.</b> Kamu dapat menambah, mengedit, dan menghapus anime melalui menu "Kelola konten" di atas.'
      : '<b>Penambahan konten dibatasi.</b> Hanya administrator resmi Wanime yang dapat menambahkan atau mengubah judul di katalog.';
  }

  document.getElementById("btn-open-login").addEventListener("click", function(){
    document.getElementById("login-user").value = "";
    document.getElementById("login-pass").value = "";
    document.getElementById("login-err").classList.remove("show");
    openSheet("sheet-login");
  });

  document.getElementById("login-form").addEventListener("submit", function(e){
    e.preventDefault();
    var user = document.getElementById("login-user").value.trim();
    var pass = document.getElementById("login-pass").value;
    var errEl = document.getElementById("login-err");
    if(!user || !pass){ errEl.textContent = "Nama pengguna dan kata sandi wajib diisi."; errEl.classList.add("show"); return; }
    errEl.classList.remove("show");

    var isAdminLogin = (user.toLowerCase() === ADMIN_USER && pass === ADMIN_PASS);
    state.loggedIn = true;
    state.isAdmin = isAdminLogin;
    state.username = isAdminLogin ? "Administrator" : user;
    closeSheets();
    renderProfil();
    renderHome(); // agar tombol admin di kartu ikut muncul/hilang
    toast(isAdminLogin ? "Berhasil masuk sebagai Administrator" : "Berhasil masuk sebagai " + user);
  });

  document.getElementById("btn-logout").addEventListener("click", function(){
    state.loggedIn = false; state.isAdmin = false; state.username = "";
    closeSheets();
    renderProfil();
    renderHome();
    showView("profil");
    toast("Berhasil keluar");
  });

  document.getElementById("profile-card-btn").addEventListener("click", function(){ openSheet("sheet-account"); });

  document.getElementById("menu-manage-content").addEventListener("click", function(){ openManageSheet(); });

  /* =========================================================
     ADMIN: KELOLA KONTEN (CRUD)
  ========================================================= */
  var formGenreRow = document.getElementById("form-genre-row");
  GENRES.forEach(function(g){
    var chip = document.createElement("div");
    chip.className = "chip"; chip.textContent = g; chip.dataset.genre = g;
    chip.addEventListener("click", function(){
      var idx = state.formGenres.indexOf(g);
      if(idx>-1){ state.formGenres.splice(idx,1); chip.classList.remove("active"); }
      else { state.formGenres.push(g); chip.classList.add("active"); }
    });
    formGenreRow.appendChild(chip);
  });

  function openManageSheet(){
    document.getElementById("manage-sub").textContent = CATALOG.length + " anime dalam katalog";
    var listEl = document.getElementById("manage-list");
    if(CATALOG.length === 0){
      listEl.innerHTML = '<div class="empty-state" style="padding:26px 16px;"><div class="eg">📭</div><h3>Katalog masih kosong</h3><p>Ketuk "Tambah anime baru" untuk mulai mengisi katalog Wanime.</p></div>';
    } else {
      listEl.innerHTML = CATALOG.slice().sort(function(a,b){return b.id-a.id;}).map(function(item){
        var thumb = item.poster ? '<img class="admin-thumb" src="'+item.poster+'" alt="">' : '<div class="admin-thumb"></div>';
        return '<div class="admin-row">' + thumb
          + '<div style="min-width:0;"><div class="a-title">'+escapeHTML(item.title)+'</div><div class="a-sub">'+escapeHTML((item.genres||[]).join(", "))+' · '+escapeHTML(item.status)+'</div></div>'
          + '<div class="a-actions">'
          + '<div class="icon-mini" data-edit="'+item.id+'"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 20h9M16.5 3.5a2.1 2.1 0 0 1 3 3L7 19l-4 1 1-4Z"/></svg></div>'
          + '<div class="icon-mini danger" data-delete="'+item.id+'"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M3 6h18M8 6V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v2m3 0-1 14a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2L4 6"/></svg></div>'
          + '</div></div>';
      }).join("");
      listEl.querySelectorAll("[data-edit]").forEach(function(b){ b.addEventListener("click", function(){ openAnimeForm(b.dataset.edit); }); });
      listEl.querySelectorAll("[data-delete]").forEach(function(b){ b.addEventListener("click", function(){ deleteAnime(b.dataset.delete); }); });
    }
    openSheet("sheet-manage");
  }

  document.getElementById("btn-add-anime").addEventListener("click", function(){ openAnimeForm(null); });

  function resetForm(){
    state.editingId = null; state.posterData = null; state.formGenres = [];
    document.getElementById("anime-form").reset();
    document.getElementById("f-status").value = "Ongoing";
    document.getElementById("f-title-err").classList.remove("show");
    document.getElementById("f-genre-err").classList.remove("show");
    formGenreRow.querySelectorAll(".chip").forEach(function(c){ c.classList.remove("active"); });
    document.getElementById("file-preview").classList.add("hidden");
    document.getElementById("file-btn-text").textContent = "Ketuk untuk unggah gambar poster";
  }

  function openAnimeForm(id){
    resetForm();
    document.getElementById("form-title").textContent = id ? "Edit anime" : "Tambah anime";
    if(id){
      var item = CATALOG.find(function(a){ return String(a.id) === String(id); });
      if(item){
        state.editingId = item.id;
        document.getElementById("f-title").value = item.title;
        document.getElementById("f-synopsis").value = item.synopsis || "";
        document.getElementById("f-episodes").value = item.episodes || "";
        document.getElementById("f-rating").value = item.rating || "";
        document.getElementById("f-status").value = item.status || "Ongoing";
        state.formGenres = (item.genres || []).slice();
        formGenreRow.querySelectorAll(".chip").forEach(function(c){ c.classList.toggle("active", state.formGenres.indexOf(c.dataset.genre) > -1); });
        if(item.poster){
          state.posterData = item.poster;
          var prev = document.getElementById("file-preview");
          prev.src = item.poster; prev.classList.remove("hidden");
          document.getElementById("file-btn-text").textContent = "Ganti gambar poster";
        }
      }
    }
    openSheet("sheet-form");
  }

  document.getElementById("poster-input").addEventListener("change", function(e){
    var file = e.target.files && e.target.files[0];
    if(!file) return;
    if(!file.type.startsWith("image/")){ toast("File harus berupa gambar"); return; }
    if(file.size > 3*1024*1024){ toast("Ukuran gambar maksimal 3MB"); return; }
    var reader = new FileReader();
    reader.onload = function(ev){
      state.posterData = ev.target.result;
      var prev = document.getElementById("file-preview");
      prev.src = state.posterData; prev.classList.remove("hidden");
      document.getElementById("file-btn-text").textContent = "Ganti gambar poster";
    };
    reader.onerror = function(){ toast("Gagal membaca file gambar"); };
    reader.readAsDataURL(file);
  });

  document.getElementById("anime-form").addEventListener("submit", function(e){
    e.preventDefault();
    var title = document.getElementById("f-title").value.trim();
    var titleErr = document.getElementById("f-title-err");
    var genreErr = document.getElementById("f-genre-err");
    var valid = true;
    if(!title){ titleErr.classList.add("show"); valid = false; } else { titleErr.classList.remove("show"); }
    if(state.formGenres.length === 0){ genreErr.classList.add("show"); valid = false; } else { genreErr.classList.remove("show"); }
    if(!valid) return;

    var data = {
      title: title,
      synopsis: document.getElementById("f-synopsis").value.trim(),
      episodes: document.getElementById("f-episodes").value,
      rating: document.getElementById("f-rating").value,
      status: document.getElementById("f-status").value,
      genres: state.formGenres.slice(),
      poster: state.posterData
    };

    if(state.editingId){
      var idx = CATALOG.findIndex(function(a){ return a.id === state.editingId; });
      if(idx > -1) CATALOG[idx] = Object.assign(CATALOG[idx], data);
      toast('"' + title + '" berhasil diperbarui');
    } else {
      data.id = nextId++;
      CATALOG.push(data);
      toast('"' + title + '" berhasil ditambahkan ke katalog');
    }
    closeSheets();
    renderHome();
    if(state.selectedGenre) selectGenre(state.selectedGenre);
    renderProfil();
  });

  function deleteAnime(id){
    var idx = CATALOG.findIndex(function(a){ return String(a.id) === String(id); });
    if(idx === -1) return;
    var title = CATALOG[idx].title;
    CATALOG.splice(idx, 1);
    toast('"' + title + '" dihapus dari katalog');
    renderHome();
    if(state.selectedGenre) selectGenre(state.selectedGenre);
    renderProfil();
    if(!document.getElementById("sheet-manage").classList.contains("hidden")) openManageSheet();
  }

  /* =========================================================
     INIT
  ========================================================= */
  renderSearchDefault();
  renderProfil();
  renderHome();
})();
</script>
</body>
</html>
