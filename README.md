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
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
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
nav .logo{font-size:28px;color:#22c55e;font-weight:700;cursor:pointer}
nav ul{display:flex;gap:20px;list-style:none;flex-wrap:wrap}
nav ul li a{color:#e5e7eb;font-weight:500;transition:.3s}
nav ul li a:hover{color:#22c55e}

/* HERO */
.hero{background:linear-gradient(to right,rgba(15,23,42,.9),rgba(15,23,42,.6)),url('https://images.unsplash.com/photo-1498050108023-c5249f4df085') center/cover;padding:140px 0;text-align:center;animation:fadeIn 2s ease}
.hero h1{font-size:52px;color:#22c55e;animation:slideIn 1.5s ease}
.hero p{margin:20px 0;max-width:700px;margin-left:auto;margin-right:auto;font-size:18px}
.btn{background:#22c55e;padding:12px 28px;border-radius:30px;font-weight:600;display:inline-block;transition:.3s;color:#fff}
.btn:hover{background:#16a34a;cursor:pointer;transform:scale(1.05)}

/* GRID */
.grid{display:grid;gap:25px}
.grid-2{grid-template-columns:repeat(auto-fit,minmax(300px,1fr))}
.grid-3{grid-template-columns:repeat(auto-fit,minmax(250px,1fr))}
.grid-4{grid-template-columns:repeat(auto-fit,minmax(200px,1fr))}

/* CARDS */
.card{background:#1e293b;padding:25px;border-radius:16px;box-shadow:0 10px 25px rgba(0,0,0,.4);text-align:center;transition:transform .3s,box-shadow .3s;cursor:pointer}
.card:hover{transform:translateY(-10px);box-shadow:0 15px 30px rgba(0,0,0,.5)}
.card i{font-size:36px;color:#38bdf8;margin-bottom:15px}

/* TITLES */
h2{text-align:center;font-size:38px;margin-bottom:50px}
.center{text-align:center}

/* PORTFOLIO ITEMS */
.portfolio-item{position:relative;overflow:hidden;border-radius:16px;cursor:pointer}
.portfolio-item img{width:100%;transition:transform .3s;border-radius:16px}
.portfolio-item:hover img{transform:scale(1.05)}
.portfolio-item .overlay{position:absolute;bottom:0;left:0;width:100%;background:rgba(0,0,0,0.8);color:#fff;padding:15px;text-align:center;opacity:0;transition:.3s;font-size:14px}
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

/* ANIMATIONS */
@keyframes fadeIn{from{opacity:0}to{opacity:1}}
@keyframes slideIn{from{transform:translateY(-50px);opacity:0}to{transform:translateY(0);opacity:1}}

/* BACK-TO-TOP */
#topBtn{position:fixed;bottom:90px;right:20px;z-index:9999;background:#22c55e;color:#fff;padding:12px 15px;border:none;border-radius:50%;font-size:18px;cursor:pointer;display:none}
#topBtn:hover{background:#16a34a;transform:scale(1.1)}
</style>
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
<p>Professional Website Development, UI/UX Design, SEO & Digital Marketing Solutions. Projects start from 5,000 PKR depends on client demand.</p>
<a href="#contact" class="btn">Start Your Project</a>
</div>
</section>

<!-- ABOUT -->
<section id="about">
<div class="container">
<h2>About Web-Hub</h2>
<p>Web-Hub provides premium digital solutions: modern website development, UI/UX design, SEO optimization, and digital marketing services worldwide. Our goal is to deliver scalable, fast, and visually stunning projects that drive results for every client. We ensure modern design, fast delivery, and full client support.</p>
</div>
</section>

<!-- SERVICES -->
<section id="services">
<div class="container">
<h2>Our Services</h2>
<div class="grid grid-4">
<div class="card"><i class="fa-solid fa-code"></i><h3>Web Development</h3><p>Fast, secure & scalable websites, custom solutions, responsive layout.</p></div>
<div class="card"><i class="fa-solid fa-paintbrush"></i><h3>UI/UX Design</h3><p>Modern & user-friendly designs, creative interfaces, interactive elements.</p></div>
<div class="card"><i class="fa-solid fa-chart-line"></i><h3>SEO Optimization</h3><p>On-page & off-page SEO, improve search rankings, analytics integration.</p></div>
<div class="card"><i class="fa-solid fa-bullhorn"></i><h3>Digital Marketing</h3><p>Social media marketing, paid ads, content strategy, email campaigns.</p></div>
<div class="card"><i class="fa-solid fa-mobile-screen-button"></i><h3>Mobile App Dev</h3><p>Android & iOS apps, responsive design, smooth UX.</p></div>
<div class="card"><i class="fa-solid fa-shop"></i><h3>E-Commerce Solutions</h3><p>Shopify, WooCommerce, custom online stores, payment integration.</p></div>
<div class="card"><i class="fa-solid fa-cloud"></i><h3>Cloud Hosting</h3><p>Reliable & fast hosting, domain setup, SSL integration.</p></div>
<div class="card"><i class="fa-solid fa-shield"></i><h3>Security Services</h3><p>Website protection, backups, vulnerability scanning, SSL security.</p></div>
</div>
</div>
</section>

<!-- PORTFOLIO -->
<section id="portfolio">
<div class="container">
<h2>Our Work</h2>
<div class="grid grid-3">
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f"><div class="overlay">Project 1: Modern Website Design<br>HTML, CSS, JS, Responsive, SEO Optimized</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4"><div class="overlay">Project 2: Mobile App UI/UX<br>iOS & Android, Smooth UX, Interactive</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1558655146-9f40138edfeb"><div class="overlay">Project 3: E-Commerce Platform<br>Shopify, WooCommerce, Payment Gateway</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c"><div class="overlay">Project 4: SEO Optimized Blog<br>Content Marketing, Keyword Analysis, Analytics</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085"><div class="overlay">Project 5: Digital Marketing Campaign<br>Social Media, Ads, Branding</div></div>
<div class="portfolio-item"><img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d"><div class="overlay">Project 6: Cloud Hosting Setup<br>Domain, SSL, Security, Backups</div></div>
</div>
</div>
</section><!-- PRICING -->
<section id="pricing">
<div class="container">
<h2>Pricing Plans</h2>
<div class="grid grid-3">
<div class="card">
<h3>Basic</h3>
<p>5,000 PKR / $15 (depends on client demand)</p>
<button class="btn" onclick="manualPayment('Basic', '5000 PKR', '$15')">Select</button>
</div>
<div class="card">
<h3>Standard</h3>
<p>10,000 PKR / $30 (depends on client demand)</p>
<button class="btn" onclick="manualPayment('Standard', '10000 PKR', '$30')">Select</button>
</div>
<div class="card">
<h3>Premium</h3>
<p>20,000 PKR / $60 (depends on client demand)</p>
<button class="btn" onclick="manualPayment('Premium', '20000 PKR', '$60')">Select</button>
</div>
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

<!-- FAQ -->
<section id="faq">
<div class="container">
<h2>FAQs</h2>
<div class="grid grid-2">
<details><summary>Is the site mobile-friendly?</summary><p>Yes, fully responsive on all devices.</p></details>
<details><summary>How long does a project take?</summary><p>Depends on project size, typically 1–4 weeks.</p></details>
<details><summary>Do you provide SEO services?</summary><p>Yes, we offer full SEO optimization.</p></details>
<details><summary>Can I request custom designs?</summary><p>Absolutely, custom UI/UX solutions available.</p></details>
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
<div class="card"><i class="fa-brands fa-react"></i><p>React</p></div>
<div class="card"><i class="fa-brands fa-node"></i><p>Node.js</p></div>
<div class="card"><i class="fa-brands fa-wordpress"></i><p>WordPress</p></div>
<div class="card"><i class="fa-brands fa-shopify"></i><p>Shopify</p></div>
<div class="card"><i class="fa-brands fa-php"></i><p>PHP</p></div>
</div>
</div>
</section>

<!-- CONTACT -->
<section id="contact">
<div class="container grid grid-2">
<div>
<h2>Contact & Payment</h2>
<p>Email: webhub262@gmail.com</p>
<p>Send your project details, payment proof & transaction ID here:</p>
<p>Select Payment Method, copy number & attach screenshot or proof.</p>
</div>
<form class="card" onsubmit="sendEmail(event)">
<input type="text" id="name" placeholder="Your Name" required>
<input type="email" id="email" placeholder="Your Email" required>
<select id="paymentMethod" required>
<option value="">Select Payment Method</option>
<option value="Easypaisa">Easypaisa</option>
<option value="Jazzcash">Jazzcash</option>
<option value="SadaPay">SadaPay</option>
<option value="Payoneer">Payoneer</option>
<option value="Binance">Binance (TRC20)</option>
</select>
<input type="text" id="paymentNumber" placeholder="Number / Wallet Address" readonly>
<input type="file" id="proof" accept="image/*" required>
<textarea id="message" rows="5" placeholder="Your Message / Project Details" required></textarea>
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
// Navbar scroll
window.addEventListener('scroll',function(){
document.getElementById('navbar').classList.toggle('scrolled', window.scrollY>50);
});

// Back to top
var topBtn=document.getElementById("topBtn");
window.onscroll=function(){if(document.body.scrollTop>100||document.documentElement.scrollTop>100){topBtn.style.display="block";}else{topBtn.style.display="none";}};
function topFunction(){document.body.scrollTop=0;document.documentElement.scrollTop=0;}

// Counter animation
const counters=document.querySelectorAll('.counter');
counters.forEach(counter=>{
counter.innerText='0';
const updateCounter=()=>{
const target=+counter.getAttribute('data-target');
const count=+counter.innerText;
const increment=target/200;
if(count<target){counter.innerText=Math.ceil(count+increment);setTimeout(updateCounter,10);}else{counter.innerText=target;}
};
updateCounter();
});

// Payment Number copy
const paymentNumbers={
"Easypaisa":"03379827882",
"Jazzcash":"03705519562",
"SadaPay":"03705519562",
"Payoneer":"nazimkhan01123@gmail.com",
"Binance":"TTSxm4pBK26RB4vXaa3Uo3hqGa5HdhxBDR"
};
$('#paymentMethod').on('change',function(){
$('#paymentNumber').val(paymentNumbers[$(this).val()]);
});

// Send email with proof
function sendEmail(e){
e.preventDefault();
const name=document.getElementById('name').value;
const email=document.getElementById('email').value;
const method=document.getElementById('paymentMethod').value;
const number=document.getElementById('paymentNumber').value;
const message=document.getElementById('message').value;
const proof=document.getElementById('proof').files[0];

if(!method){alert('Select Payment Method');return;}

const formData=new FormData();
formData.append('name',name);
formData.append('email',email);
formData.append('method',method);
formData.append('number',number);
formData.append('message',message);
formData.append('proof',proof);

// Send via email using formspree or similar
fetch("https://formspree.io/f/xaykqgla",{
method:"POST",
body:formData
}).then(res=>{if(res.ok){alert("Message sent successfully");document.querySelector('form').reset();}else{alert("Error sending message");}});
}

// Slick slider
$(document).ready(function(){
$('.testimonial-slider').slick({
infinite:true,
slidesToShow:2,
slidesToScroll:1,
autoplay:true,
autoplaySpeed:3000,
arrows:true,
dots:true,
responsive:[
{breakpoint:768,settings:{slidesToShow:1}}
]
});
});
</script>
</body>
</html>
