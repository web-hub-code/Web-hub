<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Khan Studio | Premium Digital Services</title>
<meta name="description" content="Khan Studio - Professional website development, video editing, thumbnails & branding services with neon effects.">
<meta name="keywords" content="website development, video editing, thumbnail design, branding, digital services">
<meta name="author" content="Khan Studio">
<meta name="robots" content="index, follow">
<meta name="google-site-verification" content="google8073cfacc72a7cb3">

<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<style>
/* Reset */
*{margin:0;padding:0;box-sizing:border-box;font-family:'Roboto',sans-serif;}
body{background: linear-gradient(120deg,#fdfdfd,#e6f0ff); color:#111; scroll-behavior:smooth;}

/* General */
a{text-decoration:none;color:#1a73e8;}
h1,h2,h3{font-weight:700;text-transform:uppercase;}
section{padding:50px 20px;max-width:1200px;margin:auto;}
h2{color:#1a73e8;text-align:center;margin-bottom:30px;position:relative;}
h2::after{content:"";width:60px;height:3px;background:#ff4081;display:block;margin:10px auto;border-radius:2px;}

/* Hero */
header{position:relative;height:70vh;overflow:hidden;background:#f0f0f0;border-radius:10px;}
header video{width:100%;height:100%;object-fit:cover;opacity:0.7;border-radius:10px;}
header h1{position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);font-size:3em;color:#ff4081;text-shadow:0 0 15px #1a73e8,0 0 30px #ff4081,0 0 60px #1a73e8;animation:fadeInText 2s ease-in-out;}
@keyframes fadeInText{0%{opacity:0;transform:translate(-50%,-60%);}100%{opacity:1;transform:translate(-50%,-50%);}}

/* Cards */
.card{background:#ffffff;padding:20px;border-radius:10px;flex:1 1 250px;text-align:center;box-shadow:0 0 10px rgba(26,115,232,0.3);transition:0.3s;}
.card:hover{transform:translateY(-10px) scale(1.05);box-shadow:0 0 20px #ff4081,0 0 40px #1a73e8;}
.card img{max-width:100%;border-radius:10px;}

/* Layouts */
.services,.portfolio,.stats-section,.reviews,.faq-section{display:flex;flex-wrap:wrap;gap:20px;justify-content:center;}

/* Form */
form{display:flex;flex-direction:column;gap:15px;max-width:500px;margin:auto;}
input,select,textarea{padding:10px;border-radius:5px;border:1px solid #ccc;background:#fff;color:#111;}
input::placeholder,textarea::placeholder{color:#888;}
button{padding:15px;border:none;border-radius:5px;background:#ff4081;color:#fff;font-weight:bold;cursor:pointer;transition:0.3s;text-transform:uppercase;box-shadow:0 0 5px #1a73e8;}
button:hover{background:#1a73e8;color:#fff;box-shadow:0 0 15px #ff4081,0 0 30px #1a73e8;}

/* Footer */
footer{background:#f0f0f0;padding:30px 20px;text-align:center;margin-top:50px;color:#111;}
footer a{color:#1a73e8;text-decoration:none;transition:0.3s;}
footer a:hover{color:#ff4081;}

/* Back to top button */
#topBtn{position:fixed;bottom:20px;right:20px;padding:10px 15px;background:#1a73e8;color:#fff;border:none;border-radius:5px;cursor:pointer;display:none;z-index:1000;transition:0.3s;}
#topBtn:hover{background:#ff4081;color:#fff;}

/* FAQ Accordion */
.faq-card{background:#ffffff;padding:15px;border-radius:10px;width:100%;cursor:pointer;box-shadow:0 0 10px rgba(26,115,232,0.3);transition:0.3s;margin-bottom:10px;}
.faq-card:hover{box-shadow:0 0 20px #ff4081,0 0 40px #1a73e8;}
.faq-content{max-height:0;overflow:hidden;transition:max-height 0.3s ease;}
.faq-card.active .faq-content{max-height:200px;padding-top:10px;}

/* Responsive */
@media(max-width:768px){.services,.portfolio,.stats-section,.reviews,.faq-section{flex-direction:column;}header h1{font-size:2em;}}
</style>
</head>
<body>

<!-- Hero -->
<header>
<video autoplay muted loop>
<source src="assets/video/hero.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
<h1>Khan Studio</h1>
</header>

<!-- About -->
<section id="about">
<h2>About Me</h2>
<p style="text-align:center;">Professional digital services including website development, video editing, thumbnail design, and branding. Trusted by thousands of clients worldwide. Premium neon animations.</p>
</section>

<!-- Services -->
<section id="services">
<h2>Our Services</h2>
<div class="services">
<div class="card">
<img src="assets/images/web1.jpg" alt="Website Development">
<h3>Website Development</h3>
<p>Responsive, modern & custom websites for all businesses.</p>
</div>
<div class="card">
<img src="assets/images/video1.jpg" alt="Video Editing">
<h3>Video Editing</h3>
<p>Professional edits, slow/fast motion, effects & more.</p>
</div>
<div class="card">
<img src="assets/images/thumbnail1.jpg" alt="Thumbnail Design">
<h3>Thumbnail Design</h3>
<p>Creative thumbnails to boost clicks & engagement.</p>
</div>
<div class="card">
<img src="assets/images/branding1.jpg" alt="Branding">
<h3>Branding</h3>
<p>Logo, social media branding & digital identity.</p>
</div>
<div class="card">
<img src="assets/images/seo.jpg" alt="SEO Services">
<h3>SEO Optimization</h3>
<p>Boost your website's visibility & ranking on Google.</p>
</div>
<div class="card">
<img src="assets/images/social.jpg" alt="Social Media Management">
<h3>Social Media Management</h3>
<p>Grow & manage your online presence effectively.</p>
</div>
</div>
</section>

<!-- Portfolio -->
<section id="portfolio">
<h2>Portfolio</h2>
<div class="portfolio">
<div class="card"><img src="assets/images/web1.jpg" alt="Web Project 1"><p>Website Example 1</p></div>
<div class="card"><img src="assets/images/web2.jpg" alt="Web Project 2"><p>Website Example 2</p></div>
<div class="card"><img src="assets/images/video1.jpg" alt="Video Project 1"><p>Video Editing 1</p></div>
<div class="card"><img src="assets/images/video2.jpg" alt="Video Project 2"><p>Video Editing 2</p></div>
</div>
</section>

<!-- Stats -->
<section id="stats">
<h2>Achievements</h2>
<div class="stats-section">
<div class="card"><h3>8000+</h3><p>Satisfied Clients</p></div>
<div class="card"><h3>1200+</h3><p>Websites Delivered</p></div>
<div class="card"><h3>3500+</h3><p>Videos Edited</p></div>
<div class="card"><h3>1500+</h3><p>Thumbnails Designed</p></div>
</div>
</section>

<!-- Testimonials -->
<section id="reviews">
<h2>Client Reviews</h2>
<div class="reviews">
<div class="card"><p>"Amazing service, highly recommended!"</p><p>- Ali</p></div>
<div class="card"><p>"Fast delivery and professional work."</p><p>- Sara</p></div>
<div class="card"><p>"Creative video editing, loved it!"</p><p>- Hassan</p></div>
<div class="card"><p>"Website looks great, exactly what I wanted."</p><p>- Fatima</p></div>
</div>
</section>

<!-- FAQ -->
<section id="faq">
<h2>FAQ</h2>
<div class="faq-section">
<div class="faq-card">
<h3>How can I order a service?</h3>
<div class="faq-content"><p>Fill the contact form or reach out via email/social links.</p></div>
</div>
<div class="faq-card">
<h3>How long does delivery take?</h3>
<div class="faq-content"><p>Depends on service, usually 1-7 days.</p></div>
</div>
<div class="faq-card">
<h3>Do you provide revisions?</h3>
<div class="faq-content"><p>Yes, until client satisfaction is achieved.</p></div>
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
<option>Branding</option>
<option>SEO Optimization</option>
<option>Social Media Management</option>
<option>Other</option>
</select>
<textarea name="Message" placeholder="Describe your project" required></textarea>
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
<p>Professional digital services including websites, video editing, thumbnails & branding. Trusted by thousands of clients worldwide.</p>
<p>📧 <a href="mailto:rock.earn92@gmail.com">rock.earn92@gmail.com</a></p>
<p>🌐 <a href="https://www.facebook.com/share/184Khe9iZu/" target="_blank">Facebook</a> | 📸 <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank">Instagram</a></p>
<p>© 2026 Khan Studio. All Rights Reserved.</p>
</footer>

<!-- Back to Top Button -->
<button onclick="window.scrollTo({top:0,behavior:'smooth'})" id="topBtn">Top</button>

<script>
// FAQ toggle
const faqCards = document.querySelectorAll('.faq-card');
faqCards.forEach(card => {
card.addEventListener('click', ()=>{card.classList.toggle('active');});
});
</script>

</body>
</html>
