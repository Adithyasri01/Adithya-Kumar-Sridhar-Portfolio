# Adithya-Kumar-Sridhar-Portfolio

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Adithya Kumar Sridhar - MSc AI and Data Science | Data Analyst | Business Research | London, UK">
    <meta name="keywords" content="Data Analyst, AI, Machine Learning, Python, SQL, Power BI, London">
    <title>Adithya Kumar Sridhar | Data & AI Professional</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #1a365d;
            --secondary: #2c5282;
            --accent: #3182ce;
            --text: #2d3748;
            --text-light: #718096;
            --bg: #ffffff;
            --bg-alt: #f7fafc;
            --border: #e2e8f0;
            --success: #38a169;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
            color: var(--text);
            line-height: 1.6;
            background: var(--bg);
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid var(--border);
            z-index: 1000;
            padding: 1rem 0;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text);
            font-weight: 500;
            font-size: 0.9rem;
            transition: color 0.3s;
            position: relative;
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--accent);
            transition: width 0.3s;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .mobile-menu {
            display: none;
            flex-direction: column;
            gap: 4px;
            cursor: pointer;
        }

        .mobile-menu span {
            width: 25px;
            height: 2px;
            background: var(--primary);
            transition: 0.3s;
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding: 6rem 2rem 4rem;
            background: linear-gradient(135deg, var(--bg) 0%, var(--bg-alt) 100%);
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -10%;
            width: 600px;
            height: 600px;
            background: radial-gradient(circle, rgba(49, 130, 206, 0.08) 0%, transparent 70%);
            border-radius: 50%;
        }

        .hero-container {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        .hero-content h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3.5rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
            line-height: 1.2;
        }

        .hero-content .subtitle {
            font-size: 1.25rem;
            color: var(--secondary);
            font-weight: 500;
            margin-bottom: 1.5rem;
        }

        .hero-content .tagline {
            font-size: 1.1rem;
            color: var(--text-light);
            margin-bottom: 2rem;
            max-width: 500px;
        }

        .hero-stats {
            display: flex;
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .stat {
            text-align: center;
        }

        .stat-number {
            font-size: 2rem;
            font-weight: 700;
            color: var(--accent);
            display: block;
        }

        .stat-label {
            font-size: 0.85rem;
            color: var(--text-light);
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .cta-group {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
        }

        .btn {
            padding: 0.875rem 2rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            transition: all 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }

        .btn-primary {
            background: var(--primary);
            color: white;
            border: 2px solid var(--primary);
        }

        .btn-primary:hover {
            background: var(--secondary);
            border-color: var(--secondary);
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(26, 54, 93, 0.15);
        }

        .btn-secondary {
            background: transparent;
            color: var(--primary);
            border: 2px solid var(--primary);
        }

        .btn-secondary:hover {
            background: var(--primary);
            color: white;
        }

        .hero-visual {
            position: relative;
        }

        .profile-card {
            background: white;
            padding: 2rem;
            border-radius: 12px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
            border: 1px solid var(--border);
        }

        .profile-header {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1.5rem;
            padding-bottom: 1.5rem;
            border-bottom: 1px solid var(--border);
        }

        .profile-avatar {
            width: 80px;
            height: 80px;
            background: linear-gradient(135deg, var(--primary), var(--accent));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 2rem;
            font-weight: 700;
        }

        .profile-info h3 {
            font-size: 1.25rem;
            color: var(--primary);
            margin-bottom: 0.25rem;
        }

        .profile-info p {
            color: var(--text-light);
            font-size: 0.9rem;
        }

        .contact-details {
            space-y: 0.75rem;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            padding: 0.5rem 0;
            color: var(--text);
            font-size: 0.9rem;
        }

        .contact-icon {
            width: 20px;
            height: 20px;
            color: var(--accent);
        }

        .contact-item a {
            color: var(--text);
            text-decoration: none;
            transition: color 0.3s;
        }

        .contact-item a:hover {
            color: var(--accent);
        }

        /* Section Styles */
        section {
            padding: 5rem 2rem;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-header {
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-header h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .section-header p {
            color: var(--text-light);
            font-size: 1.1rem;
        }

        /* About Section */
        .about {
            background: var(--bg-alt);
        }

        .about-grid {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 3rem;
            align-items: start;
        }

        .about-content h3 {
            font-size: 1.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
            font-family: 'Playfair Display', serif;
        }

        .about-content p {
            margin-bottom: 1rem;
            color: var(--text);
            font-size: 1.05rem;
        }

        .highlight-box {
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            border-left: 4px solid var(--accent);
            margin-top: 1.5rem;
        }

        .highlight-box h4 {
            color: var(--primary);
            margin-bottom: 0.5rem;
            font-size: 1.1rem;
        }

        .status-badge {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            background: rgba(56, 161, 105, 0.1);
            color: var(--success);
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-top: 1rem;
        }

        .status-badge::before {
            content: '';
            width: 8px;
            height: 8px;
            background: var(--success);
            border-radius: 50%;
        }

        /* Profile Image Styles - NEW */
        .about-image {
            position: relative;
        }

        .profile-photo-container {
            position: relative;
            display: inline-block;
        }

        .profile-photo {
            width: 100%;
            max-width: 350px;
            height: auto;
            border-radius: 12px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
            border: 4px solid white;
            object-fit: cover;
            aspect-ratio: 3/4;
        }

        .profile-photo-frame {
            position: absolute;
            top: 20px;
            left: 20px;
            right: -20px;
            bottom: -20px;
            border: 3px solid var(--accent);
            border-radius: 12px;
            z-index: -1;
        }

        /* Skills Section */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .skill-category {
            background: white;
            padding: 2rem;
            border-radius: 12px;
            border: 1px solid var(--border);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .skill-category:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
        }

        .skill-category h3 {
            font-size: 1.25rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
            display: flex;
            align-items: center;
            gap: 0.75rem;
        }

        .skill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.75rem;
        }

        .skill-tag {
            background: var(--bg-alt);
            color: var(--text);
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
            border: 1px solid var(--border);
            transition: all 0.3s;
        }

        .skill-tag:hover {
            background: var(--primary);
            color: white;
            border-color: var(--primary);
        }

        /* Experience Section */
        .experience {
            background: var(--bg-alt);
        }

        .timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            width: 2px;
            height: 100%;
            background: var(--border);
        }

        .timeline-item {
            position: relative;
            margin-bottom: 3rem;
            width: 50%;
            padding: 0 2rem;
        }

        .timeline-item:nth-child(odd) {
            left: 0;
            text-align: right;
        }

        .timeline-item:nth-child(even) {
            left: 50%;
            text-align: left;
        }

        .timeline-dot {
            position: absolute;
            width: 16px;
            height: 16px;
            background: var(--accent);
            border: 3px solid white;
            border-radius: 50%;
            top: 0;
            box-shadow: 0 0 0 3px var(--accent);
        }

        .timeline-item:nth-child(odd) .timeline-dot {
            right: -8px;
        }

        .timeline-item:nth-child(even) .timeline-dot {
            left: -8px;
        }

        .timeline-content {
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            border: 1px solid var(--border);
            position: relative;
        }

        .timeline-date {
            font-size: 0.85rem;
            color: var(--accent);
            font-weight: 600;
            margin-bottom: 0.5rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .timeline-title {
            font-size: 1.25rem;
            color: var(--primary);
            margin-bottom: 0.25rem;
        }

        .timeline-company {
            color: var(--text-light);
            font-size: 0.95rem;
            margin-bottom: 1rem;
        }

        .timeline-content ul {
            list-style: none;
            font-size: 0.95rem;
        }

        .timeline-content li {
            margin-bottom: 0.5rem;
            position: relative;
            padding-left: 1rem;
        }

        .timeline-item:nth-child(odd) .timeline-content li {
            padding-left: 0;
            padding-right: 1rem;
        }

        .timeline-content li::before {
            content: '•';
            color: var(--accent);
            position: absolute;
            left: 0;
        }

        .timeline-item:nth-child(odd) .timeline-content li::before {
            left: auto;
            right: 0;
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid var(--border);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }

        .project-header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 1.5rem;
        }

        .project-category {
            font-size: 0.8rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            opacity: 0.9;
            margin-bottom: 0.5rem;
        }

        .project-title {
            font-size: 1.25rem;
            font-weight: 600;
            line-height: 1.3;
        }

        .project-body {
            padding: 1.5rem;
        }

        .project-description {
            color: var(--text);
            margin-bottom: 1rem;
            font-size: 0.95rem;
            line-height: 1.6;
        }

        .project-skills {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .project-skill {
            background: var(--bg-alt);
            color: var(--secondary);
            padding: 0.25rem 0.75rem;
            border-radius: 15px;
            font-size: 0.8rem;
            font-weight: 500;
        }

        /* Education Section */
        .education {
            background: var(--bg-alt);
        }

        .education-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .education-card {
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            border: 1px solid var(--border);
            border-left: 4px solid var(--accent);
            transition: transform 0.3s;
        }

        .education-card:hover {
            transform: translateX(5px);
        }

        .education-degree {
            font-size: 1.1rem;
            color: var(--primary);
            font-weight: 600;
            margin-bottom: 0.25rem;
        }

        .education-school {
            color: var(--text-light);
            font-size: 0.95rem;
            margin-bottom: 0.5rem;
        }

        .education-status {
            display: inline-block;
            background: var(--accent);
            color: white;
            padding: 0.25rem 0.75rem;
            border-radius: 15px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        .education-status.completed {
            background: var(--success);
        }

        /* Contact Section */
        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: start;
        }

        .contact-info h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.75rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .contact-info > p {
            color: var(--text-light);
            margin-bottom: 2rem;
        }

        .contact-methods {
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .contact-method {
            display: flex;
            align-items: center;
            gap: 1rem;
            padding: 1rem;
            background: var(--bg-alt);
            border-radius: 8px;
            text-decoration: none;
            color: var(--text);
            transition: all 0.3s;
            border: 1px solid transparent;
        }

        .contact-method:hover {
            border-color: var(--accent);
            transform: translateX(5px);
        }

        .contact-method-icon {
            width: 40px;
            height: 40px;
            background: var(--primary);
            color: white;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.25rem;
        }

        .contact-method-info h4 {
            font-size: 1rem;
            color: var(--primary);
            margin-bottom: 0.25rem;
        }

        .contact-method-info p {
            font-size: 0.9rem;
            color: var(--text-light);
        }

        .contact-form {
            background: white;
            padding: 2rem;
            border-radius: 12px;
            border: 1px solid var(--border);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            color: var(--primary);
            font-weight: 500;
            font-size: 0.9rem;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 0.75rem;
            border: 1px solid var(--border);
            border-radius: 6px;
            font-family: inherit;
            font-size: 1rem;
            transition: border-color 0.3s;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--accent);
        }

        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }

        /* Footer */
        footer {
            background: var(--primary);
            color: white;
            padding: 2rem;
            text-align: center;
        }

        footer p {
            opacity: 0.8;
            font-size: 0.9rem;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-bottom: 1rem;
        }

        .social-links a {
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
            transition: all 0.3s;
        }

        .social-links a:hover {
            background: var(--accent);
            transform: translateY(-3px);
        }

        /* Responsive */
        @media (max-width: 968px) {
            .hero-container {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero-content h1 {
                font-size: 2.5rem;
            }

            .hero-stats {
                justify-content: center;
            }

            .cta-group {
                justify-content: center;
            }

            .about-grid,
            .contact-grid {
                grid-template-columns: 1fr;
            }

            .about-image {
                order: -1;
                text-align: center;
                margin-bottom: 2rem;
            }

            .profile-photo {
                max-width: 280px;
            }

            .timeline::before {
                left: 20px;
            }

            .timeline-item {
                width: 100%;
                left: 0 !important;
                padding-left: 50px;
                text-align: left !important;
            }

            .timeline-dot {
                left: 12px !important;
                right: auto !important;
            }

            .timeline-item:nth-child(odd) .timeline-content li {
                padding-left: 1rem;
                padding-right: 0;
            }

            .timeline-content li::before {
                left: 0 !important;
                right: auto !important;
            }

            .nav-links {
                display: none;
            }

            .mobile-menu {
                display: flex;
            }
        }

        @media (max-width: 640px) {
            .hero-content h1 {
                font-size: 2rem;
            }

            .section-header h2 {
                font-size: 1.75rem;
            }

            .projects-grid {
                grid-template-columns: 1fr;
            }

            .profile-photo {
                max-width: 240px;
            }
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .animate {
            animation: fadeInUp 0.8s ease-out;
        }

        /* Print Styles */
        @media print {
            nav, .hero, .contact-form, footer {
                display: none;
            }

            section {
                padding: 2rem 0;
                page-break-inside: avoid;
            }
        }
    </style>
<base target="_blank">
</head>
<body>
    <!-- Navigation -->
    <nav>
        <div class="nav-container">
            <a href="#" class="logo">AKS</a>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#education">Education</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="mobile-menu">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-container">
            <div class="hero-content animate">
                <h1>Adithya Kumar Sridhar</h1>
                <p class="subtitle">MSc Artificial Intelligence and Data Science | Data Analyst | Business Research</p>
                <p class="tagline">Building intelligent applications with Machine Learning, NLP, and Data Analytics. Transforming complex datasets into actionable business insights.</p>

                <div class="hero-stats">
                    <div class="stat">
                        <span class="stat-number">4+</span>
                        <span class="stat-label">Years Experience</span>
                    </div>
                    <div class="stat">
                        <span class="stat-number">AI</span>
                        <span class="stat-label">Specialist</span>
                    </div>
                    <div class="stat">
                        <span class="stat-number">London</span>
                        <span class="stat-label">Based</span>
                    </div>
                </div>

                <div class="cta-group">
                    <a href="#contact" class="btn btn-primary">Get In Touch</a>
                    <a href="#projects" class="btn btn-secondary">View Projects</a>
                </div>
            </div>

            <div class="hero-visual animate">
                <div class="profile-card">
                    <div class="profile-header">
                        <div class="profile-avatar">AK</div>
                        <div class="profile-info">
                            <h3>Adithya Kumar Sridhar</h3>
                            <p>Available for Opportunities</p>
                        </div>
                    </div>
                    <div class="contact-details">
                        <div class="contact-item">
                            <svg class="contact-icon" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/>
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/>
                            </svg>
                            <span>London, United Kingdom</span>
                        </div>
                        <div class="contact-item">
                            <svg class="contact-icon" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/>
                            </svg>
                            <a href="mailto:adithyak.sri01@outlook.com">adithyak.sri01@outlook.com</a>
                        </div>
                        <div class="contact-item">
                            <svg class="contact-icon" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/>
                            </svg>
                            <a href="tel:+447799275840">+44 7799 275840</a>
                        </div>
                        <div class="contact-item">
                            <svg class="contact-icon" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
                            </svg>
                            <a href="https://www.linkedin.com/in/adithya-kumar-sridhar/" target="_blank">LinkedIn Profile</a>
                        </div>
                        <div class="contact-item">
                            <svg class="contact-icon" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
                            </svg>
                            <a href="https://github.com/Adithyasri01" target="_blank">GitHub Profile</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <div class="section-header">
                <h2>Professional Summary</h2>
                <p>Data Analyst and AI-focused professional with a passion for intelligent systems</p>
            </div>
            <div class="about-grid">
                <div class="about-content">
                    <h3>About Me</h3>
                    <p>Data Analyst and AI-focused professional with over <strong>4 years of experience</strong> in data insights, marketplace analysis, and business research. Currently pursuing an <strong>MSc in Data Science and Artificial Intelligence</strong> at the University of East London.</p>
                    <p>I possess strong expertise in <strong>Python, SQL, Power BI, machine learning</strong>, and stakeholder-driven analytics, with a proven ability to translate complex datasets into actionable business strategies.</p>
                    <p>My experience spans across data cleaning, feature engineering, exploratory data analysis (EDA), and building interactive dashboards that reduce manual reporting efforts by up to 40%.</p>

                    <div class="highlight-box">
                        <h4>Current Focus</h4>
                        <p>Specialising in Explainable AI (XAI), Large Language Models (LLMs), and medical image analysis using deep learning techniques. Passionate about ethical AI and transparent diagnostic systems.</p>
                    </div>

                    <span class="status-badge">Open to Data & AI Roles</span>
                </div>

                <!-- PROFILE PHOTO SECTION -->
                <div class="about-image">
                    <div class="profile-photo-container">
                        <img src="Adithya.jpeg" alt="Adithya Kumar Sridhar - Data Analyst & AI Professional" class="profile-photo">
                        <div class="profile-photo-frame"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills">
        <div class="container">
            <div class="section-header">
                <h2>Core Competencies</h2>
                <p>Technical expertise and professional capabilities</p>
            </div>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>
                        <svg width="24" height="24" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"/>
                        </svg>
                        Programming & Data
                    </h3>
                    <div class="skill-list">
                        <span class="skill-tag">Python</span>
                        <span class="skill-tag">SQL</span>
                        <span class="skill-tag">Pandas</span>
                        <span class="skill-tag">NumPy</span>
                        <span class="skill-tag">Data Cleaning</span>
                        <span class="skill-tag">Feature Engineering</span>
                        <span class="skill-tag">EDA</span>
                    </div>
                </div>

                <div class="skill-category">
                    <h3>
                        <svg width="24" height="24" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z"/>
                        </svg>
                        Analytics & BI
                    </h3>
                    <div class="skill-list">
                        <span class="skill-tag">Power BI</span>
                        <span class="skill-tag">Looker Studio</span>
                        <span class="skill-tag">Excel (Advanced)</span>
                        <span class="skill-tag">Dashboard Design</span>
                        <span class="skill-tag">KPI Development</span>
                        <span class="skill-tag">Data Visualization</span>
                    </div>
                </div>

                <div class="skill-category">
                    <h3>
                        <svg width="24" height="24" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z"/>
                        </svg>
                        Machine Learning
                    </h3>
                    <div class="skill-list">
                        <span class="skill-tag">Regression</span>
                        <span class="skill-tag">Classification</span>
                        <span class="skill-tag">Model Evaluation</span>
                        <span class="skill-tag">CNNs</span>
                        <span class="skill-tag">Explainable AI (XAI)</span>
                        <span class="skill-tag">Deep Learning</span>
                        <span class="skill-tag">Medical Image Analysis</span>
                    </div>
                </div>

                <div class="skill-category">
                    <h3>
                        <svg width="24" height="24" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 3.055A9.001 9.001 0 1020.945 13H11V3.055z"/>
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.488 9H15V3.512A9.025 9.025 0 0120.488 9z"/>
                        </svg>
                        Web & Marketing Analytics
                    </h3>
                    <div class="skill-list">
                        <span class="skill-tag">Google Analytics</span>
                        <span class="skill-tag">Google Tag Manager</span>
                        <span class="skill-tag">Market Analysis</span>
                        <span class="skill-tag">Competitor Analysis</span>
                        <span class="skill-tag">Forecasting</span>
                    </div>
                </div>

                <div class="skill-category">
                    <h3>
                        <svg width="24" height="24" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z"/>
                        </svg>
                        Professional Skills
                    </h3>
                    <div class="skill-list">
                        <span class="skill-tag">Stakeholder Communication</span>
                        <span class="skill-tag">Business Insight</span>
                        <span class="skill-tag">Problem Solving</span>
                        <span class="skill-tag">Cross-functional Collaboration</span>
                        <span class="skill-tag">Strategic Planning</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="experience">
        <div class="container">
            <div class="section-header">
                <h2>Professional Experience</h2>
                <p>Career progression and key achievements</p>
            </div>
            <div class="timeline">
                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <div class="timeline-date">Dec 2022 - July 2025</div>
                        <h3 class="timeline-title">Data Analyst / Business Research Analyst</h3>
                        <p class="timeline-company">CraftStudio</p>
                        <ul>
                            <li>Analysed large, multi-source datasets to identify trends, risks, and growth opportunities, supporting data-driven strategic decisions</li>
                            <li>Built interactive dashboards using Power BI and Excel, reducing manual reporting efforts by approximately 40%</li>
                            <li>Conducted market and competitor analysis using structured datasets, improving forecasting accuracy and business intelligence</li>
                            <li>Collaborated with cross-functional stakeholders to define KPIs, data requirements, and reporting standards</li>
                            <li>Applied SQL and Python-based analysis to clean, transform, and validate data for downstream analytics</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <div class="timeline-date">Feb 2018 - Dec 2022</div>
                        <h3 class="timeline-title">DVP, Special Quality Assurance</h3>
                        <p class="timeline-company">Kotak Mahindra Bank Ltd</p>
                        <ul>
                            <li>Led quality assurance initiatives ensuring compliance with regulatory standards</li>
                            <li>Developed data-driven quality metrics and reporting frameworks</li>
                            <li>Collaborated with cross-functional teams to improve operational efficiency</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <div class="timeline-date">Aug 2016 - Feb 2018</div>
                        <h3 class="timeline-title">Team Leader</h3>
                        <p class="timeline-company">BCAS Electrical Division</p>
                        <ul>
                            <li>Managed team operations and performance metrics</li>
                            <li>Implemented data-driven decision making processes</li>
                            <li>Enhanced operational workflows through analytical insights</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <div class="container">
            <div class="section-header">
                <h2>Featured Projects</h2>
                <p>Academic and personal projects demonstrating technical capabilities</p>
            </div>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-header">
                        <div class="project-category">Explainable AI / Healthcare</div>
                        <h3 class="project-title">Designing User-Centric Transparency in Cancer Detection Using Big Data</h3>
                    </div>
                    <div class="project-body">
                        <p class="project-description">
                            Built an Explainable AI framework for cancer detection using CNNs and large-scale medical imaging data. Integrated Grad-CAM, SHAP, and LIME to deliver transparent, clinician-friendly diagnostic explanations. Focused on ethical AI and responsible deployment in healthcare settings.
                        </p>
                        <div class="project-skills">
                            <span class="project-skill">Explainable AI (XAI)</span>
                            <span class="project-skill">Deep Learning (CNNs)</span>
                            <span class="project-skill">Medical Image Analysis</span>
                            <span class="project-skill">Big Data</span>
                            <span class="project-skill">Python</span>
                            <span class="project-skill">SHAP</span>
                            <span class="project-skill">LIME</span>
                            <span class="project-skill">Grad-CAM</span>
                        </div>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <div class="project-category">Business Analytics / ML</div>
                        <h3 class="project-title">Customer Purchase Behavior Dashboard with ML Insights</h3>
                    </div>
                    <div class="project-body">
                        <p class="project-description">
                            Built an end-to-end analytics solution to analyse customer transaction data and identify purchasing patterns. Performed data cleaning, EDA, and feature engineering using Python. Applied machine learning models to predict customer behavior and repeat purchase likelihood. Designed an interactive Power BI dashboard to visualize KPIs and customer segments.
                        </p>
                        <div class="project-skills">
                            <span class="project-skill">Python</span>
                            <span class="project-skill">SQL</span>
                            <span class="project-skill">Power BI</span>
                            <span class="project-skill">Machine Learning</span>
                            <span class="project-skill">Business Analytics</span>
                            <span class="project-skill">Customer Segmentation</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education" class="education">
        <div class="container">
            <div class="section-header">
                <h2>Education</h2>
                <p>Academic qualifications and continuous learning</p>
            </div>
            <div class="education-grid">
                <div class="education-card">
                    <div class="education-degree">MSc Artificial Intelligence and Data Science</div>
                    <div class="education-school">University of East London</div>
                    <span class="education-status">Currently Pursuing</span>
                </div>
                <div class="education-card">
                    <div class="education-degree">M.Tech – Power Electronics and Drives</div>
                    <div class="education-school">VIT University</div>
                    <span class="education-status completed">Completed 2016</span>
                </div>
                <div class="education-card">
                    <div class="education-degree">B.Tech – Electrical and Electronics Engineering</div>
                    <div class="education-school">SASTRA University</div>
                    <span class="education-status completed">Completed 2013</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <div class="section-header">
                <h2>Get In Touch</h2>
                <p>Let's discuss how I can contribute to your data and AI initiatives</p>
            </div>
            <div class="contact-grid">
                <div class="contact-info">
                    <h3>Contact Information</h3>
                    <p>I'm currently open to new opportunities in Data Analysis, Business Intelligence, and AI/ML roles in London and remote positions.</p>

                    <div class="contact-methods">
                        <a href="mailto:adithyak.sri01@outlook.com" class="contact-method">
                            <div class="contact-method-icon">✉</div>
                            <div class="contact-method-info">
                                <h4>Email</h4>
                                <p>adithyak.sri01@outlook.com</p>
                            </div>
                        </a>

                        <a href="tel:+447799275840" class="contact-method">
                            <div class="contact-method-icon">📞</div>
                            <div class="contact-method-info">
                                <h4>Phone</h4>
                                <p>+44 7799 275840</p>
                            </div>
                        </a>

                        <a href="https://www.linkedin.com/in/adithya-kumar-sridhar/" target="_blank" class="contact-method">
                            <div class="contact-method-icon">in</div>
                            <div class="contact-method-info">
                                <h4>LinkedIn</h4>
                                <p>linkedin.com/in/adithya-kumar-sridhar</p>
                            </div>
                        </a>

                        <div class="contact-method" style="cursor: default;">
                            <div class="contact-method-icon">📍</div>
                            <div class="contact-method-info">
                                <h4>Location</h4>
                                <p>London, United Kingdom</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="contact-form">
                    <form onsubmit="event.preventDefault(); alert('Thank you for your message! I will get back to you soon.');">
                        <div class="form-group">
                            <label for="name">Full Name</label>
                            <input type="text" id="name" name="name" required placeholder="Your name">
                        </div>
                        <div class="form-group">
                            <label for="email">Email Address</label>
                            <input type="email" id="email" name="email" required placeholder="your.email@example.com">
                        </div>
                        <div class="form-group">
                            <label for="subject">Subject</label>
                            <input type="text" id="subject" name="subject" required placeholder="Job Opportunity / Collaboration">
                        </div>
                        <div class="form-group">
                            <label for="message">Message</label>
                            <textarea id="message" name="message" required placeholder="Tell me about the opportunity..."></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary" style="width: 100%; justify-content: center;">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="social-links">
            <a href="https://www.linkedin.com/in/adithya-kumar-sridhar/" target="_blank" title="LinkedIn">in</a>
            <a href="#" target="_blank" title="GitHub">GH</a>
            <a href="mailto:adithyak.sri01@outlook.com" title="Email">@</a>
        </div>
        <p>&copy; 2025 Adithya Kumar Sridhar. All rights reserved.</p>
        <p style="margin-top: 0.5rem; font-size: 0.8rem;">Built with HTML, CSS & JavaScript</p>
    </footer>

    <script>
        // Smooth scroll for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add scroll animation
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        // Observe all cards and sections
        document.querySelectorAll('.skill-category, .project-card, .education-card, .timeline-content').forEach((el) => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'opacity 0.6s ease-out, transform 0.6s ease-out';
            observer.observe(el);
        });

        // Mobile menu toggle
        const mobileMenu = document.querySelector('.mobile-menu');
        const navLinks = document.querySelector('.nav-links');

        mobileMenu.addEventListener('click', () => {
            navLinks.style.display = navLinks.style.display === 'flex' ? 'none' : 'flex';
            navLinks.style.position = 'absolute';
            navLinks.style.top = '100%';
            navLinks.style.left = '0';
            navLinks.style.right = '0';
            navLinks.style.background = 'white';
            navLinks.style.flexDirection = 'column';
            navLinks.style.padding = '1rem';
            navLinks.style.boxShadow = '0 4px 6px rgba(0,0,0,0.1)';
        });

        // Active navigation highlighting
        const sections = document.querySelectorAll('section[id]');
        const navItems = document.querySelectorAll('.nav-links a');

        window.addEventListener('scroll', () => {
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                if (scrollY >= sectionTop - 200) {
                    current = section.getAttribute('id');
                }
            });

            navItems.forEach(item => {
                item.classList.remove('active');
                if (item.getAttribute('href') === `#${current}`) {
                    item.classList.add('active');
                }
            });
        });
    </script>
</body>
</html>
