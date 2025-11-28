<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aman Singh | Developer & Writer</title>
    <style>
        :root {
            --bg-color: #0a0a0a;
            --card-bg: rgba(255, 255, 255, 0.05);
            --accent: #00ff88;
            --accent-secondary: #00d4ff;
            --text-primary: #ffffff;
            --text-secondary: #a0a0a0;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        
        body {
            background-color: var(--bg-color);
            color: var(--text-primary);
            overflow-x: hidden;
        }

        /* Animated Background */
        .bg-orb {
            position: absolute;
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, var(--accent-secondary), transparent 70%);
            opacity: 0.1;
            border-radius: 50%;
            top: -100px;
            right: -100px;
            z-index: -1;
            filter: blur(60px);
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 2rem;
        }

        /* Header / Hero */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 2rem 0;
            margin-bottom: 4rem;
        }

        .logo { font-weight: 700; font-size: 1.5rem; letter-spacing: -1px; }
        .logo span { color: var(--accent); }

        .hero {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
            min-height: 60vh;
        }

        h1 {
            font-size: 3.5rem;
            line-height: 1.1;
            margin-bottom: 1rem;
            background: linear-gradient(to right, #fff, #a5a5a5);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .tagline {
            font-size: 1.2rem;
            color: var(--accent);
            margin-bottom: 1.5rem;
            font-family: 'Courier New', monospace;
        }

        .bio {
            color: var(--text-secondary);
            line-height: 1.6;
            margin-bottom: 2rem;
            font-size: 1.1rem;
        }

        /* Buttons */
        .btn-group { display: flex; gap: 1rem; }
        .btn {
            padding: 0.8rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        .btn-primary {
            background: var(--accent);
            color: #000;
            border: 1px solid var(--accent);
        }
        .btn-outline {
            border: 1px solid var(--text-secondary);
            color: var(--text-primary);
        }
        .btn:hover { transform: translateY(-2px); box-shadow: 0 5px 15px rgba(0, 255, 136, 0.2); }

        /* Stats Card */
        .stats-card {
            background: var(--card-bg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.1);
            padding: 2rem;
            border-radius: 15px;
            position: relative;
        }
        
        .stat-item { margin-bottom: 1rem; }
        .stat-label { color: var(--text-secondary); font-size: 0.9rem; }
        .stat-value { font-size: 1.2rem; font-weight: 600; }

        /* Tech Stack Grid */
        .section-title {
            font-size: 2rem;
            margin-bottom: 2rem;
            border-left: 4px solid var(--accent);
            padding-left: 1rem;
        }

        .stack-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-bottom: 4rem;
        }

        .stack-card {
            background: var(--card-bg);
            padding: 1.5rem;
            border-radius: 10px;
            border: 1px solid rgba(255,255,255,0.05);
            transition: 0.3s;
        }
        .stack-card:hover { border-color: var(--accent); }
        
        .stack-head { color: var(--accent-secondary); margin-bottom: 1rem; font-weight: bold; }
        .stack-list { display: flex; flex-wrap: wrap; gap: 0.5rem; }
        .tag {
            background: rgba(255,255,255,0.1);
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.85rem;
        }

        /* Footer */
        footer {
            border-top: 1px solid rgba(255,255,255,0.1);
            padding: 2rem 0;
            text-align: center;
            color: var(--text-secondary);
            margin-top: 4rem;
        }

        @media (max-width: 768px) {
            .hero { grid-template-columns: 1fr; text-align: center; }
            .btn-group { justify-content: center; }
            h1 { font-size: 2.5rem; }
        }
    </style>
</head>
<body>

    <div class="bg-orb"></div>

    <div class="container">
        <header>
            <div class="logo">Aman<span>.Dev</span></div>
            <a href="https://github.com/DataLunatic69" class="btn btn-outline" style="font-size: 0.9rem;">GitHub Profile</a>
        </header>

        <section class="hero">
            <div class="hero-content">
                <div class="tagline">&lt;Developer / Writer /&gt;</div>
                <h1>Building Decentralized Systems.</h1>
                <p class="bio">
                    Hi, I'm <strong>Aman</strong>. I bridge the gap between complex backend architecture and innovative healthcare solutions. Currently mastering System Design and crafting thriller stories in my downtime.
                </p>
                <div class="btn-group">
                    <a href="#contact" class="btn btn-primary">Contact Me</a>
                    <a href="https://ai-portfolio-rose.vercel.app/" class="btn btn-outline">View Portfolio</a>
                </div>
            </div>
            
            <div class="stats-card">
                <h3>🚀 Current Status</h3>
                <hr style="border: 0; border-top: 1px solid rgba(255,255,255,0.1); margin: 1rem 0;">
                <div class="stat-item">
                    <div class="stat-label">Working On</div>
                    <div class="stat-value">Decentralized Healthcare 🏥</div>
                </div>
                <div class="stat-item">
                    <div class="stat-label">Learning</div>
                    <div class="stat-value">DevOps & Multi-Agent Systems 🤖</div>
                </div>
                <div class="stat-item">
                    <div class="stat-label">Fun Fact</div>
                    <div class="stat-value">I write thriller novels 📚</div>
                </div>
            </div>
        </section>

        <h2 class="section-title">Tech Stack</h2>
        <div class="stack-grid">
            <div class="stack-card">
                <div class="stack-head">Languages</div>
                <div class="stack-list">
                    <span class="tag">JavaScript</span>
                    <span class="tag">TypeScript</span>
                    <span class="tag">Python</span>
                    <span class="tag">Go</span>
                    <span class="tag">C++</span>
                </div>
            </div>
            <div class="stack-card">
                <div class="stack-head">Frontend</div>
                <div class="stack-list">
                    <span class="tag">React</span>
                    <span class="tag">Next.js</span>
                    <span class="tag">Vue.js</span>
                    <span class="tag">Tailwind</span>
                </div>
            </div>
            <div class="stack-card">
                <div class="stack-head">Backend</div>
                <div class="stack-list">
                    <span class="tag">Node.js</span>
                    <span class="tag">Django</span>
                    <span class="tag">FastAPI</span>
                    <span class="tag">Spring Boot</span>
                </div>
            </div>
            <div class="stack-card">
                <div class="stack-head">DevOps & DB</div>
                <div class="stack-list">
                    <span class="tag">Docker</span>
                    <span class="tag">K8s</span>
                    <span class="tag">AWS</span>
                    <span class="tag">PostgreSQL</span>
                    <span class="tag">Redis</span>
                </div>
            </div>
        </div>

        <footer id="contact">
            <p>Connect with me: <a href="mailto:amansingh2002.ap@gmail.com" style="color: var(--accent);">amansingh2002.ap@gmail.com</a></p>
            <p style="margin-top: 1rem; font-size: 0.9rem;">
                <i>"Code is like humor. When you have to explain it, it's bad."</i>
            </p>
        </footer>
    </div>
</body>
</html>
