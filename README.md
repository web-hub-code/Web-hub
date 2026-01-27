<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Khan Studio | Neon Digital Hub</title>
<meta name="description" content="Khan Studio - Premium Neon Digital Services: Websites, Video Editing, Thumbnails, Branding, SEO & Social Media Marketing.">
<meta property="og:title" content="Khan Studio | Neon Digital Hub">
<meta property="og:description" content="Professional Neon Digital Services: Websites, Video Editing, Thumbnails, Branding, SEO & Social Media.">
<meta property="og:type" content="website">
<meta property="og:url" content="https://web-hub-code.github.io/Web-hub/">
<link rel="icon" href="https://picsum.photos/32/32" type="image/png">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<style>
/* ===== General Reset ===== */
*{margin:0;padding:0;box-sizing:border-box;font-family:'Roboto',sans-serif;scroll-behavior:smooth;}
body{background:linear-gradient(135deg,#0f0f0f,#120028,#1a0028,#000000);color:#fff;transition:0.5s;overflow-x:hidden;}
a{text-decoration:none;color:#00ffff;transition:0.3s;}
a:hover{color:#ff0040;}

/* ===== Preloader ===== */
#preloader{position:fixed;top:0;left:0;width:100%;height:100%;background:#000;display:flex;justify-content:center;align-items:center;z-index:10000;}
#preloader .loader{width:50px;height:50px;border:5px solid #ff0040;border-top:5px solid #00ffff;border-radius:50%;animation:spin 1s linear infinite;}
@keyframes spin{0%{transform:rotate(0deg);}100%{transform:rotate(360deg);}}

/* ===== Header / Hero ===== */
header{position:relative;height:80vh;display:flex;justify-content:center;align-items:center;text-align:center;overflow:hidden;}
header::before{content:"";position:absolute;top:0;left:0;width:100%;height:100%;background:radial-gradient(circle,rgba(255,0,64,0.2),rgba(0,64,255,0.2),rgba(0,0,0,0.8));animation:moveBg 30s linear infinite;z-index:1;}
header h1{position:relative;font-size:4em;z-index:2;color:#fff;animation:neonPulse 2s ease-in-out infinite;}
header .cta-buttons{position:relative;z-index:2;margin-top:20px;}
header .cta-buttons button{margin:0 10px;padding:15px 25px;border:none;border-radius:5px;background:#ff0040;color:#fff;font-weight:bold;cursor:pointer;box-shadow:0 0 10px #00ffff;transition:0.3s;text-transform:uppercase;}
header .cta-buttons button:hover{background:#00ffff;color:#000;box-shadow:0 0 20px #ff0040,0 0 40px #00ffff;}
@keyframes neonPulse{0%{text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}50%{text-shadow:0 0 15px #ff0040,0 0 30px #0040ff,0 0 60px #ff0040;}100%{text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}}
@keyframes moveBg{0%{background-position:0 0;}100%{background-position:1000px 1000px;}}

/* ===== Sections ===== */
section{padding:50px 20px;}
h2{text-align:center;font-size:2.5em;color:#00ffff;text-shadow:0 0 5px #ff0040;margin-bottom:30px;position:relative;}
h2::after{content:"";width:60px;height:3px;background:#ff0040;display:block;margin:10px auto;border-radius:2px;}

/* ===== Cards ===== */
.card{background:rgba(255,255,255,0.05);padding:20px;border-radius:10px;flex:1 1 300px;text-align:left;transition:0.3s;box-shadow:0 0 10px rgba(0,255,255,0.3);margin-bottom:20px;}
.card:hover{transform:scale(1.03);box-shadow:0 0 20px #ff0040,0 0 40px #0040ff;}

/* ===== Services ===== */
.services{display:flex;flex-wrap:wrap;gap:20px;justify-content:center;}

/* ===== Portfolio / Sliders ===== */
.slider{position:relative;overflow:hidden;width:90%;margin:auto;}
.slider-track{display:flex;transition:0.5s;}
.slider-card{min-width:300px;margin:10px;flex-shrink:0;background:rgba(255,255,255,0.05);padding:20px;border-radius:10px;box-shadow:0 0 10px rgba(0,255,255,0.3);transition:0.3s;}
.slider-card:hover{transform:scale(1.03);box-shadow:0 0 20px #ff0040,0 0 40px #0040ff;}
.slider-btn{position:absolute;top:50%;transform:translateY(-50%);background:#00ffff;color:#000;border:none;padding:10px;cursor:pointer;border-radius:5px;transition:0.3s;}
.slider-btn:hover{background:#ff0040;color:#fff;}
.slider-btn.prev{left:10px;}
.slider-btn.next{right:10px;}

/* ===== Reviews ===== */
.photo-circle{width:60px;height:60px;border-radius:50%;border:3px solid #00ffff;margin-right:10px;object-fit:cover;}

/* ===== Stats ===== */
.stats-section{display:flex;flex-wrap:wrap;gap:20px;justify-content:center;}

/* ===== FAQ ===== */
.faq-section{display:flex;flex-direction:column;gap:10px;align-items:center;}
.faq-card{background:rgba(255,255,255,0.05);padding:15px;border-radius:10px;width:100%;cursor:pointer;box-shadow:0 0 10px rgba(0,255,255,0.3);}
.faq-card:hover{box-shadow:0 0 20px #ff0040,0 0 40px #0040ff;}
.faq-content{max-height:0;overflow:hidden;transition:max-height 0.3s ease;}

/* ===== Contact ===== */
form{display:flex;flex-direction:column;gap:15px;max-width:500px;margin:auto;}
input,select,textarea{padding:10px;border-radius:5px;border:1px solid #ccc;background:#111;color:#fff;}
input::placeholder,textarea::placeholder{color:#888;}
button{padding:15px;border:none;border-radius:5px;background:#ff0040;color:#fff;font-weight:bold;cursor:pointer;transition:0.3s;box-shadow:0 0 5px #00ffff;text-transform:uppercase;}
button:hover{background:#00ffff;color:#000;box-shadow:0 0 15px #ff0040,0 0 30px #00ffff;}

/* ===== Footer ===== */
footer{background:rgba(0,0,0,0.05);padding:30px 20px;text-align:center;color:#fff;}

/* ===== Back to top ===== */
#topBtn{position:fixed;bottom:20px;right:20px;padding:10px 15px;background:#00ffff;color:#000;border:none;border-radius:5px;cursor:pointer;display:none;z-index:1000;transition:0.3s;}
#topBtn:hover{background:#ff0040;color:#fff;}

/* ===== Responsive ===== */
@media(max-width:768px){.services,.portfolio,.stats-section,.reviews,.faq-section,.ads-section{flex-direction:column;}header h1{font-size:2em;}}
</style>
</head>
<body>

<!-- ===== Preloader ===== -->
<div id="preloader"><div class="loader"></div></div>

<!-- ===== Header / Hero ===== -->
<header>
<h1>Khan Studio</h1>
<div class="cta-buttons">
<button onclick="document.getElementById('portfolio').scrollIntoView({behavior:'smooth'})">View Portfolio</button>
<button onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Contact Me</button>
</div>
</header>

<!-- ===== About ===== -->
<section id="about">
<h2>About Khan Studio</h2>
<p style="text-align:left;">
Khan Studio provides **premium neon digital services** including Website Development, Video Editing, Thumbnails, Branding, SEO & Social Media Marketing. Modern, glowing, and professional results for every client.
</p>
</section>

<!-- ===== Services ===== -->
<section id="services">
<h2>Our Services</h2>
<div class="services">
<div class="card"><h3>Website Development</h3><p>Responsive websites with modern UI/UX, SEO optimized, e-commerce and dynamic pages.</p></div>
<div class="card"><h3>Video Editing</h3><p>Professional editing with effects, color grading, intros/outros, motion graphics.</p></div>
<div class="card"><h3>Thumbnails & Graphics</h3><p>Eye-catching thumbnails, banners, logos for branding and social media.</p></div>
<div class="card"><h3>Branding & Marketing</h3><p>Complete branding: logos, brand kits, social media identity.</p></div>
<div class="card"><h3>SEO & Social Media</h3><p>Improve search visibility and engagement across platforms.</p></div>
</div>
</section>

<!-- ===== Portfolio ===== -->
<section id="portfolio">
<h2>Portfolio</h2>
<div class="slider">
<button class="slider-btn prev">&#10094;</button>
<div class="slider-track">
<div class="slider-card"><h3>Website Projects</h3><p>Modern websites for businesses, blogs, and e-commerce.</p></div>
<div class="slider-card"><h3>Video Projects</h3><p>Professional video edits with effects and transitions.</p></div>
<div class="slider-card"><h3>Graphics & Branding</h3><p>Thumbnails, logos, banners, and full brand kits.</p></div>
</div>
<button class="slider-btn next">&#10095;</button>
</div>
</section>

<!-- ===== Ads ===== -->
<section id="ads">
<h2>Trusted Ads</h2>
<div class="slider">
<button class="slider-btn prev">&#10094;</button>
<div class="slider-track">
<div class="slider-card"><p>🔥 Boost Your Brand with Khan Studio!</p></div>
<div class="slider-card"><p>🚀 Premium Digital Services Available!</p></div>
<div class="slider-card"><p>💎 Trusted Solutions for Modern Businesses</p></div>
</div>
<button class="slider-btn next">&#10095;</button>
</div>
</section>

<!-- ===== Stats ===== -->
<section id="stats">
<h2>Achievements</h2>
<div class="stats-section">
<div class="card"><h3>8000+</h3><p>Satisfied Clients</p></div>
<div class="card"><h3>1200+</h3><p>Websites Delivered</p></div>
<div class="card"><h3>3500+</h3><p>Videos Edited</p></div>
<div class="card"><h3>1500+</h3><p>Thumbnails Delivered</p></div>
</div>
</section>

<!-- ===== Reviews ===== -->
<section id="reviews">
<h2>Client Reviews</h2>
<div class="slider">
<button class="slider-btn prev">&#10094;</button>
<div class="slider-track">
<!-- Example Reviews -->
<div class="slider-card" style="display:flex;align-items:center;"><img src="https://picsum.photos/60/60?random=1" class="photo-circle"><div><p>"Excellent service!"</p><p>- Ali ⭐⭐⭐⭐⭐</p></div></div>
<div class="slider-card" style="display:flex;align-items:center;"><img src="https://picsum.photos/60/60?random=2" class="photo-circle"><div><p>"Creative designs and edits!"</p><p>- Sara ⭐⭐⭐⭐⭐</p></div></div>
<div class="slider-card" style="display:flex;align-items:center;"><img src="https://picsum.photos/60/60?random=3" class="photo-circle"><div><p>"Fast and professional!"</p><p>- Hassan ⭐⭐⭐⭐⭐</p></div></div>
<!-- Add more reviews similarly up to 25 -->
</div>
<button class="slider-btn next">&#10095;</button>
</div>
</section>

<!-- ===== FAQ ===== -->
<section id="faq">
<h2>FAQ</h2>
<div class="faq-section">
<div class="faq-card"><h3>How can I order a service?</h3><div class="faq-content"><p>Fill the contact form or reach via email/social links.</p></div></div>
<div class="faq-card"><h3>Delivery Time?</h3><div class="faq-content"><p>1–7 days depending on service complexity.</p></div></div>
<div class="faq-card"><h3>Do you provide revisions?</h3><div class="faq-content"><p>Yes, unlimited revisions until satisfaction.</p></div></div>
</div>
</section>

<!-- ===== Contact ===== -->
<section id="contact">
<h2>Contact Me</h2>
<form action="https://formspree.io/f/yourformid" method="POST">
<input type="text" name="name" placeholder="Your Name" required autocomplete="name">
<input type="email" name="email" placeholder="Your Email" required autocomplete="email">
<textarea name="message" placeholder="Describe your project" required autocomplete="on"></textarea>
<button type="submit">Send Message</button>
</form>
<p style="text-align:center;margin-top:15px;">📧 <a href="mailto:rock.earn92@gmail.com">rock.earn92@gmail.com</a> | 🌐 <a href="#" target="_blank">Facebook</a> | 📸 <a href="#" target="_blank">Instagram</a></p>
</section>

<!-- ===== Footer ===== -->
<footer>
<h3>Khan Studio</h3>
<p>Professional digital services including websites, video editing, thumbnails & branding. Neon premium interface for modern businesses and creators.</p>
<p>© 2026 Khan Studio. All Rights Reserved.</p>
</footer>

<!-- ===== Back to Top ===== -->
<button onclick="window.scrollTo({top:0,behavior:'smooth'})" id="topBtn">Top</button>

<!-- ===== JS ===== -->
<script>
// Preloader
window.addEventListener('load',()=>{document.getElementById('preloader').style.display='none';});

// FAQ toggle
const faqCards=document.querySelectorAll('.faq-card');
faqCards.forEach(card=>{card.addEventListener('click',()=>{let content=card.querySelector('.faq-content');content.style.maxHeight=content.style.maxHeight?null:content.scrollHeight+"px";});});

// Sliders
const sliders=document.querySelectorAll('.slider');
sliders.forEach(slider=>{
const track=slider.querySelector('.slider-track');
const prev=slider.querySelector('.prev');
const next=slider.querySelector('.next');
let index=0;
slider.setAttribute('data-index',0);
prev.addEventListener('click',()=>{index--; if(index<0) index=track.children.length-1; slider.setAttribute('data-index',index); track.style.transform=`translateX(-${index*320}px)`;});
next.addEventListener('click',()=>{index++; if(index>=track.children.length) index=0; slider.setAttribute('data-index',index); track.style.transform=`translateX(-${index*320}px)`;});
});
// Auto-play sliders
setInterval(()=>{
sliders.forEach(slider=>{
const track=slider.querySelector('.slider-track');
let index=parseInt(slider.getAttribute('data-index'))||0;
index++; if(index>=track.children.length) index=0;
slider.setAttribute('data-index',index);
track.style.transform=`translateX(-${index*320}px)`;
});
},3000);

// Back to top
const topBtn=document.getElementById('topBtn');
window.onscroll=function(){if(document.body.scrollTop>300||document.documentElement.scrollTop>300){topBtn.style.display="block";}else{topBtn.style.display="none";}};
</script>

</body>
</html>
