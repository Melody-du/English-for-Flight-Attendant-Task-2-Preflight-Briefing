[Uploading index.html.html…]()
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>航前准备会英语 · HU7480实训系统</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
    <style>
        /* ===== 全部样式（与上一版保持一致，仅微调对话卡片） ===== */
        * { margin:0; padding:0; box-sizing:border-box; }
        body { font-family:'Segoe UI','PingFang SC',Roboto,sans-serif; background:#f0f4f9; color:#1a2a3a; padding-top:68px; line-height:1.6; }
        .navbar { position:fixed; top:0; left:0; right:0; z-index:1000; background:linear-gradient(145deg,#1a1a3e,#2c2c6e); padding:0 14px; height:64px; display:flex; align-items:center; justify-content:space-between; box-shadow:0 4px 20px rgba(26,26,62,0.35); gap:4px; flex-wrap:nowrap; }
        .navbar .brand { display:flex; align-items:center; gap:8px; color:#fff; font-weight:700; font-size:0.85rem; white-space:nowrap; }
        .navbar .brand i { color:#f5d98f; font-size:1.1rem; }
        .navbar .brand span { font-size:0.6rem; font-weight:400; opacity:0.6; }
        .navbar .nav-links { display:flex; gap:2px; flex-wrap:nowrap; overflow-x:auto; -webkit-overflow-scrolling:touch; }
        .navbar .nav-links a { color:rgba(255,255,255,0.6); text-decoration:none; padding:4px 10px; border-radius:30px; font-size:0.65rem; font-weight:600; transition:all 0.25s; white-space:nowrap; cursor:pointer; }
        .navbar .nav-links a:hover { color:#fff; background:rgba(255,255,255,0.08); }
        .navbar .nav-links a.active { color:#1a1a3e; background:#f5d98f; }
        .navbar .right-actions { display:flex; align-items:center; gap:6px; flex-shrink:0; }
        .navbar .print-btn { background:rgba(255,255,255,0.1); border:1px solid rgba(255,255,255,0.15); color:#fff; padding:3px 12px; border-radius:30px; font-size:0.6rem; font-weight:600; cursor:pointer; transition:0.2s; display:flex; align-items:center; gap:4px; white-space:nowrap; }
        .navbar .print-btn:hover { background:rgba(255,255,255,0.2); }
        .container { max-width:1100px; margin:0 auto; padding:12px 14px 30px; }
        .page { display:none; animation:fadeUp 0.3s ease; }
        .page.active { display:block; }
        @keyframes fadeUp { from { opacity:0; transform:translateY(10px); } to { opacity:1; transform:translateY(0); } }
        .card { background:#fff; border-radius:16px; padding:18px 20px; box-shadow:0 2px 12px rgba(0,0,0,0.04); margin-bottom:18px; border:1px solid rgba(0,0,0,0.02); }
        .card-title { font-size:1.05rem; font-weight:700; color:#1a1a3e; margin-bottom:12px; display:flex; align-items:center; gap:10px; }
        .card-title i { color:#c99f4a; font-size:1rem; }
        .card-title .sub { font-weight:400; font-size:0.7rem; color:#8a9eb0; margin-left:auto; }
        .section-desc { color:#4a5a6e; font-size:0.9rem; margin-bottom:12px; }
        .form-row { display:grid; grid-template-columns:repeat(auto-fit,minmax(180px,1fr)); gap:12px; }
        .form-group { display:flex; flex-direction:column; gap:3px; }
        .form-group label { font-weight:600; font-size:0.78rem; color:#1a1a3e; }
        .form-group input, .form-group textarea, .form-group select { padding:6px 12px; border-radius:8px; border:1px solid #dce4ec; font-size:0.85rem; background:#fafcff; transition:0.2s; font-family:inherit; }
        .form-group input:focus, .form-group textarea:focus, .form-group select:focus { border-color:#c99f4a; outline:none; box-shadow:0 0 0 3px rgba(201,159,74,0.08); }
        .btn { padding:5px 16px; border-radius:30px; border:none; font-weight:600; font-size:0.75rem; cursor:pointer; transition:all 0.2s; display:inline-flex; align-items:center; gap:5px; }
        .btn-primary { background:#f5d98f; color:#1a1a3e; }
        .btn-primary:hover { background:#ffe8b5; transform:translateY(-1px); }
        .btn-success { background:#2d7d5a; color:#fff; }
        .btn-success:hover { background:#3a9d72; }
        .btn-outline { background:transparent; border:1.5px solid #dce4ec; color:#5a6e82; }
        .btn-outline:hover { border-color:#b6cce0; background:#f7faff; }
        .btn-danger { background:#c0392b; color:#fff; }
        .btn-danger:hover { background:#e74c3c; }
        .btn-sm { padding:3px 12px; font-size:0.65rem; }
        .btn:disabled { opacity:0.5; cursor:not-allowed; transform:none !important; }
        .text-muted { color:#8a9eb0; font-size:0.78rem; }
        .text-gold { color:#c99f4a; }
        .text-success { color:#2d7d5a; }
        .text-danger { color:#c0392b; }

        /* 词汇卡片 */
        .vocab-grid { display:grid; grid-template-columns:repeat(auto-fill,minmax(220px,1fr)); gap:12px; }
        .vocab-card { background:#f7faff; border-radius:12px; padding:14px 16px; border:1px solid #e6edf6; transition:0.2s; }
        .vocab-card:hover { border-color:#b6cce0; background:#f0f6fe; }
        .vocab-card .word { font-weight:700; font-size:1.05rem; color:#1a1a3e; }
        .vocab-card .phonetic { font-size:0.8rem; color:#8a9eb0; margin-left:6px; font-weight:400; }
        .vocab-card .meaning { font-size:0.85rem; color:#4a5a6e; margin:2px 0 6px; }
        .vocab-card .actions { display:flex; align-items:center; gap:6px; flex-wrap:wrap; margin-top:6px; }
        .vocab-card .actions .speak-btn { background:rgba(201,159,74,0.12); border:none; color:#c99f4a; width:30px; height:30px; border-radius:50%; cursor:pointer; font-size:0.8rem; transition:0.2s; }
        .vocab-card .actions .speak-btn:hover { background:#c99f4a; color:#fff; }
        .vocab-card .actions .speak-btn.speaking { background:#2d7d5a; color:#fff; animation:pulse-icon 0.8s infinite; }
        .vocab-card .actions .record-btn { background:rgba(52,152,219,0.12); border:none; color:#2980b9; width:30px; height:30px; border-radius:50%; cursor:pointer; font-size:0.8rem; transition:0.2s; }
        .vocab-card .actions .record-btn:hover { background:#2980b9; color:#fff; }
        .vocab-card .actions .record-btn.recording { background:#c0392b; color:#fff; animation:pulse-icon 0.6s infinite; }
        .vocab-card .score-display { margin-top:6px; font-size:0.8rem; font-weight:600; display:flex; align-items:center; gap:6px; }
        .vocab-card .score-display .score-value { padding:2px 10px; border-radius:20px; font-size:0.85rem; }
        .score-excellent { background:#d4edda; color:#1a6e4a; }
        .score-good { background:#d6eaf8; color:#1a5276; }
        .score-fair { background:#fdebd0; color:#935e38; }
        .score-poor { background:#fadbd8; color:#922b21; }
        .score-none { background:#e6edf6; color:#8a9eb0; }
        @keyframes pulse-icon { 0%,100% { transform:scale(1); opacity:1; } 50% { transform:scale(0.85); opacity:0.6; } }

        /* 句型分组 */
        .phrase-section { margin-bottom:20px; }
        .phrase-section-title { font-weight:700; font-size:0.95rem; color:#1a1a3e; padding:8px 14px; background:#f0f4f9; border-radius:10px; margin-bottom:8px; display:flex; align-items:center; gap:10px; }
        .phrase-section-title .badge { font-size:0.65rem; font-weight:600; background:#c99f4a; color:#fff; padding:0 12px; border-radius:20px; line-height:1.8; }
        .phrase-list { display:flex; flex-direction:column; gap:6px; padding-left:0; }
        .phrase-item { display:flex; align-items:center; gap:10px; padding:7px 14px; background:#f7faff; border-radius:10px; border-left:4px solid #c99f4a; transition:0.2s; flex-wrap:wrap; }
        .phrase-item:hover { background:#f0f6fe; }
        .phrase-item .en { font-weight:600; font-size:0.88rem; color:#1a1a3e; min-width:160px; display:flex; align-items:center; gap:6px; flex:1; }
        .phrase-item .zh { color:#4a5a6e; font-size:0.82rem; }
        .phrase-item .speak-icon-sm { font-size:0.65rem; color:#b6cce0; cursor:pointer; transition:0.2s; }
        .phrase-item .speak-icon-sm:hover { color:#c99f4a; }

        /* ===== 对话卡片（全新设计） ===== */
        .dialogue-grid { display:grid; grid-template-columns:repeat(auto-fill,minmax(380px,1fr)); gap:18px; }
        .dialogue-card { background:#f7faff; border-radius:16px; padding:18px 20px; border:1px solid #e6edf6; transition:0.2s; display:flex; flex-direction:column; }
        .dialogue-card:hover { border-color:#b6cce0; box-shadow:0 2px 12px rgba(0,0,0,0.04); }
        .dialogue-card .d-header { display:flex; align-items:center; gap:10px; margin-bottom:12px; flex-wrap:wrap; }
        .dialogue-card .d-num { font-size:0.6rem; font-weight:700; color:#c99f4a; background:rgba(201,159,74,0.1); padding:2px 12px; border-radius:20px; display:inline-block; }
        .dialogue-card .d-title { font-weight:700; font-size:1rem; color:#1a1a3e; }
        .dialogue-card .d-scene-label { font-size:0.7rem; color:#8a9eb0; margin-left:auto; background:#e6edf6; padding:1px 12px; border-radius:20px; }
        .dialogue-card .d-body { display:flex; flex-direction:column; gap:6px; margin:4px 0 10px; }
        .dialogue-card .d-line { display:flex; align-items:flex-start; gap:8px; padding:5px 10px; border-radius:8px; background:#fff; border-left:3px solid #c99f4a; }
        .dialogue-card .d-line.purser { border-left-color:#c99f4a; background:#fcf9f0; }
        .dialogue-card .d-line.crew { border-left-color:#2980b9; background:#f0f7ff; }
        .dialogue-card .d-line .d-speaker { font-weight:700; font-size:0.75rem; color:#4a5a6e; min-width:70px; white-space:nowrap; }
        .dialogue-card .d-line .d-text { font-size:0.88rem; color:#1a1a3e; line-height:1.5; flex:1; }
        .dialogue-card .d-line .d-trans { font-size:0.78rem; color:#8a9eb0; display:block; margin-top:1px; }
        .dialogue-card .d-audio-bar { display:flex; align-items:center; gap:8px; margin-top:8px; padding-top:8px; border-top:1px dashed #e6edf6; flex-wrap:wrap; }
        .dialogue-card .d-audio-bar .btn-audio-sm { background:rgba(201,159,74,0.1); border:none; color:#c99f4a; padding:4px 12px; border-radius:20px; font-size:0.65rem; font-weight:600; cursor:pointer; transition:0.2s; display:inline-flex; align-items:center; gap:4px; }
        .dialogue-card .d-audio-bar .btn-audio-sm:hover { background:#c99f4a; color:#fff; }
        .dialogue-card .d-audio-bar .btn-audio-sm.playing { background:#2d7d5a; color:#fff; animation:pulse-icon 0.8s infinite; }
        .dialogue-card .d-audio-bar .btn-recording-sm { background:rgba(41,128,185,0.12); border:none; color:#2980b9; padding:4px 12px; border-radius:20px; font-size:0.65rem; font-weight:600; cursor:pointer; transition:0.2s; display:inline-flex; align-items:center; gap:4px; }
        .dialogue-card .d-audio-bar .btn-recording-sm:hover { background:#2980b9; color:#fff; }
        .dialogue-card .d-audio-bar .btn-recording-sm.recording { background:#c0392b; color:#fff; animation:pulse-icon 0.6s infinite; }
        .dialogue-card .d-audio-bar .d-status { font-size:0.65rem; color:#8a9eb0; }
        .dialogue-card .d-audio-bar .d-status.done { color:#2d7d5a; font-weight:600; }
        @media (max-width:600px) { .dialogue-grid { grid-template-columns:1fr; } }

        /* 案例信息卡 */
        .case-card { display:grid; grid-template-columns:1fr 1fr; gap:16px; }
        .case-card .info-item { background:#f7faff; border-radius:10px; padding:12px 16px; border:1px solid #e6edf6; }
        .case-card .info-item .label { font-weight:600; font-size:0.75rem; color:#8a9eb0; text-transform:uppercase; letter-spacing:0.5px; }
        .case-card .info-item .value { font-weight:700; font-size:1rem; color:#1a1a3e; margin-top:2px; }
        .case-card .info-item .value.en { color:#2980b9; font-weight:600; font-size:0.9rem; }
        .case-card .info-item .value.zh { color:#4a5a6e; font-size:0.85rem; }
        @media (max-width:600px) { .case-card { grid-template-columns:1fr; } }

        /* 角色与对话编排 */
        .role-grid { display:grid; grid-template-columns:repeat(auto-fit,minmax(180px,1fr)); gap:12px; }
        .role-card { background:#f7faff; border-radius:12px; padding:12px 14px; border:1px solid #e6edf6; }
        .role-card .r-title { font-weight:700; font-size:0.85rem; color:#1a1a3e; display:flex; align-items:center; gap:6px; }
        .role-card .r-title .icon { color:#c99f4a; }
        .role-card .r-name input { width:100%; padding:4px 10px; border-radius:6px; border:1px solid #dce4ec; font-size:0.8rem; background:#fff; margin-top:4px; }
        .role-card .r-name input:focus { border-color:#c99f4a; outline:none; }
        .script-step { display:flex; align-items:center; gap:10px; padding:8px 12px; background:#fafcff; border-radius:8px; border:1px solid #e6edf6; margin-bottom:6px; flex-wrap:wrap; }
        .script-step .step-num { font-weight:700; font-size:0.75rem; color:#8a9eb0; min-width:30px; }
        .script-step select, .script-step input { padding:4px 8px; border-radius:6px; border:1px solid #dce4ec; font-size:0.8rem; background:#fff; flex:1 1 140px; min-width:100px; }
        .script-step select:focus, .script-step input:focus { border-color:#c99f4a; outline:none; }
        .script-step .custom-input { flex:2 1 180px; }
        .script-step .btn-remove-step { background:transparent; border:none; color:#c0392b; cursor:pointer; font-size:0.8rem; padding:2px 6px; }
        .script-step .btn-remove-step:hover { background:rgba(192,57,43,0.1); border-radius:4px; }
        .script-preview { background:#f7faff; border-radius:10px; padding:12px 16px; border:1px solid #e6edf6; margin-top:10px; white-space:pre-wrap; font-family:'Consolas',monospace; font-size:0.85rem; line-height:1.8; max-height:300px; overflow-y:auto; }

        /* 评价 */
        .eval-item { display:flex; align-items:center; gap:12px; padding:8px 14px; background:#f7faff; border-radius:10px; border:1px solid #e6edf6; flex-wrap:wrap; }
        .eval-item .e-label { font-weight:600; font-size:0.82rem; color:#1a1a3e; min-width:100px; }
        .eval-item .e-desc { font-size:0.75rem; color:#5a6e82; flex:1; min-width:80px; }
        .eval-item .e-score-input select { padding:3px 8px; border-radius:6px; border:1px solid #dce4ec; font-size:0.8rem; background:#fff; font-weight:600; width:70px; }

        /* 成绩 */
        .score-summary { display:grid; grid-template-columns:repeat(auto-fit,minmax(160px,1fr)); gap:14px; margin-bottom:16px; }
        .score-box { background:#f7faff; border-radius:12px; padding:14px 16px; text-align:center; border:1px solid #e6edf6; }
        .score-box .label { font-size:0.72rem; color:#5a6e82; }
        .score-box .value { font-size:1.8rem; font-weight:700; color:#1a1a3e; }
        .score-box .value.gold { color:#c99f4a; }
        .score-box .value.green { color:#2d7d5a; }
        .score-box .weight { font-size:0.65rem; color:#8a9eb0; }
        .score-detail table { width:100%; border-collapse:collapse; font-size:0.82rem; }
        .score-detail th { background:#f0f4f9; padding:6px 10px; text-align:left; font-weight:700; color:#1a1a3e; border-bottom:2px solid #dce4ec; }
        .score-detail td { padding:5px 10px; border-bottom:1px solid #e6edf6; }
        .score-detail tr:hover td { background:#f7faff; }

        .toast { position:fixed; bottom:24px; right:24px; background:#1a1a3e; color:#fff; padding:8px 20px; border-radius:12px; box-shadow:0 8px 24px rgba(0,0,0,0.2); font-weight:600; transform:translateY(100px); opacity:0; transition:all 0.4s ease; z-index:999; max-width:380px; font-size:0.8rem; }
        .toast.show { transform:translateY(0); opacity:1; }
        .toast.success { background:#2d7d5a; }
        .toast.error { background:#c0392b; }
        .toast.info { background:#2980b9; }
        .footer { text-align:center; padding:14px 0 4px; color:#8a9eb0; font-size:0.65rem; border-top:1px solid #e6edf6; margin-top:4px; }
        .footer i { color:#c99f4a; }
        .recognition-status { font-size:0.75rem; color:#5a6e82; padding:4px 10px; border-radius:20px; background:#f0f4f9; display:inline-block; margin-top:4px; }
        .recognition-status.active { background:#d6eaf8; color:#1a5276; }
        .recognition-status.error { background:#fadbd8; color:#922b21; }
        .recognition-status.success { background:#d4edda; color:#1a6e4a; }

        @media print {
            body { padding-top:0; background:#fff; }
            .navbar { display:none !important; }
            .page { display:block !important; animation:none !important; }
            .card { box-shadow:none !important; border:1px solid #ddd; break-inside:avoid; page-break-inside:avoid; }
            .btn { display:none !important; }
            .container { padding:10px; }
            .vocab-grid { grid-template-columns:repeat(2,1fr); }
            .dialogue-grid { grid-template-columns:repeat(2,1fr); }
            .role-grid { grid-template-columns:repeat(2,1fr); }
            .score-summary { grid-template-columns:repeat(4,1fr); }
            .no-print { display:none !important; }
            .dialogue-card .d-audio-bar .btn-recording-sm { display:none !important; }
            .dialogue-card .d-audio-bar .btn-audio-sm { display:none !important; }
            .case-card { grid-template-columns:1fr 1fr; }
        }
        @media (max-width:820px) {
            .navbar { padding:0 10px; height:56px; flex-wrap:nowrap; gap:4px; }
            .navbar .brand { font-size:0.7rem; }
            .navbar .brand span { display:none; }
            .navbar .nav-links a { font-size:0.55rem; padding:3px 8px; }
            body { padding-top:60px; }
            .container { padding:10px; }
            .card { padding:14px; }
            .vocab-grid { grid-template-columns:repeat(auto-fill,minmax(180px,1fr)); }
            .dialogue-grid { grid-template-columns:1fr; }
            .role-grid { grid-template-columns:1fr 1fr; }
            .form-row { grid-template-columns:1fr; }
            .score-summary { grid-template-columns:1fr 1fr; }
            .script-step { flex-direction:column; align-items:stretch; }
            .script-step .step-num { min-width:auto; }
        }
        @media (max-width:480px) {
            .navbar .nav-links a { font-size:0.5rem; padding:2px 6px; }
            .navbar .brand { font-size:0.6rem; }
            .navbar .right-actions .print-btn span { display:none; }
            .vocab-grid { grid-template-columns:1fr; }
            .role-grid { grid-template-columns:1fr; }
            .score-summary { grid-template-columns:1fr; }
            .card-title { font-size:0.9rem; }
            .eval-item { flex-direction:column; align-items:stretch; gap:4px; }
            .eval-item .e-label { min-width:auto; }
            .dialogue-grid { grid-template-columns:1fr; }
            .case-card { grid-template-columns:1fr; }
            .dialogue-card .d-line { flex-direction:column; gap:2px; }
            .dialogue-card .d-line .d-speaker { min-width:auto; }
        }
    </style>
</head>
<body>

    <!-- ===== 导航 ===== -->
    <nav class="navbar" id="navbar">
        <div class="brand">
            <i class="fas fa-plane"></i>
            航前准备会 <span>· HU7480实训</span>
        </div>
        <div class="nav-links">
            <a class="active" data-page="page-info"><i class="fas fa-info-circle"></i> 小组</a>
            <a data-page="page-case"><i class="fas fa-clipboard-list"></i> 案例信息</a>
            <a data-page="page-vocab"><i class="fas fa-book-open"></i> 词汇</a>
            <a data-page="page-phrases"><i class="fas fa-comment-dots"></i> 句型</a>
            <a data-page="page-dialogue"><i class="fas fa-comments"></i> 对话卡片</a>
            <a data-page="page-performance"><i class="fas fa-user-tag"></i> 模拟展演</a>
            <a data-page="page-eval"><i class="fas fa-chalkboard-teacher"></i> 师评成绩</a>
        </div>
        <div class="right-actions">
            <button class="print-btn" onclick="window.print()"><i class="fas fa-print"></i> <span>打印</span></button>
        </div>
    </nav>

    <!-- ===== 容器 ===== -->
    <div class="container">

        <!-- ===== 小组信息 ===== -->
        <div class="page active" id="page-info">
            <div class="card">
                <div class="card-title"><i class="fas fa-info-circle"></i> 小组基本信息</div>
                <div class="form-row">
                    <div class="form-group"><label><i class="fas fa-school"></i> 班级</label><input type="text" id="className" placeholder="请输入班级" /></div>
                    <div class="form-group"><label><i class="fas fa-tag"></i> 小组名称</label><input type="text" id="groupName" placeholder="如：第1组 / Sky Team" /></div>
                    <div class="form-group"><label><i class="fas fa-hashtag"></i> 小组编号</label><input type="text" id="groupId" placeholder="如：G01" /></div>
                    <div class="form-group"><label><i class="fas fa-tasks"></i> 实训任务</label><input type="text" id="taskName" value="航前准备会英语实训" /></div>
                    <div class="form-group"><label><i class="fas fa-user-tie"></i> 指导教师</label><input type="text" id="teacherName" placeholder="请输入姓名" /></div>
                </div>
                <div style="margin-top:10px;">
                    <button class="btn btn-success" id="saveInfoBtn"><i class="fas fa-save"></i> 保存信息</button>
                    <span class="text-muted" style="margin-left:10px;">数据自动保存在浏览器</span>
                </div>
            </div>
            <div class="card">
                <div class="card-title"><i class="fas fa-clipboard-list"></i> 任务说明</div>
                <p style="color:#4a5a6e;font-size:0.92rem;">
                    本实训系统基于 <strong>HU7480 三亚→北京 航前准备会</strong> 真实案例设计。
                    通过 <strong>词汇跟读评分</strong>、<strong>对话卡片学习</strong>、<strong>模拟展演对话编排</strong> 三个环节，
                    掌握 <strong>6大情境、28个核心句型</strong>，实现“会认、会说、会用”的学习目标。
                </p>
            </div>
        </div>

        <!-- ===== 案例信息 ===== -->
        <div class="page" id="page-case">
            <div class="card">
                <div class="card-title"><i class="fas fa-clipboard-list"></i> HU7480 航班信息卡 <span class="sub">案例详情</span></div>
                <p class="section-desc">以下为本次航前准备会实训所使用的完整航班信息，所有数据均基于真实案例。</p>
                <div class="case-card">
                    <div class="info-item"><div class="label">航班号 / Flight Number</div><div class="value en">HU7480</div><div class="value zh">海南航空</div></div>
                    <div class="info-item"><div class="label">机型 / Aircraft</div><div class="value en">Airbus A330-300</div><div class="value zh">空客 A330-300</div></div>
                    <div class="info-item"><div class="label">航程 / Route</div><div class="value en">SYX (T1) → PEK (T4)</div><div class="value zh">三亚凤凰机场 T1 → 北京首都机场 T4</div></div>
                    <div class="info-item"><div class="label">日期 / Date</div><div class="value en">January 20, 2025</div><div class="value zh">2025年1月20日</div></div>
                    <div class="info-item"><div class="label">飞行时间 / Duration</div><div class="value en">3 hours 45 minutes</div><div class="value zh">3小时45分钟</div></div>
                    <div class="info-item"><div class="label">离港时间 / Departure</div><div class="value en">22:10</div><div class="value zh">晚上10点10分</div></div>
                    <div class="info-item"><div class="label">到达时间 / Arrival</div><div class="value en">01:55 (next day)</div><div class="value zh">次日凌晨1点55分</div></div>
                    <div class="info-item"><div class="label">航路天气 / Weather</div><div class="value en">Sunny, 26°C</div><div class="value zh">晴朗，26°C</div></div>
                    <div class="info-item"><div class="label">旅客总数 / Total Passengers</div><div class="value en">226 (5 First / 221 Economy)</div><div class="value zh">共226人（头等5人，经济221人）</div></div>
                    <div class="info-item"><div class="label">特殊旅客 / Special Passengers</div><div class="value en">UMNR (12y, 23A) &amp; PREG (28w, 12C)</div><div class="value zh">无人陪伴儿童（12岁，23A）&amp; 孕妇（28周，12C）</div></div>
                    <div class="info-item"><div class="label">特殊餐食 / Special Meals</div><div class="value en">AVML (14A, 25F) &amp; MOML (7B)</div><div class="value zh">亚洲素食（14A,25F）&amp; 清真餐（7B）</div></div>
                    <div class="info-item"><div class="label">安全提示 / Safety</div><div class="value en">Moderate turbulence forecast ~2h after takeoff</div><div class="value zh">预计起飞约2小时后中度颠簸</div></div>
                </div>
                <div style="margin-top:14px;background:#f7faff;border-radius:10px;padding:10px 16px;border-left:4px solid #c99f4a;">
                    <strong style="color:#1a1a3e;">📌 案例要点：</strong>
                    <span style="color:#4a5a6e;font-size:0.9rem;">夜间航班，含特殊旅客（UMNR &amp; PREG）和特殊餐食（AVML &amp; MOML），航路有中度颠簸，需重点做好安全与服务预案。</span>
                </div>
            </div>
        </div>

        <!-- ===== 词汇 ===== -->
        <div class="page" id="page-vocab">
            <div class="card">
                <div class="card-title"><i class="fas fa-book-open"></i> 航前准备会核心词汇 <span class="sub">点击 <i class="fas fa-volume-up"></i> 听发音 · 点击 <i class="fas fa-microphone"></i> 跟读评分</span></div>
                <p class="section-desc">共20个航前准备会专属词汇（HU7480案例），点击喇叭听标准发音，点击麦克风跟读评分。</p>
                <div class="vocab-grid" id="vocabGrid"></div>
                <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap;align-items:center;">
                    <button class="btn btn-outline btn-sm" id="resetVocabScoresBtn"><i class="fas fa-redo-alt"></i> 重置所有评分</button>
                    <span class="text-muted" id="vocabProgress">已学 0/20 个词汇</span>
                </div>
            </div>
        </div>

        <!-- ===== 句型 ===== -->
        <div class="page" id="page-phrases">
            <div class="card">
                <div class="card-title"><i class="fas fa-comment-dots"></i> 航前准备会常用句型 <span class="sub">6大情境 · 28个核心句型</span></div>
                <p class="section-desc">按航前准备会流程顺序分类，点击 <i class="fas fa-volume-up text-gold"></i> 听标准发音。</p>
                <div id="phraseContainer"></div>
            </div>
        </div>

        <!-- ============================================================ -->
        <!-- 对话卡片（全新：完整对话展示） -->
        <!-- ============================================================ -->
        <div class="page" id="page-dialogue">
            <div class="card">
                <div class="card-title"><i class="fas fa-comments"></i> 航前准备会对话卡片 <span class="sub">6个情境 · 完整对话</span></div>
                <p class="section-desc">
                    每个卡片展示一个完整情境的多轮对话，点击 <i class="fas fa-play text-gold"></i> 听整段对话，
                    点击 <i class="fas fa-microphone text-gold"></i> 录制你的角色扮演。
                </p>
                <div class="dialogue-grid" id="dialogueGrid"></div>
                <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap;align-items:center;">
                    <button class="btn btn-outline btn-sm" id="clearDialogueRecordingsBtn"><i class="fas fa-trash-alt"></i> 清除所有录音</button>
                    <span class="text-muted" id="dialogueProgress">已录音 0/6 个对话</span>
                </div>
            </div>
        </div>

        <!-- ===== 模拟展演 ===== -->
        <div class="page" id="page-performance">
            <div class="card">
                <div class="card-title"><i class="fas fa-user-tag"></i> 1. 角色分工（6人一组）</div>
                <p class="section-desc">为每个岗位分配成员姓名（可多选，用逗号分隔）。</p>
                <div class="role-grid" id="roleGrid"></div>
                <div style="margin-top:12px;">
                    <button class="btn btn-success" id="saveRolesBtn"><i class="fas fa-save"></i> 保存角色分配</button>
                    <span class="text-muted" style="margin-left:10px;">数据自动保存</span>
                </div>
            </div>
            <div class="card">
                <div class="card-title"><i class="fas fa-pen-fancy"></i> 2. 对话文本编写</div>
                <p class="section-desc">按航前准备会6大情境顺序，为每个步骤选择角色和对应台词。</p>
                <div id="scriptEditor">
                    <div id="scriptStepsContainer"></div>
                    <div style="margin-top:8px;display:flex;gap:8px;flex-wrap:wrap;">
                        <button class="btn btn-primary btn-sm" id="addStepBtn"><i class="fas fa-plus"></i> 添加步骤</button>
                        <button class="btn btn-outline btn-sm" id="resetScriptBtn"><i class="fas fa-redo-alt"></i> 重置为默认流程</button>
                        <span class="text-muted" style="font-size:0.7rem;align-self:center;">共 <span id="stepCount">0</span> 个步骤</span>
                    </div>
                </div>
                <div style="margin-top:14px;">
                    <button class="btn btn-success" id="previewScriptBtn"><i class="fas fa-eye"></i> 预览对话</button>
                    <button class="btn btn-primary" id="downloadScriptBtn"><i class="fas fa-download"></i> 下载对话文本</button>
                    <span class="text-muted" style="margin-left:10px;font-size:0.7rem;">预览后即可下载 .txt 文件</span>
                </div>
                <div id="scriptPreviewContainer" style="margin-top:12px;display:none;">
                    <div class="card" style="background:#f7faff;border:1px solid #e6edf6;border-radius:10px;padding:12px 16px;">
                        <div class="card-title" style="font-size:0.95rem;margin-bottom:6px;"><i class="fas fa-file-alt text-gold"></i> 对话预览</div>
                        <div class="script-preview" id="scriptPreviewText"></div>
                    </div>
                </div>
            </div>
            <div class="card">
                <div class="card-title"><i class="fas fa-clipboard-check"></i> 3. 模拟展演评分（教师用）</div>
                <p class="section-desc">教师根据小组展演表现，从以下三个维度进行评分（各占100分）。</p>
                <div id="roleplayEvalContainer"></div>
                <div style="margin-top:10px;">
                    <button class="btn btn-success" id="saveRoleplayEvalBtn"><i class="fas fa-save"></i> 保存评分</button>
                    <span class="text-muted" style="margin-left:10px;">数据自动保存</span>
                </div>
            </div>
        </div>

        <!-- ===== 师评成绩 ===== -->
        <div class="page" id="page-eval">
            <div class="card">
                <div class="card-title"><i class="fas fa-chalkboard-teacher"></i> 教师综合评价</div>
                <p class="section-desc">教师根据词汇掌握度、对话理解与应答能力、模拟展演表现三方面综合评定。</p>
                <div id="teacherEvalContainer"></div>
                <div style="margin-top:10px;">
                    <button class="btn btn-success" id="saveTeacherEvalBtn"><i class="fas fa-save"></i> 保存师评</button>
                    <span class="text-muted" style="margin-left:10px;">数据自动保存</span>
                </div>
            </div>
            <div class="card">
                <div class="card-title"><i class="fas fa-chart-bar"></i> 成绩总览</div>
                <p class="text-muted" style="margin-bottom:10px;">最终成绩 = 词汇掌握 × 20% + 对话理解 × 30% + 模拟展演 × 50%</p>
                <div id="scoreSummary"></div>
                <div id="scoreDetail" class="score-detail"></div>
            </div>
        </div>

        <div class="footer">
            <i class="fas fa-plane"></i> 航前准备会英语 · HU7480实训系统 &nbsp;|&nbsp; 数据本地存储
            <br><span style="font-size:0.6rem;">“敬畏生命、敬畏规章、敬畏职责” —— 以专业态度，学好航前准备会英语</span>
        </div>
    </div>

    <div class="toast" id="toast"></div>

    <script>
        // ================================================================
        //  数据（基于HU7480案例，6人角色）
        // ================================================================

        const STORAGE_KEY = 'preflight_briefing_system_v4';

        // ===== 20个词汇（同前） =====
        const VOCAB_DATA = [
            { word: 'briefing', phonetic: '/ˈbriːfɪŋ/', meaning: 'n. 准备会' },
            { word: 'purser', phonetic: '/ˈpɜːsə/', meaning: 'n. 乘务长' },
            { word: 'aircraft', phonetic: '/ˈeəkrɑːft/', meaning: 'n. 飞机；机型' },
            { word: 'departure', phonetic: '/dɪˈpɑːtʃə/', meaning: 'n. 离港；起飞' },
            { word: 'ETA', phonetic: '/ˌiː tiː ˈeɪ/', meaning: 'n. 预计到达时间' },
            { word: 'duration', phonetic: '/djuˈreɪʃn/', meaning: 'n. 飞行时长' },
            { word: 'First Class', phonetic: '/fɜːst klɑːs/', meaning: 'n. 头等舱' },
            { word: 'Economy Class', phonetic: '/ɪˈkɒnəmi klɑːs/', meaning: 'n. 经济舱' },
            { word: 'en-route', phonetic: '/ˌɒn ˈruːt/', meaning: 'adj. 航路的' },
            { word: 'turbulence', phonetic: '/ˈtɜːbjələns/', meaning: 'n. 颠簸（不可数）' },
            { word: 'takeoff', phonetic: '/ˈteɪkɒf/', meaning: 'n. 起飞' },
            { word: 'UMNR', phonetic: '/ˌjuː em en ˈɑː/', meaning: '无人陪伴儿童' },
            { word: 'PREG', phonetic: '/priːɡ/', meaning: '孕妇旅客' },
            { word: 'special meals', phonetic: '/ˈspeʃl miːlz/', meaning: 'n. 特殊餐食' },
            { word: 'AVML', phonetic: '/ˌeɪ viː em ˈel/', meaning: '亚洲素食餐' },
            { word: 'MOML', phonetic: '/ˌem əʊ em ˈel/', meaning: '穆斯林/清真餐' },
            { word: 'galley', phonetic: '/ˈɡæli/', meaning: 'n. 机上厨房' },
            { word: 'loose items', phonetic: '/luːs ˈaɪtəmz/', meaning: 'n. 松散物品' },
            { word: 'jumpseat', phonetic: '/ˈdʒʌmp siːt/', meaning: 'n. 乘务员折叠座' },
            { word: 'emergency exits', phonetic: '/iˈmɜːdʒənsi ˈeksɪts/', meaning: 'n. 紧急出口' }
        ];

        // ===== 28个句型（同前） =====
        const PHRASE_DATA = [
            { en: 'Good evening, everyone.', zh: '大家晚上好。', tag: '开场' },
            { en: 'Please take your seats.', zh: '请就座。', tag: '开场' },
            { en: "Let's begin the pre-flight briefing for Flight HU7480.", zh: '我们开始HU7480航前准备会。', tag: '开场' },
            { en: "First, let me go over the basic flight information.", zh: '首先，我来过一遍基本航班信息。', tag: '开场' },
            { en: 'Our aircraft is an Airbus A330-300.', zh: '我们的机型是空客A330-300。', tag: '航班信息' },
            { en: 'Departure time is 22:10.', zh: '离港时间22:10。', tag: '航班信息' },
            { en: 'Our ETA for Beijing is 01:55 tomorrow.', zh: '预计到达北京时间明天01:55。', tag: '航班信息' },
            { en: 'The flight duration is 3 hours and 45 minutes.', zh: '飞行时长3小时45分钟。', tag: '航班信息' },
            { en: 'The en-route weather is sunny at 26°C.', zh: '航路天气晴朗，26°C。', tag: '航班信息' },
            { en: 'We have 226 passengers in total.', zh: '我们共有226名旅客。', tag: '旅客信息' },
            { en: 'There are 5 in First Class and 221 in Economy.', zh: '头等舱5人，经济舱221人。', tag: '旅客信息' },
            { en: 'We have two special passengers to take care of.', zh: '我们有两位特殊旅客需要照顾。', tag: '旅客信息' },
            { en: 'One is an UMNR, aged 12, seated in 23A.', zh: '一位是12岁无人陪伴儿童，座位23A。', tag: '旅客信息' },
            { en: 'The other is a PREG, at 28 weeks, seated in 12C.', zh: '另一位是孕28周孕妇，座位12C。', tag: '旅客信息' },
            { en: 'We have special meals: two AVML for seats 14A and 25F.', zh: '我们有特殊餐食：两份亚洲素食，座位14A和25F。', tag: '服务与餐食' },
            { en: 'We also have one MOML for seat 7B.', zh: '还有一份清真餐，座位7B。', tag: '服务与餐食' },
            { en: 'Please confirm the meal types before serving.', zh: '发放前请确认餐食类型。', tag: '服务与餐食' },
            { en: 'We will serve drinks first, followed by a light meal.', zh: '我们将先提供饮料，随后是轻餐。', tag: '服务与餐食' },
            { en: 'Moderate turbulence is forecast about two hours after takeoff.', zh: '预计起飞约两小时后有中度颠簸。', tag: '安全与应急' },
            { en: 'We must be prepared.', zh: '我们必须做好准备。', tag: '安全与应急' },
            { en: 'If we encounter turbulence, we will suspend hot beverage service.', zh: '如遇颠簸，我们将停止热饮服务。', tag: '安全与应急' },
            { en: 'We will secure all loose items in the galley.', zh: '我们将固定配餐区所有松散物品。', tag: '安全与应急' },
            { en: 'Please brief your jumpseat partners on the emergency exits.', zh: '请向你的折叠座伙伴说明紧急出口位置。', tag: '安全与应急' },
            { en: 'CA1, you will handle First Class.', zh: 'CA1，你负责头等舱。', tag: '任务分配' },
            { en: 'CA2 and CA3 will cover the Economy cabin.', zh: 'CA2和CA3负责经济舱。', tag: '任务分配' },
            { en: 'CA4, please assist with the special passengers.', zh: 'CA4，请协助特殊旅客。', tag: '任务分配' },
            { en: "Let's double-check our safety equipment.", zh: '让我们再次检查安全设备。', tag: '任务分配' },
            { en: "Let's have a safe and pleasant flight!", zh: '祝飞行平安愉快！', tag: '任务分配' }
        ];

        // ===== 6个完整对话（多轮对话） =====
        const DIALOGUE_DATA = [{
            id: 1,
            title: '乘务长开场',
            scene: '开场',
            lines: [
                { speaker: 'Purser', text: 'Good evening, everyone. Please take your seats.', trans: '大家晚上好。请就座。' },
                { speaker: 'All', text: 'Good evening.', trans: '晚上好。' },
                { speaker: 'Purser',
                    text: "Let's begin the pre-flight briefing for Flight HU7480 from Sanya to Beijing.",
                    trans: '我们开始航班HU7480三亚飞往北京的航前准备会。' },
                { speaker: 'CA1', text: 'Ready.', trans: '准备好了。' },
                { speaker: 'Purser', text: "First, let me go over the basic flight information.",
                    trans: '首先，我来过一遍基本航班信息。' }
            ]
        }, {
            id: 2,
            title: '航班信息汇报',
            scene: '航班信息',
            lines: [
                { speaker: 'Purser', text: 'Our aircraft is an Airbus A330-300. Departure time is 22:10.',
                    trans: '我们的机型是空客A330-300。离港时间22:10。' },
                { speaker: 'CA2', text: 'What about the arrival time?', trans: '到达时间呢？' },
                { speaker: 'Purser', text: 'Our ETA for Beijing is 01:55 tomorrow. The flight duration is 3 hours and 45 minutes.',
                    trans: '预计到达北京时间明天01:55。飞行时长3小时45分钟。' },
                { speaker: 'CA3', text: 'And the weather?', trans: '天气情况呢？' },
                { speaker: 'Purser', text: 'The en-route weather is sunny at 26°C.',
                    trans: '航路天气晴朗，26°C。' }
            ]
        }, {
            id: 3,
            title: '旅客信息确认',
            scene: '旅客信息',
            lines: [
                { speaker: 'CA1', text: 'How many passengers do we have?', trans: '我们有多少旅客？' },
                { speaker: 'Purser', text: 'We have 226 passengers in total — 5 in First Class and 221 in Economy.',
                    trans: '我们共有226名旅客——头等舱5人，经济舱221人。' },
                { speaker: 'CA2', text: 'Do we have any special passengers?', trans: '有特殊旅客吗？' },
                { speaker: 'Purser',
                    text: 'Yes. We have two special passengers to take care of. One is an UMNR, aged 12, seated in 23A. The other is a PREG, at 28 weeks, seated in 12C.',
                    trans: '有的。我们有两位特殊旅客需要照顾。一位是12岁无人陪伴儿童，座位23A。另一位是孕28周孕妇，座位12C。' },
                { speaker: 'CA3', text: "I'll take care of the UMNR.", trans: '我来照顾这位无人陪伴儿童。' }
            ]
        }, {
            id: 4,
            title: '特殊餐食安排',
            scene: '服务与餐食',
            lines: [
                { speaker: 'CA2', text: 'Are there any special meals on board?', trans: '机上有特殊餐食吗？' },
                { speaker: 'Purser',
                    text: 'Yes. We have special meals: two AVML for seats 14A and 25F, and one MOML for seat 7B.',
                    trans: '有的。我们有特殊餐食：两份亚洲素食，座位14A和25F；一份清真餐，座位7B。' },
                { speaker: 'CA1', text: 'What is the service sequence?', trans: '服务流程是什么？' },
                { speaker: 'Purser',
                    text: 'Since it\'s a night flight, we will serve drinks first, followed by a light meal. Please confirm the meal types before serving.',
                    trans: '因为是夜间航班，我们先提供饮料，随后是轻餐。发放前请确认餐食类型。' }
            ]
        }, {
            id: 5,
            title: '安全预案',
            scene: '安全与应急',
            lines: [
                { speaker: 'CA3', text: 'What about the weather and safety procedures?',
                    trans: '天气和安全程序如何？' },
                { speaker: 'Purser',
                    text: 'The en-route weather is sunny, but moderate turbulence is forecast about two hours after takeoff. We must be prepared.',
                    trans: '航路天气晴朗，但预计起飞约两小时后有中度颠簸。我们必须做好准备。' },
                { speaker: 'CA1', text: 'What should we do if we encounter turbulence?',
                    trans: '如遇颠簸我们该怎么办？' },
                { speaker: 'Purser',
                    text: 'If we encounter turbulence, we will suspend hot beverage service immediately and secure all loose items in the galley.',
                    trans: '如遇颠簸，我们将立即停止热饮服务，并固定配餐区所有松散物品。' },
                { speaker: 'CA4',
                    text: 'Please brief your jumpseat partners on the emergency exit locations and commands.',
                    trans: '请向你的折叠座伙伴说明紧急出口位置和指令。' }
            ]
        }, {
            id: 6,
            title: '任务分配与结束',
            scene: '任务分配',
            lines: [
                { speaker: 'Purser', text: 'CA1, you will handle First Class. CA2 and CA3, you will cover the Economy cabin.',
                    trans: 'CA1，你负责头等舱。CA2和CA3，你们负责经济舱。' },
                { speaker: 'CA4', text: 'What about me?', trans: '那我呢？' },
                { speaker: 'Purser', text: 'CA4, please assist with the special passengers.',
                    trans: 'CA4，请协助特殊旅客。' },
                { speaker: 'All', text: 'Understood.', trans: '明白。' },
                { speaker: 'Purser',
                    text: "Any questions? ... Alright. Let's double-check our safety equipment and prepare for boarding. Let's have a safe and pleasant flight!",
                    trans: '有问题吗？……好的。让我们再次检查安全设备，准备登机。祝飞行平安愉快！' },
                { speaker: 'All', text: 'Safe flight!', trans: '飞行平安！' }
            ]
        }];

        // ===== 角色：6人 =====
        const ROLE_DATA = [
            { id: 'r1', title: '乘务长 (Purser)', icon: 'fa-user-tie' },
            { id: 'r2', title: '乘务员1 (CA1)', icon: 'fa-user' },
            { id: 'r3', title: '乘务员2 (CA2)', icon: 'fa-user' },
            { id: 'r4', title: '乘务员3 (CA3)', icon: 'fa-user' },
            { id: 'r5', title: '乘务员4 (CA4)', icon: 'fa-user' },
            { id: 'r6', title: '安全员 (Safety)', icon: 'fa-shield-alt' }
        ];

        // ===== 师评维度 =====
        const TEACHER_EVAL_ITEMS = [
            { id: 't1', label: '词汇掌握度', desc: '20个核心词汇的认读与发音准确度', weight: 20 },
            { id: 't2', label: '对话理解与应答', desc: '6个对话卡片的理解与跟读熟练度', weight: 30 },
            { id: 't3', label: '模拟展演表现', desc: '角色投入度、语言流畅度、服务礼仪', weight: 50 }
        ];

        const ROLEPLAY_DIMENSIONS = [
            { id: 'rp1', label: '语言流畅度', desc: '英语表达自然、连贯，无明显卡顿' },
            { id: 'rp2', label: '角色投入度', desc: '情感投入、服务态度亲切、有职业感' },
            { id: 'rp3', label: '服务礼仪', desc: '站姿、手势、微笑、眼神交流规范' }
        ];

        // ================================================================
        //  数据管理
        // ================================================================
        function getDefaultData() {
            return {
                groupInfo: { className: '', groupName: '', groupId: '', taskName: '航前准备会英语实训', teacher: '' },
                vocabScores: {},
                roles: ROLE_DATA.map(r => ({ ...r, member: '' })),
                scriptSteps: [
                    { roleId: 'r1', phraseIdx: 2, customText: '' },
                    { roleId: 'r1', phraseIdx: 3, customText: '' },
                    { roleId: 'r2', phraseIdx: 10, customText: '' },
                    { roleId: 'r3', phraseIdx: 12, customText: '' },
                    { roleId: 'r4', phraseIdx: 14, customText: '' },
                    { roleId: 'r5', phraseIdx: 18, customText: '' },
                    { roleId: 'r6', phraseIdx: 20, customText: '' },
                    { roleId: 'r1', phraseIdx: 27, customText: '' }
                ],
                dialogueRecordings: {},
                roleplayEval: {},
                teacherEval: {},
                teacherComment: '',
                updatedAt: ''
            };
        }

        function loadData() {
            try {
                const raw = localStorage.getItem(STORAGE_KEY);
                if (raw) {
                    const parsed = JSON.parse(raw);
                    if (!parsed.groupInfo) parsed.groupInfo = getDefaultData().groupInfo;
                    if (!parsed.vocabScores) parsed.vocabScores = {};
                    if (!parsed.roles || parsed.roles.length !== 6) {
                        parsed.roles = ROLE_DATA.map(r => ({ ...r, member: '' }));
                    } else {
                        parsed.roles = parsed.roles.map((r, idx) => ({ ...ROLE_DATA[idx], member: r.member || '' }));
                    }
                    if (!parsed.scriptSteps || !Array.isArray(parsed.scriptSteps) || parsed.scriptSteps.length === 0) {
                        parsed.scriptSteps = getDefaultData().scriptSteps;
                    }
                    if (!parsed.dialogueRecordings) parsed.dialogueRecordings = {};
                    if (!parsed.roleplayEval) parsed.roleplayEval = {};
                    if (!parsed.teacherEval) parsed.teacherEval = {};
                    if (parsed.teacherComment === undefined) parsed.teacherComment = '';
                    return parsed;
                }
            } catch (e) { console.warn('加载数据失败', e); }
            return getDefaultData();
        }

        function saveData(data) {
            data.updatedAt = new Date().toLocaleString();
            localStorage.setItem(STORAGE_KEY, JSON.stringify(data));
            return data;
        }

        let appData = loadData();

        // ================================================================
        //  工具函数
        // ================================================================
        function showToast(msg, type = 'success') {
            const el = document.getElementById('toast');
            el.textContent = msg;
            el.className = 'toast ' + type + ' show';
            clearTimeout(el._timer);
            el._timer = setTimeout(() => el.classList.remove('show'), 2800);
        }

        function speakText(text, lang = 'en-US', rate = 0.8, callback) {
            if (!window.speechSynthesis) {
                showToast('浏览器不支持语音合成', 'error');
                return;
            }
            window.speechSynthesis.cancel();
            const utterance = new SpeechSynthesisUtterance(text);
            utterance.lang = lang;
            utterance.rate = rate;
            utterance.pitch = 1.0;
            utterance.volume = 1;
            utterance.onend = () => {
                document.querySelectorAll('.speaking, .playing').forEach(el => el.classList.remove('speaking', 'playing'));
                if (callback) callback();
            };
            utterance.onerror = () => {
                document.querySelectorAll('.speaking, .playing').forEach(el => el.classList.remove('speaking', 'playing'));
                if (callback) callback();
            };
            window.speechSynthesis.speak(utterance);
        }

        // ================================================================
        //  导航切换
        // ================================================================
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                const pageId = this.dataset.page;
                document.querySelectorAll('.nav-links a').forEach(l => l.classList.remove('active'));
                this.classList.add('active');
                document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
                document.getElementById(pageId).classList.add('active');
                if (pageId === 'page-info') loadInfoToForm();
                if (pageId === 'page-vocab') renderVocab();
                if (pageId === 'page-phrases') renderPhrases();
                if (pageId === 'page-dialogue') renderDialogues();
                if (pageId === 'page-performance') { renderRoles();
                    renderScriptEditor();
                    renderRoleplayEval(); }
                if (pageId === 'page-eval') { renderTeacherEval();
                    renderScore(); }
            });
        });

        // ================================================================
        //  小组信息
        // ================================================================
        function loadInfoToForm() {
            const info = appData.groupInfo;
            document.getElementById('className').value = info.className || '';
            document.getElementById('groupName').value = info.groupName || '';
            document.getElementById('groupId').value = info.groupId || '';
            document.getElementById('taskName').value = info.taskName || '航前准备会英语实训';
            document.getElementById('teacherName').value = info.teacher || '';
        }
        document.getElementById('saveInfoBtn').addEventListener('click', function() {
            appData.groupInfo.className = document.getElementById('className').value.trim();
            appData.groupInfo.groupName = document.getElementById('groupName').value.trim();
            appData.groupInfo.groupId = document.getElementById('groupId').value.trim();
            appData.groupInfo.taskName = document.getElementById('taskName').value.trim();
            appData.groupInfo.teacher = document.getElementById('teacherName').value.trim();
            saveData(appData);
            showToast('小组信息已保存');
        });

        // ================================================================
        //  词汇（同前，保留）
        // ================================================================
        let recognition = null;

        function initSpeechRecognition() {
            if (!('webkitSpeechRecognition' in window) && !('SpeechRecognition' in window)) return null;
            const SR = window.SpeechRecognition || window.webkitSpeechRecognition;
            const rec = new SR();
            rec.lang = 'en-US';
            rec.continuous = false;
            rec.interimResults = false;
            rec.maxAlternatives = 1;
            return rec;
        }

        function calculateScore(recognized, target) {
            recognized = recognized.toLowerCase().trim();
            target = target.toLowerCase().trim();
            if (!recognized || !target) return 0;
            if (recognized === target) return 100;
            if (recognized.includes(target)) return 92;
            if (target.includes(recognized)) return 88;
            const recWords = recognized.split(/\s+/);
            const tarWords = target.split(/\s+/);
            let matchCount = 0;
            tarWords.forEach(tw => { if (recWords.some(rw => rw === tw)) matchCount++; });
            if (tarWords.length > 0) {
                const ratio = matchCount / tarWords.length;
                if (ratio >= 0.8) return 85;
                if (ratio >= 0.6) return 70;
                if (ratio >= 0.4) return 55;
            }
            const dist = levenshteinDistance(recognized, target);
            const maxLen = Math.max(recognized.length, target.length);
            if (maxLen === 0) return 0;
            return Math.round((1 - dist / maxLen) * 60);
        }

        function levenshteinDistance(a, b) {
            const matrix = [];
            for (let i = 0; i <= b.length; i++) matrix[i] = [i];
            for (let j = 0; j <= a.length; j++) matrix[0][j] = j;
            for (let i = 1; i <= b.length; i++) {
                for (let j = 1; j <= a.length; j++) {
                    if (b[i - 1] === a[j - 1]) { matrix[i][j] = matrix[i - 1][j - 1]; } else {
                        matrix[i][j] = Math.min(matrix[i - 1][j - 1] + 1, matrix[i][j - 1] + 1, matrix[i - 1][j] + 1);
                    }
                }
            }
            return matrix[b.length][a.length];
        }

        function getScoreClass(score) {
            if (score >= 80) return 'score-excellent';
            if (score >= 60) return 'score-good';
            if (score >= 40) return 'score-fair';
            if (score > 0) return 'score-poor';
            return 'score-none';
        }

        function getScoreLabel(score) {
            if (score >= 80) return '🌟 优秀';
            if (score >= 60) return '👍 良好';
            if (score >= 40) return '📖 一般';
            if (score > 0) return '💪 需练习';
            return '⏳ 待跟读';
        }

        function renderVocab() {
            const grid = document.getElementById('vocabGrid');
            grid.innerHTML = '';
            let learnedCount = 0;
            VOCAB_DATA.forEach((item, idx) => {
                const scoreData = appData.vocabScores[item.word] || { score: 0, attempts: 0 };
                if (scoreData.score > 0) learnedCount++;
                const div = document.createElement('div');
                div.className = 'vocab-card';
                div.innerHTML = `
                    <div><span class="word">${item.word}</span><span class="phonetic">${item.phonetic}</span></div>
                    <div class="meaning">${item.meaning}</div>
                    <div class="actions">
                        <button class="speak-btn" data-word="${item.word}"><i class="fas fa-volume-up"></i></button>
                        <button class="record-btn" data-word="${item.word}" data-idx="${idx}"><i class="fas fa-microphone"></i></button>
                        <span class="recognition-status" id="status-${idx}">点击🎤开始跟读</span>
                    </div>
                    <div class="score-display">
                        评分：<span class="score-value ${getScoreClass(scoreData.score)}" id="score-${idx}">${scoreData.score > 0 ? scoreData.score : '—'}</span>
                        <span style="font-size:0.7rem;color:#8a9eb0;">${getScoreLabel(scoreData.score)}</span>
                        ${scoreData.attempts > 0 ? `<span style="font-size:0.65rem;color:#8a9eb0;margin-left:auto;">尝试 ${scoreData.attempts} 次</span>` : ''}
                    </div>
                `;
                grid.appendChild(div);
                div.querySelector('.speak-btn').addEventListener('click', function(e) {
                    e.stopPropagation();
                    const word = this.dataset.word;
                    document.querySelectorAll('.speak-btn.speaking').forEach(b => b.classList.remove('speaking'));
                    this.classList.add('speaking');
                    speakText(word, 'en-US', 0.7, () => { this.classList.remove('speaking'); });
                    showToast(`🔊 正在发音：${word}`, 'info');
                });
                const recordBtn = div.querySelector('.record-btn');
                const statusEl = document.getElementById(`status-${idx}`);
                const scoreEl = document.getElementById(`score-${idx}`);
                recordBtn.addEventListener('click', function(e) {
                    e.stopPropagation();
                    const word = this.dataset.word;
                    const idx2 = parseInt(this.dataset.idx);
                    if (this.classList.contains('recording')) {
                        if (recognition) { try { recognition.stop(); } catch (e) {} }
                        this.classList.remove('recording');
                        statusEl.textContent = '⏹ 已停止';
                        return;
                    }
                    if (!('webkitSpeechRecognition' in window) && !('SpeechRecognition' in window)) {
                        showToast('当前浏览器不支持语音识别，请使用Chrome浏览器', 'error');
                        return;
                    }
                    if (!recognition) {
                        recognition = initSpeechRecognition();
                        if (!recognition) { showToast('无法初始化语音识别', 'error'); return; }
                    }
                    recognition.lang = 'en-US';
                    recognition.continuous = false;
                    recognition.interimResults = false;
                    recognition.onstart = function() {
                        recordBtn.classList.add('recording');
                        statusEl.textContent = '🎤 正在听...请朗读单词';
                        statusEl.className = 'recognition-status active';
                        showToast('🎤 请朗读：' + word, 'info');
                    };
                    recognition.onresult = function(event) {
                        const result = event.results[0];
                        const transcript = result[0].transcript.toLowerCase().trim();
                        const confidence = result[0].confidence || 0;
                        const score = calculateScore(transcript, word);
                        const finalScore = Math.min(100, Math.round(score * 0.85 + confidence * 15));
                        if (!appData.vocabScores[word]) appData.vocabScores[word] = { score: 0, attempts: 0 };
                        appData.vocabScores[word].score = Math.max(appData.vocabScores[word].score, finalScore);
                        appData.vocabScores[word].attempts += 1;
                        saveData(appData);
                        statusEl.textContent = `✅ 识别: "${transcript}"  评分: ${finalScore}分`;
                        statusEl.className = 'recognition-status success';
                        scoreEl.textContent = finalScore;
                        scoreEl.className = `score-value ${getScoreClass(finalScore)}`;
                        recordBtn.classList.remove('recording');
                        updateVocabProgress();
                        showToast(`📊 评分 ${finalScore}分 — ${getScoreLabel(finalScore)}`, finalScore >= 60 ? 'success' :
                            'info');
                    };
                    recognition.onerror = function(event) {
                        recordBtn.classList.remove('recording');
                        if (event.error === 'not-allowed') {
                            statusEl.textContent = '❌ 请允许麦克风权限';
                            statusEl.className = 'recognition-status error';
                            showToast('请允许浏览器使用麦克风权限', 'error');
                        } else if (event.error === 'no-speech') {
                            statusEl.textContent = '⏳ 未检测到语音，请重试';
                            statusEl.className = 'recognition-status error';
                            showToast('未检测到语音，请大声朗读', 'error');
                        } else {
                            statusEl.textContent = `❌ 错误: ${event.error}`;
                            statusEl.className = 'recognition-status error';
                            showToast('语音识别错误，请重试', 'error');
                        }
                    };
                    recognition.onend = function() {
                        recordBtn.classList.remove('recording');
                        if (statusEl.textContent.includes('正在听')) {
                            statusEl.textContent = '⏳ 未检测到语音，请重试';
                            statusEl.className = 'recognition-status error';
                        }
                    };
                    try { recognition.start(); } catch (e) {
                        showToast('语音识别启动失败，请重试', 'error');
                        recordBtn.classList.remove('recording');
                    }
                });
            });
            updateVocabProgress();
        }

        function updateVocabProgress() {
            let learned = 0;
            VOCAB_DATA.forEach(item => {
                const data = appData.vocabScores[item.word];
                if (data && data.score > 0) learned++;
            });
            document.getElementById('vocabProgress').textContent = `已学 ${learned}/${VOCAB_DATA.length} 个词汇`;
        }

        document.getElementById('resetVocabScoresBtn').addEventListener('click', function() {
            if (!confirm('重置所有词汇评分数据，确定吗？')) return;
            appData.vocabScores = {};
            saveData(appData);
            renderVocab();
            showToast('所有评分已重置');
        });

        // ================================================================
        //  句型
        // ================================================================
        function renderPhrases() {
            const container = document.getElementById('phraseContainer');
            container.innerHTML = '';
            const categoryMap = {
                '开场': '🎤 情境一：会议开场 (Opening)',
                '航班信息': '✈️ 情境二：航班信息 (Flight Information)',
                '旅客信息': '👤 情境三：旅客信息 (Passenger Information)',
                '服务与餐食': '🍽️ 情境四：服务与餐食 (Service & Meals)',
                '安全与应急': '🛡️ 情境五：安全与应急 (Safety & Emergency)',
                '任务分配': '📋 情境六：任务分配与结束 (Assignment & Closing)'
            };
            const groups = {};
            PHRASE_DATA.forEach(p => {
                if (!groups[p.tag]) groups[p.tag] = [];
                groups[p.tag].push(p);
            });
            const order = ['开场', '航班信息', '旅客信息', '服务与餐食', '安全与应急', '任务分配'];
            order.forEach(tag => {
                if (!groups[tag]) return;
                const items = groups[tag];
                const section = document.createElement('div');
                section.className = 'phrase-section';
                section.innerHTML = `
                    <div class="phrase-section-title">
                        <span>${categoryMap[tag] || tag}</span>
                        <span class="badge">${items.length} 句</span>
                    </div>
                    <div class="phrase-list">
                        ${items.map(item => `
                            <div class="phrase-item">
                                <span class="en">${item.en} <span class="speak-icon-sm" data-text="${item.en}"><i class="fas fa-volume-up"></i></span></span>
                                <span class="zh">${item.zh}</span>
                            </div>
                        `).join('')}
                    </div>
                `;
                container.appendChild(section);
                section.querySelectorAll('.speak-icon-sm').forEach(el => {
                    el.addEventListener('click', function(e) {
                        e.stopPropagation();
                        speakText(this.dataset.text, 'en-US', 0.75);
                        showToast(`🔊 ${this.dataset.text}`, 'info');
                    });
                });
            });
        }

        // ================================================================
        //  对话卡片（核心新增）
        // ================================================================
        function renderDialogues() {
            const grid = document.getElementById('dialogueGrid');
            grid.innerHTML = '';
            let recordedCount = 0;

            DIALOGUE_DATA.forEach(dial => {
                const rec = appData.dialogueRecordings[dial.id] || null;
                if (rec && rec.audioData) recordedCount++;

                const card = document.createElement('div');
                card.className = 'dialogue-card';

                // 构建完整对话HTML
                let linesHtml = '';
                dial.lines.forEach((line, idx) => {
                    const cls = (line.speaker === 'Purser' || line.speaker === 'All') ? 'purser' :
                    'crew';
                    const speakerLabel = line.speaker === 'All' ? '👥 全体' :
                        line.speaker === 'Purser' ? '👩‍✈️ 乘务长' :
                        `🧑‍✈️ ${line.speaker}`;
                    linesHtml += `
                        <div class="d-line ${cls}">
                            <span class="d-speaker">${speakerLabel}</span>
                            <div>
                                <div class="d-text">${line.text}</div>
                                <div class="d-trans">${line.trans}</div>
                            </div>
                        </div>
                    `;
                });

                // 合并所有台词为一段文本（用于整段播放）
                const fullText = dial.lines.map(l => l.text).join(' ');

                card.innerHTML = `
                    <div class="d-header">
                        <span class="d-num">情境 ${dial.id}</span>
                        <span class="d-title">${dial.title}</span>
                        <span class="d-scene-label">${dial.scene}</span>
                    </div>
                    <div class="d-body">${linesHtml}</div>
                    <div class="d-audio-bar">
                        <button class="btn-audio-sm play-full" data-text="${fullText}" title="播放整段对话"><i class="fas fa-play"></i> 整段播放</button>
                        <button class="btn-recording-sm start-rec" data-id="${dial.id}" title="开始录音"><i class="fas fa-circle" style="color:#c0392b;"></i> 录音</button>
                        <button class="btn-recording-sm stop-rec" data-id="${dial.id}" style="display:none;" title="停止录音"><i class="fas fa-stop"></i> 停止</button>
                        <button class="btn-recording-sm play-rec" data-id="${dial.id}" title="播放录音" ${!rec ? 'disabled' : ''}><i class="fas fa-play"></i> 播放</button>
                        <button class="btn-recording-sm delete-rec" data-id="${dial.id}" title="删除录音" ${!rec ? 'disabled' : ''}><i class="fas fa-trash-alt"></i> 删除</button>
                        <span class="d-status" id="dial-status-${dial.id}">${rec ? '✅ 已录音 ' + (rec.duration || 0) + 's' : '⏳ 未录音'}</span>
                        <span class="d-status" id="dial-time-${dial.id}" style="font-size:0.65rem;color:#8a9eb0;"></span>
                    </div>
                `;
                grid.appendChild(card);

                // ---- 事件绑定 ----
                // 播放整段
                card.querySelector('.play-full').addEventListener('click', function(e) {
                    e.stopPropagation();
                    const text = this.dataset.text;
                    this.classList.add('playing');
                    speakText(text, 'en-US', 0.75, () => { this.classList.remove('playing'); });
                    showToast(`🔊 播放完整对话：${dial.title}`, 'info');
                });

                // ---- 录音 ----
                const startBtn = card.querySelector('.start-rec');
                const stopBtn = card.querySelector('.stop-rec');
                const playBtn = card.querySelector('.play-rec');
                const deleteBtn = card.querySelector('.delete-rec');
                const statusEl = document.getElementById(`dial-status-${dial.id}`);
                const timeEl = document.getElementById(`dial-time-${dial.id}`);

                let mediaRecorder = null;
                let audioChunks = [];
                let recordingStartTime = 0;
                let timerInterval = null;

                startBtn.addEventListener('click', async function(e) {
                    e.stopPropagation();
                    if (appData.dialogueRecordings[dial.id] && appData.dialogueRecordings[dial.id]
                        .audioData) {
                        if (!confirm('已有录音，重新录音将覆盖之前的内容。确定继续吗？')) return;
                    }
                    try {
                        const stream = await navigator.mediaDevices.getUserMedia({ audio: true });
                        mediaRecorder = new MediaRecorder(stream, { mimeType: 'audio/webm' });
                        audioChunks = [];
                        mediaRecorder.ondataavailable = (event) => {
                            if (event.data.size > 0) audioChunks.push(event.data);
                        };
                        mediaRecorder.onstop = () => {
                            const blob = new Blob(audioChunks, { type: 'audio/webm' });
                            const reader = new FileReader();
                            reader.onload = () => {
                                const base64 = reader.result.split(',')[1];
                                const duration = Math.round((Date.now() - recordingStartTime) / 1000);
                                appData.dialogueRecordings[dial.id] = {
                                    audioData: base64,
                                    duration: duration,
                                    timestamp: new Date().toISOString()
                                };
                                saveData(appData);
                                statusEl.textContent = `✅ 已录音 ${duration}s`;
                                statusEl.className = 'd-status done';
                                playBtn.disabled = false;
                                deleteBtn.disabled = false;
                                updateDialogueProgress();
                                showToast(`✅ 对话 ${dial.id} 录音完成 (${duration}s)`, 'success');
                            };
                            reader.readAsDataURL(blob);
                            stream.getTracks().forEach(track => track.stop());
                            startBtn.style.display = 'inline-flex';
                            stopBtn.style.display = 'none';
                            startBtn.classList.remove('recording');
                            if (timerInterval) { clearInterval(timerInterval);
                                timerInterval = null; }
                            timeEl.textContent = '';
                        };
                        mediaRecorder.start();
                        recordingStartTime = Date.now();
                        startBtn.style.display = 'none';
                        stopBtn.style.display = 'inline-flex';
                        startBtn.classList.add('recording');
                        let seconds = 0;
                        timeEl.textContent = '00:00';
                        if (timerInterval) clearInterval(timerInterval);
                        timerInterval = setInterval(() => {
                            seconds++;
                            const mins = String(Math.floor(seconds / 60)).padStart(2, '0');
                            const secs = String(seconds % 60).padStart(2, '0');
                            timeEl.textContent = `${mins}:${secs}`;
                        }, 1000);
                        showToast('🎤 录音中... 点击停止完成录音', 'info');
                    } catch (err) {
                        showToast('无法访问麦克风，请检查权限设置', 'error');
                        console.error(err);
                    }
                });

                stopBtn.addEventListener('click', function(e) {
                    e.stopPropagation();
                    if (mediaRecorder && mediaRecorder.state === 'recording') {
                        mediaRecorder.stop();
                    }
                    if (timerInterval) { clearInterval(timerInterval);
                        timerInterval = null; }
                });

                playBtn.addEventListener('click', function(e) {
                    e.stopPropagation();
                    const data = appData.dialogueRecordings[dial.id];
                    if (!data || !data.audioData) {
                        showToast('没有录音可播放', 'error');
                        return;
                    }
                    try {
                        const audio = new Audio(`data:audio/webm;base64,${data.audioData}`);
                        this.classList.add('playing');
                        audio.play();
                        audio.onended = () => { this.classList.remove('playing'); };
                        audio.onerror = () => { this.classList.remove('playing');
                            showToast('播放失败', 'error'); };
                        showToast(`▶️ 播放录音 (${data.duration || 0}s)`, 'info');
                    } catch (err) {
                        showToast('播放失败', 'error');
                        console.error(err);
                    }
                });

                deleteBtn.addEventListener('click', function(e) {
                    e.stopPropagation();
                    if (!confirm('确定删除此对话的录音吗？')) return;
                    delete appData.dialogueRecordings[dial.id];
                    saveData(appData);
                    statusEl.textContent = '⏳ 未录音';
                    statusEl.className = 'd-status';
                    playBtn.disabled = true;
                    deleteBtn.disabled = true;
                    updateDialogueProgress();
                    showToast('录音已删除');
                });

                if (rec) {
                    statusEl.textContent = `✅ 已录音 ${rec.duration || 0}s`;
                    statusEl.className = 'd-status done';
                }
            });
            updateDialogueProgress();
        }

        function updateDialogueProgress() {
            let count = 0;
            DIALOGUE_DATA.forEach(d => {
                if (appData.dialogueRecordings[d.id] && appData.dialogueRecordings[d.id].audioData) count++;
            });
            document.getElementById('dialogueProgress').textContent = `已录音 ${count}/${DIALOGUE_DATA.length} 个对话`;
        }

        document.getElementById('clearDialogueRecordingsBtn').addEventListener('click', function() {
            if (!confirm('确定清除所有对话的录音数据吗？此操作不可撤销！')) return;
            appData.dialogueRecordings = {};
            saveData(appData);
            renderDialogues();
            showToast('所有录音已清除');
        });

        // ================================================================
        //  角色分工
        // ================================================================
        function renderRoles() {
            const grid = document.getElementById('roleGrid');
            grid.innerHTML = '';
            appData.roles.forEach((role, idx) => {
                const div = document.createElement('div');
                div.className = 'role-card';
                div.innerHTML = `
                    <div class="r-title"><span class="icon"><i class="fas ${role.icon}"></i></span> ${role.title}</div>
                    <div class="r-name"><input type="text" class="role-member-input" data-idx="${idx}" value="${role.member}" placeholder="姓名1, 姓名2..." /></div>
                `;
                grid.appendChild(div);
                div.querySelector('.role-member-input').addEventListener('change', function() {
                    const idx2 = parseInt(this.dataset.idx);
                    appData.roles[idx2].member = this.value.trim();
                    saveData(appData);
                    renderScriptEditor();
                });
            });
        }

        document.getElementById('saveRolesBtn').addEventListener('click', function() {
            document.querySelectorAll('.role-member-input').forEach(inp => {
                const idx = parseInt(inp.dataset.idx);
                appData.roles[idx].member = inp.value.trim();
            });
            saveData(appData);
            renderScriptEditor();
            showToast('角色分配已保存');
        });

        // ================================================================
        //  对话编排
        // ================================================================
        function renderScriptEditor() {
            const container = document.getElementById('scriptStepsContainer');
            const steps = appData.scriptSteps || [];
            container.innerHTML = '';
            steps.forEach((step, idx) => {
                const div = document.createElement('div');
                div.className = 'script-step';
                const roleSelect = document.createElement('select');
                roleSelect.className = 'role-select';
                roleSelect.dataset.idx = idx;
                appData.roles.forEach(r => {
                    const label = r.member ? `${r.title} (${r.member})` : r.title;
                    const opt = document.createElement('option');
                    opt.value = r.id;
                    opt.textContent = label;
                    if (r.id === step.roleId) opt.selected = true;
                    roleSelect.appendChild(opt);
                });
                const phraseSelect = document.createElement('select');
                phraseSelect.className = 'phrase-select';
                phraseSelect.dataset.idx = idx;
                const defaultOpt = document.createElement('option');
                defaultOpt.value = '-1';
                defaultOpt.textContent = '✏️ 自定义';
                phraseSelect.appendChild(defaultOpt);
                PHRASE_DATA.forEach((p, pi) => {
                    const opt = document.createElement('option');
                    opt.value = pi;
                    opt.textContent = `${p.en} (${p.zh})`;
                    if (pi === step.phraseIdx) opt.selected = true;
                    phraseSelect.appendChild(opt);
                });
                const customInput = document.createElement('input');
                customInput.type = 'text';
                customInput.className = 'custom-input';
                customInput.placeholder = '输入自定义台词...';
                customInput.value = step.customText || '';
                customInput.dataset.idx = idx;
                const numSpan = document.createElement('span');
                numSpan.className = 'step-num';
                numSpan.textContent = `#${idx+1}`;
                const delBtn = document.createElement('button');
                delBtn.className = 'btn-remove-step';
                delBtn.innerHTML = '<i class="fas fa-trash-alt"></i>';
                delBtn.addEventListener('click', function() {
                    if (steps.length <= 1) { showToast('至少保留一个步骤', 'error'); return; }
                    steps.splice(idx, 1);
                    saveData(appData);
                    renderScriptEditor();
                });
                div.appendChild(numSpan);
                div.appendChild(roleSelect);
                div.appendChild(phraseSelect);
                div.appendChild(customInput);
                div.appendChild(delBtn);
                container.appendChild(div);
                const saveStep = () => {
                    if (appData.scriptSteps[idx]) {
                        appData.scriptSteps[idx].roleId = roleSelect.value;
                        appData.scriptSteps[idx].phraseIdx = parseInt(phraseSelect.value);
                        appData.scriptSteps[idx].customText = customInput.value.trim();
                        saveData(appData);
                    }
                };
                roleSelect.addEventListener('change', saveStep);
                phraseSelect.addEventListener('change', function() {
                    if (this.value === '-1') customInput.focus();
                    saveStep();
                });
                customInput.addEventListener('input', saveStep);
                customInput.addEventListener('change', saveStep);
            });
            document.getElementById('stepCount').textContent = steps.length;
            const previewContainer = document.getElementById('scriptPreviewContainer');
            if (previewContainer.style.display !== 'none') generatePreview();
        }

        document.getElementById('addStepBtn').addEventListener('click', function() {
            appData.scriptSteps.push({ roleId: 'r1', phraseIdx: -1, customText: '' });
            saveData(appData);
            renderScriptEditor();
            showToast('已添加新步骤');
        });

        document.getElementById('resetScriptBtn').addEventListener('click', function() {
            if (!confirm('重置为默认对话流程，确定吗？')) return;
            appData.scriptSteps = getDefaultData().scriptSteps;
            saveData(appData);
            renderScriptEditor();
            showToast('已重置为默认流程');
        });

        // ================================================================
        //  预览与下载
        // ================================================================
        function generatePreview() {
            const steps = appData.scriptSteps || [];
            const previewContainer = document.getElementById('scriptPreviewContainer');
            const previewText = document.getElementById('scriptPreviewText');
            if (steps.length === 0) {
                previewText.textContent = '暂无步骤，请添加对话步骤。';
                previewContainer.style.display = 'block';
                return;
            }
            const groupInfo = appData.groupInfo;
            let lines =
                `航前准备会英语对话脚本 (HU7480)\n小组：${groupInfo.groupName || '未命名'} (${groupInfo.groupId || ''})\n${'='.repeat(40)}\n\n`;
            steps.forEach((step, idx) => {
                const role = appData.roles.find(r => r.id === step.roleId);
                const roleName = role ? `${role.title} (${role.member || '未分配'})` : '未知角色';
                let phrase = '';
                if (step.phraseIdx >= 0 && step.phraseIdx < PHRASE_DATA.length) {
                    phrase = PHRASE_DATA[step.phraseIdx].en;
                } else {
                    phrase = step.customText || '（未填写）';
                }
                lines += `【${roleName}】${phrase}\n`;
            });
            const fullText = lines;
            previewText.textContent = fullText;
            previewContainer.style.display = 'block';
            return fullText;
        }

        document.getElementById('previewScriptBtn').addEventListener('click', function() {
            generatePreview();
            showToast('对话预览已更新');
        });

        document.getElementById('downloadScriptBtn').addEventListener('click', function() {
            const fullText = generatePreview();
            if (!fullText || fullText.includes('暂无步骤')) {
                showToast('请先编写对话步骤', 'error');
                return;
            }
            const blob = new Blob([fullText], { type: 'text/plain;charset=utf-8' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            const groupId = appData.groupInfo.groupId || '小组';
            const dateStr = new Date().toISOString().slice(0, 10);
            a.download = `航前准备会对话_HU7480_${groupId}_${dateStr}.txt`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
            showToast('✅ 对话文本已下载');
        });

        // ================================================================
        //  模拟展演评分
        // ================================================================
        function renderRoleplayEval() {
            const container = document.getElementById('roleplayEvalContainer');
            let html = '';
            ROLEPLAY_DIMENSIONS.forEach(item => {
                const score = appData.roleplayEval[item.id] || 0;
                html += `
                    <div class="eval-item">
                        <span class="e-label">${item.label}</span>
                        <span class="e-desc">${item.desc}</span>
                        <div class="e-score-input">
                            <select class="roleplay-score" data-id="${item.id}">
                                ${[0,10,20,30,40,50,60,70,80,90,100].map(v => `<option value="${v}" ${score===v?'selected':''}>${v}</option>`).join('')}
                            </select>
                            <span>/ 100</span>
                        </div>
                    </div>
                `;
            });
            const total = ROLEPLAY_DIMENSIONS.reduce((sum, item) => sum + (appData.roleplayEval[item.id] || 0), 0);
            const avg = Math.round(total / ROLEPLAY_DIMENSIONS.length);
            html += `
                <div style="margin-top:8px;padding:8px 14px;background:#f7faff;border-radius:8px;font-weight:700;color:#1a1a3e;font-size:0.9rem;">
                    模拟展演平均分：<span id="roleplayAvg">${avg}</span> / 100
                </div>
            `;
            container.innerHTML = html;
            container.querySelectorAll('.roleplay-score').forEach(sel => {
                sel.addEventListener('change', function() {
                    const id = this.dataset.id;
                    appData.roleplayEval[id] = parseInt(this.value);
                    saveData(appData);
                    const newTotal = ROLEPLAY_DIMENSIONS.reduce((s, item) => s + (appData.roleplayEval[item.id] ||
                        0), 0);
                    const newAvg = Math.round(newTotal / ROLEPLAY_DIMENSIONS.length);
                    const avgSpan = document.getElementById('roleplayAvg');
                    if (avgSpan) avgSpan.textContent = newAvg;
                    renderScore();
                });
            });
        }

        document.getElementById('saveRoleplayEvalBtn').addEventListener('click', function() {
            saveData(appData);
            showToast('模拟展演评分已保存');
            renderScore();
        });

        // ================================================================
        //  师评
        // ================================================================
        function renderTeacherEval() {
            const container = document.getElementById('teacherEvalContainer');
            let html = '';
            TEACHER_EVAL_ITEMS.forEach(item => {
                const score = appData.teacherEval[item.id] || 0;
                html += `
                    <div class="eval-item">
                        <span class="e-label">${item.label}</span>
                        <span class="e-desc">${item.desc}（权重 ${item.weight}%）</span>
                        <div class="e-score-input">
                            <select class="teacher-score" data-id="${item.id}">
                                ${[0,10,20,30,40,50,60,70,80,90,100].map(v => `<option value="${v}" ${score===v?'selected':''}>${v}</option>`).join('')}
                            </select>
                            <span>/ 100</span>
                        </div>
                    </div>
                `;
            });
            const weightedTotal = TEACHER_EVAL_ITEMS.reduce((sum, item) => {
                const s = appData.teacherEval[item.id] || 0;
                return sum + s * (item.weight / 100);
            }, 0);
            html += `
                <div style="margin-top:10px;padding:8px 14px;background:#f7faff;border-radius:8px;font-weight:700;color:#1a1a3e;font-size:0.95rem;">
                    师评加权总分：<span id="teacherWeightedTotal">${Math.round(weightedTotal)}</span> / 100
                </div>
                <div style="margin-top:10px;">
                    <label style="font-weight:600;font-size:0.8rem;color:#1a1a3e;display:block;margin-bottom:3px;"><i class="fas fa-comment"></i> 教师评语</label>
                    <textarea id="teacherComment" rows="3" style="width:100%;padding:8px 12px;border-radius:8px;border:1px solid #dce4ec;font-size:0.85rem;font-family:inherit;resize:vertical;background:#fafcff;">${appData.teacherComment || ''}</textarea>
                </div>
            `;
            container.innerHTML = html;
            container.querySelectorAll('.teacher-score').forEach(sel => {
                sel.addEventListener('change', function() {
                    const id = this.dataset.id;
                    appData.teacherEval[id] = parseInt(this.value);
                    saveData(appData);
                    const newWeighted = TEACHER_EVAL_ITEMS.reduce((sum, item) => {
                        const s = appData.teacherEval[item.id] || 0;
                        return sum + s * (item.weight / 100);
                    }, 0);
                    const totalSpan = document.getElementById('teacherWeightedTotal');
                    if (totalSpan) totalSpan.textContent = Math.round(newWeighted);
                    renderScore();
                });
            });
            const commentArea = document.getElementById('teacherComment');
            if (commentArea) {
                commentArea.addEventListener('change', function() {
                    appData.teacherComment = this.value;
                    saveData(appData);
                });
                commentArea.addEventListener('input', function() {
                    appData.teacherComment = this.value;
                    saveData(appData);
                });
            }
        }

        document.getElementById('saveTeacherEvalBtn').addEventListener('click', function() {
            const comment = document.getElementById('teacherComment');
            if (comment) appData.teacherComment = comment.value;
            saveData(appData);
            showToast('师评已保存');
            renderScore();
        });

        // ================================================================
        //  成绩总览
        // ================================================================
        function renderScore() {
            const container = document.getElementById('scoreSummary');
            const detailContainer = document.getElementById('scoreDetail');

            let vocabTotal = 0,
                vocabCount = 0;
            VOCAB_DATA.forEach(item => {
                const data = appData.vocabScores[item.word];
                if (data && data.score > 0) { vocabTotal += data.score;
                    vocabCount++; }
            });
            const vocabAvg = vocabCount > 0 ? Math.round(vocabTotal / vocabCount) : 0;

            const dialogueScore = appData.teacherEval['t2'] || 0;

            const rpTotal = ROLEPLAY_DIMENSIONS.reduce((sum, item) => sum + (appData.roleplayEval[item.id] || 0), 0);
            const rpAvg = ROLEPLAY_DIMENSIONS.length > 0 ? Math.round(rpTotal / ROLEPLAY_DIMENSIONS.length) : 0;

            const teacherWeighted = TEACHER_EVAL_ITEMS.reduce((sum, item) => {
                const s = appData.teacherEval[item.id] || 0;
                return sum + s * (item.weight / 100);
            }, 0);
            const finalScore = Math.round(teacherWeighted);

            let grade = '待评定',
                gradeColor = '#8a9eb0';
            if (finalScore >= 90) { grade = '优秀';
                gradeColor = '#2d7d5a'; } else if (finalScore >= 80) { grade = '良好';
                gradeColor = '#2d7d5a'; } else if (finalScore >= 70) { grade = '中等';
                gradeColor = '#c99f4a'; } else if (finalScore >= 60) { grade = '及格';
                gradeColor = '#c99f4a'; } else if (finalScore > 0) { grade = '待提高';
                gradeColor = '#c0392b'; }

            container.innerHTML = `
                <div class="score-box">
                    <div class="label">词汇掌握</div>
                    <div class="value">${vocabAvg}</div>
                    <div class="weight">${vocabCount}/${VOCAB_DATA.length} 个已评分</div>
                </div>
                <div class="score-box">
                    <div class="label">对话理解</div>
                    <div class="value gold">${dialogueScore}</div>
                    <div class="weight">权重 30%</div>
                </div>
                <div class="score-box">
                    <div class="label">模拟展演</div>
                    <div class="value gold">${rpAvg}</div>
                    <div class="weight">权重 50%</div>
                </div>
                <div class="score-box" style="background:#fdf8ee;border-color:#c99f4a;">
                    <div class="label">最终成绩</div>
                    <div class="value green" style="font-size:2rem;">${finalScore}</div>
                    <div class="weight" style="color:${gradeColor};font-weight:700;font-size:0.85rem;">${grade}</div>
                </div>
            `;

            let detailHtml = `
                <h4 style="color:#1a1a3e;margin:10px 0 6px;">📋 评分明细</h4>
                <table>
                    <thead><tr><th>评价维度</th><th>得分</th><th>权重</th><th>加权得分</th></tr></thead>
                    <tbody>
                        <tr><td>词汇掌握度</td><td>${vocabAvg}</td><td>—</td><td>—</td></tr>
                        <tr><td>对话理解与应答</td><td>${dialogueScore}</td><td>30%</td><td>${Math.round(dialogueScore * 0.3)}</td></tr>
                        <tr><td>模拟展演表现</td><td>${rpAvg}</td><td>50%</td><td>${Math.round(rpAvg * 0.5)}</td></tr>
                        <tr style="font-weight:700;background:#f7faff;">
                            <td><strong>师评加权总分</strong></td>
                            <td colspan="3"><strong>${Math.round(teacherWeighted)}</strong> 分（${grade}）</td>
                        </tr>
                    </tbody>
                </table>
            `;

            let vocabDetail = '';
            VOCAB_DATA.forEach(item => {
                const data = appData.vocabScores[item.word];
                const score = data ? data.score : 0;
                vocabDetail += `<span style="display:inline-block;margin:2px 4px;padding:1px 8px;border-radius:12px;font-size:0.7rem;background:${score > 0 ? '#d4edda' : '#e6edf6'};color:${score > 0 ? '#1a6e4a' : '#8a9eb0'};">${item.word} ${score > 0 ? score : '—'}</span>`;
            });
            detailHtml += `
                <div style="margin-top:12px;">
                    <h4 style="color:#1a1a3e;margin:6px 0;">📝 词汇评分详情</h4>
                    <div style="padding:6px 0;">${vocabDetail}</div>
                </div>
            `;

            let teacherDetail = '';
            TEACHER_EVAL_ITEMS.forEach(item => {
                const s = appData.teacherEval[item.id] || 0;
                teacherDetail +=
                    `<span style="display:inline-block;margin:2px 6px;font-size:0.78rem;">${item.label}: <strong>${s}</strong></span>`;
            });
            detailHtml += `
                <div style="margin-top:8px;">
                    <h4 style="color:#1a1a3e;margin:6px 0;">👩‍🏫 师评详情</h4>
                    <div style="padding:4px 0;">${teacherDetail}</div>
                    ${appData.teacherComment ? `<div style="padding:6px 12px;background:#f7faff;border-radius:8px;border-left:3px solid #c99f4a;margin-top:4px;font-size:0.82rem;"><strong>评语：</strong>${appData.teacherComment}</div>` : ''}
                </div>
            `;

            detailContainer.innerHTML = detailHtml;
        }

        // ================================================================
        //  初始化
        // ================================================================
        function init() {
            loadInfoToForm();
            renderVocab();
            renderPhrases();
            renderDialogues();
            renderRoles();
            renderScriptEditor();
            renderRoleplayEval();
            renderTeacherEval();
            renderScore();

            if (!('webkitSpeechRecognition' in window) && !('SpeechRecognition' in window)) {
                showToast('⚠️ 当前浏览器不支持语音识别，请使用Chrome浏览器进行跟读评分', 'error');
            } else {
                showToast('✈ HU7480航前准备会英语实训系统 v4 已加载（对话卡片）', 'success');
            }
            console.log('📦 HU7480航前准备会英语实训系统 v4 已启动（对话卡片）');
        }

        setInterval(() => { saveData(appData); }, 30000);
        window.addEventListener('beforeunload', () => { saveData(appData); });

        if (document.readyState === 'complete') {
            init();
        } else {
            window.addEventListener('load', init);
        }
    </script>
</body>
</html>
