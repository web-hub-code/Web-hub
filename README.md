<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Khan Studio | Premium Digital Services</title>
<meta name="description" content="Khan Studio - Professional digital services including website development, video editing, thumbnail design, branding, and more. Premium neon animated interface.">
<meta name="keywords" content="digital services, website development, video editing, branding, thumbnails, neon, premium">
<meta name="author" content="Khan Studio">
<meta name="google-site-verification" content="google8073cfacc72a7cb3">

<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

<style>
/* Reset & Body */
*{margin:0;padding:0;box-sizing:border-box;font-family:'Roboto',sans-serif;}
body{background: linear-gradient(135deg,#f0f0f0,#1a1a1a,#ff0040,#0040ff); color:#fff; scroll-behavior:smooth; transition:0.5s;}

/* Neon Headings */
h1,h2,h3{font-weight:700;text-transform:uppercase;text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}
h2{color:#00ffff;text-align:center;margin-bottom:30px;position:relative;}
h2::after{content:"";width:60px;height:3px;background:#ff0040;display:block;margin:10px auto;border-radius:2px;}

/* Hero */
header{position:relative;height:70vh;overflow:hidden;border-radius:15px;display:flex;justify-content:center;align-items:center;text-align:center;}
header::before{content:"";position:absolute;top:0;left:0;width:100%;height:100%;background:linear-gradient(135deg,rgba(0,0,0,0.3),rgba(255,0,64,0.2),rgba(0,64,255,0.2)); z-index:1;}
header h1{position:relative;z-index:2;font-size:3em;animation:neonPulse 2s ease-in-out infinite;}

/* Neon Pulse Animation */
@keyframes neonPulse{
0%{text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}
50%{text-shadow:0 0 15px #ff0040,0 0 30px #0040ff,0 0 60px #ff0040;}
100%{text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}
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
input,select,textarea{padding:10px;border-radius:5px;border:1px solid #ccc;background:#fff;color:#111;}
input::placeholder,textarea::placeholder{color:#888;}

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
Khan Studio is a leading digital service provider with a focus on **website development, video editing, thumbnail design, branding, SEO optimization, and social media management**. Our goal is to deliver **premium digital solutions** with neon-animated interfaces for businesses, content creators, and professionals worldwide. We focus on **speed, quality, innovation, and client satisfaction**.
</p>
</section>

<!-- Services -->
<section id="services">
<h2>Our Services</h2>
<div class="services">
<div class="card">
<h3>Website Development</h3>
<p>Create **responsive, fast, and modern websites** with custom UI/UX, e-commerce support, blogs, portfolios, and full SEO optimization. We ensure **secure, scalable, and reliable websites** for clients of all industries.</p>
</div>
<div class="card">
<h3>Video Editing</h3>
<p>Professional video editing including **slow motion, fast motion, color grading, transitions, intros/outros, subtitles, and special effects**. We handle YouTube, reels, short films, ads, and social media campaigns with creative precision.</p>
</div>
<div class="card">
<h3>Thumbnail & Graphics Design</h3>
<p>Design **eye-catching thumbnails, banners, logos, social media graphics**, and promotional content. Our designs maximize **click-through rates, engagement, and brand identity**.</p>
</div>
<div class="card">
<h3>Branding & Marketing</h3>
<p>Build complete branding solutions including **logos, brand kits, social media branding**, and marketing creatives. Our strategy enhances your **digital presence and recognition** across platforms.</p>
</div>
<div class="card">
<h3>SEO & Social Media</h3>
<p>Improve your **search engine visibility and social media engagement** with advanced SEO strategies, content optimization, and social media management services.</p>
</div>
</div>
</section>

<!-- Portfolio -->
<section id="portfolio">
<h2>Portfolio</h2>
<div class="portfolio">
<div class="card">
<h3>Website Projects</h3>
<p>Delivered multiple responsive websites with modern UI/UX, e-commerce, and blogs for various clients worldwide.</p>
</div>
<div class="card">
<h3>Video Projects</h3>
<p>Edited and delivered professional videos for YouTube, Instagram, and ads, including motion graphics, intros, and color grading.</p>
</div>
<div class="card">
<h3>Graphics & Branding</h3>
<p>Created branding packages, logos, banners, and thumbnail designs, helping clients establish a strong digital identity.</p>
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

<!-- Testimonials -->
<section id="reviews">
<h2>Client Reviews</h2>
<div class="reviews">
<div class="card"><p>"Amazing service, highly recommended! Professional and fast delivery."</p><p>- Ali</p></div>
<div class="card"><p>"Khan Studio transformed my YouTube channel branding. Excellent work!"</p><p>- Sara</p></div>
<div class="card"><p>"Creative video editing and website design. Truly premium services."</p><p>- Hassan</p></div>
</div>
</section>

<!-- FAQ -->
<section id="faq">
<h2>FAQ</h2>
<div class="faq-section">
<div class="faq-card">
<h3>How can I order a service?</h3>
<div class="faq-content"><p>You can fill the contact form below or directly reach out via email or social media links.</p></div>
</div>
<div class="faq-card">
<h3>How long does delivery take?</h3>
<div class="faq-content"><p>Delivery depends on the service. Usually between 1-7 days depending on complexity.</p></div>
</div>
<div class="faq-card">
<h3>Do you provide revisions?</h3>
<div class="faq-content"><p>Yes, we provide unlimited revisions until the client is fully satisfied.</p></div>
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
<option>Thumbnail Design</option>
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
<p>Professional digital services including websites, video editing, thumbnails & branding. Premium neon animated interface for modern businesses and creators.</p>
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
