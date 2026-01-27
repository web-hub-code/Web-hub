<html lang="en">
<head>
<meta charset="UTF-8">
<title>Web-Hub | Pro Digital Solutions</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<!-- Google Fonts & Icons -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.css"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick-theme.min.css"/>

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Poppins,sans-serif}
body{background:#0b1120;color:#e5e7eb;line-height:1.6;scroll-behavior:smooth}
a{text-decoration:none;color:inherit}
.container{width:90%;max-width:1200px;margin:auto}
section{padding:80px 0}

/* NAVIGATION */
nav{position:fixed;width:100%;top:0;left:0;background:rgba(2,6,23,0.95);display:flex;justify-content:space-between;align-items:center;padding:15px 5%;z-index:999;}
nav .logo{font-size:28px;color:#22c55e;font-weight:700}
nav ul{display:flex;gap:25px;list-style:none}
nav ul li a{color:#e5e7eb;font-weight:500;transition:.3s}
nav ul li a:hover{color:#22c55e}

/* HERO */
.hero{
background:linear-gradient(to right,rgba(2,6,23,.9),rgba(2,6,23,.6)),
url("https://images.unsplash.com/photo-1498050108023-c5249f4df085") center/cover;
padding:140px 0;text-align:center;animation: fadeIn 2s ease;
}
.hero h1{font-size:52px;color:#22c55e;animation: slideIn 1.5s ease;}
.hero p{margin:20px 0;max-width:600px;margin-left:auto;margin-right:auto}
.btn{background:#22c55e;padding:12px 28px;border-radius:30px;font-weight:600;display:inline-block}
.btn:hover{background:#16a34a;cursor:pointer}

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
transition:transform .3s;
cursor:pointer;
}
.card:hover{transform:translateY(-10px);}
.card i{font-size:36px;color:#38bdf8;margin-bottom:15px}

/* TITLES */
h2{text-align:center;font-size:38px;margin-bottom:50px}
.center{text-align:center}

/* IMAGES */
img{width:100%;border-radius:16px;cursor:pointer;}

/* STATS */
.stats h3{font-size:40px;color:#22c55e}
.counter{font-weight:bold;color:#22c55e;font-size:32px}

/* FAQ */
details{
background:#020617;
padding:18px;
border-radius:12px;
margin-bottom:10px;
cursor:pointer;
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

/* Animations */
@keyframes fadeIn{from{opacity:0}to{opacity:1}}
@keyframes slideIn{from{transform:translateY(-50px);opacity:0}to{transform:translateY(0);opacity:1}}

/* Back-to-top */
#topBtn{position:fixed;bottom:90px;right:20px;z-index:9999;background:#22c55e;color:#fff;padding:12px 15px;border:none;border-radius:50%;font-size:18px;cursor:pointer;display:none;}
#topBtn:hover{background:#16a34a}

/* ABOUT SECTION */
#about{background:#0a0f1c;padding:80px 0;text-align:center;color:#e5e7eb}
#about p{max-width:800px;margin:auto}
</style>
</head>

<body>

<!-- NAVIGATION -->
<nav>
<div class="logo">Web-Hub</div>
<ul>
<li><a href="#hero">Home</a></li>
<li><a href="#about">About</a></li>
<li><a href="#services">Services</a></li>
<li><a href="#portfolio">Portfolio</a></li>
<li><a href="#pricing">Pricing</a></li>
<li><a href="#testimonials">Testimonials</a></li>
<li><a href="#faq">FAQ</a></li>
<li><a href="#technologies">Technologies</a></li>
<li><a href="#contact">Contact</a></li>
</ul>
</nav>

<!-- HERO -->
<section id="hero" class="hero">
<div class="container">
<h1>Web-Hub</h1>
<p>Professional Website Development, UI/UX Design, SEO & Digital Marketing Solutions</p>
<a href="#contact" class="btn">Start Your Project</a>
</div>
</section>

<!-- ABOUT -->
<section id="about">
<div class="container">
<h2>About Web-Hub</h2>
<p>Web-Hub is a premium digital solutions company offering modern, innovative, and scalable website development, UI/UX design, SEO optimization, and digital marketing services for businesses worldwide.</p>
</div>
</section>

<!-- SERVICES -->
<section id="services">
<div class="container">
<h2>Our Services</h2>
<div class="grid grid-4">
<div class="card"><i class="fa-solid fa-code"></i><h3>Web Development</h3><p>Fast, secure & scalable websites</p></div>
<div class="card"><i class="fa-solid fa-paintbrush"></i><h3>UI/UX Design</h3><p>Modern & user-friendly designs</p></div>
<div class="card"><i class="fa-solid fa-chart-line"></i><h3>SEO Optimization</h3><p>Rank higher on search engines</p></div>
<div class="card"><i class="fa-solid fa-bullhorn"></i><h3>Digital Marketing</h3><p>Grow your online presence</p></div>
<div class="card"><i class="fa-solid fa-mobile-screen-button"></i><h3>Mobile App Dev</h3><p>Android & iOS applications</p></div>
<div class="card"><i class="fa-solid fa-shop"></i><h3>E-Commerce Solutions</h3><p>Shopify, WooCommerce & more</p></div>
</div>
</div>
</section>

<!-- PORTFOLIO -->
<section id="portfolio">
<div class="container">
<h2>Our Work</h2>
<div class="portfolio-slider">
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">
<img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4">
<img src="https://images.unsplash.com/photo-1558655146-9f40138edfeb">
<img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c">
<img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085">
<img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d">
</div>
</div>
</section>

<!-- PRICING -->
<section id="pricing">
<div class="container">
<h2>Pricing Plans</h2>
<div class="grid grid-3">
<div class="card"><h3>Basic</h3><p>$99 / month</p><button class="btn">Get Started</button></div>
<div class="card"><h3>Standard</h3><p>$199 / month</p><button class="btn">Get Started</button></div>
<div class="card"><h3>Premium</h3><p>$299 / month</p><button class="btn">Get Started</button></div>
<div class="card"><h3>Enterprise</h3><p>$499 / month</p><button class="btn">Get Started</button></div>
</div>
</div>
</section>

<!-- TESTIMONIALS -->
<section id="testimonials">
<div class="container">
<h2>Client Reviews</h2>
<div class="testimonial-slider">
<div class="card"><p>"Great service! Highly recommended."</p><strong>- John D.</strong></div>
<div class="card"><p>"Professional & fast delivery."</p><strong>- Sarah K.</strong></div>
<div class="card"><p>"Our website looks amazing thanks to Web-Hub."</p><strong>- Mike L.</strong></div>
<div class="card"><p>"Excellent communication and support."</p><strong>- Linda P.</strong></div>
<div class="card"><p>"Creative designs, very happy."</p><strong>- Kevin R.</strong></div>
<div class="card"><p>"Fast, reliable & professional."</p><strong>- Emma W.</strong></div>
</div>
</div>
</section>

<!-- STATS -->
<section>
<div class="container grid grid-4 center stats">
<div><h3 class="counter">250</h3><p>Projects</p></div>
<div><h3 class="counter">120</h3><p>Clients</p></div>
<div><h3 class="counter">5</h3><p>Years Experience</p></div>
<div><h3 class="counter">24</h3><p>Support</p></div>
</div>
</section>

<!-- FAQ -->
<section id="faq">
<div class="container">
<h2>FAQs</h2>
<div class="grid grid-2">
<details><summary>Are images showing correctly?</summary><p>Yes, all images are stock CDN links for guaranteed display.</p></details>
<details><summary>Is the site mobile-friendly?</summary><p>Yes, fully responsive on all devices.</p></details>
<details><summary>Do you provide SEO services?</summary><p>Yes, our SEO experts improve your search rankings.</p></details>
<details><summary>Can I request custom designs?</summary><p>Absolutely, we offer fully custom UI/UX solutions.</p></details>
<details><summary>How long does a project take?</summary><p>Depends on project size, typically 1–4 weeks.</p></details>
<details><summary>Do you provide support after delivery?</summary><p>Yes, 24/7 support available.</p></details>
<details><summary>Is the contact form secure?</summary><p>Yes, integrated with EmailJS and HTTPS recommended.</p></details>
<details><summary>Can I request revisions?</summary><p>Yes, client revisions are included per project.</p></details>
</div>
</div>
</section>

<!-- TECHNOLOGIES -->
<section id="technologies">
<div class="container">
<h2>Technologies & Tools</h2>
<div class="grid grid-4 center">
<div class="card"><i class="fa-brands fa-html5"></i><p>HTML5</p></div>
<div class="card"><i class="fa-brands fa-css3-alt"></i><p>CSS3</p></div>
<div class="card"><i class="fa-brands fa-js"></i><p>JavaScript</p></div>
<div class="card"><i class="fa-brands fa-php"></i><p>PHP</p></div>
<div class="card"><i class="fa-brands fa-react"></i><p>React</p></div>
<div class="card"><i class="fa-brands fa-node"></i><p>Node.js</p></div>
<div class="card"><i class="fa-brands fa-wordpress"></i><p>WordPress</p></div>
<div class="card"><i class="fa-brands fa-shopify"></i><p>Shopify</p></div>
</div>
</div>
</section>

<!-- CONTACT -->
<section id="contact">
<div class="container grid grid-2">
<div>
<h2>Contact Us</h2>
<p>Email: rock.earn92@gmail.com</p>
<p>Use the form to send message directly to Email.</p>
</div>
<form class="card" id="contact-form">
<input type="text" name="user_name" placeholder="Your Name" required>
<input type="email" name="user_email" placeholder="Your Email" required>
<textarea name="message" rows="5" placeholder="Your Message" required></textarea>
<br>
<button class="btn" type="submit">Send Message</button>
</form>
</div>
</section>

<!-- BACK TO TOP -->
<button id="topBtn" onclick="topFunction()"><i class="fa-solid fa-angle-up"></i></button>

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

<!-- FLOATING SOCIAL -->
<div class="floating-social">
  <a href="mailto:rock.earn92@gmail.com" class="email" title="Email"><i class="fa-solid fa-envelope"></i></a>
  <a href="https://www.instagram.com/mr_nazim073" target="_blank" class="instagram" title="Instagram"><i class="fab fa-instagram"></i></a>
  <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="facebook" title="Facebook"><i class="fab fa-facebook-f"></i></a>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/emailjs-com@3/dist/email.min.js"></script>
<script>
// Portfolio slider
$('.portfolio-slider').slick({slidesToShow:3,slidesToScroll:1,autoplay:true,autoplaySpeed:2000,dots:true,responsive:[{breakpoint:768,settings:{slidesToShow:1}}]});
// Testimonial slider
$('.testimonial-slider').slick({slidesToShow:2,slidesToScroll:1,autoplay:true,autoplaySpeed:2500,dots:true,responsive:[{breakpoint:768,settings:{slidesToShow:1}}]});
// Counters
$('.counter').each(function(){$(this).prop('Counter',0).animate({Counter:$(this).text()},{duration:2000,easing:'swing',step:function(now){$(this).text(Math.ceil(now));}});});
// EmailJS Contact
emailjs.init("YOUR_USER_ID"); // replace with your EmailJS userID
document.getElementById('contact-form').addEventListener('submit',function(event){
event.preventDefault();
emailjs.sendForm('YOUR_SERVICE_ID','YOUR_TEMPLATE_ID',this)
.then(function(){alert("Message sent successfully!");},function(err){alert("Error sending message: "+JSON.stringify(err));});
});
// Back to top
window.onscroll=function(){scrollFunction()};
function scrollFunction(){document.getElementById("topBtn").style.display=(document.body.scrollTop>300||document.documentElement.scrollTop>300)?"block":"none";}
function topFunction(){document.body.scrollTop=0;document.documentElement.scrollTop=0;}
</script>

</body>
</html>
