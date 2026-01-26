<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MrKhan PRO Services</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap');

body {
    margin: 0;
    padding: 0;
    font-family: 'Orbitron', sans-serif;
    background: #0a0a0a;
    color: #fff;
    line-height: 1.6;
    scroll-behavior: smooth;
}

.container {
    max-width: 450px;
    margin: 20px auto;
    padding: 20px;
    background: linear-gradient(135deg, #111, #1a1a2e);
    border-radius: 15px;
    box-shadow: 0 0 20px rgba(0,0,0,0.7);
}

/* Hero */
h1 {
    text-align: center;
    color: #00ffff;
    text-shadow: 0 0 10px #00ffff;
    font-size: 22px;
    margin-bottom: 5px;
    animation: fadeIn 1s forwards;
}
p.tagline {
    text-align: center;
    font-size: 14px;
    margin-bottom: 20px;
    color: #aaa;
    animation: fadeIn 1.5s forwards;
}
@keyframes fadeIn { to { opacity:1; } }

/* Section Titles */
h2 {
    font-size: 18px;
    color: #ff00ff;
    margin-bottom: 10px;
    border-bottom: 1px solid #ff00ff;
    padding-bottom: 5px;
}

/* Services */
.services, .benefits, .portfolio, .testimonials, .faq {
    list-style: none;
    padding: 0;
    margin-bottom: 20px;
}
.services li, .benefits li, .portfolio li, .faq li {
    margin-bottom: 10px;
    font-size: 14px;
    transition: transform 0.3s, color 0.3s;
}
.services li:hover, .portfolio li:hover { transform: scale(1.05); color: #00ffff; }

/* Testimonials Slider */
.testimonials { position: relative; overflow: hidden; height: 100px; }
.testimonials ul { display: flex; padding: 0; margin: 0; animation: slide 40s linear infinite; }
.testimonials li { flex: 0 0 100%; list-style: none; padding: 10px; box-sizing: border-box; }

/* Benefits */
.benefits li { margin-bottom: 8px; font-size: 14px; }

/* Portfolio */
.portfolio li {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: rgba(255,255,255,0.05);
    padding: 8px;
    border-radius: 8px;
}

/* FAQ */
.faq li { cursor: pointer; background: rgba(255,255,255,0.05); padding: 8px; border-radius: 8px; }
.faq li span.answer { display: none; margin-top: 5px; font-size: 13px; color: #aaa; }

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
.btn:hover { transform: scale(1.05); background: linear-gradient(45deg, #ff0044, #00ffff); color: #000; }

/* Contact Form */
form { display: flex; flex-direction: column; gap: 10px; margin-bottom: 15px; }
form input, form textarea { padding: 10px; border-radius: 8px; border: none; outline: none; font-size: 14px; }
form button { padding: 12px; border-radius: 10px; border: none; font-weight: bold; background: #00ffff; color: #000; cursor: pointer; transition: 0.3s; }
form button:hover { background: #ff00ff; color: #fff; }

/* Floating Email Button */
.floating-email {
    position: fixed; bottom: 20px; right: 20px;
    background: #ff0044; color: #fff; padding: 15px;
    border-radius: 50%; text-align: center; font-size: 20px;
    z-index: 1000; text-decoration: none;
}

/* Animations */
@keyframes slide { 0% { transform: translateX(0); } 100% { transform: translateX(-100%); } }

/* Responsive */
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

<!-- Hero -->
<h1>🚀 Boost Your Online Presence</h1>
<p class="tagline">Websites, Videos & Branding by MrKhan</p>

<!-- Services -->
<h2>Services</h2>
<ul class="services">
<li>💻 Custom Websites & Bio-Link Pages</li>
<li>🔐 Secure Firebase Login / Signup</li>
<li>🎬 Viral Video Editing</li>
<li>🖼 Eye-Catching Thumbnails & Branding</li>
</ul>

<!-- Benefits -->
<h2>Why Choose Me?</h2>
<ul class="benefits">
<li>✔ Professional & Clean Designs</li>
<li>✔ Boost Social Engagement</li>
<li>✔ Fast Delivery & Affordable</li>
<li>✔ Mobile-Friendly & Modern</li>
</ul>

<!-- Portfolio -->
<h2>Portfolio</h2>
<ul class="portfolio">
<li>Website Example 1 🌐</li>
<li>Thumbnail Example 🎨</li>
<li>Viral Video Sample 🎬</li>
<li>Brand Logo Sample 🖌️</li>
</ul>

<!-- Testimonials Slider -->
<h2>Testimonials</h2>
<div class="testimonials">
<ul>
<li>“Amazing website & videos!” — Ahmed</li>
<li>“Social reach doubled!” — Sana</li>
<li>“Fast delivery & professional!” — Ali</li>
<li>“Creative thumbnails, great work!” — Zara</li>
<li>“Very affordable & clean design!” — Bilal</li>
<li>“Loved the content quality!” — Fatima</li>
<li>“Best video editing ever!” — Hamza</li>
<li>“Highly recommend MrKhan!” — Aisha</li>
<li>“Super fast & responsive!” — Omar</li>
<li>“Engagement increased after posts!” — Hina</li>
<li>“Great branding & logo!” — Sara</li>
<li>“Excellent work ethic!” — Kamran</li>
<li>“Professional & friendly!” — Mehreen</li>
<li>“Boosted my social media!” — Usman</li>
<li>“Very creative & unique!” — Noor</li>
<li>“Reliable & fast delivery!” — Danish</li>
<li>“Loved the thumbnails & videos!” — Maryam</li>
<li>“Awesome work & attention to detail!” — Imran</li>
<li>“Highly skilled & professional!” — Sana</li>
<li>“Amazing support & guidance!” — Ahmed</li>
</ul>
</div>

<!-- FAQ -->
<h2>FAQ</h2>
<ul class="faq">
<li onclick="toggleAnswer(this)">Delivery Time? <span class="answer">Usually 1–3 days depending on complexity.</span></li>
<li onclick="toggleAnswer(this)">Revisions? <span class="answer">Yes, free revisions until satisfaction.</span></li>
<li onclick="toggleAnswer(this)">Do you handle social media content? <span class="answer">Yes, Reels, Shorts & thumbnails included.</span></li>
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

<!-- Floating Email Button -->
<a href="mailto:nazimkhan01123@gmail.com" class="floating-email" target="_blank">📧</a>

<script>
function toggleAnswer(element){
    let ans = element.querySelector(".answer");
    ans.style.display = (ans.style.display === "block") ? "none" : "block";
}
</script>
</body>
</html>
