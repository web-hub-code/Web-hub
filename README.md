<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Khan Studio | Neon Premium Digital Services</title>
<meta name="description" content="Khan Studio - Website Development, Video Editing, Branding, Thumbnails, SEO & Social Media Services. Neon premium modern interface.">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Roboto',sans-serif;}
body{background:linear-gradient(135deg,#0f0f0f,#120028,#1a0028,#000000);color:#fff;scroll-behavior:smooth;transition:0.5s;}
a{text-decoration:none;color:#00ffff;transition:0.3s;}
a:hover{color:#ff0040;}
h1,h2,h3{font-weight:700;text-transform:uppercase;text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}
h2{color:#00ffff;text-align:center;margin-bottom:30px;position:relative;}
h2::after{content:"";width:60px;height:3px;background:#ff0040;display:block;margin:10px auto;border-radius:2px;}
header{position:relative;height:70vh;display:flex;justify-content:center;align-items:center;text-align:center;overflow:hidden;}
header::before{content:"";position:absolute;top:0;left:0;width:100%;height:100%;background:radial-gradient(circle,rgba(255,0,64,0.2),rgba(0,64,255,0.2),rgba(0,0,0,0.8)); z-index:1;animation:moveBackground 30s linear infinite;}
header h1{position:relative;z-index:2;font-size:3em;animation:neonPulse 2s ease-in-out infinite;}
@keyframes neonPulse{0%{text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}50%{text-shadow:0 0 15px #ff0040,0 0 30px #0040ff,0 0 60px #ff0040;}100%{text-shadow:0 0 5px #ff0040,0 0 10px #0040ff,0 0 20px #ff0040;}}
@keyframes moveBackground{0%{background-position:0 0;}100%{background-position:1000px 1000px;}}
.card{background:rgba(255,255,255,0.05);padding:20px;border-radius:10px;flex:1 1 300px;text-align:left;transition:0.3s;box-shadow:0 0 10px rgba(0,255,255,0.3);margin-bottom:20px;}
.card:hover{transform:scale(1.03);box-shadow:0 0 20px #ff0040,0 0 40px #0040ff;}
.services,.portfolio,.stats-section,.reviews,.faq-section,.ads-section{display:flex;flex-wrap:wrap;gap:20px;justify-content:center;}
button{padding:15px;border:none;border-radius:5px;background:#ff0040;color:#fff;font-weight:bold;cursor:pointer;transition:0.3s;box-shadow:0 0 5px #00ffff;text-transform:uppercase;}
button:hover{background:#00ffff;color:#000;box-shadow:0 0 15px #ff0040,0 0 30px #00ffff;}
form{display:flex;flex-direction:column;gap:15px;max-width:500px;margin:auto;}
input,select,textarea{padding:10px;border-radius:5px;border:1px solid #ccc;background:#111;color:#fff;}
input::placeholder,textarea::placeholder{color:#888;}
.photo-circle{width:60px;height:60px;border-radius:50%;border:3px solid #00ffff;margin-right:10px;object-fit:cover;}
footer{background:rgba(0,0,0,0.05);padding:30px 20px;text-align:center;color:#fff;}
#topBtn{position:fixed;bottom:20px;right:20px;padding:10px 15px;background:#00ffff;color:#000;border:none;border-radius:5px;cursor:pointer;display:none;z-index:1000;transition:0.3s;}
#topBtn:hover{background:#ff0040;color:#fff;}
.faq-card{background:rgba(255,255,255,0.05);padding:15px;border-radius:10px;width:100%;cursor:pointer;box-shadow:0 0 10px rgba(0,255,255,0.3);margin-bottom:10px;}
.faq-card:hover{box-shadow:0 0 20px #ff0040,0 0 40px #0040ff;}
.faq-content{max-height:0;overflow:hidden;transition:max-height 0.3s ease;}
.slider{position:relative;overflow:hidden;width:90%;margin:auto;}
.slider-track{display:flex;transition:0.5s;}
.slider-card{min-width:300px;margin:10px;flex-shrink:0;background:rgba(255,255,255,0.05);padding:20px;border-radius:10px;box-shadow:0 0 10px rgba(0,255,255,0.3);transition:0.3s;}
.slider-card:hover{transform:scale(1.03);box-shadow:0 0 20px #ff0040,0 0 40px #0040ff;}
.slider-btn{position:absolute;top:50%;transform:translateY(-50%);background:#00ffff;color:#000;border:none;padding:10px;cursor:pointer;border-radius:5px;transition:0.3s;}
.slider-btn:hover{background:#ff0040;color:#fff;}
.slider-btn.prev{left:10px;}
.slider-btn.next{right:10px;}
@media(max-width:768px){.services,.portfolio,.stats-section,.reviews,.faq-section,.ads-section{flex-direction:column;}header h1{font-size:2em;}}
</style>
</head>
<body>

<header><h1>Khan Studio</h1></header>

<section id="about">
<h2>About Khan Studio</h2>
<p style="text-align:left;">
Khan Studio provides premium digital services: Website Development, Video Editing, Branding, Thumbnails, SEO & Social Media. We deliver **modern, neon-glowing, professional results** for every client.
</p>
</section>

<section id="services">
<h2>Our Services</h2>
<div class="services">
<div class="card"><h3>Website Development</h3><p>Responsive websites with modern UI/UX, e-commerce, SEO optimized.</p></div>
<div class="card"><h3>Video Editing</h3><p>Professional editing with color grading, intros/outros, motion graphics.</p></div>
<div class="card"><h3>Thumbnails & Graphics</h3><p>Eye-catching thumbnails, banners, logos for branding and social media.</p></div>
<div class="card"><h3>Branding & Marketing</h3><p>Complete branding: logos, brand kits, social media identity.</p></div>
<div class="card"><h3>SEO & Social Media</h3><p>Improve search visibility and engagement for all platforms.</p></div>
</div>
</section>

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

<section id="stats">
<h2>Achievements</h2>
<div class="stats-section">
<div class="card"><h3>8000+</h3><p>Satisfied Clients</p></div>
<div class="card"><h3>1200+</h3><p>Websites Delivered</p></div>
<div class="card"><h3>3500+</h3><p>Videos Edited</p></div>
<div class="card"><h3>1500+</h3><p>Thumbnails Delivered</p></div>
</div>
</section>

<section id="reviews">
<h2>Client Reviews</h2>
<div class="slider">
<button class="slider-btn prev">&#10094;</button>
<div class="slider-track">
<!-- 25 reviews with picsum placeholders -->
<div class="slider-card" style="display:flex;align-items:center;"><img src="https://picsum.photos/60/60?random=1" class="photo-circle"><div><p>"Excellent service!"</p><p>- Ali</p></div></div>
<div class="slider-card" style="display:flex;align-items:center;"><img src="https://picsum.photos/60/60?random=2" class="photo-circle"><div><p>"Creative designs and edits!"</p><p>- Sara</p></div></div>
<div class="slider-card" style="display:flex;align-items:center;"><img src="https://picsum.photos/60/60?random=3" class="photo-circle"><div><p>"Fast and professional!"</p><p>- Hassan</p></div></div>
<div class="slider-card" style="display:flex;align-items:center;"><img src="https://picsum.photos/60/60?random=4" class="photo-circle"><div><p>"Highly recommend Khan Studio."</p><p>- Zoya</p></div></div>
<!-- Add up to 25 reviews in same style -->
</div>
<button class="slider-btn next">&#10095;</button>
</div>
</section>

<section id="faq">
<h2>FAQ</h2>
<div class="faq-section">
<div class="faq-card"><h3>How can I order a service?</h3><div class="faq-content"><p>Fill the contact form or reach via email/social links.</p></div></div>
<div class="faq-card"><h3>Delivery Time?</h3><div class="faq-content"><p>1–7 days depending on service complexity.</p></div></div>
<div class="faq-card"><h3>Do you provide revisions?</h3><div class="faq-content"><p>Yes, unlimited revisions until satisfaction.</p></div></div>
</div>
</section>

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

<footer>
<h3>Khan Studio</h3>
<p>Professional digital services including websites, video editing, thumbnails & branding. Neon premium interface for modern businesses and creators.</p>
<p>© 2026 Khan Studio. All Rights Reserved.</p>
</footer>

<button onclick="window.scrollTo({top:0,behavior:'smooth'})" id="topBtn">Top</button>

<script>
// FAQ toggle
const faqCards=document.querySelectorAll('.faq-card');
faqCards.forEach(card=>{card.addEventListener('click',()=>{card.classList.toggle('active');});});

// Sliders manual + auto-play
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
index++;
if(index>=track.children.length) index=0;
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
