<html lang="en">
<head>
<meta charset="UTF-8">
<title>Web-Hub | Complete Digital Solutions</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Poppins}
body{background:#0b1220;color:#e5e7eb;scroll-behavior:smooth}
a{text-decoration:none;color:inherit}
img{max-width:100%;border-radius:16px}
section{padding:90px 8%}
h2{font-size:36px;color:#22c55e;text-align:center;margin-bottom:10px}
p.sub{text-align:center;color:#9ca3af;margin-bottom:40px}
.btn{display:inline-block;background:#22c55e;color:#000;padding:12px 28px;border-radius:30px;font-weight:600}
.btn:hover{background:#16a34a}
.grid{display:grid;gap:24px}
.g3{grid-template-columns:repeat(auto-fit,minmax(240px,1fr))}
.card{background:#111827;border-radius:20px;padding:26px;box-shadow:0 10px 30px #0005}
nav{position:fixed;top:0;left:0;width:100%;z-index:1000;background:#020617e6;backdrop-filter:blur(10px);display:flex;justify-content:space-between;align-items:center;padding:14px 8%}
nav .logo{color:#22c55e;font-size:22px;font-weight:700}
nav a{margin-left:18px;font-weight:500}
nav a:hover{color:#22c55e}

/* HERO */
.hero{min-height:100vh;background:linear-gradient(#0008,#0008),url('https://images.unsplash.com/photo-1498050108023-c5249f4df085') center/cover;display:flex;align-items:center}
.hero h1{font-size:56px;color:#22c55e}
.hero p{max-width:600px;margin:14px 0;color:#cbd5f5}

/* STATS */
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:20px}
.stat{background:#020617;border-radius:18px;padding:26px;text-align:center}
.stat h3{font-size:38px;color:#22c55e}

/* SLIDER */
.slider{display:flex;gap:20px;overflow-x:auto;scroll-snap-type:x mandatory}
.slide{min-width:300px;scroll-snap-align:start}

/* PRICING */
.price{font-size:34px;color:#22c55e;margin:10px 0}

/* PAYMENT */
.pay button{width:100%;padding:14px;border:none;border-radius:12px;background:#1f2937;color:#fff;margin:6px 0;cursor:pointer}
.pay button:hover{background:#374151}
#copymsg{text-align:center;color:#22c55e;margin-top:8px}

/* FOOTER */
footer{background:#020617;padding:50px 8%;text-align:center}
footer a{display:inline-block;margin:6px;padding:12px 16px;border-radius:12px;background:#1f2937}
footer a:hover{background:#22c55e;color:#000}

/* POPUP */
.popup{display:none;position:fixed;inset:0;background:#000a;align-items:center;justify-content:center;z-index:2000}
.popup-box{background:#fff;color:#000;padding:28px;border-radius:20px;text-align:center;max-width:360px}

@media(max-width:768px){
.hero h1{font-size:38px}
section{padding:70px 6%}
}
</style>
</head>

<body>

<nav>
<div class="logo">Web-Hub</div>
<div>
<a href="#services">Services</a>
<a href="#tech">Tech</a>
<a href="#portfolio">Portfolio</a>
<a href="#pricing">Pricing</a>
<a href="#payment">Payment</a>
<a href="#contact">Contact</a>
</div>
</nav>

<section class="hero">
<div>
<h1>Grow Your Business Online</h1>
<p>High-performance websites, UI/UX, SEO & digital growth — trusted by clients worldwide.</p>
<a href="#contact" class="btn">Get Started</a>
</div>
</section>

<section id="services">
<h2>Our Services</h2>
<p class="sub">Everything you need to go digital</p>
<div class="grid g3">
<div class="card"><i class="fa fa-code"></i><h3>Web Development</h3><p>Fast, secure, scalable websites.</p></div>
<div class="card"><i class="fa fa-palette"></i><h3>UI / UX</h3><p>Modern, conversion-focused design.</p></div>
<div class="card"><i class="fa fa-chart-line"></i><h3>SEO</h3><p>Rank higher & get traffic.</p></div>
<div class="card"><i class="fa fa-cart-shopping"></i><h3>E-Commerce</h3><p>Sell online professionally.</p></div>
<div class="card"><i class="fa fa-mobile"></i><h3>Responsive</h3><p>Perfect on all devices.</p></div>
<div class="card"><i class="fa fa-cloud"></i><h3>Hosting Setup</h3><p>Domain & server configuration.</p></div>
</div>
</section>

<section id="tech">
<h2>Technologies</h2>
<div class="grid g3">
<div class="card">HTML5 / CSS3 / JS</div>
<div class="card">React UI</div>
<div class="card">Node Concepts</div>
<div class="card">SEO Tools</div>
<div class="card">Cloud Platforms</div>
<div class="card">Analytics</div>
</div>
</section>

<section>
<h2>Our Numbers</h2>
<div class="stats">
<div class="stat"><h3>150+</h3><p>Clients</p></div>
<div class="stat"><h3>260+</h3><p>Projects</p></div>
<div class="stat"><h3>5+</h3><p>Years</p></div>
</div>
</section>

<section id="portfolio">
<h2>Portfolio</h2>
<p class="sub">Recent work</p>
<div class="grid g3">
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">
<img src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d">
<img src="https://images.unsplash.com/photo-1492724441997-5dc865305da7">
</div>
</section>

<section>
<h2>Testimonials</h2>
<div class="slider">
<div class="card slide">“Excellent service & fast delivery.”</div>
<div class="card slide">“Professional team, great support.”</div>
<div class="card slide">“Our sales increased after launch.”</div>
</div>
</section>

<section id="pricing">
<h2>Pricing</h2>
<div class="grid g3">
<div class="card"><h3>Basic</h3><div class="price">PKR 5,000</div><p>1-Page Website</p></div>
<div class="card"><h3>Standard</h3><div class="price">PKR 15,000</div><p>Business Website</p></div>
<div class="card"><h3>Premium</h3><div class="price">PKR 30,000+</div><p>E-Commerce / Custom</p></div>
</div>
<p class="sub">*Price depends on client demand & features</p>
</section>

<section id="payment">
<h2>Payment Methods</h2>
<div class="pay">
<button onclick="copyPay('03379827882')">EasyPaisa</button>
<button onclick="copyPay('03705519562')">JazzCash</button>
<button onclick="copyPay('03705519562')">SadaPay</button>
<button onclick="copyPay('nazimkhan01123@gmail.com')">Payoneer</button>
<button onclick="copyPay('TTSxm4pBK26RB4vXaa3Uo3hqGa5HdhxBDR')">Binance (TRC20)</button>
<p id="copymsg"></p>
</div>
<br>
<a class="btn" href="mailto:nazimkhan01123@gmail.com?subject=Payment%20Details&body=Method:%0AAmount:%0ATransaction%20ID:">
Send Payment Details via Email
</a>
</section>

<section id="contact">
<h2>Contact Us</h2>
<p class="sub">
Email:
<a href="mailto:nazimkhan01123@gmail.com" style="color:#22c55e">nazimkhan01123@gmail.com</a>
</p>
</section>

<footer>
<a href="https://www.facebook.com" target="_blank"><i class="fab fa-facebook"></i></a>
<a href="https://www.instagram.com" target="_blank"><i class="fab fa-instagram"></i></a>
<a href="mailto:nazimkhan01123@gmail.com"><i class="fa fa-envelope"></i></a>
<p style="margin-top:14px;color:#94a3b8">© 2026 Web-Hub</p>
</footer>

<div class="popup" id="pop">
<div class="popup-box">
<h3>👋 Still here?</h3>
<p>Let’s build something amazing together 🚀</p>
<button class="btn" onclick="closePop()">Close</button>
</div>
</div>

<script>
function copyPay(t){navigator.clipboard.writeText(t);document.getElementById('copymsg').innerText='Copied: '+t;}
setTimeout(()=>{document.getElementById('pop').style.display='flex';},60000);
function closePop(){document.getElementById('pop').style.display='none';}
</script>

</body>
</html>
