<html lang="en">
<head>
<meta charset="UTF-8">
<title>Web-Hub | Pro Digital Solutions</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.css"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick-theme.min.css"/>

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Poppins,sans-serif}
body{background:#0b1120;color:#e5e7eb;line-height:1.6}
a{text-decoration:none;color:inherit}
.container{width:90%;max-width:1200px;margin:auto}
section{padding:80px 0}

/* HERO */
.hero{
background:linear-gradient(to right,rgba(2,6,23,.9),rgba(2,6,23,.6)),
url("https://images.unsplash.com/photo-1498050108023-c5249f4df085") center/cover;
padding:120px 0;
text-align:center;
animation: fadeIn 2s ease;
}
.hero h1{font-size:52px;color:#22c55e;animation: slideIn 1.5s ease;}
.hero p{margin:20px 0;max-width:600px;margin-left:auto;margin-right:auto}
.btn{background:#22c55e;padding:12px 28px;border-radius:30px;font-weight:600;display:inline-block}
.btn:hover{background:#16a34a}

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
}
.card:hover{transform:translateY(-10px);}
.card i{font-size:36px;color:#38bdf8;margin-bottom:15px}

/* TITLES */
h2{text-align:center;font-size:38px;margin-bottom:50px}
.center{text-align:center}

/* IMAGES */
img{width:100%;border-radius:16px;}

/* STATS */
.stats h3{font-size:40px;color:#22c55e}
.counter{font-weight:bold;color:#22c55e;font-size:32px}

/* FAQ */
details{
background:#020617;
padding:18px;
border-radius:12px;
margin-bottom:10px;
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
</style>
</head>

<body>

<!-- HERO -->
<section class="hero">
<div class="container">
<h1>Web-Hub</h1>
<p>Professional Website Development, UI/UX Design, SEO & Digital Marketing Solutions</p>
<a href="#contact" class="btn">Start Your Project</a>
</div>
</section>

<!-- SERVICES -->
<section>
<div class="container">
<h2>Our Services</h2>
<div class="grid grid-4">
<div class="card"><i class="fa-solid fa-code"></i><h3>Web Development</h3><p>Fast, secure & scalable websites</p></div>
<div class="card"><i class="fa-solid fa-paintbrush"></i><h3>UI/UX Design</h3><p>Modern & user-friendly designs</p></div>
<div class="card"><i class="fa-solid fa-chart-line"></i><h3>SEO Optimization</h3><p>Rank higher on search engines</p></div>
<div class="card"><i class="fa-solid fa-bullhorn"></i><h3>Digital Marketing</h3><p>Grow your online presence</p></div>
</div>
</div>
</section>

<!-- PORTFOLIO SLIDER -->
<section>
<div class="container">
<h2>Our Work</h2>
<div class="portfolio-slider">
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">
<img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4">
<img src="https://images.unsplash.com/photo-1558655146-9f40138edfeb">
<img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c">
</div>
</div>
</section>

<!-- TESTIMONIALS SLIDER -->
<section>
<div class="container">
<h2>Client Reviews</h2>
<div class="testimonial-slider">
<div class="card"><p>"Great service! Highly recommended."</p><strong>- John D.</strong></div>
<div class="card"><p>"Professional & fast delivery."</p><strong>- Sarah K.</strong></div>
<div class="card"><p>"Our website looks amazing thanks to Web-Hub."</p><strong>- Mike L.</strong></div>
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
<section>
<div class="container">
<h2>FAQs</h2>
<div class="grid grid-2">
<details><summary>Are images showing correctly?</summary><p>Yes, all images are stock CDN links for guaranteed display.</p></details>
<details><summary>Is the site mobile-friendly?</summary><p>Yes, fully responsive on all devices.</p></details>
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

<!-- FLOATING SOCIAL BUTTONS -->
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
$('.counter').each(function(){$(this).prop('Counter',0).animate({Counter:$(this).text()}, {duration:2000, easing:'swing', step:function(now){$(this).text(Math.ceil(now));}});});
// EmailJS Contact
emailjs.init("YOUR_USER_ID"); // replace with your EmailJS userID
document.getElementById('contact-form').addEventListener('submit', function(event){
event.preventDefault();
emailjs.sendForm('YOUR_SERVICE_ID','YOUR_TEMPLATE_ID',this)
.then(function(){alert("Message sent successfully!");},function(err){alert("Error sending message: "+JSON.stringify(err));});
});
</script>
</body>
</html>
