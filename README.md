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

        /* Background Visuals */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .overlay-fx { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle at 50% 50%, transparent 10%, #000 90%); z-index: -1; }

        /* Header Cover */
        .header-cover { width: 100%; height: 300px; position: relative; overflow: hidden; border-bottom: 3px solid var(--primary); }
        .cover-img { width: 100%; height: 100%; object-fit: cover; filter: brightness(0.5); }
        .cover-fade { position: absolute; bottom: 0; width: 100%; height: 100px; background: linear-gradient(to top, var(--bg), transparent); }

        .container { width: 100%; max-width: 550px; margin: -90px auto 0; padding: 0 15px 50px; position: relative; z-index: 10; }

        /* Profile Hub */
        .profile-section { text-align: center; margin-bottom: 25px; }
        .profile-img { width: 150px; height: 150px; border-radius: 50%; border: 4px solid var(--primary); box-shadow: 0 0 40px rgba(0, 242, 254, 0.5); object-fit: cover; background: #000; }
        .pulse-badge { display: inline-block; padding: 6px 16px; background: rgba(0, 255, 136, 0.1); border: 1px solid #00ff88; color: #00ff88; border-radius: 50px; font-size: 0.7rem; margin-top: 15px; font-weight: 800; animation: pulse 2s infinite; }
        @keyframes pulse { 0% { opacity: 1; } 50% { opacity: 0.5; } 100% { opacity: 1; } }

        /* Cards */
        .card { background: var(--glass); backdrop-filter: blur(50px); border: 1px solid var(--border); border-radius: 40px; padding: 30px; margin-bottom: 25px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); transform: translateY(-5px); }
        .logo-main { font-size: 3.5rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--secondary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-transform: uppercase; text-align: center; letter-spacing: -2px; }

        /* Service Hub */
        .service-box { display: block; text-decoration: none; color: white; background: rgba(255,255,255,0.03); border: 1px solid var(--border); padding: 25px; border-radius: 30px; margin-bottom: 15px; transition: 0.3s; }
        .service-box:hover { background: rgba(0, 242, 254, 0.1); border-color: var(--primary); }
        .service-box h4 { color: var(--primary); font-size: 1.1rem; margin-bottom: 8px; font-weight: 800; display: flex; align-items: center; gap: 10px; }
        .service-box p { font-size: 0.8rem; opacity: 0.7; line-height: 1.6; }

        /* Footer (As per HighLevel Screenshot) */
        .footer-elite { text-align: left; padding: 40px 20px; background: rgba(0,0,0,0.5); border-radius: 35px; border: 1px solid var(--border); }
        .hq-title { color: white; font-weight: 800; font-size: 1.2rem; margin-bottom: 20px; letter-spacing: 2px; }
        .hq-info { font-size: 0.9rem; opacity: 0.7; line-height: 1.8; margin-bottom: 25px; border-left: 2px solid var(--primary); padding-left: 15px; }
        
        .social-icons { display: flex; gap: 15px; margin-top: 20px; }
        .social-icons a { width: 45px; height: 45px; background: var(--glass); border: 1px solid var(--border); display: flex; align-items: center; justify-content: center; border-radius: 50%; color: white; text-decoration: none; transition: 0.3s; font-size: 1.2rem; }
        .social-icons a:hover { background: var(--primary); color: #000; transform: scale(1.1); }

        .legal-area { margin-top: 40px; text-align: center; border-top: 1px solid var(--border); padding-top: 30px; }
        .legal-links { display: flex; justify-content: center; gap: 15px; font-size: 0.7rem; opacity: 0.6; margin-top: 15px; }
        .legal-links a { color: white; text-decoration: none; }

        footer { text-align: center; padding: 40px; opacity: 0.2; font-size: 0.7rem; letter-spacing: 5px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay-fx"></div>

    <div class="header-cover">
        <img src="FB_IMG_1769869953605.jpg" class="cover-img" alt="Web-Hub Agency">
        <div class="cover-fade"></div>
    </div>

    <div class="container">
        <div class="profile-section" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" class="profile-img" alt="Muhammad Nazim">
            <br>
            <div class="pulse-badge">🟢 WEB-HUB GLOBAL ONLINE</div>
        </div>

        <section class="card" data-aos="fade-up">
            <h1 class="logo-main">Web-Hub</h1>
            <p style="text-align: center; font-size: 0.85rem; line-height: 1.6; opacity: 0.8; margin-top: 15px;">
                Muhammad Nazim ki sarbarahi mein, Web-Hub aapke har digital khuwab ko haqiqat banata hai.
            </p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-th-large"></i> Our Expertise</h3>
            
            <a href="https://wa.me/923332637235" target="_blank" class="service-box">
                <h4><i class="fas fa-code"></i> Web Development</h4>
                <p>Premium websites jo fast aur SEO friendly hon.</p>
            </a>

            <a href="https://wa.me/923332637235" target="_blank" class="service-box">
                <h4><i class="fas fa-palette"></i> UI/UX Design</h4>
                <p>Modern layouts aur branding designs.</p>
            </a>
        </div>

        <section class="footer-elite card" data-aos="fade-up">
            <div class="hq-title">CONTACT US</div>
            <div class="hq-info">
                <strong>Corporate HQ</strong><br>
                Karachi, Pakistan | Web-Hub Center<br>
                Suite 262, Online Excellence<br>
                Toll Free: <a href="tel:+923332637235" style="color: var(--primary); text-decoration: none;">+92 333 2637235</a>
            </div>

            <div class="hq-title">SOCIAL CONNECT</div>
            <div class="social-icons">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank"><i class="fab fa-facebook-f"></i></a>
                <a href="https://wa.me/923332637235" target="_blank"><i class="fab fa-whatsapp"></i></a>
                <a href="mailto:webhub262@gmail.com"><i class="fas fa-envelope"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-linkedin-in"></i></a>
            </div>

            <div class="legal-area">
                <h2 style="font-weight: 800; font-size: 1.8rem;">Web-Hub</h2>
                <div style="font-size: 0.7rem; opacity: 0.5; margin: 15px 0;">
                    © 2026 Web-Hub, Inc. | All Rights Reserved<br>
                    Official Portal of Muhammad Nazim
                </div>
                <div class="legal-links">
                    <a href="#">Privacy Policy</a>
                    <a href="#">Terms</a>
                    <a href="#">Security</a>
                </div>
            </div>
        </section>

        <footer>BEYOND THE LIMITS | WEB-HUB 2026</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 1000, once: true });</script>
</body>
</html>
