<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated GitHub README Demo</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            color: #24292e;
            background-color: #f6f8fa;
        }
        
        .markdown-body {
            background-color: white;
            padding: 30px;
            border-radius: 6px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.12);
        }
        
        .header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 30px;
        }
        
        h1 {
            border-bottom: 1px solid #eaecef;
            padding-bottom: 0.3em;
        }
        
        .badges {
            margin: 20px 0;
            display: flex;
            gap: 10px;
        }
        
        /* Animation examples */
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        @keyframes spin {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        .animated-icon {
            animation: bounce 2s infinite;
        }
        
        .spinning-icon {
            display: inline-block;
            animation: spin 4s linear infinite;
        }
        
        .terminal {
            background: #0f172a;
            color: #f8fafc;
            padding: 15px;
            border-radius: 6px;
            font-family: monospace;
            position: relative;
            overflow: hidden;
        }
        
        .terminal-cursor {
            display: inline-block;
            width: 10px;
            height: 20px;
            background: #f8fafc;
            vertical-align: middle;
            animation: blink 1s infinite;
        }
        
        @keyframes blink {
            50% { opacity: 0; }
        }
        
        .graph-container {
            height: 200px;
            margin: 30px 0;
            position: relative;
        }
        
        .graph-wave {
            position: absolute;
            bottom: 0;
            width: 100%;
            height: 100%;
            background: repeating-linear-gradient(
                to right,
                #1d4ed8,
                #1d4ed8 2px,
                transparent 2px,
                transparent 20px
            );
            animation: wave 4s linear infinite;
        }
        
        @keyframes wave {
            0% { transform: translateX(0); }
            100% { transform: translateX(-20px); }
        }
    </style>
</head>
<body>
    <div class="markdown-body">
        <div class="header">
            <h1>🚢 Belajar Docker - Petualangan Containerization! 🚢</h1>
            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/d8758c13-d97f-4a59-86ae-f35a9652ce1c.png" alt="Logo Docker" class="animated-icon">
        </div>
        
        <div class="badges">
            <img src="https://img.shields.io/badge/status-belajar-success" alt="Status Belajar">
            <img src="https://img.shields.io/badge/bahasa-indonesia-brightgreen" alt="Bahasa Indonesia">
            <img src="https://img.shields.io/badge/docker-%F0%9F%90%B3-blue" alt="Docker">
            <span class="spinning-icon">🐳</span>
        </div>
        
        <p>Halo! Ini adalah repo tempat aku belajar Docker dari dasar sampai mahir 💻</p>
        <p>Docker itu seperti kotak ajaib untuk aplikasi kita - sekali bungkus, jalan di mana saja! ✨</p>
        <p>Mari belajar bersama-sama!</p>
        
        <h2>📊 Usage Statistics</h2>
        <div class="graph-container">
            <div class="graph-wave"></div>
        </div>
        
        <h2>🛠 Installation</h2>
        <div class="terminal">
            $ npm install animated-readme<span class="terminal-cursor"></span>
        </div>
        
        <h2>🚀 Features</h2>
        <ul>
            <li>Animated badges and icons</li>
            <li>Interactive elements</li>
            <li>Terminal-like code blocks</li>
            <li>Visual statistics</li>
        </ul>
        
        <h2>📝 Notes</h2>
        <p>Note: Actual GitHub markdown has limitations:</p>
        <ol>
            <li>No JavaScript support</li>
            <li>Limited CSS animations</li>
            <li>Only certain HTML is rendered</li>
        </ol>
        
        <p>For true animation in GitHub READMEs:</p>
        <ul>
            <li>Use animated GIFs</li>
            <li>Include SVG with SMIL animation</li>
            <li>Utilize badge services (like shields.io)</li>
            <li>Add terminal recording GIFs</li>
        </ul>
    </div>
</body>
</html>

