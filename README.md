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

/* STATS */
.stats h3{font-size:40px;color:#22c55e}
.counter{font-weight:bold;color:#22c55e;font-size:32px}

/* FAQ */
details{background:#1e293b;padding:18px;border-radius:12px;margin-bottom:10px;cursor:pointer;transition:.3s}
details:hover{background:#273449}
details summary{cursor:pointer;font-weight:600}

/* CONTACT FORM */
input,textarea,select{width:100%;padding:12px;border-radius:10px;border:none;margin-bottom:10px;background:#0f172a;color:#e5e7eb}
button.btn.submit-btn{background:#22c55e;padding:12px 28px;border-radius:30px;font-weight:600;display:inline-block;transition:.3s;color:#fff;border:none;cursor:pointer}
button.btn.submit-btn:hover{background:#16a34a;transform:scale(1.05)}/* CONTINUATION OF STYLE */
.floating-social{position:fixed;right:20px;bottom:20px;display:flex;flex-direction:column;gap:12px;z-index:9999}
.floating-social a{width:52px;height:52px;border-radius:50%;display:flex;align-items:center;justify-content:center;color:#fff;font-size:22px;box-shadow:0 8px 20px rgba(0,0,0,.4);transition:transform .3s}
.floating-social a:hover{transform:scale(1.1)}
.email{background:#22c55e}
.instagram{background:linear-gradient(45deg,#f58529,#dd2a7b,#8134af)}
.facebook{background:#1877f2}

/* Animations */
@keyframes fadeIn{from{opacity:0}to{opacity:1}}
@keyframes slideIn{from{transform:translateY(-50px);opacity:0}to{transform:translateY(0);opacity:1}}

/* Back-to-top */
#topBtn{position:fixed;bottom:90px;right:20px;z-index:9999;background:#22c55e;color:#fff;padding:12px 15px;border:none;border-radius:50%;font-size:18px;cursor:pointer;display:none}
#topBtn:hover{background:#16a34a;transform:scale(1.1)}
</style>
</head>
<body>

<!-- PRICING -->
<section id="pricing">
<div class="container">
<h2>Pricing Plans</h2>
<div class="grid grid-3">
<div class="card">
<h3>Basic</h3>
<p>PKR 5,000 / USD 15 <br><small>Depends on client demand</small></p>
<button class="btn" onclick="manualPayment('Basic', 'PKR 5,000 / USD 15')">Get Started</button>
</div>
<div class="card">
<h3>Standard</h3>
<p>PKR 10,000 / USD 30 <br><small>Depends on client demand</small></p>
<button class="btn" onclick="manualPayment('Standard', 'PKR 10,000 / USD 30')">Get Started</button>
</div>
<div class="card">
<h3>Premium</h3>
<p>PKR 15,000 / USD 45 <br><small>Depends on client demand</small></p>
<button class="btn" onclick="manualPayment('Premium', 'PKR 15,000 / USD 45')">Get Started</button>
</div>
</div>
</div>
</section>

<!-- PAYMENT METHODS -->
<section id="payments">
<div class="container">
<h2>Payment Methods</h2>
<p>Select your preferred payment method and copy the account details:</p>
<div class="grid grid-2">
<div class="card">
<h3>Easypaisa</h3>
<p id="easypaisaNumber">03379827882 <button onclick="copyToClipboard('easypaisaNumber')">Copy</button></p>
</div>
<div class="card">
<h3>JazzCash</h3>
<p id="jazzcashNumber">03705519562 <button onclick="copyToClipboard('jazzcashNumber')">Copy</button></p>
</div>
<div class="card">
<h3>SadaPay</h3>
<p id="sadaPayNumber">03705519562 <button onclick="copyToClipboard('sadaPayNumber')">Copy</button></p>
</div>
<div class="card">
<h3>Payoneer</h3>
<p id="payoneerEmail">nazimkhan01123@gmail.com <button onclick="copyToClipboard('payoneerEmail')">Copy</button></p>
</div>
<div class="card">
<h3>Binance (TRC20)</h3>
<p id="binanceWallet">TTSxm4pBK26RB4vXaa3Uo3hqGa5HdhxBDR <button onclick="copyToClipboard('binanceWallet')">Copy</button></p>
</div>
</div>
</div>
</section>

<!-- PORTFOLIO (clickable details) -->
<section id="portfolio">
<div class="container">
<h2>Our Work</h2>
<div class="grid grid-3">
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">
<div class="overlay">
<h3>Project 1: Modern Website Design</h3>
<p>HTML5, CSS3, JavaScript, Responsive, SEO Optimized</p>
<a href="#" class="btn">View Project</a>
</div>
</div>
<div class="portfolio-item">
<img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4">
<div class="overlay">
<h3>Project 2: Mobile App UI/UX</h3>
<p>Android & iOS, User-friendly UI, Modern Design</p>
<a href="#" class="btn">View Project</a>
</div>
</div>
<!-- Add more portfolio items as needed -->
</div>
</div>
</section>

<!-- CONTACT FORM -->
<section id="contact">
<div class="container grid grid-2">
<div>
<h2>Contact Us</h2>
<p>Email: webhub262@gmail.com</p>
<p>Send your message and payment details; we'll respond ASAP.</p>
</div>
<form class="card" onsubmit="sendEmail(event)">
<input type="text" id="name" placeholder="Your Name" required>
<input type="email" id="email" placeholder="Your Email" required>
<select id="paymentMethod" required>
<option value="">Select Payment Method</option>
<option value="Easypaisa">Easypaisa</option>
<option value="JazzCash">JazzCash</option>
<option value="SadaPay">SadaPay</option>
<option value="Payoneer">Payoneer</option>
<option value="Binance">Binance</option>
</select>
<input type="text" id="transactionID" placeholder="Transaction ID / Screenshot Link" required>
<textarea id="message" rows="5" placeholder="Additional Message / Request" required></textarea>
<button class="btn submit-btn" type="submit">Send Message</button>
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
<script>
// Back to top
window.onscroll=function(){scrollFunction()};
function scrollFunction(){document.getElementById("topBtn").style.display=(document.body.scrollTop>20||document.documentElement.scrollTop>20)?"block":"none"}
function topFunction(){document.body.scrollTop=0;document.documentElement.scrollTop=0}

// Copy account numbers
function copyToClipboard(id){
let copyText=document.getElementById(id).innerText.split(" ")[0];
navigator.clipboard.writeText(copyText);
alert(copyText+" copied to clipboard!");
}

// Counter Animation
const counters=document.querySelectorAll(".counter");
counters.forEach(counter=>{
counter.innerText="0";
const updateCounter=()=>{
const target=+counter.getAttribute("data-target");
const c=+counter.innerText;
const increment=target/200;
if(c<target){counter.innerText=Math.ceil(c+increment);setTimeout(updateCounter,10);}else{counter.innerText=target;}
};
updateCounter();
});

// Send Email with form
function sendEmail(event){
event.preventDefault();
const name=document.getElementById("name").value;
const email=document.getElementById("email").value;
const method=document.getElementById("paymentMethod").value;
const transaction=document.getElementById("transactionID").value;
const message=document.getElementById("message").value;
const subject="Web-Hub Payment / Query from "+name;
const body=`Name: ${name}%0D%0AEmail: ${email}%0D%0APayment Method: ${method}%0D%0ATransaction ID / Screenshot: ${transaction}%0D%0AMessage: ${message}`;
window.location.href=`mailto:webhub262@gmail.com?subject=${subject}&body=${body}`;
alert("Email client opened. Please send the email.");
}
</script>
</body>
</html>
