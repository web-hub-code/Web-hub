<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub Official | Muhammad Nazim</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #7000ff;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Animated Tech BG */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 20%, #000 100%); z-index: -1; }

        /* Header & Profile */
        .cover-box { width: 100%; height: 320px; position: relative; overflow: hidden; border-bottom: 3px solid var(--primary); }
        .cover-img { width: 100%; height: 100%; object-fit: cover; filter: brightness(0.5); }
        .container { width: 100%; max-width: 600px; margin: -100px auto 0; padding: 0 15px 80px; position: relative; z-index: 10; }
        .p-wrap { text-align: center; margin-bottom: 25px; }
        .p-img { width: 160px; height: 160px; border-radius: 50%; border: 5px solid var(--primary); box-shadow: 0 0 40px rgba(0, 242, 254, 0.6); object-fit: cover; }

        /* Elite Card & Typography */
        .card { background: var(--glass); backdrop-filter: blur(50px); border: 1px solid var(--border); border-radius: 40px; padding: 35px; margin-bottom: 30px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); transform: translateY(-5px); }
        .logo-main { font-size: 3.8rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-align: center; letter-spacing: -2px; }

        /* Pricing Grid */
        .price-table { display: grid; grid-template-columns: 1fr; gap: 15px; margin-top: 20px; }
        .price-item { background: rgba(255,255,255,0.03); border: 1px solid var(--border); border-radius: 25px; padding: 25px; text-align: center; transition: 0.3s; }
        .price-item:hover { border-color: var(--primary); background: rgba(0, 242, 254, 0.05); }
        .price-title { font-size: 1.4rem; color: var(--primary); font-weight: 800; }
        .price-tag { font-size: 2rem; margin: 10px 0; font-weight: 800; }
        .price-features { font-size: 0.85rem; opacity: 0.7; list-style: none; line-height: 2; margin-bottom: 20px; }

        /* Testimonials */
        .testimonial { font-style: italic; font-size: 0.9rem; opacity: 0.8; margin-bottom: 15px; border-left: 3px solid var(--primary); padding-left: 15px; }
        .client-name { font-weight: 800; color: var(--secondary); font-size: 0.8rem; text-transform: uppercase; }

        /* Action Buttons */
        .btn-order { display: inline-block; width: 100%; padding: 15px; background: linear-gradient(45deg, var(--primary), var(--secondary)); border-radius: 15px; color: #000; font-weight: 800; text-decoration: none; text-transform: uppercase; font-size: 0.9rem; transition: 0.3s; }
        .btn-order:hover { letter-spacing: 2px; box-shadow: 0 0 20px var(--primary); }

        /* Footer (HighLevel Screenshot Style) */
        .footer-elite { text-align: left; padding: 40px 25px; background: rgba(0,0,0,0.8); border-radius: 40px; border: 1px solid var(--border); }
        .hq-title { color: white; font-weight: 800; font-size: 1.3rem; margin-bottom: 20px; letter-spacing: 2px; border-bottom: 2px solid var(--primary); display: inline-block; padding-bottom: 5px; }
        .hq-info { font-size: 0.95rem; opacity: 0.7; line-height: 2; margin-bottom: 30px; }
        
        .social-row { display: flex; gap: 15px; margin-top: 20px; }
        .social-link { width: 50px; height: 50px; background: var(--glass); border: 1px solid var(--border); display: flex; align-items: center; justify-content: center; border-radius: 50%; color: white; text-decoration: none; font-size: 1.3rem; transition: 0.3s; }
        .social-link:hover { background: var(--primary); color: #000; transform: rotate(360deg); }

        .legal { text-align: center; margin-top: 40px; border-top: 1px solid var(--border); padding-top: 30px; }
        .legal-links { display: flex; justify-content: center; gap: 20px; font-size: 0.75rem; opacity: 0.6; margin-top: 15px; }
        .legal-links a { color: white; text-decoration: none; }

        footer { text-align: center; padding: 40px; opacity: 0.2; font-size: 0.75rem; letter-spacing: 4px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="cover-box">
        <img src="FB_IMG_1769869953605.jpg" class="cover-img" alt="Web-Hub Agency">
    </div>

    <div class="container">
        <div class="p-wrap" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" class="p-img" alt="Muhammad Nazim">
            <div style="margin-top: 15px; color: #00ff88; font-weight: 800; font-size: 0.75rem; letter-spacing: 2px;">● AGENCY FOUNDER & LEAD DEVELOPER</div>
        </div>

        <section class="card" data-aos="fade-up">
            <h1 class="logo-main">Web-Hub</h1>
            <p style="text-align: center; opacity: 0.6; letter-spacing: 8px; font-size: 0.7rem; margin-bottom: 20px;">DIGITAL EMPIRE</p>
            <p style="text-align: center; line-height: 1.8; opacity: 0.9;">
                Web-Hub aik premium software house hai jo Karachi, Pakistan se operate hota hai. Humne worldwide clients ko modern web apps, SEO strategies, aur stunning graphics ke zariye grow karne mein help ki hai. Humara waada hai quality aur fast delivery.
            </p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 25px;"><i class="fas fa-tags"></i> Premium Packages</h3>
            <div class="price-table">
                <div class="price-item">
                    <div class="price-title">Startup Web</div>
                    <div class="price-tag">$99 <span style="font-size: 0.8rem; opacity: 0.5;">/ Only</span></div>
                    <ul class="price-features">
                        <li>5 Pages Professional Site</li>
                        <li>Responsive Design</li>
                        <li>SEO Optimized</li>
                        <li>1 Month Free Support</li>
                    </ul>
                    <a href="https://wa.me/923332637235?text=Hi%20Nazim!%20I%20want%20the%20Startup%20Web%20Package." class="btn-order">Select Package</a>
                </div>
                
                <div class="price-item" style="border-color: var(--primary);">
                    <div class="price-title">Elite E-Commerce</div>
                    <div class="price-tag">$249 <span style="font-size: 0.8rem; opacity: 0.5;">/ Only</span></div>
                    <ul class="price-features">
                        <li>Unlimited Products Store</li>
                        <li>Payment Integration</li>
                        <li>Inventory Management</li>
                        <li>Lifetime Hosting Access</li>
                    </ul>
                    <a href="https://wa.me/923332637235?text=Hi%20Nazim!%20I%20want%20the%20Elite%20E-Commerce%20Package." class="btn-order">Select Package</a>
                </div>
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-quote-left"></i> Client Success Stories</h3>
            <div class="testimonial">
                "Web-Hub ne meri purani website ko bilkul modern look diya. Meri sales 40% barh gayi hain!"
                <div class="client-name">— Ahmed Khan, CEO of AK Tech</div>
            </div>
            <div class="testimonial">
                "Nazim bhai ki delivery speed aur quality kamal ki hai. Highly recommended for graphics!"
                <div class="client-name">— Sarah J., Brand Manager</div>
            </div>
        </div>

        <section class="footer-elite card" data-aos="fade-up">
            <div class="hq-title">CORPORATE OFFICE</div>
            <div class="hq-info">
                <strong>Main Headquarters</strong><br>
                Karachi, Pakistan | Web-Hub Hub Center<br>
                Suite 262, Online Excellence Towers<br>
                Toll Free: <a href="tel:+923332637235" style="color: var(--primary); text-decoration: none;">+92 333 2637235</a><br>
                Support: webhub262@gmail.com
            </div>

            <div class="hq-title">GLOBAL CONNECT</div>
            <div class="social-row">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-link"><i class="fab fa-facebook-f"></i></a>
                <a href="https://wa.me/923332637235" target="_blank" class="social-link"><i class="fab fa-whatsapp"></i></a>
                <a href="mailto:webhub262@gmail.com" class="social-link"><i class="fas fa-envelope"></i></a>
                <a href="#" class="social-link"><i class="fab fa-linkedin-in"></i></a>
                <a href="#" class="social-link"><i class="fab fa-instagram"></i></a>
            </div>

            <div class="legal">
                <h2 style="font-weight: 900; letter-spacing: -1px; font-size: 2.2rem;">Web-Hub</h2>
                <div style="font-size: 0.75rem; opacity: 0.5; margin: 15px 0;">
                    © 2026 Web-Hub, Inc. • A Muhammad Nazim Signature Project<br>
                    Global Digital Agency Solutions
                </div>
                <div class="legal-links">
                    <a href="#">Privacy Policy</a>
                    <a href="#">Terms of Service</a>
                    <a href="#">Security</a>
                </div>
            </div>
        </section>

        <footer>BEYOND THE LIMITS • POWERED BY NAZIM • 2026</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 1000, once: true });</script>
</body>
</html>
