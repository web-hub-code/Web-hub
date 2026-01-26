<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MrKhan PRO Services</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap');
body{margin:0;padding:0;font-family:'Orbitron',sans-serif;background:#0a0a0a;color:#fff;scroll-behavior:smooth;transition:0.3s;}
body.light{background:#f5f5f5;color:#111;}
.container{max-width:460px;margin:20px auto;padding:20px;background:linear-gradient(135deg,#111,#1a1a2e);border-radius:15px;box-shadow:0 0 25px rgba(0,0,0,0.7);transition:0.3s;}
body.light .container{background:#fff;color:#111;box-shadow:0 0 20px rgba(0,0,0,0.2);}
.hero{text-align:center;padding:20px 0;border-radius:10px;position:relative;overflow:hidden;}
.hero h1{font-size:24px;margin:0 0 5px 0;text-shadow:0 0 10px #00ffff;}
.hero p{font-size:14px;color:#ccc;}
.hero video{width:100%;border-radius:10px;}
h2{font-size:18px;color:#ff00ff;border-bottom:1px solid #ff00ff;padding-bottom:5px;margin-bottom:10px;}
.services li{margin-bottom:10px;font-size:14px;position:relative;cursor:pointer;}
.services li span.tooltip{display:none;position:absolute;left:105%;top:50%;transform:translateY(-50%);background:rgba(255,0,255,0.9);padding:5px 8px;border-radius:5px;white-space:nowrap;font-size:12px;}
.services li:hover span.tooltip{display:block;}
.portfolio{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:15px;}
.portfolio img{width:100%;border-radius:8px;transition:0.3s;}
.portfolio img:hover{transform:scale(1.05);}
.counters{display:flex;justify-content:space-between;margin:15px 0;}
.counters div{text-align:center;}
.counters div h3{font-size:20px;margin:0;color:#00ffff;}
.counters div p{font-size:12px;color:#ccc;}
.progress-bar{background:#222;border-radius:10px;overflow:hidden;height:10px;margin-top:5px;}
.progress-bar span{display:block;height:100%;background:#00ffff;width:0;}
.pricing{display:flex;flex-direction:column;gap:10px;margin-bottom:20px;}
.pricing div{background: rgba(255,255,255,0.05);padding:12px;border-radius:10px;text-align:center;transition:0.3s;}
.pricing div:hover{transform:scale(1.05);background:#ff00ff;color:#000;}
.pricing div span{font-weight:bold;color:#00ffff;}
.testimonials{overflow:hidden;height:140px;margin-bottom:15px;}
.testimonials ul{display:flex;animation:slide 60s linear infinite;padding:0;margin:0;}
.testimonials li{flex:0 0 100%;list-style:none;padding:10px;box-sizing:border-box;}
.star{color:#ff0;}
.faq li{cursor:pointer;background: rgba(255,255,255,0.05);padding:8px;border-radius:8px;margin-bottom:5px;}
.faq li span.answer{display:none;font-size:13px;color:#ccc;margin-top:5px;}
.btn{display:block;width:90%;margin:8px auto;padding:12px;border-radius:10px;background:linear-gradient(45deg,#00f,#ff0044);color:#fff;font-weight:bold;text-align:center;text-decoration:none;transition:0.3s;}
.btn:hover{transform:scale(1.05);background:linear-gradient(45deg,#ff0044,#00ffff);color:#000;}
form{display:flex;flex-direction:column;gap:10px;margin-bottom:15px;}
form input, form textarea, form select{padding:10px;border-radius:8px;border:none;outline:none;font-size:14px;}
form button{padding:12px;border-radius:10px;border:none;font-weight:bold;background:#00ffff;color:#000;cursor:pointer;transition:0.3s;}
form button:hover{background:#ff00ff;color:#fff;}
.floating-email{position:fixed;bottom:20px;right:20px;background:#ff0044;color:#fff;padding:15px;border-radius:50%;text-align:center;font-size:20px;z-index:1000;text-decoration:none;}
.sticky-cta{position:fixed;bottom:0;left:0;width:100%;background:#111;color:#fff;text-align:center;padding:10px;font-weight:bold;cursor:pointer;z-index:999;border-top:3px solid #00ffff;}
@keyframes slide{0%{transform:translateX(0);}100%{transform:translateX(-100%);}}
.reveal{opacity:0;transform:translateY(20px);transition:0.6s;}
.reveal.active{opacity:1;transform:translateY(0);}
footer{margin-top:20px;padding:15px;background:#111;border-radius:12px;text-align:left;font-size:12px;color:#ccc;}
footer a{color:#00ffff;text-decoration:none;}
footer ul{list-style:disc;margin-left:15px;}
.light-toggle{position:fixed;top:20px;right:20px;background:#00ffff;color:#000;padding:10px;border-radius:50%;cursor:pointer;z-index:1000;}
@media only screen and (max-width:500px){h1{font-size:20px;}h2{font-size:16px;}.btn,form input,form textarea,form select,form button{font-size:13px;}.container{padding:15px;}.portfolio{grid-template-columns:1fr;}}
</style>
</head>
<body>

<div class="light-toggle" onclick="document.body.classList.toggle('light')">🌞/🌙</div>

<div class="container">

<div class="hero reveal">
<h1>🚀 Boost Your Online Presence</h1>
<p>Websites, Videos & Branding by MrKhan</p>
<video src="https://www.w3schools.com/html/mov_bbb.mp4" controls muted autoplay loop></video>
</div>

<h2 class="reveal">Services</h2>
<ul class="services reveal">
<li>💻 Custom Websites <span class="tooltip">Responsive & modern websites</span></li>
<li>🔐 Firebase Login/Signup <span class="tooltip">Secure authentication system</span></li>
<li>🎬 Video Editing <span class="tooltip">Reels, Shorts, YouTube</span></li>
<li>🖼 Thumbnails & Branding <span class="tooltip">Eye-catching design</span></li>
</ul>

<h2 class="reveal">Portfolio</h2>
<div class="portfolio reveal">
<img src="https://picsum.photos/200/120?random=1" alt="Website Example">
<img src="https://picsum.photos/200/120?random=2" alt="Thumbnail">
<img src="https://picsum.photos/200/120?random=3" alt="Video">
<img src="https://picsum.photos/200/120?random=4" alt="Logo">
<img src="https://picsum.photos/200/120?random=5" alt="Website Example">
<img src="https://picsum.photos/200/120?random=6" alt="Thumbnail">
<img src="https://picsum.photos/200/120?random=7" alt="Video">
<img src="https://picsum.photos/200/120?random=8" alt="Logo">
</div>

<h2 class="reveal">Our Stats</h2>
<div class="counters reveal">
<div><h3>500+</h3><p>Satisfied Clients</p><div class="progress-bar"><span style="width:80%"></span></div></div>
<div><h3>150+</h3><p>Websites Delivered</p><div class="progress-bar"><span style="width:75%"></span></div></div>
<div><h3>300+</h3><p>Videos Edited</p><div class="progress-bar"><span style="width:90%"></span></div></div>
</div>

<h2 class="reveal">Premium Packages</h2>
<div class="pricing reveal">
<div>Basic <span>Specified for Clients 5000+</span></div>
<div>Standard <span>Specified for Clients 5000+</span></div>
<div>Premium <span>Specified for Clients 5000+</span></div>
</div>

<h2 class="reveal">Testimonials</h2>
<div class="testimonials reveal">
<ul>
<li>“Amazing website!” <span class="star">★★★★★</span> — Ahmed</li>
<li>“Social reach doubled!” <span class="star">★★★★★</span> — Sana</li>
<li>“Fast & professional!” <span class="star">★★★★★</span> — Ali</li>
<li>“Creative thumbnails!” <span class="star">★★★★★</span> — Zara</li>
<li>“Very affordable!” <span class="star">★★★★★</span> — Bilal</li>
</ul>
</div>

<h2 class="reveal">FAQ</h2>
<ul class="faq reveal">
<li onclick="toggleAnswer(this)">Delivery Time? <span class="answer">1-3 days depending on complexity.</span></li>
<li onclick="toggleAnswer(this)">Revisions? <span class="answer">Free revisions until satisfaction.</span></li>
<li onclick="toggleAnswer(this)">Social Media Content? <span class="answer">Yes, Reels, Shorts & thumbnails included.</span></li>
</ul>

<h2 class="reveal">Contact / Request Service</h2>
<form class="reveal" action="mailto:nazimkhan01123@gmail.com" method="post" enctype="text/plain">
<input type="text" name="Name" placeholder="Your Name" required>
<input type="email" name="Email" placeholder="Your Email" required>
<select name="Service" required>
<option value="">Select Service</option>
<option>Custom Website</option>
<option>Firebase Login/Signup</option>
<option>Video Editing</option>
<option>Thumbnails & Branding</option>
</select>
<textarea name="Message" placeholder="Your Message" rows="3" required></textarea>
<button type="submit">Send Message</button>
</form>

<a class="btn reveal" href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank">Instagram</a>
<a class="btn reveal" href="https://www.facebook.com/share/184Khe9iZu/" target="_blank">Facebook</a>
<a class="btn reveal" href="mailto:nazimkhan01123@gmail.com">Email</a>

</div>

<div class="sticky-cta reveal" onclick="window.scrollTo({top:0,behavior:'smooth'})">⬆ Back to Top / Request Service</div>

<a href="mailto:nazimkhan01123@gmail.com" class="floating-email" target="_blank">📧</a>

<footer class="reveal">
<h3>About MrKhan PRO Services</h3>
<p>We provide premium websites, video editing, thumbnails & branding services. Trusted by over 5000 clients worldwide, our professional services ensure top-notch results every time.</p>
<p>Benefits:</p>
<ul>
<li>Responsive & modern websites</li>
<li>Secure Firebase login/signup integration</li>
<li>Engaging video content & creative thumbnails</li>
<li>Trusted by thousands of clients globally</li>
<li>Fast delivery & free revisions</li>
<li>Premium customer support</li>
<li>High-quality branding solutions</li>
</ul>
<p>Contact via <a href="mailto:nazimkhan01123@gmail.com">Email</a>, <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank">Instagram</a>, <a href="https://www.facebook.com/share/184Khe9iZu/" target="_blank">Facebook</a>.</p>
<p>© 2026 MrKhan PRO Services. All Rights Reserved.</p>
</footer>

<script>
function toggleAnswer(el){ let ans = el.querySelector(".answer"); ans.style.display = (ans.style.display==="block")?"none":"block";}
window.addEventListener('scroll', ()=>{document.querySelectorAll('.reveal').forEach(el=>{let top = el.getBoundingClientRect().top;let height = window.innerHeight;if(top < height-50){el.classList.add('active');}});});
</script>

</body>
</html>
