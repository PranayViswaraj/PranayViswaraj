<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pranay V | Hardware + Software Developer</title>
    
    <!-- Fonts: Inter for UI, JetBrains Mono for Data -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=JetBrains+Mono:wght@400;700&display=swap" rel="stylesheet">

    <style>
        :root {
            --bg-dark: #0d1117;
            --bg-card: #161b22;
            --bg-card-hover: #1c2128;
            --border-color: #30363d;
            --text-main: #c9d1d9;
            --text-muted: #8b949e;
            --accent-blue: #58a6ff;
            --accent-green: #3fb950;
            --accent-purple: #a371f7;
            --accent-red: #f85149;
            --accent-gold: #d29922;
            --glow-blue: 0 0 20px rgba(88, 166, 255, 0.15);
            --font-ui: 'Inter', sans-serif;
            --font-code: 'JetBrains Mono', monospace;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-main);
            font-family: var(--font-ui);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* --- Layout & Container --- */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        section {
            margin-bottom: 80px;
            opacity: 0;
            transform: translateY(20px);
            animation: fadeUp 0.8s forwards;
        }

        @keyframes fadeUp {
            to { opacity: 1; transform: translateY(0); }
        }

        /* --- Typography --- */
        h1, h2, h3 {
            font-weight: 700;
            color: #ffffff;
        }

        h1 { font-size: 3rem; letter-spacing: -1px; margin-bottom: 0.5rem; }
        h2 { font-size: 1.8rem; margin-bottom: 1.5rem; border-left: 4px solid var(--accent-blue); padding-left: 15px; }
        h3 { font-size: 1.2rem; margin-bottom: 0.5rem; color: var(--accent-blue); }
        
        .subtitle {
            color: var(--text-muted);
            font-size: 1.1rem;
            margin-bottom: 2rem;
        }

        .tagline {
            font-family: var(--font-code);
            color: var(--accent-green);
            font-size: 0.9rem;
            background: rgba(63, 185, 80, 0.1);
            padding: 4px 10px;
            border-radius: 4px;
            display: inline-block;
            margin-bottom: 20px;
        }

        /* --- Header --- */
        header {
            text-align: center;
            padding: 60px 0;
            background: radial-gradient(circle at 50% 50%, rgba(88, 166, 255, 0.08), transparent 70%);
        }

        .avatar-frame {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 3px solid var(--accent-blue);
            padding: 4px;
            margin: 0 auto 20px;
            box-shadow: var(--glow-blue);
        }

        .avatar {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            background-color: var(--bg-card);
            background-image: url('https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:16324a,100:0d1117&height=240&section=header&text=PV&fontSize=60&fontColor=ffffff'); /* Placeholder */
            background-size: cover;
        }

        /* --- Stats Bar --- */
        .stats-bar {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin: 30px 0;
        }

        .stat-item {
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            padding: 10px 20px;
            border-radius: 8px;
            font-family: var(--font-code);
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            gap: 8px;
            transition: transform 0.2s;
        }

        .stat-item:hover { transform: translateY(-3px); border-color: var(--accent-blue); }
        .stat-label { color: var(--text-muted); }
        .stat-value { font-weight: 700; color: #fff; }

        /* --- Grid Layouts --- */
        .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 30px; }
        .grid-3 { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 25px; }
        .grid-4 { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; }

        @media (max-width: 768px) {
            .grid-2, .grid-3, .grid-4 { grid-template-columns: 1fr; }
            h1 { font-size: 2.2rem; }
        }

        /* --- Cards (General) --- */
        .card {
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 25px;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .card:hover {
            background: var(--bg-card-hover);
            border-color: var(--accent-blue);
            box-shadow: 0 10px 30px -10px rgba(0,0,0,0.5);
            transform: translateY(-5px);
        }

        .card-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .card-title { font-weight: 600; font-size: 1.1rem; color: #fff; }
        .card-sub { font-size: 0.85rem; color: var(--text-muted); font-family: var(--font-code); }

        /* --- Tech Stack Pills --- */
        .tech-pill {
            display: inline-flex;
            align-items: center;
            gap: 6px;
            background: rgba(88, 166, 255, 0.1);
            color: var(--accent-blue);
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            margin: 0 5px 8px 0;
            border: 1px solid rgba(88, 166, 255, 0.2);
        }
        
        .tech-pill.green { background: rgba(63, 185, 80, 0.1); color: var(--accent-green); border-color: rgba(63, 185, 80, 0.2); }
        .tech-pill.purple { background: rgba(163, 113, 247, 0.1); color: var(--accent-purple); border-color: rgba(163, 113, 247, 0.2); }
        .tech-pill.red { background: rgba(248, 81, 73, 0.1); color: var(--accent-red); border-color: rgba(248, 81, 73, 0.2); }

        /* --- Dashboard Specifics (The "Sensor" Look) --- */
        .dashboard-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 15px;
            margin-bottom: 20px;
        }

        .sensor-card {
            background: linear-gradient(145deg, #161b22, #0d1117);
            border: 1px solid var(--border-color);
            border-radius: 10px;
            padding: 15px;
            text-align: center;
        }

        .sensor-label { font-size: 0.75rem; color: var(--text-muted); text-transform: uppercase; letter-spacing: 1px; margin-bottom: 5px; }
        .sensor-value { font-family: var(--font-code); font-size: 1.8rem; font-weight: 700; color: #fff; }
        .sensor-unit { font-size: 0.9rem; color: var(--text-muted); }
        .sensor-status { 
            font-size: 0.7rem; 
            padding: 2px 8px; 
            border-radius: 10px; 
            margin-top: 8px; 
            display: inline-block;
            font-weight: 600;
        }
        .status-ok { background: rgba(63, 185, 80, 0.2); color: var(--accent-green); }
        .status-warn { background: rgba(210, 153, 34, 0.2); color: var(--accent-gold); }
        .status-crit { background: rgba(248, 81, 73, 0.2); color: var(--accent-red); }

        /* --- Experience Timeline --- */
        .timeline-item {
            border-left: 2px solid var(--border-color);
            padding-left: 25px;
            padding-bottom: 30px;
            position: relative;
        }
        .timeline-item::before {
            content: '';
            position: absolute;
            left: -6px;
            top: 0;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background: var(--accent-blue);
            box-shadow: 0 0 10px var(--accent-blue);
        }
        .timeline-date { font-family: var(--font-code); font-size: 0.85rem; color: var(--accent-blue); margin-bottom: 5px; }
        .timeline-role { font-size: 1.1rem; font-weight: 600; color: #fff; margin-bottom: 5px; }
        .timeline-company { color: var(--text-muted); font-size: 0.95rem; margin-bottom: 10px; }

        /* --- Code Block --- */
        .code-block {
            background: #0d1117;
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 20px;
            font-family: var(--font-code);
            font-size: 0.9rem;
            color: #c9d1d9;
            position: relative;
        }
        .code-block::before {
            content: '● ● ●';
            position: absolute;
            top: 10px;
            left: 15px;
            color: var(--text-muted);
            font-size: 0.8rem;
            letter-spacing: 2px;
        }
        .keyword { color: #ff7b72; }
        .string { color: #a5d6ff; }
        .function { color: #d2a8ff; }
        .comment { color: #8b949e; font-style: italic; }

        /* --- Buttons & Links --- */
        .btn {
            display: inline-block;
            padding: 10px 20px;
            background: var(--accent-blue);
            color: #fff;
            text-decoration: none;
            border-radius: 6px;
            font-weight: 600;
            font-size: 0.9rem;
            transition: background 0.2s;
        }
        .btn:hover { background: #388bfd; }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 20px;
        }
        .social-icon {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--text-muted);
            transition: all 0.2s;
        }
        .social-icon:hover {
            color: #fff;
            border-color: var(--accent-blue);
            background: var(--accent-blue);
            transform: translateY(-3px);
        }

        /* --- Footer --- */
        footer {
            text-align: center;
            padding: 40px 0;
            border-top: 1px solid var(--border-color);
            color: var(--text-muted);
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <div class="container">
        
        <!-- HEADER -->
        <header>
            <div class="avatar-frame">
                <div class="avatar"></div>
            </div>
            <h1>Pranay V</h1>
            <div class="subtitle">Hardware + Software Developer — VLSI Honours, SVCE</div>
            <div class="tagline">Building AI-powered Products from Idea to Deployment</div>
            
            <div class="stats-bar">
                <div class="stat-item"><span class="stat-label">Internships</span> <span class="stat-value">3</span></div>
                <div class="stat-item"><span class="stat-label">Hackathon Wins</span> <span class="stat-value">10+</span></div>
                <div class="stat-item"><span class="stat-label">Patents Filed</span> <span class="stat-value">2</span></div>
                <div class="stat-item"><span class="stat-label">Live in Prod</span> <span class="stat-value">2</span></div>
            </div>

            <div class="social-links">
                <a href="#" class="social-icon" title="GitHub">GH</a>
                <a href="#" class="social-icon" title="LinkedIn">IN</a>
                <a href="#" class="social-icon" title="Email">✉</a
