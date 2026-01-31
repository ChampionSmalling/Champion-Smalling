<!DOCTYPE html
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechHub Solutions - Innovative Tech Services</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Orbitron:wght@500;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background-color: #0a0e17;
            color: #f0f0f0;
            overflow-x: hidden;
            position: relative;
        }
        
        /* Animated Background */
        #animated-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            opacity: 0.3;
        }
        
        .particle {
            position: absolute;
            background: rgba(0, 150, 255, 0.7);
            border-radius: 50%;
        }
        
        /* Header */
        header {
            padding: 20px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: rgba(10, 14, 23, 0.9);
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.3);
        }
        
        .logo {
            font-family: 'Orbitron', sans-serif;
            font-size: 28px;
            font-weight: 700;
            background: linear-gradient(90deg, #00c6ff, #0072ff);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav li {
            margin-left: 30px;
        }
        
        nav a {
            color: #f0f0f0;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
            font-size: 16px;
        }
        
        nav a:hover {
            color: #00c6ff;
        }
        
        /* Hero Section */
        .hero {
            padding: 100px 5%;
            text-align: center;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            font-family: 'Orbitron', sans-serif;
            background: linear-gradient(90deg, #00c6ff, #0072ff);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 40px;
            line-height: 1.6;
            color: #b0b0b0;
        }
        
        /* WhatsApp Button */
        .whatsapp-btn {
            display: inline-flex;
            align-items: center;
            background-color: #25D366;
            color: white;
            padding: 15px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 18px;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(37, 211, 102, 0.3);
        }
        
        .whatsapp-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(37, 211, 102, 0.4);
        }
        
        .whatsapp-btn i {
            margin-right: 10px;
            font-size: 24px;
        }
        
        /* Services Section */
        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 60px;
            font-family: 'Orbitron', sans-serif;
            color: #f0f0f0;
        }
        
        .services {
            padding: 80px 5%;
            max-width: 1400px;
            margin: 0 auto;
        }
        
        .cards-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }
        
        .card {
            background: rgba(20, 25, 40, 0.8);
            border-radius: 15px;
            overflow: hidden;
            transition: transform 0.4s, box-shadow 0.4s;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            border: 1px solid rgba(0, 150, 255, 0.1);
        }
        
        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 150, 255, 0.3);
        }
        
        .card-img {
            height: 200px;
            width: 100%;
            object-fit: cover;
        }
        
        .card-content {
            padding: 25px;
        }
        
        .card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: #00c6ff;
        }
        
        .card p {
            color: #b0b0b0;
            line-height: 1.6;
            margin-bottom: 20px;
        }
        
        .card-btn {
            display: inline-block;
            background: linear-gradient(90deg, #00c6ff, #0072ff);
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s;
        }
        
        .card-btn:hover {
            opacity: 0.9;
            transform: scale(1.05);
        }
        
        /* Call to Action */
        .cta {
            text-align: center;
            padding: 80px 5%;
            background: rgba(20, 25, 40, 0.5);
            margin: 60px 0;
            border-radius: 20px;
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .cta h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            font-family: 'Orbitron', sans-serif;
            color: #f0f0f0;
        }
        
        .cta p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 40px;
            color: #b0b0b0;
        }
        
        /* Footer */
        footer {
            background-color: rgba(10, 14, 23, 0.95);
            padding: 60px 5% 30px;
            margin-top: 80px;
            border-top: 1px solid rgba(0, 150, 255, 0.2);
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .footer-column h3 {
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: #00c6ff;
        }
        
        .footer-column p, .footer-column a {
            color: #b0b0b0;
            line-height: 1.8;
            text-decoration: none;
        }
        
        .footer-column a:hover {
            color: #00c6ff;
        }
        
        .social-icons {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-icons a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(0, 150, 255, 0.1);
            border-radius: 50%;
            color: #f0f0f0;
            transition: all 0.3s;
        }
        
        .social-icons a:hover {
            background-color: #00c6ff;
            transform: translateY(-3px);
        }
        
        .copyright {
            text-align: center;
            margin-top: 50px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #b0b0b0;
            font-size: 0.9rem;
        }
        
        .champion-footer {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.2rem;
            color: #00c6ff;
            text-align: center;
            margin-top: 10px;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                padding: 15px 5%;
            }
            
            nav ul {
                margin-top: 20px;
            }
            
            nav li {
                margin: 0 10px;
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
    <div id="animated-bg"></div>
    
    <!-- Header -->
    <header>
        <div class="logo">TechHub Solutions</div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- Hero Section -->
    <section class="hero" id="home">
        <h1>Innovative Tech Solutions For Modern Businesses</h1>
        <p>Providing cutting-edge technology services including WhatsApp bots, data bundles, gaming consoles, digital solutions, and more to help your business thrive in the digital age.</p>
        <a href="https://wa.me/1234567890?text=Hello%20TechHub%20Solutions%20I%20need%20your%20services" class="whatsapp-btn" target="_blank">
            <i class="fab fa-whatsapp"></i> Chat on WhatsApp
        </a>
    </section>
    
    <!-- Services Section -->
    <section class="services" id="services">
        <h2 class="section-title">Our Tech Services</h2>
        <div class="cards-container">
            <!-- WhatsApp Bot Card -->
            <div class="card">
                <img src="https://images.unsplash.com/photo-1611605698335-8b1569810432?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1074&q=80" alt="WhatsApp Bot" class="card-img">
                <div class="card-content">
                    <h3>WhatsApp Business Bots</h3>
                    <p>Automate customer service, sales, and support with our custom WhatsApp bots. Boost engagement and streamline communication.</p>
                    <a href="https://wa.me/1234567890?text=I'm%20interested%20in%20WhatsApp%20Bot%20services" class="card-btn" target="_blank">Get Quote</a>
                </div>
            </div>
            
            <!-- Data Bundle Card -->
            <div class="card">
                <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80" alt="Data Bundles" class="card-img">
                <div class="card-content">
                    <h3>Data Bundle Solutions</h3>
                    <p>Affordable and reliable data bundles for individuals and businesses. Stay connected with our fast and stable data services.</p>
                    <a href="https://wa.me/1234567890?text=I'm%20interested%20in%20Data%20Bundle%20services" class="card-btn" target="_blank">Order Now</a>
                </div>
            </div>
            
            <!-- PlayStation Console Card -->
            <div class="card">
                <img src="https://images.unsplash.com/photo-1606144042614-b2417e99c4e3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80" alt="PlayStation Console" class="card-img">
                <div class="card-content">
                    <h3>Gaming Consoles & Accessories</h3>
                    <p>Latest PlayStation consoles, games, and accessories. Enhance your gaming experience with premium products and support.</p>
                    <a href="https://wa.me/1234567890?text=I'm%20interested%20in%20PlayStation%20Console" class="card-btn" target="_blank">Shop Now</a>
                </div>
            </div>
            
            <!-- Male Outfits Card -->
            <div class="card">
                <img src="https://images.unsplash.com/photo-1490481651871-ab68de25d43d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80" alt="Male Outfits" class="card-img">
                <div class="card-content">
                    <h3>Premium Male Outfits</h3>
                    <p>Stylish and modern clothing for men. From casual wear to formal attire, we offer quality outfits for every occasion.</p>
                    <a href="https://wa.me/1234567890?text=I'm%20interested%20in%20Male%20Outfits" class="card-btn" target="_blank">View Collection</a>
                </div>
            </div>
            
            <!-- Tech Gadgets Card -->
            <div class="card">
                <img src="https://images.unsplash.com/photo-1517077304055-6e89abbf09b0?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1169&q=80" alt="Tech Gadgets" class="card-img">
                <div class="card-content">
                    <h3>Latest Tech Gadgets</h3>
                    <p>Cutting-edge technology gadgets and accessories. Stay ahead with our collection of innovative tech products.</p>
                    <a href="https://wa.me/1234567890?text=I'm%20interested%20in%20Tech%20Gadgets" class="card-btn" target="_blank">Explore</a>
                </div>
            </div>
            
            <!-- Picture Framing Card -->
            <div class="card">
                <img src="https://images.unsplash.com/photo-1513475382585-d06e58bcb0e0?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80" alt="Picture Framing" class="card-img">
                <div class="card-content">
                    <h3>Digital Picture Framing</h3>
                    <p>Transform your memories into art with our digital picture framing services. Custom designs for homes and offices.</p>
                    <a href="https://wa.me/1234567890?text=I'm%20interested%20in%20Picture%20Framing%20services" class="card-btn" target="_blank">Learn More</a>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Call to Action -->
    <section class="cta" id="about">
        <h2>Ready to Elevate Your Business?</h2>
        <p>We provide comprehensive tech solutions tailored to your needs. From digital automation to hardware solutions, we have everything to help your business succeed in today's digital landscape.</p>
        <a href="https://wa.me/1234567890?text=Hello%20TechHub%20Solutions%20I%20want%20to%20discuss%20business%20opportunities" class="whatsapp-btn" target="_blank">
            <i class="fab fa-whatsapp"></i> Start a Conversation
        </a>
    </section>
    
    <!-- Footer -->
    <footer id="contact">
        <div class="footer-content">
            <div class="footer-column">
                <h3>TechHub Solutions</h3>
                <p>Providing innovative tech solutions for modern businesses. We specialize in digital services, tech products, and business automation.</p>
                <div class="social-icons">
                    <a href="#"><i class="fab fa-facebook-f"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-linkedin-in"></i></a>
                </div>
            </div>
            
            <div class="footer-column">
                <h3>Our Services</h3>
                <a href="#">WhatsApp Business Bots</a><br>
                <a href="#">Data Bundle Solutions</a><br>
                <a href="#">Gaming Consoles</a><br>
                <a href="#">Tech Gadgets</a><br>
                <a href="#">Male Outfits</a><br>
                <a href="#">Digital Picture Framing</a>
            </div>
            
            <div class="footer-column">
                <h3>Contact Us</h3>
                <p><i class="fas fa-map-marker-alt"></i> 123 Tech Street, Digital City</p>
                <p><i class="fas fa-phone"></i> +1 234 567 8900</p>
                <p><i class="fas fa-envelope"></i> info@techhubsolutions.com</p>
                <p><i class="fab fa-whatsapp"></i> +1 234 567 8901</p>
            </div>
        </div>
        
        <div class="copyright">
            <p>&copy; 2023 TechHub Solutions. All rights reserved.</p>
            <div class="champion-footer">Champion Smalling - Innovating Tomorrow's Tech Today</div>
        </div>
    </footer>
    
    <script>
        // Create animated background particles
        function createParticles() {
            const bg = document.getElementById('animated-bg');
            const particleCount = 30;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                
                // Random size between 2px and 6px
                const size = Math.random() * 4 + 2;
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                
                // Random position
                particle.style.left = `${Math.random() * 100}%`;
                particle.style.top = `${Math.random() * 100}%`;
                
                // Random color with blue tint
                const blueShade = Math.floor(Math.random() * 155) + 100;
                particle.style.backgroundColor = `rgba(0, ${blueShade}, 255, 0.7)`;
                
                // Random animation
                const duration = Math.random() * 20 + 10;
                const delay = Math.random() * 5;
                particle.style.animation = `float ${duration}s ease-in-out ${delay}s infinite alternate`;
                
                bg.appendChild(particle);
            }
        }
        
        // Add floating animation to particles
        const style = document.createElement('style');
        style.textContent = `
            @keyframes float {
                0% {
                    transform: translate(0, 0) scale(1);
                    opacity: 0.7;
                }
                50% {
                    opacity: 1;
                }
                100% {
                    transform: translate(${Math.random() * 100 - 50}px, ${Math.random() * 100 - 50}px) scale(1.2);
                    opacity: 0.7;
                }
            }
        `;
        document.head.appendChild(style);
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetSection = document.querySelector(targetId);
                
                window.scrollTo({
                    top: targetSection.offsetTop - 80,
                    behavior: 'smooth'
                });
            });
        });
        
        // Add hover effect to cards
        document.querySelectorAll('.card').forEach(card => {
            card.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-10px)';
            });
            
            card.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0)';
            });
        });
        
        // Initialize when page loads
        window.addEventListener('DOMContentLoaded', () => {
            createParticles();
        });
    </script>
</body>
</html>
