<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eric Data Service | Cheap Data & Airtime</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>

    <header>
        <nav class="navbar">
            <div class="logo">Eric<span>Data</span></div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a href="login.html" class="btn-login">Login</a></li>
                <li><a href="register.html" class="btn-register">Register</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Reliable & Automated Data Services</h1>
            <p>Buy cheap data, airtime, and pay bills instantly. High-speed delivery 24/7.</p>
            <div class="hero-btns">
                <a href="register.html" class="btn-primary">Get Started</a>
                <a href="#pricing" class="btn-secondary">View Prices</a>
            </div>
        </div>
        <div class="hero-image">
            <img src="https://via.placeholder.com/500x400" alt="Data Service Illustration">
        </div>
    </section>

    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="service-grid">
            <div class="service-card">
                <i class="fas fa-mobile-alt"></i>
                <h3>Buy Data</h3>
                <p>Cheap SME & Gifting data for all networks.</p>
            </div>
            <div class="service-card">
                <i class="fas fa-phone"></i>
                <h3>Airtime Topup</h3>
                <p>Instant airtime recharge with discount.</p>
            </div>
            <div class="service-card">
                <i class="fas fa-tv"></i>
                <h3>Cable Sub</h3>
                <p>DSTV, GOTV, and Startimes subscriptions.</p>
            </div>
            <div class="service-card">
                <i class="fas fa-lightbulb"></i>
                <h3>Utility Bills</h3>
                <p>Pay electricity bills across all discos.</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Eric Data Service. All Rights Reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

:root {
    --primary-color: #2563eb;
    --secondary-color: #1e293b;
    --accent-color: #f59e0b;
    --bg-light: #f8fafc;
}

body {
    background-color: var(--bg-light);
    color: var(--secondary-color);
}

/* Navbar */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 10%;
    background: #fff;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

.logo {
    font-size: 24px;
    font-weight: bold;
    color: var(--primary-color);
}

.logo span { color: var(--secondary-color); }

.nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
    align-items: center;
}

.nav-links a {
    text-decoration: none;
    color: var(--secondary-color);
    font-weight: 500;
}

.btn-register {
    background: var(--primary-color);
    color: #fff !important;
    padding: 10px 20px;
    border-radius: 5px;
}

/* Hero Section */
.hero {
    display: flex;
    align-items: center;
    padding: 80px 10%;
    background: linear-gradient(135deg, #fff 0%, #e0e7ff 100%);
}

.hero-content h1 {
    font-size: 48px;
    margin-bottom: 20px;
    line-height: 1.2;
}

.hero-btns {
    margin-top: 30px;
    display: flex;
    gap: 15px;
}

.btn-primary {
    background: var(--primary-color);
    color: white;
    padding: 15px 30px;
    text-decoration: none;
    border-radius: 5px;
}

/* Services */
.services {
    padding: 60px 10%;
    text-align: center;
}

.service-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    margin-top: 40px;
}

.service-card {
    background: #fff;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
    transition: transform 0.3s;
}

.service-card:hover { transform: translateY(-10px); }

.service-card i {
    font-size: 40px;
    color: var(--primary-color);
    margin-bottom: 15px;
}

footer {
    text-align: center;
    padding: 40px;
    background: var(--secondary-color);
    color: white;
}
