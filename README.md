<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Web-Hub</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
<style>
/* Reset & basic */
* {margin:0; padding:0; box-sizing:border-box; font-family:'Poppins', sans-serif;}
body {background:#0b0b0b; color:#fff; overflow-x:hidden;}
img {max-width:100%; border-radius:10px;}
a {text-decoration:none; color:#fff; transition:0.3s;}
a:hover {color:#00f;}
header {position:fixed; width:100%; top:0; left:0; background:rgba(0,0,0,0.85); z-index:1000; padding:15px 50px; display:flex; justify-content:space-between; align-items:center;}
nav a {margin-left:20px;}

/* Hero */
.hero {height:100vh; display:flex; flex-direction:column; justify-content:center; align-items:center; text-align:center; background:linear-gradient(135deg, #0f0c29, #302b63, #24243e); position:relative; overflow:hidden;}
.hero h1 {font-size:3rem; color:#0ff; animation:fadeIn 2s ease-in-out;}
.hero p {color:#ff004c; font-size:1.5rem; margin-top:15px; animation:fadeIn 2s 0.5s ease-in-out;}
.hero button {padding:12px 30px; margin-top:25px; border:none; background:#ff004c; color:#fff; font-size:1rem; cursor:pointer; transition:0.3s;}
.hero button:hover {background:#00f;}
@keyframes fadeIn {from{opacity:0;} to{opacity:1;}}

/* Sections */
.section {padding:100px 50px;}
.section h2 {text-align:center; font-size:2.5rem; margin-bottom:50px; color:#0ff;}

/* Services */
.services {display:flex; justify-content:space-around; flex-wrap:wrap; gap:30px;}
.service-card {background:rgba(255,255,255,0.05); padding:30px; border-radius:15px; text-align:center; transition:0.3s; flex:1 1 250px;}
.service-card:hover {background:#ff004c; transform:scale(1.05);}
.service-card img {height:80px; margin-bottom:20px;}

/* Portfolio */
.portfolio-slider {display:flex; overflow-x:auto; gap:20px; scroll-behavior:smooth; padding-bottom:20px;}
.portfolio-item {min-width:300px; background:rgba(255,255,255,0.05); border-radius:15px; padding:20px; flex-shrink:0;}

/* Testimonials */
.testimonial-slider {display:flex; overflow-x:auto; gap:20px; scroll-behavior:smooth; padding-bottom:20px;}
.testimonial-item {min-width:250px; background:rgba(255,255,255,0.05); border-radius:15px; padding:20px; flex-shrink:0; text-align:center;}
.testimonial-item img {width:60px; height:60px; border-radius:50%; margin-bottom:15px;}

/* Stats */
.stats {display:flex; justify-content:space-around; flex-wrap:wrap; gap:50px; text-align:center; margin-top:50px;}
.stats div {flex:1 1 150px;}
.stats div h3 {font-size:2.5rem; color:#ff004c;}

/* Team */
.team {display:flex; justify-content:space-around; flex-wrap:wrap; gap:30px;}
.team-member {flex:1 1 250px; text-align:center;}
.team-member img {border-radius:50%; width:150px; height:150px; margin-bottom:15px;}

/* Contact */
.contact-form {display:flex; flex-direction:column; gap:15px; max-width:500px; margin:0 auto;}
.contact-form input, .contact-form textarea {padding:12px; border:none; border-radius:10px;}
.contact-form button {padding:12px; border:none; background:#0ff; color:#000; cursor:pointer; transition:0.3s;}
.contact-form button:hover {background:#ff004c; color:#fff;}

/* Footer */
footer {background:rgba(0,0,0,0.85); text-align:center; padding:30px; color:#fff; margin-top:50px;}

/* Back to top */
.back-to-top {position:fixed; bottom:30px; right:30px; background:#ff004c; color:#fff; padding:12px 15px; border-radius:50%; cursor:pointer; display:none;}
</style>
</head>
<body>

<header>
<div class="logo">Web-Hub</div>
<nav>
<a href="#services">Services</a>
<a href="#portfolio">Portfolio</a>
<a href="#testimonials">Reviews</a>
<a href="#team">Team</a>
<a href="#contact">Contact</a>
</nav>
</header>

<section class="hero">
<h1>Welcome to Web-Hub</h1>
<p>Premium digital solutions for modern businesses</p>
<button onclick="document.querySelector('#services').scrollIntoView({behavior:'smooth'})">Explore Services</button>
</section>

<section class="section" id="services">
<h2>Our Services</h2>
<div class="services">
<div class="service-card">
<img src="https://images.unsplash.com/photo-1581091012184-8f8f537e63b0" alt="Web Development">
<h3>Web Development</h3>
<p>Responsive, modern websites tailored for your brand.</p>
</div>
<div class="service-card">
<img src="https://images.unsplash.com/photo-1591696205602-776658df01fb" alt="Mobile Apps">
<h3>Mobile Apps</h3>
<p>iOS & Android apps designed for user engagement.</p>
</div>
<div class="service-card">
<img src="https://images.unsplash.com/photo-1581091215367-55bc6b09b83d" alt="UI/UX Design">
<h3>UI/UX Design</h3>
<p>Interactive and modern user experience design.</p>
</div>
</div>
</section>

<section class="section" id="portfolio">
<h2>Portfolio</h2>
<div class="portfolio-slider">
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1605902711622-cfb43c443bf1" alt="Project 1"></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1612831455543-623f0b94fded" alt="Project 2"></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1581091012184-8f8f537e63b0" alt="Project 3"></div>
</div>
</section>

<section class="section" id="testimonials">
<h2>Reviews</h2>
<div class="testimonial-slider">
<div class="testimonial-item">
<img src="https://images.unsplash.com/photo-1603415526960-f8fdf33e7d4b" alt="Client 1">
<h4>John Doe</h4>
<p>★★★★★ Amazing service and support!</p>
</div>
<div class="testimonial-item">
<img src="https://images.unsplash.com/photo-1603415526960-f8fdf33e7d4b" alt="Client 2">
<h4>Jane Smith</h4>
<p>★★★★★ Professional and creative solutions.</p>
</div>
</div>
</section>

<section class="section stats">
<div><h3>50+</h3><p>Clients</p></div>
<div><h3>120+</h3><p>Projects</p></div>
<div><h3>2000+</h3><p>Hours Worked</p></div>
</section>

<section class="section" id="team">
<h2>Our Team</h2>
<div class="team">
<div class="team-member">
<img src="https://images.unsplash.com/photo-1603415526960-f8fdf33e7d4b" alt="Team 1">
<h4>Khan</h4>
<p>Founder & CEO</p>
</div>
<div class="team-member">
<img src="https://images.unsplash.com/photo-1603415526960-f8fdf33e7d4b" alt="Team 2">
<h4>Ali</h4>
<p>Lead Designer</p>
</div>
</div>
</section>

<section class="section" id="contact">
<h2>Contact Us</h2>
<form class="contact-form">
<input type="text" placeholder="Your Name" required>
<input type="email" placeholder="Your Email" required>
<textarea rows="5" placeholder="Your Message" required></textarea>
<button type="submit">Send Message</button>
</form>
</section>

<footer>
<p>© 2026 Web-Hub. All rights reserved.</p>
</footer>

<div class="back-to-top" onclick="window.scrollTo({top:0, behavior:'smooth'});">↑</div>

<script>
// Back to top button
window.addEventListener('scroll', function(){
    document.querySelector('.back-to-top').style.display = window.scrollY > 300 ? 'block' : 'none';
});
</script>

</body>
</html>
