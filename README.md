<html lang="en">
<head>
<meta charset="UTF-8">
<title>Web-Hub | Professional Digital Solutions</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"/>

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Poppins,sans-serif}
body{background:#0b1120;color:#e5e7eb;line-height:1.6}
a{text-decoration:none;color:inherit}
.container{width:90%;max-width:1200px;margin:auto}
section{padding:80px 0}

/* HERO */
.hero{
background:linear-gradient(to right,rgba(2,6,23,.9),rgba(2,6,23,.6)),
url("https://images.unsplash.com/photo-1498050108023-c5249f4df085") center/cover;
padding:120px 0;
text-align:center;
}
.hero h1{font-size:52px}
.hero p{margin:20px 0;max-width:600px;margin-left:auto;margin-right:auto}
.btn{background:#22c55e;padding:12px 28px;border-radius:30px;font-weight:600;display:inline-block}
.btn:hover{background:#16a34a}

/* GRID */
.grid{display:grid;gap:25px}
.grid-2{grid-template-columns:repeat(auto-fit,minmax(300px,1fr))}
.grid-3{grid-template-columns:repeat(auto-fit,minmax(250px,1fr))}
.grid-4{grid-template-columns:repeat(auto-fit,minmax(200px,1fr))}

/* CARDS */
.card{
background:#020617;
padding:30px;
border-radius:16px;
box-shadow:0 10px 25px rgba(0,0,0,.4);
text-align:center;
}
.card i{font-size:36px;color:#38bdf8;margin-bottom:15px}

/* TITLES */
h2{text-align:center;font-size:38px;margin-bottom:50px}
.center{text-align:center}

/* IMAGES */
img{width:100%;border-radius:16px;}

/* STATS */
.stats h3{font-size:40px;color:#22c55e}

/* FAQ */
details{
background:#020617;
padding:18px;
border-radius:12px;
margin-bottom:10px;
}
details summary{cursor:pointer;font-weight:600}

/* CONTACT FORM */
input,textarea{
width:100%;
padding:12px;
border-radius:10px;
border:none;
margin-bottom:10px;
}

/* FOOTER */
footer{background:#020617;padding:50px 0;text-align:center}
.social i{font-size:22px;margin:0 10px;color:#38bdf8}

/* FLOATING SOCIAL BUTTONS */
.floating-social {
  position: fixed;
  right: 20px;
  bottom: 20px;
  display: flex;
  flex-direction: column;
  gap: 12px;
  z-index: 9999;
}
.floating-social a {
  width: 52px;
  height: 52px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #fff;
  font-size: 22px;
  box-shadow: 0 8px 20px rgba(0,0,0,.4);
  transition: transform .3s;
}
.floating-social a:hover {transform: scale(1.1);}
.email {background:#22c55e;}
.instagram {background:linear-gradient(45deg,#f58529,#dd2a7b,#8134af);}
.facebook {background:#1877f2;}
</style>
</head>

<body>

<!-- HERO -->
<section class="hero">
<div class="container">
<h1>Web-Hub</h1>
<p>Professional Website Development, UI/UX Design, SEO & Digital Marketing Solutions</p>
<a href="#contact" class="btn">Start Your Project</a>
</div>
</section>

<!-- SERVICES -->
<section>
<div class="container">
<h2>Our Services</h2>
<div class="grid grid-4">
<div class="card"><i class="fa-solid fa-code"></i><h3>Web Development</h3><p>Fast, secure & scalable websites</p></div>
<div class="card"><i class="fa-solid fa-paintbrush"></i><h3>UI/UX Design</h3><p>Modern & user-friendly designs</p></div>
<div class="card"><i class="fa-solid fa-chart-line"></i><h3>SEO Optimization</h3><p>Rank higher on search engines</p></div>
<div class="card"><i class="fa-solid fa-bullhorn"></i><h3>Digital Marketing</h3><p>Grow your online presence</p></div>
</div>
</div>
</section>

<!-- ABOUT -->
<section>
<div class="container grid grid-2">
<img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c">
<div>
<h2>About Web-Hub</h2>
<p>We provide high-quality web solutions like top global agencies. Our goal is to deliver premium results at affordable pricing, with 100% client satisfaction.</p>
</div>
</div>
</section>

<!-- STATS -->
<section>
<div class="container grid grid-4 center stats">
<div><h3>250+</h3><p>Projects</p></div>
<div><h3>120+</h3><p>Clients</p></div>
<div><h3>5+</h3><p>Years Experience</p></div>
<div><h3>24/7</h3><p>Support</p></div>
</div>
</section>

<!-- PORTFOLIO -->
<section>
<div class="container">
<h2>Our Work</h2>
<div class="grid grid-3">
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">
<img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4">
<img src="https://images.unsplash.com/photo-1558655146-9f40138edfeb">
</div>
</div>
</section>

<!-- PRICING -->
<section>
<div class="container">
<h2>Pricing Plans</h2>
<div class="grid grid-3 center">
<div class="card"><h3>Basic</h3><h2>$99</h2><p>Landing Page</p></div>
<div class="card"><h3>Standard</h3><h2>$199</h2><p>Business Website</p></div>
<div class="card"><h3>Premium</h3><h2>$399</h2><p>Complete Solution</p></div>
</div>
</div>
</section>

<!-- TESTIMONIALS -->
<section>
<div class="container">
<h2>Client Reviews</h2>
<div class="grid grid-3">
<div class="card"><p>"Great service! Highly recommended."</p><strong>- John D.</strong></div>
<div class="card"><p>"Professional & fast delivery."</p><strong>- Sarah K.</strong></div>
<div class="card"><p>"Our website looks amazing thanks to Web-Hub."</p><strong>- Mike L.</strong></div>
</div>
</div>
</section>

<!-- FAQ -->
<section>
<div class="container">
<h2>FAQs</h2>
<div class="grid grid-2">
<details><summary>Are images showing correctly?</summary><p>Yes, all images are stock CDN links for guaranteed display.</p></details>
<details><summary>Is the site mobile-friendly?</summary><p>Yes, fully responsive on all devices.</p></details>
</div>
</div>
</section>

<!-- CONTACT -->
<section id="contact">
<div class="container grid grid-2">
<div>
<h2>Contact Us</h2>
<p>Email: rock.earn92@gmail.com</p>
<p>Facebook & Instagram links available via floating buttons</p>
</div>
<form class="card">
<input type="text" placeholder="Your Name">
<input type="email" placeholder="Your Email">
<textarea rows="5" placeholder="Your Message"></textarea>
<br>
<button class="btn">Send Message</button>
</form>
</div>
</section>

<!-- FOOTER -->
<footer>
<h3>Web-Hub</h3>
<div class="social">
<a href="https://www.facebook.com/profile.php?id=100084218946114"><i class="fab fa-facebook"></i></a>
<a href="https://www.instagram.com/mr_nazim073"><i class="fab fa-instagram"></i></a>
<a href="mailto:rock.earn92@gmail.com"><i class="fa-solid fa-envelope"></i></a>
</div>
<p>© 2026 Web-Hub. All Rights Reserved.</p>
</footer>

<!-- FLOATING SOCIAL BUTTONS -->
<div class="floating-social">
  <a href="mailto:rock.earn92@gmail.com" class="email" title="Email"><i class="fa-solid fa-envelope"></i></a>
  <a href="https://www.instagram.com/mr_nazim073" target="_blank" class="instagram" title="Instagram"><i class="fab fa-instagram"></i></a>
  <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="facebook" title="Facebook"><i class="fab fa-facebook-f"></i></a>
</div>

</body>
</html>
