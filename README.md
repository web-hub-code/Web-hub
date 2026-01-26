<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MrKhan PRO Services</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap');

/* Body & Background */
body {
    margin: 0;
    padding: 0;
    font-family: 'Orbitron', sans-serif;
    background: #000;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    overflow-x: hidden;
}

body::before {
    content: '';
    position: fixed;
    width: 100%;
    height: 100%;
    background: radial-gradient(circle, rgba(0,255,255,0.05) 0%, transparent 80%);
    animation: flicker 3s infinite;
    z-index: -1;
}

@keyframes flicker {
    0%,19%,21%,23%,25%,54%,56%,100% { opacity:0.05; }
    20%,22%,24%,55% { opacity:0.15; }
}

/* Container */
.container {
    background: linear-gradient(135deg, #0a0a0a, #1a1a2e);
    border-radius: 20px;
    padding: 25px 20px;
    text-align: center;
    max-width: 95%;
    width: 420px;
    box-shadow: 0 0 25px rgba(0,0,0,0.7);
    animation: glow 2s infinite alternate;
}

@keyframes glow {
    0% { box-shadow: 0 0 15px #00f, 0 0 25px #f00; }
    50% { box-shadow: 0 0 30px #00f, 0 0 50px #f00; }
    100% { box-shadow: 0 0 15px #00f, 0 0 25px #f00; }
}

/* Headline */
h1 {
    font-size: 24px;
    color: #00ffff;
    text-shadow: 0 0 8px #00ffff, 0 0 15px #ff00ff;
    margin-bottom: 10px;
    animation: neon 1.5s infinite alternate;
}

@keyframes neon {
    0% { text-shadow: 0 0 3px #00ffff, 0 0 8px #ff00ff; }
    50% { text-shadow: 0 0 12px #00ffff, 0 0 20px #ff00ff; }
    100% { text-shadow: 0 0 3px #00ffff, 0 0 8px #ff00ff; }
}

p {
    color: #fff;
    text-shadow: 0 0 4px #00f, 0 0 8px #f00;
    font-size: 14px;
    margin: 5px 0 15px 0;
}

/* Benefits Section */
.benefits {
    text-align: left;
    margin: 15px 0;
    padding: 0 10px;
}

.benefits li {
    margin: 8px 0;
    font-size: 14px;
}

/* Services Section */
.services {
    list-style: none;
    padding: 0;
    margin: 15px 0;
}

.services li {
    margin: 10px 0;
    font-size: 15px;
}

/* CTA Buttons */
.contact {
    margin-top: 20px;
}

.btn {
    display: block;
    width: 90%;
    margin: 10px auto;
    padding: 14px;
    border-radius: 12px;
    background: linear-gradient(45deg, #00f, #ff0044);
    color: #fff;
    font-weight: bold;
    font-size: 14px;
    text-decoration: none;
    text-shadow: 0 0 3px #fff;
    transition: all 0.3s ease;
    animation: pulse 2s infinite;
}

.btn:hover {
    transform: scale(1.05);
    background: linear-gradient(45deg, #ff0044, #00ffff);
    color: #000;
    text-shadow: 0 0 8px #fff;
}

@keyframes pulse {
    0% { box-shadow: 0 0 8px #00f, 0 0 15px #ff0044; }
    50% { box-shadow: 0 0 15px #00f, 0 0 30px #ff0044; }
    100% { box-shadow: 0 0 8px #00f, 0 0 15px #ff0044; }
}

/* Testimonials Section */
.testimonial {
    background: rgba(255,255,255,0.05);
    margin: 15px 0;
    padding: 10px;
    border-radius: 10px;
    font-size: 13px;
    color: #fff;
    text-shadow: 0 0 3px #00f, 0 0 5px #f00;
}

/* Note */
.note {
    margin-top: 15px;
    font-size: 12px;
    color: #aaa;
    text-shadow: 0 0 4px #f00;
}

/* Responsive adjustments */
@media only screen and (max-width: 500px) {
    h1 { font-size: 20px; }
    p, .services li, .benefits li { font-size: 13px; }
    .btn { font-size: 13px; padding: 12px; }
    .container { padding: 20px 15px; }
}
</style>
</head>
<body>
<div class="container">
    <!-- Hero Section -->
    <h1>🚀 Boost Your Online Presence with MrKhan</h1>
    <p>Professional websites & viral content to make your brand shine!</p>
    
    <!-- Benefits Section -->
    <ul class="benefits">
        <li>✔ Get noticed online instantly</li>
        <li>✔ Save time with ready-to-use solutions</li>
        <li>✔ Engage your audience like never before</li>
    </ul>
    
    <!-- Services Section -->
    <ul class="services">
        <li>💻 Stunning Websites & Bio-Link Pages</li>
        <li>🔐 Secure Firebase Login / Signup</li>
        <li>🎬 Viral Video Editing for Reels & YouTube</li>
        <li>🖼 Eye-Catching Thumbnails & Branding</li>
    </ul>
    
    <!-- Testimonials Section -->
    <div class="testimonial">
        “MrKhan ne meri website aur content banaya — results amazing the!”  
        <br>— Ahmed, Small Business Owner
    </div>
    <div class="testimonial">
        “Viral videos aur thumbnails ne meri social reach double kar di!”  
        <br>— Sana, Content Creator
    </div>
    
    <!-- CTA Buttons -->
    <div class="contact">
        <a class="btn" href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank">Instagram</a>
        <a class="btn" href="https://www.facebook.com/share/184Khe9iZu/" target="_blank">Facebook</a>
        <a class="btn" href="mailto:nazimkhan01123@gmail.com">Email</a>
    </div>
    
    <!-- Note -->
    <p class="note">Fast Delivery • Low Budget • Scroll-Stopping Design • Premium Neon Style</p>
</div>
</body>
</html>
