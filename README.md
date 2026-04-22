<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dhaval Satasiya | Full Stack Developer</title>
    <style>
        :root {
            --bg-color: #ffffff;
            --text-color: #2c3e50;
            --card-bg: #f4f4f4;
            --accent-color: #3498db;
            --secondary-text: #555;
        }

        [data-theme="dark"] {
            --bg-color: #1a1a1a;
            --text-color: #ecf0f1;
            --card-bg: #2d2d2d;
            --accent-color: #5dade2;
            --secondary-text: #bdc3c7;
        }

        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            transition: all 0.3s ease;
            margin: 0;
            padding: 20px;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .header {
            margin-bottom: 40px;
        }

        .theme-toggle {
            cursor: pointer;
            padding: 10px 20px;
            border-radius: 20px;
            border: none;
            background: var(--accent-color);
            color: white;
            font-weight: bold;
            margin-bottom: 20px;
        }

        .card {
            background-color: var(--card-bg);
            padding: 25px;
            margin: 20px auto;
            border-radius: 15px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            text-align: left;
            transition: transform 0.2s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        h1, h2 { color: var(--accent-color); }
        
        p { line-height: 1.6; color: var(--secondary-text); }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 10px;
        }

        .skills span {
            background-color: var(--accent-color);
            color: white;
            padding: 8px 15px;
            border-radius: 25px;
            font-size: 0.9em;
            font-weight: bold;
        }

        .contact-btn {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 25px;
            background-color: var(--accent-color);
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
        }

        @media (max-width: 600px) {
            .card { width: 95%; padding: 15px; }
        }
    </style>
</head>
<body>

<div class="container">
    <button class="theme-toggle" onclick="toggleTheme()">🌓 Switch Theme</button>
    
    <div class="header">
        <h1>👋 Hi, I'm Dhaval Satasiya</h1>
        <p><b>💻 IT Student | 🚀 Future Full Stack Developer</b></p>
    </div>

    <div class="card">
        <h2>👨‍💻 About Me</h2>
        <p>🎓 IT Student passionate about Web Development.</p>
        <p>🏫 Learning at <b>Red & White Skill Education</b>.</p>
        <p>🎯 <b>Goal:</b> To become a Professional Full Stack Developer.</p>
    </div>

    <div class="card">
        <h2>🛠️ Skills</h2>
        <div class="skills">
            <span>HTML5</span>
            <span>CSS3</span>
            <span>JavaScript (Learning)</span>
            <span>PHP (Learning)</span>
            <span>MySQL (Learning)</span>
        </div>
    </div>

    <div class="card">
        <h2>🚀 Projects</h2>
        <p><b>🛺 Taxi Booking System</b> (Ongoing)</p>
        <p>Practicing database integration and advanced JavaScript logic.</p>
    </div>

    <div class="card">
        <h2>📫 Contact</h2>
        <p>Ready to collaborate or chat about tech!</p>
        <a href="mailto:dhavalsatasiya7@gmail.com" class="contact-btn">Email Me</a>
    </div>

    <p style="margin-top: 40px; opacity: 0.7;">⭐ Thanks for visiting my profile!</p>
</div>

<script>
    function toggleTheme() {
        const body = document.body;
        const currentTheme = body.getAttribute('data-theme');
        if (currentTheme === 'dark') {
            body.removeAttribute('data-theme');
        } else {
            body.setAttribute('data-theme', 'dark');
        }
    }
</script>

</body>
</html>
