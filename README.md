[Uploading index.html.html…]()
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>航前准备会英语 · 实训任务系统</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
    <style>
        /* ===== 全部样式 ===== */
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
        .btn-xs { padding:2px 8px; font-size:0.6rem; border-radius:20px; }
        .btn:disabled { opacity:0.5; cursor:not-allowed; transform:none !important; }
        .flex-between { display:flex; justify-content:space-between; align-items:center; flex-wrap:wrap; gap:8px; }
        .flex-center { display:flex; align-items:center; gap:8px; flex-wrap:wrap; }
        .mt-12 { margin-top:12px; }
        .mb-12 { margin-bottom:12px; }
        .text-muted { color:#8a9eb0; font-size:0.78rem; }
        .text-gold { color:#c99f4a; }
        .text-success { color:#2d7d5a; }
        .text-danger { color:#c0392b; }

        /* 词汇 */
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

        /* 句型 */
        .phrase-list { display:flex; flex-direction:column; gap:8px; }
        .phrase-item { display:flex; align-items:center; gap:10px; padding:8px 14px; background:#f7faff; border-radius:10px; border-left:4px solid #c99f4a; transition:0.2s; flex-wrap:wrap; }
        .phrase-item:hover { background:#f0f6fe; }
        .phrase-item .en { font-weight:600; font-size:0.92rem; color:#1a1a3e; min-width:140px; display:flex; align-items:center; gap:6px; }
        .phrase-item .zh { color:#4a5a6e; font-size:0.85rem; }
        .phrase-item .tag { margin-left:auto; font-size:0.6rem; color:#8a9eb0; background:#e6edf6; padding:1px 10px; border-radius:20px; }
        .phrase-item .speak-icon-sm { font-size:0.7rem; color:#b6cce0; cursor:pointer; transition:0.2s; }
        .phrase-item .speak-icon-sm:hover { color:#c99f4a; }

        /* 情境卡片 */
        .scene-grid { display:grid; grid-template-columns:repeat(auto-fill,minmax(360px,1fr)); gap:16px; }
        .scene-card { background:#f7faff; border-radius:14px; padding:16px 18px; border:1px solid #e6edf6; transition:0.2s; display:flex; flex-direction:column; }
        .scene-card:hover { border-color:#b6cce0; }
        .scene-card .scene-num { font-size:0.6rem; font-weight:700; color:#c99f4a; background:rgba(201,159,74,0.1); padding:1px 10px; border-radius:20px; display:inline-block; margin-bottom:4px; align-self:flex-start; }
        .scene-card .scene-title { font-weight:700; font-size:0.95rem; color:#1a1a3e; margin-bottom:8px; }
        .scene-card .scene-category { font-size:0.6rem; font-weight:600; color:#fff; background:#2c2c6e; padding:1px 10px; border-radius:20px; display:inline-block; margin-bottom:6px; align-self:flex-start; }
        .scene-card .dialogue-block { margin:3px 0; display:flex; align-items:center; flex-wrap:wrap; gap:4px 8px; }
        .scene-card .dialogue-block .speaker-label { font-weight:600; font-size:0.78rem; color:#4a5a6e; min-width:60px; }
        .scene-card .dialogue-block .pax-text { color:#2980b9; font-weight:500; font-size:0.9rem; flex:1; min-width:80px; }
        .scene-card .dialogue-block .crew-text { color:#c99f4a; font-weight:500; font-size:0.9rem; flex:1; min-width:80px; }
        .scene-card .btn-audio { background:rgba(201,159,74,0.1); border:none; color:#c99f4a; width:28px; height:28px; border-radius:50%; cursor:pointer; font-size:0.7rem; transition:0.2s; display:inline-flex; align-items:center; justify-content:center; flex-shrink:0; }
        .scene-card .btn-audio:hover { background:#c99f4a; color:#fff; }
        .scene-card .btn-audio.playing { background:#2d7d5a; color:#fff; }
        .scene-card .divider { border-top:1px dashed #e6edf6; margin:8px 0; }

        .student-answer-area { background:#f0f7ff; border-radius:10px; padding:10px 14px; margin:6px 0; border-left:3px solid #2980b9; }
        .student-answer-area .answer-label { font-size:0.7rem; font-weight:600; color:#2980b9; margin-bottom:4px; display:flex; align-items:center; gap:6px; }
        .student-answer-area .audio-controls { display:flex; align-items:center; gap:6px; flex-wrap:wrap; }
        .student-answer-area .audio-controls .btn-rec { background:rgba(41,128,185,0.12); border:none; color:#2980b9; padding:3px 12px; border-radius:20px; font-size:0.7rem; font-weight:600; cursor:pointer; transition:0.2s; display:inline-flex; align-items:center; gap:4px; }
        .student-answer-area .audio-controls .btn-rec:hover { background:#2980b9; color:#fff; }
        .student-answer-area .audio-controls .btn-rec.recording { background:#c0392b; color:#fff; animation:pulse-icon 0.6s infinite; }
        .student-answer-area .audio-controls .btn-rec:disabled { opacity:0.4; cursor:not-allowed; }
        .student-answer-area .audio-controls .status-text { font-size:0.7rem; color:#5a6e82; }
        .student-answer-area .audio-controls .status-text.done { color:#2d7d5a; font-weight:600; }
        .student-answer-area .audio-controls .rec-time { font-size:0.65rem; color:#8a9eb0; min-width:30px; }

        .reference-area { background:#fcf9f0; border-radius:10px; padding:8px 14px; margin:4px 0; border-left:3px solid #c99f4a; }
        .reference-area .ref-header { display:flex; align-items:center; justify-content:space-between; flex-wrap:wrap; gap:6px; }
        .reference-area .ref-header .ref-label { font-size:0.7rem; font-weight:600; color:#c99f4a; display:flex; align-items:center; gap:6px; }
        .reference-area .btn-hint { background:rgba(201,159,74,0.12); border:none; color:#c99f4a; padding:2px 14px; border-radius:20px; font-size:0.65rem; font-weight:600; cursor:pointer; transition:0.2s; }
        .reference-area .btn-hint:hover { background:#c99f4a; color:#fff; }
        .reference-area .ref-content { display:none; margin-top:6px; padding-top:6px; border-top:1px dashed #e6edf6; }
        .reference-area .ref-content.show { display:block; }
        .reference-area .ref-content .ref-text { font-size:0.9rem; color:#2a3a4a; font-weight:500; }
        .reference-area .ref-content .ref-trans { font-size:0.8rem; color:#5a6e82; margin-top:2px; }
        .reference-area .ref-content .ref-actions { display:flex; align-items:center; gap:6px; margin-top:4px; }

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

        .eval-item { display:flex; align-items:center; gap:12px; padding:8px 14px; background:#f7faff; border-radius:10px; border:1px solid #e6edf6; flex-wrap:wrap; }
        .eval-item .e-label { font-weight:600; font-size:0.82rem; color:#1a1a3e; min-width:100px; }
        .eval-item .e-desc { font-size:0.75rem; color:#5a6e82; flex:1; min-width:80px; }
        .eval-item .e-score-input select { padding:3px 8px; border-radius:6px; border:1px solid #dce4ec; font-size:0.8rem; background:#fff; font-weight:600; width:70px; }

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

        @media print { body { padding-top:0; background:#fff; } .navbar { display:none !important; } .page { display:block !important; animation:none !important; } .card { box-shadow:none !important; border:1px solid #ddd; break-inside:avoid; page-break-inside:avoid; } .btn { display:none !important; } .container { padding:10px; } .vocab-grid { grid-template-columns:repeat(2,1fr); } .scene-grid { grid-template-columns:repeat(2,1fr); } .role-grid { grid-template-columns:repeat(2,1fr); } .score-summary { grid-template-columns:repeat(4,1fr); } .form-group input,.form-group textarea,.role-card .r-name input { border-color:#ccc !important; background:#fafafa !important; } .vocab-card .actions .record-btn { display:none !important; } .no-print { display:none !important; } .student-answer-area .audio-controls .btn-rec { display:none !important; } .reference-area .btn-hint { display:none !important; } .reference-area .ref-content { display:block !important; } .script-step .btn-remove-step { display:none !important; } }
        @media (max-width:820px) { .navbar { padding:0 10px; height:56px; flex-wrap:nowrap; gap:4px; } .navbar .brand { font-size:0.7rem; } .navbar .brand span { display:none; } .navbar .nav-links a { font-size:0.55rem; padding:3px 8px; } body { padding-top:60px; } .container { padding:10px; } .card { padding:14px 14px; } .vocab-grid { grid-template-columns:repeat(auto-fill,minmax(180px,1fr)); } .scene-grid { grid-template-columns:1fr; } .role-grid { grid-template-columns:1fr 1fr; } .form-row { grid-template-columns:1fr; } .score-summary { grid-template-columns:1fr 1fr; } .script-step { flex-direction:column; align-items:stretch; } .script-step .step-num { min-width:auto; } }
        @media (max-width:480px) { .navbar .nav-links a { font-size:0.5rem; padding:2px 6px; } .navbar .brand { font-size:0.6rem; } .navbar .right-actions .print-btn span { display:none; } .vocab-grid { grid-template-columns:1fr; } .role-grid { grid-template-columns:1fr; } .score-summary { grid-template-columns:1fr; } .card-title { font-size:0.9rem; } .eval-item { flex-direction:column; align-items:stretch; gap:4px; } .eval-item .e-label { min-width:auto; } .scene-card .dialogue-block .speaker-label { min-width:auto; } .scene-grid { grid-template-columns:1fr; } }
        .toast { position:fixed; bottom:24px; right:24px; background:#1a1a3e; color:#fff; padding:8px 20px; border-radius:12px; box-shadow:0 8px 24px rgba(0,0,0,0.2); font-weight:600; transform:translateY(100px); opacity:0; transition:all 0.4s ease; z-index:999; max-width:380px; font-size:0.8rem; }
        .toast.show { transform:translateY(0); opacity:1; }
        .toast.success { background:#2d7d5a; }
        .toast.error { background:#c0392b; }
        .toast.info { background:#2980b9; }
        .footer { text-align:center; padding:14px 0 4px; color:#8a9eb0; font-size:0.65rem; border-top:1px solid #e6edf6; margin-top:4px; }
        .footer i { color:#c99f4a; }
        .empty-state { text-align:center; padding:16px; color:#8a9eb0; }
        .empty-state i { font-size:1.6rem; display:block; margin-bottom:4px; color:#dce4ec; }
        .recognition-status { font-size:0.75rem; color:#5a6e82; padding:4px 10px; border-radius:20px; background:#f0f4f9; display:inline-block; margin-top:4px; }
        .recognition-status.active { background:#d6eaf8; color:#1a5276; }
        .recognition-status.error { background:#fadbd8; color:#922b21; }
        .recognition-status.success { background:#d4edda; color:#1a6e4a; }
    </style>
</head>
<body>

    <!-- ===== 导航 ===== -->
    <nav class="navbar" id="navbar">
        <div class="brand"><i class="fas fa-plane"></i> 航前准备会 <span>· 英语实训</span></div>
        <div class="nav-links">
            <a class="active" data-page="page-info"><i class="fas fa-info-circle"></i> 小组</a>
            <a data-page="page-vocab"><i class="fas fa-book-open"></i> 词汇</a>
            <a data-page="page-phrases"><i class="fas fa-comment-dots"></i> 句型</a>
            <a data-page="page-scene"><i class="fas fa-images"></i> 情境卡片</a>
            <a data-page="page-roleplay"><i class="fas fa-user-tag"></i> 情景模拟</a>
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
                    <div class="form-group"><label><i class="fas fa-tasks"></i> 实训任务</label><input type="text" id="taskName" value="航前准备会英语实训 · HU7480" /></div>
                    <div class="form-group"><label><i class="fas fa-user-tie"></i> 指导教师</label><input type="text" id="teacherName" placeholder="请输入姓名" /></div>
                </div>
                <div style="margin-top:10px;"><button class="btn btn-success" id="saveInfoBtn"><i class="fas fa-save"></i> 保存信息</button><span class="text-muted" style="margin-left:10px;">数据自动保存在浏览器</span></div>
            </div>
            <div class="card">
                <div class="card-title"><i class="fas fa-clipboard-list"></i> 任务说明</div>
                <p style="color:#4a5a6e;font-size:0.92rem;">本实训基于 <strong>HU7480 航班（三亚→北京）</strong> 实际数据，聚焦航前准备会英语问答。通过 <strong>词汇跟读</strong>、<strong>情境卡片录音</strong>、<strong>情景模拟对话</strong> 三个环节，掌握航班信息、服务信息、旅客信息、安全信息及 <strong>特情处置</strong> 的核心英语表达。</p>
                <div style="background:#f7faff;padding:10px 14px;border-radius:8px;margin-top:8px;font-size:0.85rem;border-left:3px solid #c99f4a;">
                    <strong>📋 航班速览</strong><br>航班号 HU7480 · 机型 A330-300 · 航程 SYX → PEK · 飞行 3h45min<br>旅客：头等5 / 经济221 · 特殊：UMNR / PREG · 特殊餐：AVML/MOML
                </div>
            </div>
        </div>

        <!-- ===== 词汇 ===== -->
        <div class="page" id="page-vocab">
            <div class="card">
                <div class="card-title"><i class="fas fa-book-open"></i> 航前准备会核心词汇 <span class="sub">点击 <i class="fas fa-volume-up"></i> 听发音 · 点击 <i class="fas fa-microphone"></i> 跟读评分</span></div>
                <p class="section-desc">包含航班、服务、旅客、安全及特情处置相关词汇。</p>
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
                <div class="card-title"><i class="fas fa-comment-dots"></i> 航前准备会常用句型 <span class="sub">点击 <i class="fas fa-volume-up"></i> 听发音</span></div>
                <p class="section-desc">覆盖航班信息、服务信息、旅客信息、安全信息及特情处置。</p>
                <div class="phrase-list" id="phraseList"></div>
            </div>
        </div>

        <!-- ===== 情境卡片 ===== -->
        <div class="page" id="page-scene">
            <div class="card">
                <div class="card-title"><i class="fas fa-images"></i> 情境卡片 · 特殊疑问句 + 特情处置 <span class="sub">听提问→录回答→看提示</span></div>
                <p class="section-desc"><span class="text-gold">①</span> 点击 <i class="fas fa-play text-gold"></i> 听乘务长提问 &nbsp;|&nbsp; <span class="text-gold">②</span> 点击 <i class="fas fa-microphone text-gold"></i> 录音你的回答 &nbsp;|&nbsp; <span class="text-gold">③</span> 点击 <strong>提示</strong> 查看参考回答</p>
                <div class="scene-grid" id="sceneGrid"></div>
                <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap;align-items:center;">
                    <button class="btn btn-outline btn-sm" id="clearSceneRecordingsBtn"><i class="fas fa-trash-alt"></i> 清除所有录音</button>
                    <span class="text-muted" id="sceneRecordingsProgress">已录音 0/14 个场景</span>
                </div>
            </div>
        </div>

        <!-- ===== 情景模拟 ===== -->
        <div class="page" id="page-roleplay">
            <div class="card">
                <div class="card-title"><i class="fas fa-user-tag"></i> 1. 角色分工</div>
                <p class="section-desc">为每个岗位分配成员姓名（可多选，用逗号分隔）。</p>
                <div class="role-grid" id="roleGrid"></div>
                <div style="margin-top:12px;"><button class="btn btn-success" id="saveRolesBtn"><i class="fas fa-save"></i> 保存角色分配</button><span class="text-muted" style="margin-left:10px;">数据自动保存</span></div>
            </div>
            <div class="card">
                <div class="card-title"><i class="fas fa-pen-fancy"></i> 2. 对话文本编写</div>
                <p class="section-desc">按照航前准备会流程顺序，为每个步骤选择角色和对应台词。</p>
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
                <div style="margin-top:10px;"><button class="btn btn-success" id="saveRoleplayEvalBtn"><i class="fas fa-save"></i> 保存评分</button><span class="text-muted" style="margin-left:10px;">数据自动保存</span></div>
            </div>
        </div>

        <!-- ===== 师评成绩 ===== -->
        <div class="page" id="page-eval">
            <div class="card">
                <div class="card-title"><i class="fas fa-chalkboard-teacher"></i> 教师综合评价</div>
                <p class="section-desc">教师根据词汇掌握度、情境应答能力、模拟展演表现三方面综合评定。</p>
                <div id="teacherEvalContainer"></div>
                <div style="margin-top:10px;"><button class="btn btn-success" id="saveTeacherEvalBtn"><i class="fas fa-save"></i> 保存师评</button><span class="text-muted" style="margin-left:10px;">数据自动保存</span></div>
            </div>
            <div class="card">
                <div class="card-title"><i class="fas fa-chart-bar"></i> 成绩总览</div>
                <p class="text-muted" style="margin-bottom:10px;">最终成绩 = 词汇掌握 × 20% + 情境应答 × 30% + 模拟展演 × 50%</p>
                <div id="scoreSummary"></div>
                <div id="scoreDetail" class="score-detail"></div>
            </div>
        </div>

        <div class="footer"><i class="fas fa-plane"></i> 航前准备会英语 · 实训任务系统 &nbsp;|&nbsp; 数据本地存储<br><span style="font-size:0.6rem;">“敬畏生命、敬畏规章、敬畏职责” —— 以专业态度，学好航前准备会英语</span></div>
    </div>

    <div class="toast" id="toast"></div>

    <script>
        // ================================================================
        //  数据定义
        // ================================================================

        const STORAGE_KEY = 'preflight_briefing_system_v3';

        const VOCAB_DATA = [
            { word: 'flight number', phonetic: '/flaɪt ˈnʌmbə/', meaning: 'n. 航班号' },
            { word: 'aircraft type', phonetic: '/ˈeəkrɑːft taɪp/', meaning: 'n. 机型' },
            { word: 'route', phonetic: '/ruːt/', meaning: 'n. 航程' },
            { word: 'duration', phonetic: '/djʊəˈreɪʃn/', meaning: 'n. 飞行时间' },
            { word: 'weather', phonetic: '/ˈweðə/', meaning: 'n. 天气' },
            { word: 'special meal', phonetic: '/ˈspeʃəl miːl/', meaning: 'n. 特殊餐食' },
            { word: 'unaccompanied minor', phonetic: '/ˌʌnəˈkʌmpənid ˈmaɪnə/', meaning: 'n. 无人陪伴儿童' },
            { word: 'pregnant', phonetic: '/ˈpreɡnənt/', meaning: 'adj. 怀孕的' },
            { word: 'vegetarian', phonetic: '/ˌvedʒəˈteəriən/', meaning: 'n. 素食者' },
            { word: 'first class', phonetic: '/fɜːst klɑːs/', meaning: 'n. 头等舱' },
            { word: 'economy class', phonetic: '/iˈkɒnəmi klɑːs/', meaning: 'n. 经济舱' },
            { word: 'departure time', phonetic: '/dɪˈpɑːtʃə taɪm/', meaning: 'n. 离港时间' },
            { word: 'duty free', phonetic: '/ˈdjuːti friː/', meaning: 'n. 免税品' },
            { word: 'altitude', phonetic: '/ˈæltɪtjuːd/', meaning: 'n. 飞行高度' },
            { word: 'emergency', phonetic: '/iˈmɜːdʒənsi/', meaning: 'n. 紧急情况' },
            { word: 'delay', phonetic: '/dɪˈleɪ/', meaning: 'n. 延误' },
            { word: 'diversion', phonetic: '/daɪˈvɜːʃn/', meaning: 'n. 备降' },
            { word: 'medical', phonetic: '/ˈmedɪkl/', meaning: 'adj. 医疗的' },
            { word: 'assistance', phonetic: '/əˈsɪstəns/', meaning: 'n. 协助' },
            { word: 'passenger list', phonetic: '/ˈpæsɪndʒə lɪst/', meaning: 'n. 旅客名单' }
        ];

        const PHRASE_DATA = [
            { en: 'What is the flight number?', zh: '航班号是多少？', tag: '航班信息' },
            { en: 'What is the aircraft type?', zh: '机型是什么？', tag: '航班信息' },
            { en: 'What is the route?', zh: '航程是什么？', tag: '航班信息' },
            { en: 'How long is the flight?', zh: '飞行时间多长？', tag: '航班信息' },
            { en: 'What is the departure time?', zh: '离港时间是什么？', tag: '航班信息' },
            { en: 'What special meals do we have?', zh: '有哪些特殊餐食？', tag: '服务信息' },
            { en: 'What services are offered onboard?', zh: '机上提供哪些服务？', tag: '服务信息' },
            { en: 'How many passengers on board?', zh: '机上有多少旅客？', tag: '旅客信息' },
            { en: 'Are there any special passengers?', zh: '有特殊旅客吗？', tag: '旅客信息' },
            { en: 'What is the operating altitude?', zh: '飞行高度是多少？', tag: '安全信息' },
            { en: 'What is the weather en route?', zh: '航路天气如何？', tag: '安全信息' },
            { en: 'What should we do if the flight is delayed?', zh: '如果航班延误，我们该怎么办？', tag: '特情处置' },
            { en: 'What should we do if a passenger feels sick?', zh: '如果旅客感到不适，我们该怎么办？', tag: '特情处置' },
            { en: 'What should we do in an emergency?', zh: '紧急情况下我们该怎么办？', tag: '特情处置' }
        ];

        const SCENE_DATA = [{
            id: 1,
            category: '航班信息',
            title: '询问航班号',
            pax: 'What is the flight number?',
            crew: 'The flight number is HU7480.',
            trans: '航班号是HU7480。'
        }, {
            id: 2,
            category: '航班信息',
            title: '询问机型',
            pax: 'What is the aircraft type?',
            crew: 'The aircraft type is Airbus 330-300.',
            trans: '机型是空客330-300。'
        }, {
            id: 3,
            category: '航班信息',
            title: '询问航程',
            pax: 'What is the route?',
            crew: 'The route is from SYX to PEK.',
            trans: '航程是从三亚到北京。'
        }, {
            id: 4,
            category: '航班信息',
            title: '询问飞行时间',
            pax: 'How long is the flight?',
            crew: 'It is 3 hours and 45 minutes.',
            trans: '飞行时间为3小时45分钟。'
        }, {
            id: 5,
            category: '航班信息',
            title: '询问离港时间',
            pax: 'What is the departure time?',
            crew: 'Departure time is 22:10.',
            trans: '离港时间为22:10。'
        }, {
            id: 6,
            category: '服务信息',
            title: '询问特殊餐食',
            pax: 'What special meals do we have?',
            crew: 'We have AVML and MOML.',
            trans: '我们有亚洲素食餐和穆斯林餐。'
        }, {
            id: 7,
            category: '服务信息',
            title: '询问机上服务',
            pax: 'What services are offered onboard?',
            crew: 'We offer food, drinks and duty-free sales.',
            trans: '我们提供餐食、饮品和免税品销售。'
        }, {
            id: 8,
            category: '旅客信息',
            title: '询问旅客人数',
            pax: 'How many passengers on board?',
            crew: 'We have 5 in first class and 221 in economy.',
            trans: '头等舱5人，经济舱221人。'
        }, {
            id: 9,
            category: '旅客信息',
            title: '询问特殊旅客',
            pax: 'Are there any special passengers?',
            crew: 'Yes, one UMNR and one PREG.',
            trans: '是的，一名无人陪伴儿童和一名孕妇。'
        }, {
            id: 10,
            category: '安全信息',
            title: '询问飞行高度',
            pax: 'What is the operating altitude?',
            crew: 'The altitude is 10 kilometers.',
            trans: '飞行高度为10公里。'
        }, {
            id: 11,
            category: '安全信息',
            title: '询问航路天气',
            pax: 'What is the weather en route?',
            crew: 'It is sunny, 26°C.',
            trans: '天气晴朗，26°C。'
        }, {
            id: 12,
            category: '特情处置',
            title: '航班延误处置',
            pax: 'What should we do if the flight is delayed?',
            crew: 'We will inform passengers and provide assistance.',
            trans: '我们会通知旅客并提供协助。'
        }, {
            id: 13,
            category: '特情处置',
            title: '旅客突发疾病',
            pax: 'What should we do if a passenger feels sick?',
            crew: 'We will give first aid and call for medical help.',
            trans: '我们会进行急救并呼叫医疗帮助。'
        }, {
            id: 14,
            category: '特情处置',
            title: '紧急情况应对',
            pax: 'What should we do in an emergency?',
            crew: 'We will follow the emergency procedures.',
            trans: '我们会遵循紧急程序。'
        }];

        const ROLE_DATA = [
            { id: 'r1', title: '乘务长 (Purser)', icon: 'fa-user-tie' },
            { id: 'r2', title: '客舱乘务员1', icon: 'fa-user' },
            { id: 'r3', title: '客舱乘务员2', icon: 'fa-user' },
            { id: 'r4', title: '客舱乘务员3', icon: 'fa-user' },
            { id: 'r5', title: '客舱乘务员4', icon: 'fa-user' },
            { id: 'r6', title: '安全员', icon: 'fa-shield-alt' }
        ];

        const TEACHER_EVAL_ITEMS = [
            { id: 't1', label: '词汇掌握度', desc: '20个核心词汇的认读与发音准确度', weight: 20 },
            { id: 't2', label: '情境应答能力', desc: '14个情境（含特情）的应答熟练度', weight: 30 },
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
                groupInfo: { className: '', groupName: '', groupId: '', taskName: '航前准备会英语实训 · HU7480', teacher: '' },
                vocabScores: {},
                roles: ROLE_DATA.map(r => ({ ...r, member: '' })),
                scriptSteps: [
                    { roleId: 'r1', phraseIdx: 0, customText: '' },
                    { roleId: 'r2', phraseIdx: 1, customText: '' },
                    { roleId: 'r1', phraseIdx: 2, customText: '' },
                    { roleId: 'r3', phraseIdx: 3, customText: '' },
                    { roleId: 'r4', phraseIdx: 4, customText: '' },
                    { roleId: 'r2', phraseIdx: 5, customText: '' },
                    { roleId: 'r3', phraseIdx: 6, customText: '' },
                    { roleId: 'r4', phraseIdx: 7, customText: '' },
                    { roleId: 'r5', phraseIdx: 8, customText: '' },
                    { roleId: 'r1', phraseIdx: 11, customText: '' },
                    { roleId: 'r5', phraseIdx: 12, customText: '' },
                    { roleId: 'r6', phraseIdx: 13, customText: '' }
                ],
                sceneRecordings: {},
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
                    if (!parsed.sceneRecordings) parsed.sceneRecordings = {};
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
                // 渲染对应内容
                if (pageId === 'page-info') loadInfoToForm();
                else if (pageId === 'page-vocab') renderVocab();
                else if (pageId === 'page-phrases') renderPhrases();
                else if (pageId === 'page-scene') renderScenes();
                else if (pageId === 'page-roleplay') { renderRoles();
                    renderScriptEditor();
                    renderRoleplayEval(); }
                else if (pageId === 'page-eval') { renderTeacherEval();
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
            document.getElementById('taskName').value = info.taskName || '航前准备会英语实训 · HU7480';
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
        //  词汇（跟读评分）
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
                    if (b[i - 1] === a[j - 1]) {
                        matrix[i][j] = matrix[i - 1][j - 1];
                    } else {
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
            const list = document.getElementById('phraseList');
            list.innerHTML = '';
            PHRASE_DATA.forEach(item => {
                const div = document.createElement('div');
                div.className = 'phrase-item';
                div.innerHTML = `
                    <span class="en">${item.en}<span class="speak-icon-sm" data-text="${item.en}"><i class="fas fa-volume-up"></i></span></span>
                    <span class="zh">${item.zh}</span>
                    <span class="tag">${item.tag}</span>
                `;
                div.querySelector('.speak-icon-sm').addEventListener('click', function(e) {
                    e.stopPropagation();
                    speakText(this.dataset.text, 'en-US', 0.75);
                    showToast(`🔊 ${this.dataset.text}`, 'info');
                });
                list.appendChild(div);
            });
        }

        // ================================================================
        //  情境卡片（录音+提示）
        // ================================================================

        let activeRecorders = {};

        function renderScenes() {
            const grid = document.getElementById('sceneGrid');
            grid.innerHTML = '';
            let recordedCount = 0;

            SCENE_DATA.forEach(scene => {
                const recording = appData.sceneRecordings[scene.id] || null;
                if (recording && recording.audioData) recordedCount++;

                const div = document.createElement('div');
                div.className = 'scene-card';
                div.dataset.sceneId = scene.id;

                let html = `
                    <div class="scene-num">卡片 ${scene.id}</div>
                    <div class="scene-category">${scene.category}</div>
                    <div class="scene-title">${scene.title}</div>
                    <div class="dialogue-block">
                        <span class="speaker-label">🧑 乘务长：</span>
                        <span class="pax-text">${scene.pax}</span>
                        <button class="btn-audio play-pax" data-text="${scene.pax}" title="播放提问"><i class="fas fa-play"></i></button>
                    </div>
                    <div class="student-answer-area">
                        <div class="answer-label"><i class="fas fa-microphone text-gold"></i> 你的回答</div>
                        <div class="audio-controls">
                            <button class="btn-rec btn-start-rec" data-scene="${scene.id}" title="开始录音"><i class="fas fa-circle" style="color:#c0392b;"></i> 录音</button>
                            <button class="btn-rec btn-stop-rec" data-scene="${scene.id}" style="display:none;" title="停止录音"><i class="fas fa-stop"></i> 停止</button>
                            <button class="btn-rec btn-play-rec" data-scene="${scene.id}" title="播放录音" ${!recording ? 'disabled' : ''}><i class="fas fa-play"></i> 播放</button>
                            <button class="btn-rec btn-delete-rec" data-scene="${scene.id}" title="删除录音" ${!recording ? 'disabled' : ''}><i class="fas fa-trash-alt"></i></button>
                            <span class="status-text" id="rec-status-${scene.id}">${recording ? '✅ 已录音 ' + (recording.duration || 0) + 's' : '⏳ 未录音'}</span>
                            <span class="rec-time" id="rec-time-${scene.id}"></span>
                        </div>
                    </div>
                    <div class="reference-area">
                        <div class="ref-header">
                            <span class="ref-label"><i class="fas fa-lightbulb text-gold"></i> 参考回答</span>
                            <button class="btn-hint" data-scene="${scene.id}"><i class="fas fa-chevron-down"></i> 提示</button>
                        </div>
                        <div class="ref-content" id="ref-content-${scene.id}">
                            <div class="ref-text">👩‍✈️ ${scene.crew}</div>
                            <div class="ref-trans">📖 ${scene.trans}</div>
                            <div class="ref-actions">
                                <button class="btn-audio play-crew" data-text="${scene.crew}" title="播放参考发音"><i class="fas fa-play"></i> 听发音</button>
                            </div>
                        </div>
                    </div>
                `;
                div.innerHTML = html;
                grid.appendChild(div);

                // 播放提问
                div.querySelector('.play-pax').addEventListener('click', function(e) {
                    e.stopPropagation();
                    const text = this.dataset.text;
                    this.classList.add('playing');
                    speakText(text, 'en-US', 0.75, () => { this.classList.remove('playing'); });
                    showToast(`🔊 乘务长：${text}`, 'info');
                });

                // 播放参考
                div.querySelector('.play-crew').addEventListener('click', function(e) {
                    e.stopPropagation();
                    const text = this.dataset.text;
                    this.classList.add('playing');
                    speakText(text, 'en-US', 0.75, () => { this.classList.remove('playing'); });
                    showToast(`🔊 参考：${text}`, 'info');
                });

                // 提示按钮
                div.querySelector('.btn-hint').addEventListener('click', function(e) {
                    e.stopPropagation();
                    const sceneId = this.dataset.scene;
                    const content = document.getElementById(`ref-content-${sceneId}`);
                    const icon = this.querySelector('i');
                    if (content.classList.contains('show')) {
                        content.classList.remove('show');
                        icon.className = 'fas fa-chevron-down';
                        showToast('已收起提示', 'info');
                    } else {
                        content.classList.add('show');
                        icon.className = 'fas fa-chevron-up';
                        showToast('💡 参考回答已展开', 'info');
                    }
                });

                // ---- 录音 ----
                const startBtn = div.querySelector('.btn-start-rec');
                const stopBtn = div.querySelector('.btn-stop-rec');
                const playBtn = div.querySelector('.btn-play-rec');
                const deleteBtn = div.querySelector('.btn-delete-rec');
                const statusEl = document.getElementById(`rec-status-${scene.id}`);
                const timeEl = document.getElementById(`rec-time-${scene.id}`);

                let mediaRecorder = null;
                let audioChunks = [];
                let recordingStartTime = 0;
                let timerInterval = null;

                startBtn.addEventListener('click', async function(e) {
                    e.stopPropagation();
                    if (appData.sceneRecordings[scene.id] && appData.sceneRecordings[scene.id].audioData) {
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
                                appData.sceneRecordings[scene.id] = {
                                    audioData: base64,
                                    duration: duration,
                                    timestamp: new Date().toISOString()
                                };
                                saveData(appData);
                                statusEl.textContent = `✅ 已录音 ${duration}s`;
                                statusEl.className = 'status-text done';
                                playBtn.disabled = false;
                                deleteBtn.disabled = false;
                                updateSceneProgress();
                                showToast(`✅ 场景 ${scene.id} 录音完成 (${duration}s)`, 'success');
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
                    const data = appData.sceneRecordings[scene.id];
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
                    if (!confirm('确定删除此场景的录音吗？')) return;
                    delete appData.sceneRecordings[scene.id];
                    saveData(appData);
                    statusEl.textContent = '⏳ 未录音';
                    statusEl.className = 'status-text';
                    playBtn.disabled = true;
                    deleteBtn.disabled = true;
                    updateSceneProgress();
                    showToast('录音已删除');
                });

                if (recording) {
                    statusEl.textContent = `✅ 已录音 ${recording.duration || 0}s`;
                    statusEl.className = 'status-text done';
                }
            });
            updateSceneProgress();
        }

        function updateSceneProgress() {
            let count = 0;
            SCENE_DATA.forEach(scene => {
                if (appData.sceneRecordings[scene.id] && appData.sceneRecordings[scene.id].audioData) count++;
            });
            document.getElementById('sceneRecordingsProgress').textContent = `已录音 ${count}/${SCENE_DATA.length} 个场景`;
        }

        document.getElementById('clearSceneRecordingsBtn').addEventListener('click', function() {
            if (!confirm('确定清除所有场景的录音数据吗？此操作不可撤销！')) return;
            appData.sceneRecordings = {};
            saveData(appData);
            renderScenes();
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
                `航前准备会英语对话脚本\n小组：${groupInfo.groupName || '未命名'} (${groupInfo.groupId || ''})\n${'='.repeat(40)}\n\n`;
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
            a.download = `航前准备会对话_${groupId}_${dateStr}.txt`;
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

            const sceneScore = appData.teacherEval['t2'] || 0;

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
                    <div class="label">情境应答</div>
                    <div class="value gold">${sceneScore}</div>
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
                        <tr><td>情境应答能力</td><td>${sceneScore}</td><td>30%</td><td>${Math.round(sceneScore * 0.3)}</td></tr>
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
            renderScenes();
            renderRoles();
            renderScriptEditor();
            renderRoleplayEval();
            renderTeacherEval();
            renderScore();

            if (!('webkitSpeechRecognition' in window) && !('SpeechRecognition' in window)) {
                showToast('⚠️ 当前浏览器不支持语音识别，请使用Chrome浏览器进行跟读评分', 'error');
            } else {
                showToast('✈ 航前准备会英语实训系统已加载（完整版）', 'success');
            }
            console.log('📦 系统启动成功');
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
