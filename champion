<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ernest Addai | Tech Business Solutions</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Orbitron:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #00b4d8;
            --secondary: #0077b6;
            --dark: #03045e;
            --light: #caf0f8;
            --accent: #ff6b6b;
            --card-bg: rgba(255, 255, 255, 0.1);
            --text: #333;
            --text-light: #f8f9fa;
        }

        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: var(--text);
            background-color: #0a192f;
            overflow-x: hidden;
            position: relative;
        }

        /* Animated background */
        .background-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            overflow: hidden;
        }

        .circle {
            position: absolute;
            border-radius: 50%;
            background: rgba(0, 180, 216, 0.1);
            animation: float 6s ease-in-out infinite;
        }

        .circle:nth-child(1) {
            width: 80px;
            height: 80px;
            top: 10%;
            left: 10%;
            animation-delay: 0s;
        }

        .circle:nth-child(2) {
            width: 100px;
            height: 100px;
            top: 60%;
            left: 80%;
            animation-delay: 2s;
        }

        .circle:nth-child(3) {
            width: 120px;
            height: 120px;
            top: 20%;
            left: 85%;
            animation-delay: 4s;
        }

        .circle:nth-child(4) {
            width: 60px;
            height: 60px;
            top: 70%;
            left: 15%;
            animation-delay: 1s;
        }

        @keyframes float {
            0%, 100% {
                transform: translateY(0) translateX(0);
            }
            50% {
                transform: translateY(-20px) translateX(10px);
            }
        }

        /* Header */
        header {
            padding: 1.5rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: rgba(10, 25, 47, 0.9);
            backdrop-filter: blur(10px);
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.2);
        }

        .logo {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
            display: flex;
            align-items: center;
        }

        .logo i {
            margin-right: 10px;
            color: var(--accent);
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            color: var(--text-light);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
            font-size: 1.1rem;
        }

        nav ul li a:hover {
            color: var(--primary);
        }

        /* Hero Section */
        .hero {
            padding: 6rem 5% 4rem;
            text-align: center;
            color: var(--text-light);
            max-width: 1200px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            font-family: 'Orbitron', sans-serif;
        }

        .hero h1 span {
            color: var(--primary);
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
            color: #b0b8c5;
        }

        /* Services Section */
        .section-title {
            text-align: center;
            color: var(--text-light);
            font-size: 2.5rem;
            margin-bottom: 3rem;
            font-family: 'Orbitron', sans-serif;
        }

        .section-title span {
            color: var(--primary);
        }

        .services {
            padding: 5rem 5%;
            max-width: 1400px;
            margin: 0 auto;
        }

        .cards-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }

        .card {
            background: var(--card-bg);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            overflow: hidden;
            padding: 2rem;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            transition: transform 0.4s, box-shadow 0.4s;
            border: 1px solid rgba(255, 255, 255, 0.1);
            color: var(--text-light);
        }

        .card:hover {
            transform: translateY(-15px);
            box-shadow: 0 15px 40px rgba(0, 180, 216, 0.2);
            border-color: var(--primary);
        }

        .card-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
        }

        .card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: white;
        }

        .card p {
            color: #b0b8c5;
            margin-bottom: 1.5rem;
        }

        .card-btn {
            display: inline-block;
            background: linear-gradient(to right, var(--primary), var(--secondary));
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
        }

        .card-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(0, 180, 216, 0.4);
        }

        /* WhatsApp Button */
        .whatsapp-btn {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: #25D366;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            box-shadow: 0 5px 20px rgba(37, 211, 102, 0.5);
            z-index: 1000;
            text-decoration: none;
            transition: all 0.3s;
        }

        .whatsapp-btn:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 25px rgba(37, 211, 102, 0.7);
        }

        /* Footer */
        footer {
            background-color: rgba(5, 15, 30, 0.95);
            color: var(--text-light);
            padding: 4rem 5% 2rem;
            margin-top: 4rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .footer-column h3 {
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
            color: var(--primary);
            font-family: 'Orbitron', sans-serif;
        }

        .footer-column p {
            color: #b0b8c5;
            margin-bottom: 1rem;
        }

        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
        }

        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            font-size: 1.2rem;
            transition: all 0.3s;
        }

        .social-links a:hover {
            background-color: var(--primary);
            transform: translateY(-5px);
        }

        .copyright {
            text-align: center;
            padding-top: 3rem;
            margin-top: 3rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #b0b8c5;
            font-size: 0.9rem;
        }

        .copyright span {
            color: var(--primary);
            font-weight: 600;
        }

        /* Responsive */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                padding: 1rem 5%;
            }
            
            .logo {
                margin-bottom: 1rem;
            }
            
            nav ul {
                flex-wrap: wrap;
                justify-content: center;
            }
            
            nav ul li {
                margin: 0.5rem 1rem;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .section-title {
                font-size: 2rem;
            }
            
            .cards-container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Animated Background -->
    <div class="background-animation">
        <div class="circle"></div>
        <div class="circle"></div>
        <div class="circle"></div>
        <div class="circle"></div>
    </div>

    <!-- Header -->
    <header>
        <div class="logo">
            <i class="fas fa-robot"></i>
            <span>Ernest Addai Tech</span>
        </div>
        <nav>
            <ul>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <h1>Tech Solutions for <span>Modern Businesses</span></h1>
        <p>Providing cutting-edge technology services including WhatsApp bots, Heroku hosting, account management, billing systems, and more to streamline your business operations.</p>
        <a href="#contact" class="card-btn">Get In Touch</a>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <h2 class="section-title">Our <span>Services</span></h2>
        <div class="cards-container">
            <!-- WhatsApp Bot Card -->
            <div class="card">
                <div class="card-icon">
                    <i class="fab fa-whatsapp"></i>
                </div>
                <h3>WhatsApp Business Bot</h3>
                <p>Custom WhatsApp bots for automated customer service, order processing, notifications, and marketing campaigns. Increase efficiency and customer engagement.</p>
                <a href="#" class="card-btn">Learn More</a>
            </div>

            <!-- Heroku Account Card -->
            <div class="card">
                <div class="card-icon">
                    <i class="fas fa-cloud"></i>
                </div>
                <h3>Heroku Account Setup & Management</h3>
                <p>Full Heroku account setup, configuration, deployment, and ongoing management for your applications. We handle the technical details so you can focus on your business.</p>
                <a href="#" class="card-btn">Get Started</a>
            </div>

            <!-- Billing Solutions Card -->
            <div class="card">
                <div class="card-icon">
                    <i class="fas fa-credit-card"></i>
                </div>
                <h3>Billing & Payment Solutions</h3>
                <p>Secure and reliable billing systems integrated with payment gateways. Automate invoices, subscriptions, and payment processing for your business.</p>
                <a href="#" class="card-btn">View Plans</a>
            </div>

            <!-- Tech Consultation Card -->
            <div class="card">
                <div class="card-icon">
                    <i class="fas fa-laptop-code"></i>
                </div>
                <h3>Tech Consultation</h3>
                <p>Expert advice on technology stack, infrastructure, automation, and digital transformation strategies tailored to your business needs.</p>
                <a href="#" class="card-btn">Consult Now</a>
            </div>

            <!-- Account Management Card -->
            <div class="card">
                <div class="card-icon">
                    <i class="fas fa-user-cog"></i>
                </div>
                <h3>Account Management</h3>
                <p>Comprehensive management of your digital accounts, services, and subscriptions to ensure optimal performance and cost-efficiency.</p>
                <a href="#" class="card-btn">Manage Accounts</a>
            </div>

            <!-- Custom Solutions Card -->
            <div class="card">
                <div class="card-icon">
                    <i class="fas fa-cogs"></i>
                </div>
                <h3>Custom Tech Solutions</h3>
                <p>Bespoke software and automation solutions designed specifically for your business requirements and workflow.</p>
                <a href="#" class="card-btn">Build Solution</a>
            </div>
        </div>
    </section>

    <!-- WhatsApp Floating Button -->
    <a href="https://wa.me/1234567890?text=Hi%20Ernest,%20I'm%20interested%20in%20your%20tech%20services" class="whatsapp-btn" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Footer -->
    <footer id="contact">
        <div class="footer-content">
            <div class="footer-column">
                <h3>Ernest Addai Tech</h3>
                <p>Providing cutting-edge technology solutions for modern businesses. Specializing in WhatsApp bots, cloud hosting, billing systems, and account management.</p>
                <div class="social-links">
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-linkedin-in"></i></a>
                    <a href="#"><i class="fab fa-github"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                </div>
            </div>
            
            <div class="footer-column">
                <h3>Quick Links</h3>
                <p><a href="#services" style="color: #b0b8c5; text-decoration: none;">Services</a></p>
                <p><a href="#" style="color: #b0b8c5; text-decoration: none;">Portfolio</a></p>
                <p><a href="#" style="color: #b0b8c5; text-decoration: none;">Testimonials</a></p>
                <p><a href="#" style="color: #b0b8c5; text-decoration: none;">Blog</a></p>
            </div>
            
            <div class="footer-column">
                <h3>Contact Info</h3>
                <p><i class="fas fa-map-marker-alt" style="color: var(--primary); margin-right: 10px;"></i> Accra, Ghana</p>
                <p><i class="fas fa-phone" style="color: var(--primary); margin-right: 10px;"></i> +233 123 456 789</p>
                <p><i class="fas fa-envelope" style="color: var(--primary); margin-right: 10px;"></i> ernest@addai-tech.com</p>
                <p><i class="fab fa-whatsapp" style="color: var(--primary); margin-right: 10px;"></i> WhatsApp: +233 123 456 789</p>
            </div>
        </div>
        
        <div class="copyright">
            <p>&copy; <span id="currentYear"></span> <span>Ernest Addai</span> Tech Solutions. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Set current year in footer
        document.getElementById('currentYear').textContent = new Date().getFullYear();
        
        // Add smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Add hover effect to cards on load
        document.addEventListener('DOMContentLoaded', function() {
            const cards = document.querySelectorAll('.card');
            cards.forEach((card, index) => {
                // Add slight delay to each card for staggered effect
                card.style.animationDelay = `${index * 0.1}s`;
            });
        });
    </script>
</body>
</html>
