<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub | Muhammad Nazim | Global Agency</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;900&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #7000ff;
            --success: #00ff88; --bg: #010204; --glass: rgba(255, 255, 255, 0.03);
            --border: rgba(0, 242, 254, 0.25);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Background */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 0%, #000 100%); z-index: -1; }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 40px 18px 100px; }

        /* Card System */
        .glass-card { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 40px; padding: 35px; margin-bottom: 25px; transition: 0.4s; position: relative; }
        .glass-card:hover { border-color: var(--primary); transform: translateY(-5px); }

        .brand-logo { font-size: 3.8rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--success)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-align: center; letter-spacing: -2px; }

        /* Interactive Stats */
        .stats-box { display: flex; justify-content: space-around; margin: 30px 0; text-align: center; }
        .stat-val { font-size: 1.5rem; font-weight: 900; color: var(--primary); display: block; }
        .stat-lab { font-size: 0.65rem; opacity: 0.5; letter-spacing: 2px; text-transform: uppercase; }

        /* Live Portfolio Slider */
        .swiper { width: 100%; border-radius: 25px; margin: 20px 0; border: 1px solid var(--border); }
        .swiper-slide img { width: 100%; height: 250px; object-fit: cover; filter: brightness(0.8); }

        /* Feature List (Clickable) */
        .feat-item { display: flex; align-items: center; gap: 15px; padding: 20px; background: rgba(255,255,255,0.02); border: 1px solid var(--border); border-radius: 20px; margin-bottom: 15px; cursor: pointer; transition: 0.3s; }
        .feat-item:hover { background: rgba(0, 242, 254, 0.1); border-color: var(--primary); }
        .feat-item i { font-size: 1.5rem; color: var(--success); }

        /* Ultimate Button */
        .main-btn { display: flex; align-items: center; justify-content: center; gap: 12px; width: 100%; padding: 22px; background: linear-gradient(45deg, var(--primary), var(--secondary)); border-radius: 25px; color: #000; font-weight: 900; text-decoration: none; text-transform: uppercase; margin-top: 15px; box-shadow: 0 10px 30px rgba(0, 242, 254, 0.3); transition: 0.4s; }
        .main-btn:hover { transform: scale(1.02); box-shadow: 0 15px 40px rgba(0, 242, 254, 0.5); }

        /* Footer (Corporate Elite) */
        .footer-hq { background: rgba(0,0,0,0.85); border: 1px solid var(--border); border-radius: 45px; padding: 45px 30px; }
        .hq-line { border-left: 3px solid var(--primary); padding-left: 20px; margin-bottom: 30px; }
        
        .social-wrap { display: flex; gap: 12px; margin: 30px 0; flex-wrap: wrap; }
        .social-btn { width: 50px; height: 50px; background: var(--glass); border: 1px solid var(--border); border-radius: 50%; display: flex; align-items: center; justify-content: center; color: white; text-decoration: none; font-size: 1.3rem; transition: 0.4s; }
        .social-btn:hover { background: var(--primary); color: #000; transform: rotate(360deg); }

        /* Modal Overlay */
        .modal { display: none; position: fixed; z-index: 10000; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.95); backdrop-filter: blur(15px); }
        .modal-card { background: #0a0a0a; margin: 15% auto; padding: 40px; border: 1px solid var(--primary); width: 90%; max-width: 450px; border-radius: 40px; text-align: center; position: relative; }
        .close-btn { position: absolute; top: 15px; right: 20px; font-size: 30px; color: var(--primary); cursor: pointer; }

        footer { text-align: center; padding: 50px; opacity: 0.3; font-size: 0.7rem; letter-spacing: 5px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        
        <section class="glass-card" data-aos="zoom-in">
            <h1 class="brand-logo">Web-Hub</h1>
            <div class="stats-box">
                <div><span class="stat-val">150+</span><span class="stat-lab">Projects</span></div>
                <div><span class="stat-val">99%</span><span class="stat-lab">Trust</span></div>
                <div><span class="stat-val">24/7</span><span class="stat-lab">Support</span></div>
            </div>
            <p style="text-align: center; font-size: 0.9rem; opacity: 0.7; line-height: 1.8;">
                Welcome to the digital era. Web-Hub provides next-gen web development and branding solutions under the leadership of Muhammad Nazim.
            </p>
        </section>

        <div class="swiper mySwiper" data-aos="fade-up">
            <div class="swiper-wrapper">
                <div class="swiper-slide"><img src="FB_IMG_1769869953605.jpg" alt="Work 1"></div>
                <div class="swiper-slide"><img src="Snapchat-2096615446.jpg" alt="Work 2"></div>
                <div class="swiper-slide"><img src="FB_IMG_1769869953605.jpg" alt="Work 3"></div>
            </div>
            <div style="text-align: center; padding: 10px; font-size: 0.7rem; opacity: 0.5;">Swipe to see our work</div>
        </div>

        <div data-aos="fade-up">
            <div class="feat-item" onclick="openDetails('AI Web Solutions', 'Hum websites ko AI features ke sath build karte hain jo customers se khud baat karti hain aur sales barhati hain.')">
                <i class="fas fa-microchip"></i>
                <div>
                    <h4 style="color: var(--primary);">AI Web Solutions</h4>
                    <p style="font-size: 0.75rem; opacity: 0.6;">Smart websites with automation.</p>
                </div>
            </div>

            <div class="feat-item" onclick="openDetails('Digital Branding', 'Logos, Social Media kit, aur complete brand guidelines jo aapke business ko aik international brand banati hain.')">
                <i class="fas fa-palette"></i>
                <div>
                    <h4 style="color: var(--primary);">Full Branding</h4>
                    <p style="font-size: 0.75rem; opacity: 0.6;">Visuals that tell your story.</p>
                </div>
            </div>

            <a href="https://wa.me/923332637235?text=Hi%20Nazim!%20I%20am%20interested%20in%20Web-Hub%20services.%20Let's%20discuss%20pricing." class="main-btn">
                <i class="fab fa-whatsapp"></i> Chat With Specialist
            </a>
        </div>

        <section class="footer-hq" data-aos="fade-up" style="margin-top: 40px;">
            <div class="hq-line">
                <h3 style="letter-spacing: 2px;">CORPORATE HEADQUARTERS</h3>
                <p style="opacity: 0.7; font-size: 0.9rem; margin-top: 10px;">
                    Suite 262, Online Excellence Towers<br>
                    Karachi, Pakistan | Web-Hub Global<br>
                    Toll Free: <a href="tel:+923332637235" style="color: var(--primary); text-decoration: none;">+92 333 2637235</a>
                </p>
            </div>

            <div class="social-wrap">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-btn"><i class="fab fa-facebook-f"></i></a>
                <a href="https://wa.me/923332637235" target="_blank" class="social-btn"><i class="fab fa-whatsapp"></i></a>
                <a href="mailto:webhub262@gmail.com" class="social-btn"><i class="fas fa-envelope"></i></a>
                <a href="#" class="social-btn"><i class="fab fa-instagram"></i></a>
                <a href="#" class="social-btn"><i class="fab fa-linkedin-in"></i></a>
            </div>

            <div style="text-align: center; border-top: 1px solid rgba(255,255,255,0.1); padding-top: 30px;">
                <h2 style="font-weight: 900; font-size: 2.5rem; letter-spacing: -1.5px;">Web-Hub</h2>
                <p style="font-size: 0.7rem; opacity: 0.4; margin: 10px 0;">© 2026 Web-Hub, Inc. | Muhammad Nazim Signature Project</p>
                <div style="display: flex; justify-content: center; gap: 15px; font-size: 0.75rem;">
                    <span style="color: var(--primary); cursor: pointer;" onclick="openDetails('Privacy Policy', 'Aapka data 100% secure hai. Hum koi bhi information third-party ke sath share nahi karte.')">Privacy</span>
                    <span style="color: var(--primary); cursor: pointer;" onclick="openDetails('Terms', 'Projects 50% advance par start hote hain. Delivery time project ke scope par depend karta hai.')">Terms</span>
                    <span style="color: var(--primary); cursor: pointer;" onclick="openDetails('Security', 'Our sites use SSL encryption and high-level firewall protection.')">Security</span>
                </div>
            </div>
        </section>

        <footer>BEYOND THE LIMITS • 2026</footer>
    </div>

    <div id="infoModal" class="modal">
        <div class="modal-card">
            <span class="close-btn" onclick="closeDetails()">&times;</span>
            <h3 id="modalTitle" style="color: var(--primary); margin-bottom: 20px;"></h3>
            <p id="modalBody" style="font-size: 0.9rem; line-height: 1.8; opacity: 0.8;"></p>
            <a href="https://wa.me/923332637235" class="main-btn" style="padding: 15px; font-size: 0.8rem; margin-top: 25px;">Book a Session</a>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        
        var swiper = new Swiper(".mySwiper", {
            loop: true,
            autoplay: { delay: 3000 },
        });

        function openDetails(t, b) {
            document.getElementById('modalTitle').innerText = t;
            document.getElementById('modalBody').innerText = b;
            document.getElementById('infoModal').style.display = "block";
        }
        function closeDetails() {
            document.getElementById('infoModal').style.display = "none";
        }
        window.onclick = function(e) { if(e.target.className == 'modal') closeDetails(); }
    </script>
</body>
</html>
