<html lang="en">
<head>
<meta charset="UTF-8">
<title>Web-Hub | Pro Digital Solutions</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Web-Hub provides professional web development, UI/UX design, SEO, and digital marketing solutions worldwide.">
<meta property="og:title" content="Web-Hub | Pro Digital Solutions">
<meta property="og:description" content="Professional Website Development, UI/UX Design, SEO & Digital Marketing Solutions.">
<meta property="og:image" content="https://images.unsplash.com/photo-1498050108023-c5249f4df085">
<meta property="og:url" content="https://web-hub-code.github.io/Web-hub/">
<meta name="twitter:card" content="summary_large_image">

<!-- Google Fonts & Icons -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.css"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick-theme.min.css"/>

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Poppins,sans-serif}
body{background:#0f172a;color:#e5e7eb;line-height:1.6;scroll-behavior:smooth}
a{text-decoration:none;color:inherit}
.container{width:90%;max-width:1200px;margin:auto}
section{padding:80px 0}

/* NAVIGATION */
nav{position:fixed;width:100%;top:0;left:0;background:rgba(15,23,42,0.95);display:flex;justify-content:space-between;align-items:center;padding:15px 5%;z-index:999;transition:0.3s}
nav.scrolled{background:rgba(15,23,42,1)}
nav .logo{font-size:28px;color:#22c55e;font-weight:700}
nav ul{display:flex;gap:20px;list-style:none;flex-wrap:wrap}
nav ul li a{color:#e5e7eb;font-weight:500;transition:.3s}
nav ul li a:hover{color:#22c55e}

/* HERO */
.hero{background:linear-gradient(to right,rgba(15,23,42,.9),rgba(15,23,42,.6)),url('https://images.unsplash.com/photo-1498050108023-c5249f4df085') center/cover;padding:140px 0;text-align:center;animation:fadeIn 2s ease}
.hero h1{font-size:52px;color:#22c55e;animation:slideIn 1.5s ease}
.hero p{margin:20px 0;max-width:600px;margin-left:auto;margin-right:auto}
.btn{background:#22c55e;padding:12px 28px;border-radius:30px;font-weight:600;display:inline-block;transition:.3s}
.btn:hover{background:#16a34a;cursor:pointer;transform:scale(1.05)}

/* GRID */
.grid{display:grid;gap:25px}
.grid-2{grid-template-columns:repeat(auto-fit,minmax(300px,1fr))}
.grid-3{grid-template-columns:repeat(auto-fit,minmax(250px,1fr))}
.grid-4{grid-template-columns:repeat(auto-fit,minmax(200px,1fr))}

/* CARDS */
.card{background:#1e293b;padding:30px;border-radius:16px;box-shadow:0 10px 25px rgba(0,0,0,.4);text-align:center;transition:transform .3s, box-shadow .3s;cursor:pointer}
.card:hover{transform:translateY(-10px);box-shadow:0 15px 30px rgba(0,0,0,.5)}
.card i{font-size:36px;color:#38bdf8;margin-bottom:15px}

/* TITLES */
h2{text-align:center;font-size:38px;margin-bottom:50px}
.center{text-align:center}

/* PORTFOLIO ITEMS */
.portfolio-item{position:relative;overflow:hidden;border-radius:16px}
.portfolio-item img{width:100%;transition:transform .3s}
.portfolio-item:hover img{transform:scale(1.05)}
.portfolio-item .overlay{position:absolute;bottom:0;left:0;width:100%;background:rgba(0,0,0,0.8);color:#fff;padding:20px;text-align:left;opacity:0;transition:.3s}
.portfolio-item:hover .overlay{opacity:1}

/* STATS */
.stats h3{font-size:40px;color:#22c55e}
.counter{font-weight:bold;color:#22c55e;font-size:32px}

/* FAQ */
details{background:#1e293b;padding:18px;border-radius:12px;margin-bottom:10px;cursor:pointer;transition:.3s}
details:hover{background:#273449}
details summary{cursor:pointer;font-weight:600}

/* CONTACT FORM */
input,textarea{width:100%;padding:12px;border-radius:10px;border:none;margin-bottom:10px;background:#0f172a;color:#e5e7eb}

/* FOOTER */
footer{background:#1e293b;padding:50px 0;text-align:center}
.social i{font-size:22px;margin:0 10px;color:#38bdf8;transition:.3s}
.social i:hover{transform:scale(1.2)}

/* FLOATING SOCIAL BUTTONS */
.floating-social{position:fixed;right:20px;bottom:20px;display:flex;flex-direction:column;gap:12px;z-index:9999}
.floating-social a{width:52px;height:52px;border-radius:50%;display:flex;align-items:center;justify-content:center;color:#fff;font-size:22px;box-shadow:0 8px 20px rgba(0,0,0,.4);transition:transform .3s}
.floating-social a:hover{transform:scale(1.1)}
.email{background:#22c55e}
.instagram{background:linear-gradient(45deg,#f58529,#dd2a7b,#8134af)}
.facebook{background:#1877f2}

/* BACK-TO-TOP */
#topBtn{position:fixed;bottom:90px;right:20px;z-index:9999;background:#22c55e;color:#fff;padding:12px 15px;border:none;border-radius:50%;font-size:18px;cursor:pointer;display:none}
#topBtn:hover{background:#16a34a;transform:scale(1.1)}
</style>
</head>
<body>

<!-- NAVIGATION -->
<nav id="navbar">
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
<p>Professional Website Development, UI/UX Design, SEO & Digital Marketing Solutions. Affordable & Trusted.</p>
<a href="#contact" class="btn">Start Your Project</a>
</div>
</section>

<!-- ABOUT -->
<section id="about">
<div class="container">
<h2>About Web-Hub</h2>
<p>Web-Hub provides premium digital solutions in Pakistan and worldwide: websites, apps, SEO, and marketing. <strong>Prices depend on client demand</strong>. We deliver visually stunning, fast, and reliable projects tailored to your needs.</p>
</div>
</section>

<!-- SERVICES -->
<section id="services">
<div class="container">
<h2>Our Services</h2>
<div class="grid grid-4">
<div class="card"><i class="fa-solid fa-code"></i><h3>Web Development</h3><p>Fast, secure & scalable websites for every business</p></div>
<div class="card"><i class="fa-solid fa-paintbrush"></i><h3>UI/UX Design</h3><p>Modern, responsive & user-friendly designs</p></div>
<div class="card"><i class="fa-solid fa-chart-line"></i><h3>SEO Optimization</h3><p>Improve your search rankings & traffic</p></div>
<div class="card"><i class="fa-solid fa-bullhorn"></i><h3>Digital Marketing</h3><p>Grow your online presence & sales</p></div>
<div class="card"><i class="fa-solid fa-mobile-screen-button"></i><h3>Mobile App Dev</h3><p>Android & iOS applications with sleek UI</p></div>
<div class="card"><i class="fa-solid fa-shop"></i><h3>E-Commerce Solutions</h3><p>Shopify, WooCommerce & other platforms</p></div>
<div class="card"><i class="fa-solid fa-cloud"></i><h3>Cloud Hosting</h3><p>Fast, reliable, secure hosting solutions</p></div>
<div class="card"><i class="fa-solid fa-shield"></i><h3>Security Services</h3><p>Protect your website & client data from threats</p></div>
</div>
</div>
</section>

<!-- PORTFOLIO -->
<section id="portfolio">
<div class="container">
<h2>Our Portfolio</h2>
<div class="grid grid-3">
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">
<div class="overlay">
<h3>Project 1: Modern Website Design</h3>
<p>Developed a responsive website with clean UI, SEO optimized, fast loading speed, and integrated CMS for client content management.</p>
<a href="#" class="btn">View Live</a>
</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4">
<div class="overlay">
<h3>Project 2: Mobile App UI/UX</h3>
<p>Designed an interactive mobile application with smooth navigation, onboarding screens, and modern interface for Android & iOS.</p>
<a href="#" class="btn">View Live</a>
</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1558655146-9f40138edfeb">
<div class="overlay">
<h3>Project 3: E-Commerce Platform</h3>
<p>Built an online store with WooCommerce & Shopify, secure payment integration, and optimized product catalog for conversions.</p>
<a href="#" class="btn">View Live</a>
</div>
</div>

<!-- More projects will continue in Part 2 -->

</div>
</div>
</section><!-- Portfolio remaining projects -->
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c">
<div class="overlay">
<h3>Project 4: SEO Optimized Blog</h3>
<p>Custom blog setup with SEO strategies, responsive layout, fast loading, and analytics integration.</p>
<a href="#" class="btn">View Live</a>
</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085">
<div class="overlay">
<h3>Project 5: Digital Marketing Campaign</h3>
<p>Managed digital campaigns including social media ads, email marketing, and content optimization for max ROI.</p>
<a href="#" class="btn">View Live</a>
</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d">
<div class="overlay">
<h3>Project 6: Cloud Hosting Setup</h3>
<p>Setup secure and fast cloud hosting, configured domains, SSL, and server optimization for high traffic websites.</p>
<a href="#" class="btn">View Live</a>
</div>
</div>

</div>
</section>

<!-- PRICING -->
<section id="pricing">
<div class="container">
<h2>Pricing Plans</h2>
<div style="text-align:center;margin-bottom:30px;">
<label for="currency">Select Currency: </label>
<select id="currency" onchange="updatePricing()">
<option value="PKR">PKR</option>
<option value="USD">USD</option>
</select>
</div>
<div class="grid grid-3" id="pricing-cards">
<!-- Pricing cards will update dynamically via JS -->
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
<div><h3 class="counter" data-target="250">0</h3><p>Projects</p></div>
<div><h3 class="counter" data-target="120">0</h3><p>Clients</p></div>
<div><h3 class="counter" data-target="5">0</h3><p>Years Experience</p></div>
<div><h3 class="counter" data-target="24">0</h3><p>Support</p></div>
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
<p>Email: <a href="mailto:webhub262@gmail.com">webhub262@gmail.com</a></p>
<p>Click send and your default email client will open with message ready.</p>
</div>
<form class="card" onsubmit="sendEmail(event)">
<input type="text" id="name" placeholder="Your Name" required>
<input type="email" id="email" placeholder="Your Email" required>
<textarea id="message" rows="5" placeholder="Your Message" required></textarea>
<button class="btn" type="submit">Send Message</button>
</form>
</div>
</section>

<!-- FOOTER -->
<footer>
<h3>Web-Hub</h3>
<div class="social">
<a href="https://www.facebook.com/profile.php?id=100084218946114"><i class="fab fa-facebook"></i></a>
<a href="https://www.instagram.com/mr_nazim073"><i class="fab fa-instagram"></i></a>
<a href="mailto:webhub262@gmail.com"><i class="fa-solid fa-envelope"></i></a>
</div>
<p>© 2026 Web-Hub. All Rights Reserved.</p>
</footer>

<!-- FLOATING SOCIAL -->
<div class="floating-social">
<a href="mailto:webhub262@gmail.com" class="email" title="Email"><i class="fa-solid fa-envelope"></i></a>
<a href="https://www.instagram.com/mr_nazim073" target="_blank" class="instagram" title="Instagram"><i class="fab fa-instagram"></i></a>
<a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="facebook" title="Facebook"><i class="fab fa-facebook-f"></i></a>
</div>

<!-- BACK TO TOP BUTTON -->
<button id="topBtn" onclick="topFunction()" title="Go to top"><i class="fas fa-arrow-up"></i></button>

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.7.0/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.js"></script>
<script>
// Back-to-top
var topBtn = document.getElementById("topBtn");
window.onscroll = function() {scrollFunction()};
function scrollFunction() { topBtn.style.display = (document.body.scrollTop > 300 || document.documentElement.scrollTop > 300) ? "block" : "none";}
function topFunction() {document.body.scrollTop = 0;document.documentElement.scrollTop = 0;}

// Testimonial slider
$(document).ready(function(){
$('.testimonial-slider').slick({dots:true,infinite:true,autoplay:true,autoplaySpeed:4000});
});

// Counter animation
const counters = document.querySelectorAll('.counter');
counters.forEach(counter => {
counter.innerText = '0';
const updateCounter = () => {
const target = +counter.getAttribute('data-target');
const c = +counter.innerText;
const increment = target/200;
if(c < target){counter.innerText = `${Math.ceil(c + increment)}`; setTimeout(updateCounter, 10);}
else{counter.innerText = target;}
};
updateCounter();
});

// Pricing toggle
const pricingData = {
PKR: [{plan:'Basic',price:'5,000 PKR'},{plan:'Standard',price:'10,000 PKR'},{plan:'Premium',price:'15,000 PKR'},{plan:'Enterprise',price:'25,000 PKR'}],
USD: [{plan:'Basic',price:'15 USD'},{plan:'Standard',price:'30 USD'},{plan:'Premium',price:'45 USD'},{plan:'Enterprise',price:'75 USD'}]
};
function updatePricing(){
const currency = document.getElementById('currency').value;
const cards = document.getElementById('pricing-cards');
cards.innerHTML = '';
pricingData[currency].forEach(p => {
cards.innerHTML += `<div class="card"><h3>${p.plan}</h3><p>${p.price}</p><button class="btn">Get Started</button></div>`;
});
}
updatePricing();

// Payment method copy feature & proof upload (added in future enhancements)
</script>
</body>
</html>
