<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Khan Studio | Premium Neon Digital Services</title>
<meta name="description" content="Khan Studio - Website Development, Video Editing, Branding, Thumbnails, SEO & Social Media Services. Neon premium modern interface.">
<meta name="keywords" content="digital services, website development, video editing, branding, thumbnails, neon, modern">
<meta name="author" content="Khan Studio">
<meta name="google-site-verification" content="google8073cfacc72a7cb3">

<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

<style>
/* Reset & Body */
*{margin:0;padding:0;box-sizing:border-box;font-family:'Roboto',sans-serif;}
body{background: linear-gradient(135deg,#0f0f0f,#120028,#1a0028,#000000); color:#fff; scroll-behavior:smooth; transition:0.5s;}

/* Neon Headings */
h1,h2,h3{font-weight:700;text-transform:uppercase;text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}
h2{color:#00ffff;text-align:center;margin-bottom:30px;position:relative;}
h2::after{content:"";width:60px;height:3px;background:#ff0040;display:block;margin:10px auto;border-radius:2px;}

/* Hero Section */
header{position:relative;height:70vh;overflow:hidden;display:flex;justify-content:center;align-items:center;text-align:center;}
header::before{content:"";position:absolute;top:0;left:0;width:100%;height:100%;background:radial-gradient(circle,rgba(255,0,64,0.2),rgba(0,64,255,0.2),rgba(0,0,0,0.8)); z-index:1;animation:moveBackground 30s linear infinite;}
header h1{position:relative;z-index:2;font-size:3em;animation:neonPulse 2s ease-in-out infinite;text-align:center;}
@keyframes neonPulse{
0%{text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}
50%{text-shadow:0 0 15px #ff0040,0 0 30px #0040ff,0 0 60px #ff0040;}
100%{text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}
}
@keyframes moveBackground{
0%{background-position:0 0;}
100%{background-position:1000px 1000px;}
}

/* Cards */
.card{background: rgba(255,255,255,0.05); padding:20px; border-radius:10px; flex:1 1 300px; text-align:left; transition:0.3s; box-shadow:0 0 10px rgba(0,255,255,0.3); margin-bottom:20px;}
.card:hover{transform:scale(1.03); box-shadow:0 0 20px #ff0040,0 0 40px #0040ff;}

/* Layouts */
.services,.portfolio,.stats-section,.reviews,.faq-section{display:flex;flex-wrap:wrap;gap:20px;justify-content:center;}

/* Buttons */
button{padding:15px;border:none;border-radius:5px;background:#ff0040;color:#fff;font-weight:bold;cursor:pointer;transition:0.3s;box-shadow:0 0 5px #00ffff;text-transform:uppercase;}
button:hover{background:#00ffff;color:#000;box-shadow:0 0 15px #ff0040,0 0 30px #00ffff;}

/* Form */
form{display:flex;flex-direction:column;gap:15px;max-width:500px;margin:auto;}
input,select,textarea{padding:10px;border-radius:5px;border:1px solid #ccc;background:#111;color:#fff;}
input::placeholder,textarea::placeholder{color:#888;}

/* Portfolio Review Photos */
.photo-circle{width:60px;height:60px;border-radius:50%;border:3px solid #00ffff;margin-right:10px;object-fit:cover;}

/* Footer */
footer{background: rgba(0,0,0,0.05); padding:30px 20px;text-align:center;color:#fff;}
footer a{color:#00ffff;text-decoration:none;}
footer a:hover{color:#ff0040;}

/* Back to top */
#topBtn{position:fixed;bottom:20px;right:20px;padding:10px 15px;background:#00ffff;color:#000;border:none;border-radius:5px;cursor:pointer;display:none;z-index:1000;transition:0.3s;}
#topBtn:hover{background:#ff0040;color:#fff;}

/* FAQ */
.faq-card{background: rgba(255,255,255,0.05); padding:15px; border-radius:10px; width:100%; cursor:pointer; box-shadow:0 0 10px rgba(0,255,255,0.3); margin-bottom:10px;}
.faq-card:hover{box-shadow:0 0 20px #ff0040,0 0 40px #0040ff;}
.faq-content{max-height:0;overflow:hidden;transition:max-height 0.3s ease;}
.faq-card.active .faq-content{max-height:300px;padding-top:10px;}

/* Responsive */
@media(max-width:768px){.services,.portfolio,.stats-section,.reviews,.faq-section{flex-direction:column;}header h1{font-size:2em;}}
</style>
</head>
<body>

<!-- Hero -->
<header>
<h1>Khan Studio</h1>
</header>

<!-- About -->
<section id="about">
<h2>About Khan Studio</h2>
<p style="text-align:left;">
Khan Studio is a **premium digital service provider** delivering Website Development, Video Editing, Branding, Thumbnails, SEO & Social Media services. Our **goal** is to give every client a **modern, professional, and neon-glowing digital experience**. We focus on speed, quality, innovation, and 100% client satisfaction.
</p>
</section>

<!-- Services -->
<section id="services">
<h2>Our Services</h2>
<div class="services">
<div class="card">
<h3>Website Development</h3>
<p>Responsive, fast, modern websites with custom UI/UX, e-commerce support, SEO optimization, and secure architecture for businesses, portfolios, and blogs.</p>
</div>
<div class="card">
<h3>Video Editing</h3>
<p>Professional edits including color grading, effects, transitions, intros/outros, subtitles, and YouTube/Reels/Ads videos.</p>
</div>
<div class="card">
<h3>Thumbnail & Graphics</h3>
<p>Eye-catching thumbnails, banners, logos, social media graphics to maximize engagement and brand recognition.</p>
</div>
<div class="card">
<h3>Branding & Marketing</h3>
<p>Complete branding solutions: logos, brand kits, social media identity, and marketing creatives to enhance digital presence.</p>
</div>
<div class="card">
<h3>SEO & Social Media</h3>
<p>Improve search engine visibility and social engagement with content optimization, SEO strategies, and social media management.</p>
</div>
</div>
</section>

<!-- Portfolio -->
<section id="portfolio">
<h2>Portfolio</h2>
<div class="portfolio">
<div class="card">
<h3>Website Projects</h3>
<p>Delivered multiple responsive websites with modern UI/UX, e-commerce, and blogs worldwide.</p>
</div>
<div class="card">
<h3>Video Projects</h3>
<p>Edited professional videos with effects, intros/outros, color grading, and motion graphics.</p>
</div>
<div class="card">
<h3>Graphics & Branding</h3>
<p>Created logos, thumbnails, banners, and full branding packages to establish client identity.</p>
</div>
</div>
</section>

<!-- Stats -->
<section id="stats">
<h2>Achievements</h2>
<div class="stats-section">
<div class="card"><h3>8000+</h3><p>Satisfied Clients Worldwide</p></div>
<div class="card"><h3>1200+</h3><p>Websites Delivered</p></div>
<div class="card"><h3>3500+</h3><p>Videos Edited</p></div>
<div class="card"><h3>1500+</h3><p>Thumbnails & Branding Delivered</p></div>
</div>
</section>

<!-- Testimonials / Reviews -->
<section id="reviews">
<h2>Client Reviews</h2>
<div class="reviews">
<div class="card" style="display:flex;align-items:center;">
<img src="https://picsum.photos/60/60?random=1" class="photo-circle" alt="Client Photo">
<div><p>"Amazing service, highly recommended!"</p><p>- Ali</p></div>
</div>
<div class="card" style="display:flex;align-items:center;">
<img src="https://picsum.photos/60/60?random=2" class="photo-circle" alt="Client Photo">
<div><p>"Creative video editing and website design. Truly premium services."</p><p>- Sara</p></div>
</div>
<div class="card" style="display:flex;align-items:center;">
<img src="https://picsum.photos/60/60?random=3" class="photo-circle" alt="Client Photo">
<div><p>"Fast delivery and professional work!"</p><p>- Hassan</p></div>
</div>
<!-- Add up to 20-25 reviews similarly -->
</div>
</section>

<!-- FAQ -->
<section id="faq">
<h2>FAQ</h2>
<div class="faq-section">
<div class="faq-card">
<h3>How can I order a service?</h3>
<div class="faq-content"><p>Fill the contact form below or reach out via email or social media links.</p></div>
</div>
<div class="faq-card">
<h3>How long does delivery take?</h3>
<div class="faq-content"><p>Delivery depends on service complexity. Usually 1-7 days.</p></div>
</div>
<div class="faq-card">
<h3>Do you provide revisions?</h3>
<div class="faq-content"><p>Yes, unlimited revisions until satisfaction.</p></div>
</div>
</div>
</section>

<!-- Contact -->
<section id="contact">
<h2>Contact Me</h2>
<form action="mailto:rock.earn92@gmail.com" method="post" enctype="text/plain">
<input type="text" name="Name" placeholder="Your Name" required>
<input type="email" name="Email" placeholder="Your Email" required>
<select name="Service">
<option>Website Development</option>
<option>Video Editing</option>
<option>Thumbnail & Graphics</option>
<option>Branding & Marketing</option>
<option>SEO & Social Media</option>
<option>Other</option>
</select>
<textarea name="Message" placeholder="Describe your project in detail" required></textarea>
<button type="submit">Send Message</button>
</form>
<p style="text-align:center;margin-top:15px;">
📧 <a href="mailto:rock.earn92@gmail.com">rock.earn92@gmail.com</a> |  
🌐 <a href="https://www.facebook.com/share/184Khe9iZu/" target="_blank">Facebook</a> |  
📸 <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank">Instagram</a>
</p>
</section>

<!-- Footer -->
<footer>
<h3>Khan Studio</h3>
<p>Professional digital services including websites, video editing, thumbnails & branding. Neon premium interface for modern businesses and creators.</p>
<p>© 2026 Khan Studio. All Rights Reserved.</p>
</footer>

<!-- Back to Top -->
<button onclick="window.scrollTo({top:0,behavior:'smooth'})" id="topBtn">Top</button>

<script>
// FAQ toggle
const faqCards = document.querySelectorAll('.faq-card');
faqCards.forEach(card => {card.addEventListener('click', ()=>{card.classList.toggle('active');});});
</script>

</body>
</html>
