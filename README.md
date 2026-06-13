<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Soumen Giri | Software Developer</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        /* CSS Reset & Variables */
        :root {
            --primary-color: #2563eb;
            --secondary-color: #1e40af;
            --bg-color: #f8fafc;
            --text-color: #334155;
            --heading-color: #0f172a;
            --card-bg: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        /* Container */
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Navbar */
        nav {
            background-color: var(--card-bg);
            padding: 20px 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        nav .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav .logo {
            font-size: 24px;
            font-weight: 700;
            color: var(--heading-color);
        }

        nav .logo span {
            color: var(--primary-color);
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 600;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: var(--primary-color);
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 100px 0;
            background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
        }

        .hero h1 {
            font-size: 48px;
            color: var(--heading-color);
            margin-bottom: 10px;
        }

        .hero h2 {
            font-size: 24px;
            color: var(--primary-color);
            font-weight: 400;
            margin-bottom: 20px;
        }

        .hero p {
            max-width: 600px;
            margin: 0 auto 30px;
            font-size: 18px;
        }

        .btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: #fff;
            padding: 12px 28px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: background 0.3s, transform 0.2s;
        }

        .btn:hover {
            background-color: var(--secondary-color);
            transform: translateY(-3px);
        }

        /* Sections General */
        section {
            padding: 80px 0;
        }

        .section-title {
            text-align: center;
            font-size: 32px;
            color: var(--heading-color);
            margin-bottom: 40px;
        }

        /* Skills Section */
        .skills-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
        }

        .skill-badge {
            background-color: var(--card-bg);
            padding: 10px 20px;
            border-radius: 20px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            font-weight: 600;
            color: var(--heading-color);
            border: 1px solid #e2e8f0;
            transition: transform 0.3s;
        }

        .skill-badge:hover {
            transform: translateY(-5px);
            border-color: var(--primary-color);
            color: var(--primary-color);
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
        }

        .project-card {
            background-color: var(--card-bg);
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s, box-shadow 0.3s;
            border-top: 4px solid var(--primary-color);
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }

        .project-card h3 {
            font-size: 22px;
            color: var(--heading-color);
            margin-bottom: 10px;
        }

        .project-card .tech-stack {
            font-size: 14px;
            color: var(--primary-color);
            font-weight: 600;
            margin-bottom: 15px;
        }

        .project-card p {
            font-size: 15px;
            margin-bottom: 20px;
        }

        .project-card ul {
            list-style-position: inside;
            font-size: 14px;
            color: var(--text-color);
        }

        /* Footer */
        footer {
            background-color: var(--heading-color);
            color: #fff;
            text-align: center;
            padding: 40px 0;
        }

        footer .social-icons {
            margin-bottom: 20px;
        }

        footer .social-icons a {
            color: #fff;
            font-size: 24px;
            margin: 0 10px;
            transition: color 0.3s;
        }

        footer .social-icons a:hover {
            color: var(--primary-color);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero h1 { font-size: 36px; }
            .hero h2 { font-size: 20px; }
            nav ul { display: none; } /* Hide menu on mobile for simplicity */
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav>
        <div class="container">
            <div class="logo">Soumen<span>.Dev</span></div>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="hero" id="about">
        <div class="container">
            <h1>Hi 👋, I'm Soumen Giri</h1>
            <h2>MCA Student | Aspiring Software Developer</h2>
            <p>I am a passionate Computer Applications student specializing in Backend Development and building scalable, robust web applications using Java, Spring Boot, and modern web technologies.</p>
            <a href="#projects" class="btn">View My Work</a>
        </div>
    </header>

    <!-- Skills Section -->
    <section id="skills" class="container">
        <h2 class="section-title">Technical Skills</h2>
        <div class="skills-grid">
            <div class="skill-badge"><i class="fa-brands fa-java"></i> Java</div>
            <div class="skill-badge"><i class="fa-solid fa-leaf"></i> Spring Boot</div>
            <div class="skill-badge"><i class="fa-solid fa-database"></i> Hibernate / JPA</div>
            <div class="skill-badge"><i class="fa-solid fa-network-wired"></i> REST API</div>
            <div class="skill-badge"><i class="fa-solid fa-database"></i> MySQL</div>
            <div class="skill-badge"><i class="fa-brands fa-python"></i> Python</div>
            <div class="skill-badge"><i class="fa-brands fa-html5"></i> HTML5</div>
            <div class="skill-badge"><i class="fa-brands fa-css3-alt"></i> CSS3</div>
            <div class="skill-badge"><i class="fa-brands fa-bootstrap"></i> Bootstrap</div>
            <div class="skill-badge"><i class="fa-brands fa-js"></i> JavaScript</div>
            <div class="skill-badge"><i class="fa-brands fa-git-alt"></i> Git & GitHub</div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" style="background-color: #f1f5f9;">
        <div class="container">
            <h2 class="section-title">Featured Projects</h2>
            <div class="projects-grid">
                
                <!-- Project 1 -->
                <div class="project-card">
                    <h3>🎓 Education Employment System</h3>
                    <div class="tech-stack">Spring Boot • JPA • MySQL • JSP</div>
                    <p>A full-stack web application designed to connect students, job seekers, and administrators seamlessly.</p>
                    <ul>
                        <li>Secure User Registration & Login</li>
                        <li>Job Seeker Module & Admin Dashboard</li>
                        <li>Course & Job Management</li>
                    </ul>
                </div>

                <!-- Project 2 -->
                <div class="project-card">
                    <h3>🛒 NeoShop - E-Commerce</h3>
                    <div class="tech-stack">Spring MVC • Hibernate • HTML/CSS</div>
                    <p>A dynamic e-commerce platform built to provide a complete and intuitive online shopping experience.</p>
                    <ul>
                        <li>MVC Architecture implementation</li>
                        <li>Product & Shopping Cart Management</li>
                        <li>Secure Database Connectivity</li>
                    </ul>
                </div>

                <!-- Project 3 -->
                <div class="project-card">
                    <h3>🏫 Attendance Management</h3>
                    <div class="tech-stack">Core Java • Servlets • JSP • MySQL</div>
                    <p>A web-based attendance tracking system streamlining academic record-keeping and role management.</p>
                    <ul>
                        <li>Faculty & Student Modules</li>
                        <li>Daily Attendance Tracking</li>
                        <li>CRUD Operations with MySQL</li>
                    </ul>
                </div>

            </div>
        </div>
    </section>

    <!-- Footer / Contact -->
    <footer id="contact">
        <div class="container">
            <h2 style="margin-bottom: 20px;">Let's Connect</h2>
            <p style="margin-bottom: 20px; color: #cbd5e1;">Currently looking for new opportunities to learn and grow as a software developer.</p>
            <div class="social-icons">
                <a href="#" target="_blank"><i class="fa-brands fa-github"></i></a>
                <a href="#" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
                <a href="mailto:your.email@example.com"><i class="fa-solid fa-envelope"></i></a>
            </div>
            <p style="color: #94a3b8; font-size: 14px;">&copy; 2026 Soumen Giri. All rights reserved.</p>
        </div>
    </footer>

</body>
</html>
