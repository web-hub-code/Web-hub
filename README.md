<html lang="en">
<head>
<meta charset="UTF-8">
<title>Web-Hub | Pro Digital Solutions</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Web-Hub provides professional web development, UI/UX design, SEO, and digital marketing solutions worldwide.">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.css"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick-theme.min.css"/>
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Poppins,sans-serif}
body{background:#0f172a;color:#e5e7eb;line-height:1.6;scroll-behavior:smooth}
a{text-decoration:none;color:inherit}
.container{width:90%;max-width:1200px;margin:auto}
section{padding:80px 0;position:relative}
/* NAV */
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
/* PORTFOLIO */
.portfolio-item{position:relative;overflow:hidden;border-radius:16px;cursor:pointer;transition:transform .3s}
.portfolio-item img{width:100%;transition:transform .3s}
.portfolio-item:hover img{transform:scale(1.05)}
.portfolio-item .overlay{position:absolute;bottom:0;left:0;width:100%;background:rgba(0,0,0,0.8);color:#fff;padding:15px;text-align:center;opacity:0;transition:.3s}
.portfolio-item:hover .overlay{opacity:1}
/* TESTIMONIALS */
.testimonial-slider{max-width:900px;margin:auto}
.testimonial-slider .slick-slide{background:#1e293b;padding:30px;border-radius:16px;text-align:center;color:#e5e7eb;box-shadow:0 10px 20px rgba(0,0,0,.3)}
.testimonial-slider .slick-slide p{font-style:italic;margin-bottom:10px}
.testimonial-slider .slick-slide h3{color:#22c55e;margin-top:10px}
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
/* FLOATING SOCIAL */
.floating-social{position:fixed;right:20px;bottom:20px;display:flex;flex-direction:column;gap:12px;z-index:9999}
.floating-social a{width:52px;height:52px;border-radius:50%;display:flex;align-items:center;justify-content:center;color:#fff;font-size:22px;box-shadow:0 8px 20px rgba(0,0,0,.4);transition:transform .3s}
.floating-social a:hover{transform:scale(1.1)}
.email{background:#22c55e}
.instagram{background:linear-gradient(45deg,#f58529,#dd2a7b,#8134af)}
.facebook{background:#1877f2}
/* Animations */
@keyframes fadeIn{from{opacity:0}to{opacity:1}}
@keyframes slideIn{from{transform:translateY(-50px);opacity:0}to{transform:translateY(0);opacity:1}}
/* PAYMENT */
.payment-dropdown{position:relative;margin-bottom:20px}
.payment-btn{width:100%;padding:15px;background:#1e293b;border-radius:12px;border:none;color:#e5e7eb;font-size:16px;text-align:left;cursor:pointer;display:flex;justify-content:space-between;align-items:center;transition:.3s}
.payment-btn:hover{background:#273449}
.payment-options{display:none;position:absolute;top:60px;width:100%;background:#1e293b;border-radius:12px;box-shadow:0 5px 15px rgba(0,0,0,.3);z-index:10}
.payment-options button{width:100%;padding:12px;text-align:left;border:none;background:none;color:#e5e7eb;cursor:pointer;transition:.3s}
.payment-options button:hover{background:#273449}
.copy-notif{color:#22c55e;font-size:14px;margin-top:5px;display:none}
</style>
</head>
<body>

<!-- NAV -->
<nav id="navbar">
<div class="logo">Web-Hub</div>
<ul>
<li><a href="#hero">Home</a></li>
<li><a href="#about">About</a></li>
<li><a href="#services">Services</a></li>
<li><a href="#portfolio">Portfolio</a></li>
<li><a href="#pricing">Pricing</a></li>
<li><a href="#payments">Payments</a></li>
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
<p>We deliver modern websites, SEO, digital marketing, UI/UX, mobile apps, and cloud solutions worldwide. Focused on performance, scalability, and creativity.</p>
</div>
</section>

<!-- SERVICES -->
<section id="services">
<div class="container">
<h2>Our Services</h2>
<div class="grid grid-4">
<div class="card"><i class="fa-solid fa-code"></i><h3>Web Development</h3><p>Secure, scalable, modern websites</p></div>
<div class="card"><i class="fa-solid fa-paintbrush"></i><h3>UI/UX Design</h3><p>User-friendly, modern interface design</p></div>
<div class="card"><i class="fa-solid fa-chart-line"></i><h3>SEO Optimization</h3><p>Boost your search rankings</p></div>
<div class="card"><i class="fa-solid fa-bullhorn"></i><h3>Digital Marketing</h3><p>Grow your online presence</p></div>
<div class="card"><i class="fa-solid fa-mobile-screen-button"></i><h3>Mobile App Dev</h3><p>iOS & Android Apps</p></div>
<div class="card"><i class="fa-solid fa-shop"></i><h3>E-Commerce</h3><p>Shopify/WooCommerce integration</p></div>
<div class="card"><i class="fa-solid fa-cloud"></i><h3>Cloud Hosting</h3><p>Secure and fast hosting</p></div>
<div class="card"><i class="fa-solid fa-shield"></i><h3>Security Services</h3><p>Protect your website & data</p></div>
</div>
</div>
</section>

<!-- PORTFOLIO -->
<section id="portfolio">
<div class="container">
<h2>Our Work & Clients</h2>
<div class="grid grid-3">
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">
<div class="overlay">Corporate Website: Full responsive layout for a tech company. Interactive elements and modern design.</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4">
<div class="overlay">E-commerce Store: Shopify integration with payment gateways, product management, and responsive design.</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1558655146-9f40138edfeb">
<div class="overlay">Mobile App UI/UX: Sleek, modern interface design for iOS & Android apps with custom animations.</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c">
<div class="overlay">SEO Blog: Optimized for search engines with fast loading and user-friendly layout.</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085">
<div class="overlay">Digital Marketing Dashboard: Analytics, reporting, and campaign tracking for multiple clients.</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d">
<div class="overlay">Cloud Hosting Setup: Fast, secure, with uptime monitoring and backup services for businesses.</div>
</div>
</div>
</div>
</section>

<!-- PRICING -->
<section id="pricing">
<div class="container">
<h2>Pricing Plans</h2>
<div class="grid grid-3">
<div class="card"><h3>Basic</h3><p>PKR 5,000 / month (≈ $15) - Depends on client demand</p><button class="btn">Get Started</button></div>
<div class="card"><h3>Standard</h3><p>PKR 15,000 / month (≈ $45) - Depends on client demand</p><button class="btn">Get Started</button></div>
<div class="card"><h3>Premium</h3><p>PKR 25,000 / month (≈ $75) - Depends on client demand</p><button class="btn">Get Started</button></div>
<div class="card"><h3>Enterprise</h3><p>PKR 50,000 / month (≈ $150) - Depends on client demand</p><button class="btn">Get Started</button></div>
</div>
</div>
</section>

<!-- PAYMENT -->
<section id="payments">
<div class="container">
<h2>Payment Methods</h2>
<div class="payment-dropdown">
<button class="payment-btn" onclick="toggleDropdown()">Select Payment Method <i class="fa fa-chevron-down"></i></button>
<div class="payment-options">
<button onclick="selectPayment('Easypaisa','03379827882')">Easypaisa</button>
<button onclick="selectPayment('JazzCash','03705519562')">JazzCash</button>
<button onclick="selectPayment('SadaPay','03705519562')">SadaPay</button>
<button onclick="selectPayment('Payoneer','nazimkhan01123@gmail.com')">Payoneer</button>
<button onclick="selectPayment('Binance TRC20','TTSxm4pBK26RB4vXaa3Uo3hqGa5HdhxBDR')">Binance TRC20</button>
</div>
<div class="copy-notif" id="copyNotif">Copied!</div>
</div>
<div id="paymentDisplay" style="margin-top:15px;font-size:18px;color:#e5e7eb;"></div>
<p style="font-size:14px;color:#a1a1aa;margin-top:5px;">After selecting, copy the number/email and send payment. Then send details via email.</p>
</div>
</section>

<!-- TESTIMONIALS -->
<section id="testimonials">
<div class="container">
<h2>Client Testimonials</h2>
<div class="testimonial-slider">
<div><p>"Web-Hub transformed our website into a modern, fast-loading platform!"</p><h3>- Ali R.</h3></div>
<div><p>"Excellent UI/UX design, our users love the new interface."</p><h3>- Sara K.</h3></div>
<div><p>"Professional service, responsive team, and great results."</p><h3>- Imran S.</h3></div>
</div>
</div>
</section>

<!-- FAQ -->
<section id="faq">
<div class="container">
<h2>Frequently Asked Questions</h2>
<details><summary>What services does Web-Hub provide?</summary><p>Website, UI/UX, SEO, Digital Marketing, Apps, Hosting.</p></details>
<details><summary>How can I contact you?</summary><p>Email or social links below.</p></details>
<details><summary>Do you offer post-delivery support?</summary><p>Yes, 24/7 maintenance packages available.</p></details>
</div>
</section>

<!-- TECHNOLOGIES -->
<section id="technologies">
<div class="container">
<h2>Technologies We Use</h2>
<div class="grid grid-4">
<div class="card"><i class="fa-brands fa-html5"></i><h3>HTML5</h3></div>
<div class="card"><i class="fa-brands fa-css3-alt"></i><h3>CSS3</h3></div>
<div class="card"><i class="fa-brands fa-js"></i><h3>JavaScript</h3></div>
<div class="card"><i class="fa-brands fa-react"></i><h3>React</h3></div>
<div class="card"><i class="fa-brands fa-node"></i><h3>Node.js</h3></div>
<div class="card"><i class="fa-brands fa-php"></i><h3>PHP</h3></div>
<div class="card"><i class="fa-brands fa-sass"></i><h3>SASS</h3></div>
<div class="card"><i class="fa-brands fa-git-alt"></i><h3>Git</h3></div>
</div>
</div>
</section>

<!-- CONTACT -->
<section id="contact">
<div class="container">
<h2>Contact Us</h2>
<form onsubmit="sendEmail(event)">
<input type="text" placeholder="Your Name" required>
<input type="email" placeholder="Your Email" required>
<textarea placeholder="Message" rows="5" required></textarea>
<button class="btn" type="submit">Send Message</button>
</form>
</div>
</section>

<footer>
<p>© 2026 Web-Hub. All Rights Reserved.</p>
<div class="social">
<a href="#" class="facebook"><i class="fab fa-facebook-f"></i></a>
<a href="#" class="instagram"><i class="fab fa-instagram"></i></a>
<a href="mailto:webhub262@gmail.com" class="email"><i class="fa fa-envelope"></i></a>
</div>
</footer>

<!-- FLOATING SOCIAL -->
<div class="floating-social">
<a href="#" class="facebook"><i class="fab fa-facebook-f"></i></a>
<a href="#" class="instagram"><i class="fab fa-instagram"></i></a>
<a href="mailto:webhub262@gmail.com" class="email"><i class="fa fa-envelope"></i></a>
</div>

<!-- BACK TO TOP -->
<button id="topBtn" onclick="scrollTop()">↑</button>

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.4/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.js"></script>
<script>
// NAV SCROLL EFFECT
window.addEventListener('scroll', function() {
  const nav = document.getElementById('navbar');
  if(window.scrollY > 50){ nav.classList.add('scrolled'); } 
  else { nav.classList.remove('scrolled'); }
});

// PAYMENT DROPDOWN
function toggleDropdown(){
  const options = document.querySelector('.payment-options');
  options.style.display = options.style.display === 'block' ? 'none' : 'block';
}

function selectPayment(method, value){
  const display = document.getElementById('paymentDisplay');
  display.innerHTML = `<strong>${method}:</strong> <span id="paymentValue">${value}</span> <button onclick="copyPayment()">Copy</button>`;
}

function copyPayment(){
  const value = document.getElementById('paymentValue').innerText;
  navigator.clipboard.writeText(value);
  const notif = document.getElementById('copyNotif');
  notif.style.display = 'block';
  setTimeout(()=>{ notif.style.display='none'; }, 1500);
}

// TESTIMONIAL SLIDER
$('.testimonial-slider').slick({
  dots: true,
  arrows: false,
  infinite: true,
  autoplay: true,
  autoplaySpeed: 4000,
  slidesToShow: 1,
  adaptiveHeight: true
});

// BACK TO TOP
function scrollTop(){ window.scrollTo({top:0, behavior:'smooth'}); }

// CONTACT FORM (dummy)
function sendEmail(e){
  e.preventDefault();
  alert('Thank you! Your message has been sent.');
  e.target.reset();
}

// SMOOTH SCROLL
document.querySelectorAll('nav ul li a').forEach(link=>{
  link.addEventListener('click', function(e){
    e.preventDefault();
    document.querySelector(this.getAttribute('href')).scrollIntoView({behavior:'smooth'});
  });
});
</script>
</body>
</html>
