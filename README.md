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
.portfolio-item .overlay{position:absolute;bottom:0;left:0;width:100%;background:rgba(0,0,0,0.7);color:#fff;padding:15px;text-align:center;opacity:0;transition:.3s}
.portfolio-item:hover .overlay{opacity:1}

/* PRICING */
#pricing .card p{font-size:16px;margin:15px 0}

/* PAYMENT METHOD CARDS */
.payment-card{background:#1e293b;padding:20px;border-radius:16px;display:flex;align-items:center;justify-content:space-between;margin-bottom:15px;cursor:pointer;transition:.3s}
.payment-card:hover{background:#273449}
.copy-btn{background:#22c55e;border:none;padding:6px 12px;border-radius:8px;color:#fff;cursor:pointer;transition:.3s}
.copy-btn:hover{background:#16a34a;transform:scale(1.05)}

/* FOOTER */
footer{background:#1e293b;padding:50px 0;text-align:center;color:#e5e7eb}
footer .social i{font-size:22px;margin:0 10px;color:#38bdf8;transition:.3s}
footer .social i:hover{transform:scale(1.2)}
footer p{margin-top:15px}

/* FLOATING SOCIAL BUTTONS */
.floating-social{position:fixed;right:20px;bottom:20px;display:flex;flex-direction:column;gap:12px;z-index:9999}
.floating-social a{width:52px;height:52px;border-radius:50%;display:flex;align-items:center;justify-content:center;color:#fff;font-size:22px;box-shadow:0 8px 20px rgba(0,0,0,.4);transition:transform .3s}
.floating-social a:hover{transform:scale(1.1)}
.email{background:#22c55e}
.instagram{background:linear-gradient(45deg,#f58529,#dd2a7b,#8134af)}
.facebook{background:#1877f2}

/* ANIMATIONS */
@keyframes fadeIn{from{opacity:0}to{opacity:1}}
@keyframes slideIn{from{transform:translateY(-50px);opacity:0}to{transform:translateY(0);opacity:1}}

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
<li><a href="#payments">Payments</a></li>
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
<p>Web-Hub provides premium digital solutions including modern website development, responsive UI/UX design, SEO optimization, and full digital marketing services. We deliver fast, scalable, and visually stunning projects for all clients.</p>
</div>
</section>

<!-- SERVICES -->
<section id="services">
<div class="container">
<h2>Our Services</h2>
<div class="grid grid-4">
<div class="card"><i class="fa-solid fa-code"></i><h3>Web Development</h3><p>Fast, secure & scalable websites.</p></div>
<div class="card"><i class="fa-solid fa-paintbrush"></i><h3>UI/UX Design</h3><p>Modern & user-friendly designs.</p></div>
<div class="card"><i class="fa-solid fa-chart-line"></i><h3>SEO Optimization</h3><p>Improve search engine rankings.</p></div>
<div class="card"><i class="fa-solid fa-bullhorn"></i><h3>Digital Marketing</h3><p>Grow your online presence effectively.</p></div>
<div class="card"><i class="fa-solid fa-mobile-screen-button"></i><h3>Mobile App Development</h3><p>Android & iOS applications.</p></div>
<div class="card"><i class="fa-solid fa-shop"></i><h3>E-Commerce Solutions</h3><p>Shopify, WooCommerce & custom stores.</p></div>
<div class="card"><i class="fa-solid fa-cloud"></i><h3>Cloud Hosting</h3><p>Reliable & fast hosting solutions.</p></div>
<div class="card"><i class="fa-solid fa-shield"></i><h3>Security Services</h3><p>Protect your website & data.</p></div>
</div>
</div>
</section>

<!-- PORTFOLIO -->
<section id="portfolio">
<div class="container">
<h2>Our Work</h2>
<div class="grid grid-3">
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f"><div class="overlay">Corporate website with responsive layout & interactive UI elements.</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4"><div class="overlay">Mobile app design with seamless user experience & custom animations.</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1558655146-9f40138edfeb"><div class="overlay">E-commerce platform with full Shopify integration & payment gateways.</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c"><div class="overlay">SEO-optimized blog with analytics dashboard for performance tracking.</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085"><div class="overlay">Digital marketing campaign dashboard with reporting & insights.</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d"><div class="overlay">Cloud hosting & server setup with security, speed, uptime monitoring.</div></div>
</div>
</div>
</section>

<!-- PRICING -->
<section id="pricing">
<div class="container">
<h2>Pricing Plans</h2>
<div class="grid grid-3">
<div class="card"><h3>Basic</h3><p>PKR 5,000 / month (≈ $15) – Depends on client demand</p><button class="btn">Get Started</button></div>
<div class="card"><h3>Standard</h3><p>PKR 15,000 / month (≈ $45) – Depends on client demand</p><button class="btn">Get Started</button></div>
<div class="card"><h3>Premium</h3><p>PKR 25,000 / month (≈ $75) – Depends on client demand</p><button class="btn">Get Started</button></div>
<div class="card"><h3>Enterprise</h3><p>PKR 50,000 / month (≈ $150) – Depends on client demand</p><button class="btn">Get Started</button></div>
</div>
</div>
</section>

<!-- PAYMENT METHODS -->
<section id="payments">
<div class="container">
<h2>Payment Methods</h2>
<div class="payment-card" onclick="copyText('easypaisa')"><span>Easypaisa: 03379827882</span><button class="copy-btn">Copy</button></div>
<div class="payment-card" onclick="copyText('jazzcash')"><span>JazzCash: 03705519562</span><button class="copy-btn">Copy</button></div>
<div class="payment-card" onclick="copyText('sadapay')"><span>SadaPay: 03705519562</span><button class="copy-btn">Copy</button></div>
<div class="payment-card" onclick="copyText('payoneer')"><span>Payoneer: nazimkhan01123@gmail.com</span><button class="copy-btn">Copy</button></div>
<div class="payment-card" onclick="copyText('binance')"><span>Binance TRC20: TTSxm4pBK26RB4vXaa3Uo3hqGa5HdhxBDR</span><button class="copy-btn">Copy</button></div>

<!-- Hidden spans for copy -->
<span id="easypaisa" style="display:none;">03379827882</span>
<span id="jazzcash" style="display:none;">03705519562</span>
<span id="sadapay" style="display:none;">03705519562</span>
<span id="payoneer" style="display:none;">nazimkhan01123@gmail.com</span>
<span id="binance" style="display:none;">TTSxm4pBK26RB4vXaa3Uo3hqGa5HdhxBDR</span>
</div>
</section>

<script>
function copyText(id){
  var copyText = document.getElementById(id).innerText;
  navigator.clipboard.writeText(copyText).then(()=>{alert("Copied: " + copyText);});
}
</script><!-- TESTIMONIALS -->
<section id="testimonials">
<div class="container">
<h2>Client Reviews</h2>
<div class="grid grid-3">
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
<section id="stats">
<div class="container grid grid-4 center stats">
<div><h3 class="counter" data-target="250">0</h3><p>Projects</p></div>
<div><h3 class="counter" data-target="120">0</h3><p>Clients</p></div>
<div><h3 class="counter" data-target="5">0</h3><p>Years Experience</p></div>
<div><h3 class="counter" data-target="24">0</h3><p>Support</p></div>
</div>
</section>

<!-- FAQ -->
<section id="faq">
<div class="container">
<h2>FAQs</h2>
<div class="grid grid-2">
<details><summary>Are images showing correctly?</summary><p>Yes, all images are CDN links for guaranteed display.</p></details>
<details><summary>Is the site mobile-friendly?</summary><p>Yes, fully responsive on all devices.</p></details>
<details><summary>Do you provide SEO services?</summary><p>Yes, our SEO experts improve your search rankings.</p></details>
<details><summary>Can I request custom designs?</summary><p>Absolutely, we offer fully custom UI/UX solutions.</p></details>
<details><summary>How long does a project take?</summary><p>Depends on project size, typically 1–4 weeks.</p></details>
<details><summary>Do you provide support after delivery?</summary><p>Yes, 24/7 support available.</p></details>
<details><summary>Is the contact form secure?</summary><p>Yes, clicking send will open your default email client safely.</p></details>
<details><summary>Can I request revisions?</summary><p>Yes, client revisions are included per project.</p></details>
</div>
</div>
</section>

<!-- TECHNOLOGIES & TOOLS -->
<section id="technologies">
<div class="container">
<h2>Technologies & Tools</h2>
<div class="grid grid-4 center">
<div class="card"><i class="fa-brands fa-html5"></i><p>HTML5 - Structure & Semantic Markup</p></div>
<div class="card"><i class="fa-brands fa-css3-alt"></i><p>CSS3 - Styling & Layout</p></div>
<div class="card"><i class="fa-brands fa-js"></i><p>JavaScript - Interactive Features</p></div>
<div class="card"><i class="fa-brands fa-php"></i><p>PHP - Server-Side Programming</p></div>
<div class="card"><i class="fa-brands fa-react"></i><p>React - Frontend Frameworks</p></div>
<div class="card"><i class="fa-brands fa-node"></i><p>Node.js - Backend & APIs</p></div>
<div class="card"><i class="fa-brands fa-wordpress"></i><p>WordPress - CMS & E-Commerce</p></div>
<div class="card"><i class="fa-solid fa-database"></i><p>MySQL - Database Management</p></div>
</div>
</div>
</section>

<!-- CONTACT FORM -->
<section id="contact">
<div class="container">
<h2>Contact Us</h2>
<form action="mailto:webhub262@gmail.com" method="post" enctype="text/plain">
<input type="text" name="name" placeholder="Your Name" required>
<input type="email" name="email" placeholder="Your Email" required>
<input type="text" name="subject" placeholder="Subject" required>
<textarea name="message" placeholder="Your Message" rows="6" required></textarea>
<button type="submit" class="btn">Send Message</button>
</form>
</div>
</section>

<!-- FOOTER -->
<footer>
<div class="container">
<div class="social">
<a href="https://facebook.com" target="_blank"><i class="fab fa-facebook-f"></i></a>
<a href="https://instagram.com" target="_blank"><i class="fab fa-instagram"></i></a>
<a href="mailto:webhub262@gmail.com"><i class="fa-solid fa-envelope"></i></a>
</div>
<p>&copy; 2026 Web-Hub. All Rights Reserved.</p>
</div>
</footer>

<!-- FLOATING SOCIAL BUTTONS -->
<div class="floating-social">
<a href="mailto:webhub262@gmail.com" class="email"><i class="fa-solid fa-envelope"></i></a>
<a href="https://instagram.com" class="instagram" target="_blank"><i class="fab fa-instagram"></i></a>
<a href="https://facebook.com" class="facebook" target="_blank"><i class="fab fa-facebook-f"></i></a>
</div>

<script>
// Counter Animation
const counters = document.querySelectorAll('.counter');
counters.forEach(counter => {
  counter.innerText = '0';
  const updateCounter = () => {
    const target = +counter.getAttribute('data-target');
    const count = +counter.innerText;
    const increment = target / 200;
    if(count < target){
      counter.innerText = Math.ceil(count + increment);
      setTimeout(updateCounter, 20);
    } else {
      counter.innerText = target;
    }
  };
  updateCounter();
});
</script>

</body>
</html>
