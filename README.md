<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Mr Khan Pro Services | Neon Premium</title>
<meta name="description" content="Professional website, video editing, thumbnails & digital services by Mr Khan. Trusted by thousands of clients worldwide.">
<meta name="keywords" content="website development, video editing, thumbnail design, branding, digital services">
<meta name="author" content="Mr Khan Pro Services">
<meta name="robots" content="index, follow">
<meta name="google-site-verification" content="google8073cfacc72a7cb3">

<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<style>
/* Reset */
*{margin:0;padding:0;box-sizing:border-box;font-family:'Roboto',sans-serif;}
body{background:linear-gradient(135deg,#0a0a0a,#1a1a1a);color:#fff;scroll-behavior:smooth;}

/* General */
a{text-decoration:none;color:#00f0ff;}
h1,h2,h3{font-weight:700;text-transform:uppercase;}
section{padding:50px 20px;max-width:1200px;margin:auto;}
h2{color:#00f0ff;text-align:center;margin-bottom:30px;position:relative;}
h2::after{content:"";width:60px;height:3px;background:#ff0040;display:block;margin:10px auto;border-radius:2px;}

/* Hero */
header{position:relative;height:70vh;overflow:hidden;background:#000;}
header video{width:100%;height:100%;object-fit:cover;opacity:0.7;}
header h1{position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);font-size:3em;color:#00ffff;text-shadow:0 0 15px #ff0040,0 0 30px #00f0ff,0 0 60px #ff0040;animation:fadeInText 2s ease-in-out;}
@keyframes fadeInText{0%{opacity:0;transform:translate(-50%,-60%);}100%{opacity:1;transform:translate(-50%,-50%);}}

/* Cards */
.card{background:#111;padding:20px;border-radius:10px;flex:1 1 250px;text-align:center;box-shadow:0 0 15px #00f0ff;transition:0.3s;}
.card:hover{transform:translateY(-10px) scale(1.05);box-shadow:0 0 30px #ff0040,0 0 60px #00ffff;}
.card img{max-width:100%;border-radius:10px;}

/* Layouts */
.services,.portfolio,.stats-section,.reviews{display:flex;flex-wrap:wrap;gap:20px;justify-content:center;}

/* Form */
form{display:flex;flex-direction:column;gap:15px;max-width:500px;margin:auto;}
input,select,textarea{padding:10px;border-radius:5px;border:none;background:#222;color:#fff;}
input::placeholder,textarea::placeholder{color:#aaa;}
button{padding:15px;border:none;border-radius:5px;background:#ff0040;color:#fff;font-weight:bold;cursor:pointer;transition:0.3s;text-transform:uppercase;box-shadow:0 0 10px #00ffff;}
button:hover{background:#00ffff;color:#000;box-shadow:0 0 15px #ff0040,0 0 30px #00ffff;}

/* Footer */
footer{background:#111;padding:30px 20px;text-align:center;margin-top:50px;color:#aaa;}
footer a{color:#00ffff;text-decoration:none;transition:0.3s;}
footer a:hover{color:#ff0040;}

/* Back to top button */
#topBtn{position:fixed;bottom:20px;right:20px;padding:10px 15px;background:#00f0ff;color:#000;border:none;border-radius:5px;cursor:pointer;display:none;z-index:1000;transition:0.3s;}
#topBtn:hover{background:#ff0040;color:#fff;}

/* Responsive */
@media(max-width:768px){.services,.portfolio,.stats-section,.reviews{flex-direction:column;}header h1{font-size:2em;}}
</style>
</head>
<body>

<!-- Hero -->
<header>
<video autoplay muted loop>
<source src="assets/video/hero.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
<h1>Mr Khan Pro Services</h1>
</header>

<!-- About -->
<section id="about">
<h2>About Me</h2>
<p style="text-align:center;">Professional digital services including website development, video editing, thumbnail design, and branding. Trusted by thousands of clients worldwide. Premium neon design & animations.</p>
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
<p>Logo, social media branding & complete digital identity.</p>
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
<!-- Add more reviews here -->
</div>
</section>

<!-- FAQ -->
<section id="faq">
<h2>FAQ</h2>
<div class="card">
<h3>How can I order a service?</h3>
<p>You can fill the contact form or reach out via email or social media.</p>
</div>
<div class="card">
<h3>How long does delivery take?</h3>
<p>Delivery depends on service complexity, usually 1-7 days.</p>
</div>
<div class="card">
<h3>Do you provide revisions?</h3>
<p>Yes, revisions are included until client satisfaction.</p>
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
<h3>Mr Khan Pro Services</h3>
<p>Professional digital services including websites, video editing, thumbnails & branding. Trusted by thousands of clients worldwide.</p>
<p>📧 <a href="mailto:rock.earn92@gmail.com">rock.earn92@gmail.com</a></p>
<p>🌐 <a href="https://www.facebook.com/share/184Khe9iZu/" target="_blank">Facebook</a> | 📸 <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank">Instagram</a></p>
<p>© 2026 Mr Khan Pro Services. All Rights Reserved.</p>
</footer>

<!-- Back to Top Button -->
<button onclick="window.scrollTo({top:0,behavior:'smooth'})" id="topBtn">Top</button>

</body>
</html>
