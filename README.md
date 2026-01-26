<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MrKhan PRO Services</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap');

/* Body */
body {
    margin: 0;
    padding: 0;
    font-family: 'Orbitron', sans-serif;
    background: #0a0a0a;
    color: #fff;
    line-height: 1.6;
}

/* Container */
.container {
    max-width: 420px;
    margin: 20px auto;
    padding: 20px;
    background: linear-gradient(135deg, #111, #1a1a2e);
    border-radius: 15px;
    box-shadow: 0 0 20px rgba(0,0,0,0.7);
}

/* Hero Section */
h1 {
    text-align: center;
    color: #00ffff;
    text-shadow: 0 0 10px #00ffff;
    font-size: 22px;
    margin-bottom: 5px;
}

p.tagline {
    text-align: center;
    font-size: 14px;
    margin-bottom: 20px;
    color: #aaa;
}

/* Section Titles */
h2 {
    font-size: 18px;
    color: #ff00ff;
    margin-bottom: 10px;
    border-bottom: 1px solid #ff00ff;
    padding-bottom: 5px;
}

/* Services */
.services, .benefits, .testimonials {
    list-style: none;
    padding: 0;
    margin-bottom: 20px;
}

.services li, .benefits li, .testimonials li {
    margin-bottom: 10px;
    font-size: 14px;
}

/* CTA Buttons */
.btn {
    display: block;
    width: 90%;
    margin: 10px auto;
    padding: 12px;
    border-radius: 10px;
    background: linear-gradient(45deg, #00f, #ff0044);
    color: #fff;
    font-weight: bold;
    text-align: center;
    text-decoration: none;
    transition: all 0.3s ease;
}

.btn:hover {
    transform: scale(1.05);
    background: linear-gradient(45deg, #ff0044, #00ffff);
    color: #000;
}

/* Contact Form */
form {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-bottom: 15px;
}

form input, form textarea {
    padding: 10px;
    border-radius: 8px;
    border: none;
    outline: none;
    font-size: 14px;
}

form button {
    padding: 12px;
    border-radius: 10px;
    border: none;
    font-weight: bold;
    background: #00ffff;
    color: #000;
    cursor: pointer;
    transition: 0.3s;
}

form button:hover {
    background: #ff00ff;
    color: #fff;
}

/* Testimonials */
.testimonials {
    background: rgba(255,255,255,0.05);
    padding: 10px;
    border-radius: 10px;
}

/* Mobile Responsive */
@media only screen and (max-width: 500px) {
    h1 { font-size: 20px; }
    h2 { font-size: 16px; }
    .btn, form input, form textarea, form button { font-size: 13px; }
    .container { padding: 15px; }
}
</style>
</head>
<body>
<div class="container">
    <!-- Hero Section -->
    <h1>🚀 Boost Your Online Presence</h1>
    <p class="tagline">Professional Websites, Viral Videos & Branding by MrKhan</p>

    <!-- Services Section -->
    <h2>Services</h2>
    <ul class="services">
        <li>💻 Custom Websites & Bio-Link Pages</li>
        <li>🔐 Secure Firebase Login / Signup</li>
        <li>🎬 Viral Video Editing for Reels & YouTube</li>
        <li>🖼 Eye-Catching Thumbnails & Branding</li>
    </ul>

    <!-- Benefits Section -->
    <h2>Why Choose Me?</h2>
    <ul class="benefits">
        <li>✔ Get noticed online instantly</li>
        <li>✔ Professional & clean designs</li>
        <li>✔ Boost social engagement</li>
        <li>✔ Affordable & fast delivery</li>
    </ul>

    <!-- Testimonials Section -->
    <h2>Testimonials</h2>
    <ul class="testimonials">
        <li>“MrKhan ne meri website aur content banaya — results amazing the!” — Ahmed</li>
        <li>“Viral videos aur thumbnails ne meri social reach double kar di!” — Sana</li>
    </ul>

    <!-- CTA Buttons -->
    <a class="btn" href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank">Instagram</a>
    <a class="btn" href="https://www.facebook.com/share/184Khe9iZu/" target="_blank">Facebook</a>
    <a class="btn" href="mailto:nazimkhan01123@gmail.com">Email</a>

    <!-- Contact Form -->
    <h2>Contact Me</h2>
    <form>
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea placeholder="Your Message" rows="3" required></textarea>
        <button type="submit">Send Message</button>
    </form>

</div>
</body>
</html>
