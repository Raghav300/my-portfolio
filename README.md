my-portfolio
!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cyber Security Portfolio</title>
    <style>
        /* Global Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: #0b0f19;
            color: #e2e8f0;
            line-height: 1.6;
        }
        a {
            text-decoration: none;
            color: inherit;
        }

        /* Navigation Bar */
        nav {
            background: #111827;
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #1f2937;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .logo {
            font-size: 1.2rem;
            font-weight: bold;
            color: #38bdf8;
        }
        .nav-links {
            list-style: none;
            display: flex;
            gap: 2rem;
        }
        .nav-links a:hover {
            color: #38bdf8;
        }

        /* Hero Section */
        .hero {
            padding: 6rem 5%;
            text-align: center;
            background: radial-gradient(circle at center, #1e293b 0%, #0b0f19 70%);
        }
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #f8fafc;
        }
        .hero h1 span {
            color: #38bdf8;
        }
        .hero p {
            font-size: 1.1rem;
            color: #94a3b8;
            max-width: 600px;
            margin: 0 auto 2rem auto;
        }
        .btn {
            display: inline-block;
            background: #0284c7;
            color: white;
            padding: 0.75rem 1.5rem;
            border-radius: 5px;
            font-weight: bold;
            transition: 0.3s;
        }
        .btn:hover {
            background: #0369a1;
        }

        /* Sections General */
        section {
            padding: 4rem 5%;
            border-bottom: 1px solid #1f2937;
        }
        section h2 {
            font-size: 2rem;
            margin-bottom: 2rem;
            text-align: center;
            color: #38bdf8;
        }

        /* About & Skills Grid */
        .about-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }
        .skill-card {
            background: #111827;
            padding: 1.5rem;
            border-radius: 8px;
            border: 1px solid #1f2937;
            text-align: center;
        }

        /* Projects Grid */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }
        .project-card {
            background: #111827;
            border: 1px solid #1f2937;
            border-radius: 8px;
            padding: 1.5rem;
        }
        .project-card h3 {
            color: #f8fafc;
            margin-bottom: 0.5rem;
        }
        .project-card p {
            color: #94a3b8;
            font-size: 0.95rem;
            margin-bottom: 1rem;
        }

        /* Contact Form */
        form {
            max-width: 600px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }
        input, textarea {
            width: 100%;
            padding: 0.75rem;
            background: #111827;
            border: 1px solid #374151;
            border-radius: 5px;
            color: white;
        }
        input:focus, textarea:focus {
            outline: none;
            border-color: #38bdf8;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            color: #64748b;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav>
        <div class="logo">./portfolio</div>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#projects">Projects & Write-ups</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h1>Hi, I'm <span>Cyber Security Enthusiast</span></h1>
        <p>BCA Final-Year Student | Focusing on Network Security, Penetration Testing, and OSINT.</p>
        <a href="#projects" class="btn">Explore My Work</a>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Me & Skills</h2>
        <div class="about-content">
            <p>I am passionate about information security, ethical hacking, and exploring system vulnerabilities. Constantly learning and solving labs on platforms like TryHackMe and HackTheBox.</p>
            
            <div class="skills-grid">
                <div class="skill-card">
                    <h3>PenTesting</h3>
                    <p>Nmap, Wireshark, Metasploit, Burp Suite</p>
                </div>
                <div class="skill-card">
                    <h3>OSINT & Tools</h3>
                    <p>Sherlock, theHarvester, Maltego, Python</p>
                </div>
                <div class="skill-card">
                    <h3>OS & Networking</h3>
                    <p>Kali Linux, Windows, TCP/IP, Linux Admin</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2>Projects & CTF Write-ups</h2>
        <div class="projects-grid">
            <div class="project-card">
                <h3>Python Port Scanner</h3>
                <p>A custom network port scanner built in Python using socket programming to identify open ports on a target IP.</p>
                <a href="#" style="color: #38bdf8; font-weight: bold;">View on GitHub →</a>
            </div>
            <div class="project-card">
                <h3>CTF Write-up: Machine X</h3>
                <p>Step-by-step documentation of exploiting web vulnerabilities and privilege escalation on a lab machine.</p>
                <a href="#" style="color: #38bdf8; font-weight: bold;">Read Write-up →</a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Get In Touch</h2>
        <form action="https://formspree.io/f/your-form-id" method="POST">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
            <button type="submit" class="btn">Send Message</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Portfolio. Built with HTML & CSS.</p>
    </footer>

</body>
</html>
