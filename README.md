<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Your Name] - Penetration Tester | Cybersecurity Professional</title>
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;600&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #0a0c0f 0%, #1a1e24 100%);
            color: #e1e4e8;
            line-height: 1.6;
            min-height: 100vh;
            padding: 2rem 1rem;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(22, 27, 34, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 24px;
            padding: 2rem;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
            border: 1px solid rgba(48, 54, 61, 0.5);
        }

        /* Header Section */
        .header {
            text-align: center;
            margin-bottom: 3rem;
            padding-bottom: 2rem;
            border-bottom: 1px solid #30363d;
        }

        .header h1 {
            font-size: 2.5rem;
            font-weight: 600;
            background: linear-gradient(135deg, #58a6ff, #7ee3ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 0.5rem;
        }

        .header h1 i {
            -webkit-text-fill-color: initial;
            color: #58a6ff;
            margin-right: 10px;
        }

        .subtitle {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin: 1.5rem 0;
        }

        .subtitle span {
            font-size: 1.1rem;
            padding: 0.5rem 1rem;
            background: rgba(48, 54, 61, 0.5);
            border-radius: 50px;
            border: 1px solid #30363d;
        }

        .subtitle i {
            margin-right: 8px;
            color: #7ee3ff;
        }

        .typing-text {
            font-family: 'Fira Code', monospace;
            font-size: 1.2rem;
            color: #7ee3ff;
            margin-top: 1rem;
        }

        /* About Section */
        .section {
            margin-bottom: 3rem;
        }

        .section-title {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 1.5rem;
            padding-left: 1rem;
            border-left: 4px solid #7ee3ff;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .section-title i {
            color: #7ee3ff;
        }

        .about-text {
            background: rgba(13, 17, 23, 0.7);
            padding: 1.5rem;
            border-radius: 12px;
            border: 1px solid #30363d;
        }

        .focus-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
            margin-top: 1.5rem;
        }

        .focus-item {
            display: flex;
            align-items: center;
            gap: 10px;
            padding: 1rem;
            background: rgba(22, 27, 34, 0.8);
            border-radius: 8px;
            border: 1px solid #30363d;
            transition: all 0.3s ease;
        }

        .focus-item:hover {
            transform: translateY(-2px);
            border-color: #7ee3ff;
            box-shadow: 0 5px 15px rgba(126, 227, 255, 0.1);
        }

        .focus-item i {
            color: #7ee3ff;
            font-size: 1.2rem;
        }

        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .skill-category {
            background: rgba(13, 17, 23, 0.7);
            padding: 1.5rem;
            border-radius: 12px;
            border: 1px solid #30363d;
        }

        .skill-category h3 {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 1rem;
            color: #7ee3ff;
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .skill-tag {
            background: rgba(48, 54, 61, 0.5);
            padding: 0.3rem 1rem;
            border-radius: 50px;
            font-size: 0.9rem;
            border: 1px solid #30363d;
            transition: all 0.3s ease;
        }

        .skill-tag:hover {
            background: #7ee3ff;
            color: #0a0c0f;
            border-color: #7ee3ff;
        }

        /* Projects */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .project-card {
            background: rgba(13, 17, 23, 0.7);
            border-radius: 12px;
            padding: 1.5rem;
            border: 1px solid #30363d;
            transition: all 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-5px);
            border-color: #7ee3ff;
            box-shadow: 0 10px 30px rgba(126, 227, 255, 0.15);
        }

        .project-card h3 {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 0.5rem;
            color: #58a6ff;
        }

        .project-desc {
            color: #8b949e;
            font-size: 0.95rem;
            margin: 1rem 0;
        }

        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .tech-tag {
            background: rgba(126, 227, 255, 0.1);
            color: #7ee3ff;
            padding: 0.2rem 0.8rem;
            border-radius: 50px;
            font-size: 0.8rem;
            border: 1px solid rgba(126, 227, 255, 0.3);
        }

        /* GitHub Stats */
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-bottom: 1.5rem;
        }

        .stat-card {
            background: rgba(13, 17, 23, 0.7);
            padding: 1.5rem;
            border-radius: 12px;
            border: 1px solid #30363d;
            text-align: center;
        }

        .stat-card img {
            max-width: 100%;
            border-radius: 8px;
        }

        .streak-stat {
            grid-column: 1 / -1;
            text-align: center;
            background: rgba(13, 17, 23, 0.7);
            padding: 1.5rem;
            border-radius: 12px;
            border: 1px solid #30363d;
        }

        /* Certifications */
        .certs-list {
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .cert-item {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 1rem;
            background: rgba(13, 17, 23, 0.7);
            border-radius: 8px;
            border: 1px solid #30363d;
        }

        .cert-item i {
            color: #f1c40f;
            font-size: 1.5rem;
        }

        .cert-info h4 {
            color: #58a6ff;
            margin-bottom: 0.2rem;
        }

        .cert-info p {
            color: #8b949e;
            font-size: 0.9rem;
        }

        /* Connect Section */
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
            flex-wrap: wrap;
            margin: 2rem 0;
        }

        .social-link {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 0.8rem 1.5rem;
            background: rgba(13, 17, 23, 0.7);
            border: 1px solid #30363d;
            border-radius: 8px;
            color: #e1e4e8;
            text-decoration: none;
            transition: all 0.3s ease;
        }

        .social-link:hover {
            background: #7ee3ff;
            color: #0a0c0f;
            transform: translateY(-2px);
        }

        .social-link:hover i {
            color: #0a0c0f;
        }

        .social-link i {
            font-size: 1.2rem;
            transition: all 0.3s ease;
        }

        /* Footer */
        .footer {
            margin-top: 3rem;
            padding-top: 2rem;
            border-top: 1px solid #30363d;
            text-align: center;
        }

        .warning {
            display: inline-block;
            padding: 0.5rem 1.5rem;
            background: rgba(255, 193, 7, 0.1);
            border: 1px solid #ffc107;
            border-radius: 50px;
            color: #ffc107;
            font-size: 0.9rem;
        }

        .warning i {
            margin-right: 8px;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .container {
                padding: 1rem;
            }

            .header h1 {
                font-size: 2rem;
            }

            .subtitle span {
                font-size: 0.9rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <header class="header">
            <h1>
                <i class="fas fa-shield-hal"></i>
                Hi, I'm [Your Name]
            </h1>
            <div class="subtitle">
                <span><i class="fas fa-bug"></i> Penetration Tester</span>
                <span><i class="fas fa-globe"></i> Web App Security Researcher</span>
                <span><i class="fas fa-shield"></i> Cyber Security Enthusiast</span>
            </div>
            <div class="typing-text">
                <i class="fas fa-terminal"></i>
                I break things to make them secure.
            </div>
        </header>

        <!-- About Me -->
        <section class="section">
            <h2 class="section-title">
                <i class="fas fa-user-secret"></i>
                About Me
            </h2>
            <div class="about-text">
                <p>I'm a passionate <strong>Cyber Security learner</strong> with a strong focus on <strong>Web Application Penetration Testing</strong>. I enjoy breaking things ethically to help organizations build more secure applications. I'm constantly learning and applying real-world exploitation techniques to understand how attackers think and how to stop them.</p>
                
                <div class="focus-grid">
                    <div class="focus-item">
                        <i class="fas fa-search"></i>
                        <span>Manual Web App Testing</span>
                    </div>
                    <div class="focus-item">
                        <i class="fas fa-flask"></i>
                        <span>OWASP Top 10 Deep Dive</span>
                    </div>
                    <div class="focus-item">
                        <i class="fas fa-bug"></i>
                        <span>Bug Bounty Methodology</span>
                    </div>
                    <div class="focus-item">
                        <i class="fas fa-robot"></i>
                        <span>Automation with Python</span>
                    </div>
                    <div class="focus-item">
                        <i class="fas fa-lock"></i>
                        <span>Secure Coding Practices</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Technical Skills -->
        <section class="section">
            <h2 class="section-title">
                <i class="fas fa-tools"></i>
                Technical Arsenal
            </h2>
            
            <div class="skills-grid">
                <div class="skill-category">
                    <h3><i class="fas fa-bug"></i> Web App Security</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">SQL Injection</span>
                        <span class="skill-tag">XSS</span>
                        <span class="skill-tag">CSRF</span>
                        <span class="skill-tag">IDOR</span>
                        <span class="skill-tag">File Upload</span>
                        <span class="skill-tag">Auth Bypass</span>
                    </div>
                </div>

                <div class="skill-category">
                    <h3><i class="fas fa-microchip"></i> Tools & Platforms</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Burp Suite</span>
                        <span class="skill-tag">OWASP ZAP</span>
                        <span class="skill-tag">Nmap</span>
                        <span class="skill-tag">Metasploit</span>
                        <span class="skill-tag">SQLmap</span>
                        <span class="skill-tag">Wireshark</span>
                        <span class="skill-tag">Kali Linux</span>
                    </div>
                </div>

                <div class="skill-category">
                    <h3><i class="fas fa-code"></i> Programming</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Python</span>
                        <span class="skill-tag">Bash</span>
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">Linux CLI</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Featured Projects -->
        <section class="section">
            <h2 class="section-title">
                <i class="fas fa-code-branch"></i>
                Featured Projects
            </h2>

            <div class="projects-grid">
                <div class="project-card">
                    <h3><i class="fas fa-spider"></i> Web Vulnerability Scanner</h3>
                    <p class="project-desc">A Python-based scanner to detect common web vulnerabilities like XSS, SQLi, and Open Redirects.</p>
                    <div class="project-tech">
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">Requests</span>
                        <span class="tech-tag">BeautifulSoup</span>
                    </div>
                </div>

                <div class="project-card">
                    <h3><i class="fas fa-database"></i> XSS Payload Collection</h3>
                    <p class="project-desc">A curated list of XSS payloads for testing and bypassing filters in modern web apps.</p>
                    <div class="project-tech">
                        <span class="tech-tag">JavaScript</span>
                        <span class="tech-tag">HTML</span>
                    </div>
                </div>

                <div class="project-card">
                    <h3><i class="fas fa-robot"></i> Bug Bounty Automation</h3>
                    <p class="project-desc">Bash & Python scripts to automate recon and scanning during bug bounty hunting.</p>
                    <div class="project-tech">
                        <span class="tech-tag">Bash</span>
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">Subfinder</span>
                    </div>
                </div>

                <div class="project-card">
                    <h3><i class="fas fa-flask"></i> OWASP Top 10 Lab</h3>
                    <p class="project-desc">Hands-on labs covering each OWASP Top 10 vulnerability with exploitation and mitigation steps.</p>
                    <div class="project-tech">
                        <span class="tech-tag">Docker</span>
                        <span class="tech-tag">WebGoat</span>
                        <span class="tech-tag">DVWA</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- GitHub Stats -->
        <section class="section">
            <h2 class="section-title">
                <i class="fab fa-github"></i>
                GitHub Stats
            </h2>

            <div class="stats-container">
                <div class="stat-card">
                    <img src="https://github-readme-stats.vercel.app/api?username=yourusername&show_icons=true&theme=radical" alt="GitHub Stats">
                </div>
                <div class="stat-card">
                    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=yourusername&layout=compact&theme=radical" alt="Top Languages">
                </div>
            </div>
            <div class="streak-stat">
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=yourusername&theme=radical" alt="GitHub Streak">
            </div>
        </section>

        <!-- Certifications -->
        <section class="section">
            <h2 class="section-title">
                <i class="fas fa-certificate"></i>
                Certifications & Achievements
            </h2>

            <div class="certs-list">
                <div class="cert-item">
                    <i class="fas fa-certificate"></i>
                    <div class="cert-info">
                        <h4>eJPT (Junior Penetration Tester)</h4>
                        <p>In Progress</p>
                    </div>
                </div>
                <div class="cert-item">
                    <i class="fas fa-trophy"></i>
                    <div class="cert-info">
                        <h4>TryHackMe</h4>
                        <p>Top 5% | Completed Web Fundamentals, OWASP Top 10</p>
                    </div>
                </div>
                <div class="cert-item">
                    <i class="fas fa-flag"></i>
                    <div class="cert-info">
                        <h4>HackTheBox</h4>
                        <p>Active Player | 10+ Machines Owned</p>
                    </div>
                </div>
                <div class="cert-item">
                    <i class="fas fa-shield"></i>
                    <div class="cert-info">
                        <h4>PortSwigger Web Security Academy</h4>
                        <p>Completed SQLi, XSS, and SSRF labs</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Connect -->
        <section class="section">
            <h2 class="section-title">
                <i class="fas fa-link"></i>
                Let's Connect
            </h2>

            <div class="social-links">
                <a href="#" class="social-link">
                    <i class="fab fa-linkedin"></i>
                    LinkedIn
                </a>
                <a href="#" class="social-link">
                    <i class="fas fa-envelope"></i>
                    Email
                </a>
                <a href="#" class="social-link">
                    <i class="fab fa-hackerone"></i>
                    HackerOne
                </a>
                <a href="#" class="social-link">
                    <i class="fas fa-bug"></i>
                    Bugcrowd
                </a>
            </div>
        </section>

        <!-- Footer -->
        <footer class="footer">
            <div class="warning">
                <i class="fas fa-exclamation-triangle"></i>
                Ethical Hacking Only | Responsible Disclosure
            </div>
            <p style="margin-top: 1rem; color: #8b949e; font-size: 0.9rem;">
                All my work is done with permission and intended for educational & defensive purposes only.
            </p>
        </footer>
    </div>

    <!-- Typing Animation Script (Optional) -->
    <script>
        // Optional: Add dynamic typing animation
        const texts = [
            "I break things to make them secure.",
            "Web App Security is my passion.",
            "Ethical Hacker | Security Researcher"
        ];
        let index = 0;
        let charIndex = 0;
        const typingElement = document.querySelector('.typing-text');

        function typeText() {
            if (charIndex < texts[index].length) {
                typingElement.innerHTML = '<i class="fas fa-terminal"></i> ' + texts[index].substring(0, charIndex + 1);
                charIndex++;
                setTimeout(typeText, 100);
            } else {
                setTimeout(eraseText, 2000);
            }
        }

        function eraseText() {
            if (charIndex > 0) {
                typingElement.innerHTML = '<i class="fas fa-terminal"></i> ' + texts[index].substring(0, charIndex - 1);
                charIndex--;
                setTimeout(eraseText, 50);
            } else {
                index = (index + 1) % texts.length;
                setTimeout(typeText, 500);
            }
        }

        // Start animation
        // typeText(); // Uncomment to enable typing animation
    </script>
</body>
</html>
