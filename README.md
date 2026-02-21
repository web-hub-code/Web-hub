<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub | Muhammad Nazim Official Agency</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #7000ff;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Background Visuals */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .glow-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle at 50% 50%, transparent 20%, #000 100%); z-index: -1; }

        /* Cover & Profile */
        .cover-box { width: 100%; height: 280px; position: relative; overflow: hidden; border-bottom: 2px solid var(--primary); }
        .cover-img { width: 100%; height: 100%; object-fit: cover; filter: brightness(0.6); }
        .container { width: 100%; max-width: 550px; margin: -90px auto 0; padding: 0 15px 120px; position: relative; z-index: 10; }
        .p-wrap { text-align: center; margin-bottom: 20px; }
        .p-img { width: 145px; height: 145px; border-radius: 50%; border: 4px solid var(--primary); box-shadow: 0 0 30px rgba(0, 242, 254, 0.4); object-fit: cover; }

        /* Card Master Style */
        .card { background: var(--glass); backdrop-filter: blur(45px); border: 1px solid var(--border); border-radius: 40px; padding: 30px; margin-bottom: 25px; transition: 0.3s; }
        .card:hover { border-color: var(--primary); }

        /* Text Styles */
        .h-logo { font-size: 3.2rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--secondary)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-transform: uppercase; text-align: center; }
        .sub-text { text-align: center; letter-spacing: 5px; font-size: 0.75rem; opacity: 0.7; margin: 10px 0 20px; }

        /* Service List (Detailed) */
        .service-item { display: block; text-decoration: none; color: white; background: rgba(255,255,255,0.03); border: 1px solid var(--border); padding: 20px; border-radius: 25px; margin-bottom: 15px; transition: 0.3s; }
        .service-item:hover { background: rgba(0, 242, 254, 0.1); border-color: var(--primary); transform: translateX(10px); }
        .service-head { display: flex; align-items: center; gap: 12px; margin-bottom: 8px; font-weight: 800; color: var(--primary); }
        .service-desc { font-size: 0.8rem; opacity: 0.6; line-height: 1.5; }

        /* Contact Dock */
        .nav-dock { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 92%; background: rgba(0,0,0,0.85); backdrop-filter: blur(35px); border-radius: 40px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; box-shadow: 0 10px 40px rgba(0,0,0,0.5); }
        .nav-btn { color: white; font-size: 1.4rem; transition: 0.3s; opacity: 0.6; }
        .nav-btn:hover { color: var(--primary); opacity: 1; transform: scale(1.2); }

        /* Footer HQ (HighLevel Style) */
        .hq-box { text-align: left; border-top: 1px solid var(--border); padding-top: 25px; }
        .hq-title { color: var(--primary); font-weight: 800; font-size: 1.1rem; margin-bottom: 15px; }
        .hq-detail { font-size: 0.9rem; opacity: 0.7; line-height: 1.8; margin-bottom: 25px; }
        .social-row { display: flex; gap: 20px; margin-bottom: 30px; }
        .social-row a { color: white; font-size: 1.3rem; transition: 0.3s; }
        .social-row a:hover { color: var(--primary); }

        footer { text-align: center; padding-bottom: 40px; opacity: 0.3; font-size: 0.7rem; letter-spacing: 3px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="glow-overlay"></div>

    <div class="cover-box">
        <img src="FB_IMG_1769869953605.jpg" class="cover-img" alt="Web-Hub Agency">
    </div>

    <nav class="nav-dock">
        <a href="#" class="nav-btn"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-btn"><i class="fab fa-whatsapp"></i></a>
        <a href="tel:+923332637235" class="nav-btn"><i class="fas fa-phone-alt"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-btn"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-btn"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <div class="p-wrap" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" class="p-img" alt="Muhammad Nazim">
            <div style="margin-top: 10px; color: #00ff88; font-size: 0.7rem; font-weight: 800;">● VERIFIED AGENCY OWNER</div>
        </div>

        <section class="card" data-aos="fade-up">
            <h1 class="h-logo">Web-Hub</h1>
            <p class="sub-text">OFFICIAL DIGITAL PORTAL</p>
            <p style="text-align: center; font-size: 0.85rem; opacity: 0.8; line-height: 1.6;">
                Hum technology aur creativity ko mila kar aapke business ko brand banate hain. Web-Hub aapka bharosay mand digital partner hai.
            </p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-stars"></i> Our Expert Services</h3>
            
            <a href="https://wa.me/923332637235?text=I%20want%20to%20order%20a%20Professional%20Website" class="service-item">
                <div class="service-head"><i class="fas fa-code"></i> High-End Web Development</div>
                <div class="service-desc">Personal blogs se lekar heavy E-commerce stores tak, hum fast aur secure websites banate hain.</div>
            </a>

            <a href="https://wa.me/923332637235?text=I%20want%20to%20order%20Graphic%20Designing" class="service-item">
                <div class="service-head"><i class="fas fa-paint-brush"></i> Creative UI/UX Design</div>
                <div class="service-desc">Logo, Social Media Posts, aur Website UI jo aapke brand ki value barha dega.</div>
            </a>

            <a href="https://wa.me/923332637235?text=I%20want%20SEO%20and%20Marketing" class="service-item">
                <div class="service-head"><i class="fas fa-bullhorn"></i> SEO & Digital Growth</div>
                <div class="service-desc">Google ranking aur social media ads ke zariye aapke sales aur reach ko double karein.</div>
            </a>
        </div>

        <section class="card hq-box" data-aos="fade-up">
            <div class="hq-title">CONTACT US</div>
            <div class="hq-detail">
                <strong>Corporate HQ</strong><br>
                Karachi, Pakistan | Web-Hub Center<br>
                Suite 262, Online Digital Solutions<br>
                Toll Free: <a href="tel:+923332637235" style="color: var(--primary); text-decoration: none;">+92 333 2637235</a>
            </div>

            <div class="hq-title">SOCIALS</div>
            <div class="social-row">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank"><i class="fab fa-facebook-f"></i></a>
                <a href="https://wa.me/923332637235" target="_blank"><i class="fab fa-whatsapp"></i></a>
                <a href="mailto:webhub262@gmail.com"><i class="fas fa-envelope"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-linkedin"></i></a>
            </div>

            <div style="text-align: center; border-top: 1px solid var(--border); padding-top: 30px;">
                <h2 style="font-weight: 800; font-size: 1.5rem; letter-spacing: -1px;"><i class="fas fa-cubes" style="color: var(--primary);"></i> Web-Hub</h2>
                <div style="font-size: 0.75rem; opacity: 0.5; margin-top: 10px;">
                    © 2026 Web-Hub, Inc. | All Rights Reserved<br>
                    Do Not Sell or Share My Information
                </div>
                <div style="display: flex; justify-content: center; gap: 15px; font-size: 0.7rem; opacity: 0.6; margin-top: 15px;">
                    <a href="#" style="color: white; text-decoration: none;">Privacy Policy</a>
                    <a href="#" style="color: white; text-decoration: none;">Terms of Service</a>
                    <a href="#" style="color: white; text-decoration: none;">Security</a>
                </div>
            </div>
        </section>

        <footer>OFFICIAL IDENTITY OF MUHAMMAD NAZIM</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 1000, once: true });</script>
</body>
</html>
