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
            --glow: 0 0 20px rgba(0, 242, 254, 0.4);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; scroll-behavior: smooth; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        /* Background Visuals */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .gradient-bg { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle at 50% 50%, transparent 20%, #000 100%); z-index: -1; }

        /* Header Cover */
        .cover-wrap { width: 100%; height: 260px; position: relative; overflow: hidden; }
        .cover-photo { width: 100%; height: 100%; object-fit: cover; filter: brightness(0.5) contrast(1.1); }
        .cover-fade { position: absolute; bottom: 0; width: 100%; height: 100px; background: linear-gradient(to top, var(--bg), transparent); }

        .container { width: 100%; max-width: 550px; margin: -80px auto 0; padding: 0 15px 120px; position: relative; z-index: 10; }

        /* Profile & Branding */
        .profile-area { text-align: center; margin-bottom: 20px; }
        .p-pic { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); box-shadow: var(--glow); object-fit: cover; background: #000; }
        .live-badge { display: inline-block; padding: 4px 12px; background: rgba(0, 255, 136, 0.15); border: 1px solid #00ff88; color: #00ff88; border-radius: 50px; font-size: 0.65rem; margin-top: 10px; font-weight: 800; text-transform: uppercase; letter-spacing: 1px; }

        /* Elite Cards */
        .card { background: var(--glass); backdrop-filter: blur(45px); border: 1px solid var(--border); border-radius: 35px; padding: 30px; margin-bottom: 25px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); transform: translateY(-5px); }
        .h-title { font-size: 3rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--secondary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-transform: uppercase; line-height: 1; }

        /* Tech Stack Bubbles */
        .tech-hub { display: flex; flex-wrap: wrap; gap: 10px; justify-content: center; margin-top: 20px; }
        .tech-pill { padding: 8px 16px; background: rgba(255,255,255,0.05); border: 1px solid var(--border); border-radius: 50px; font-size: 0.75rem; display: flex; align-items: center; gap: 8px; transition: 0.3s; cursor: pointer; }
        .tech-pill:hover { background: var(--primary); color: #000; font-weight: 800; }

        /* Working Service Links */
        .s-link { display: flex; align-items: center; justify-content: space-between; padding: 18px; background: rgba(255,255,255,0.03); border-radius: 20px; margin-bottom: 12px; text-decoration: none; color: white; border: 1px solid var(--border); transition: 0.3s; }
        .s-link:hover { background: rgba(0, 242, 254, 0.1); border-color: var(--primary); padding-left: 25px; }
        .s-link i { font-size: 1.2rem; color: var(--primary); }

        /* Contact Action Hub */
        .hub-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-top: 20px; }
        .hub-btn { padding: 15px; border-radius: 20px; text-decoration: none; text-align: center; color: white; font-weight: 700; font-size: 0.85rem; display: flex; flex-direction: column; align-items: center; gap: 8px; border: 1px solid var(--border); background: var(--glass); transition: 0.3s; }
        .hub-btn:hover { background: var(--primary); color: #000; border-color: var(--primary); }
        .hub-btn i { font-size: 1.5rem; }

        /* Bottom Menu */
        .nav-dock { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 92%; background: rgba(0,0,0,0.85); backdrop-filter: blur(30px); border-radius: 40px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 16px; z-index: 1000; }
        .nav-link { color: rgba(255,255,255,0.5); font-size: 1.4rem; transition: 0.3s; }
        .nav-link:hover, .nav-link.active { color: var(--primary); transform: scale(1.2); text-shadow: var(--glow); }

        /* Gallery */
        .work-gallery { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-top: 15px; }
        .work-item { width: 100%; height: 110px; border-radius: 18px; object-fit: cover; border: 1px solid var(--border); }

        footer { text-align: center; padding: 30px; opacity: 0.3; font-size: 0.7rem; letter-spacing: 4px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="gradient-bg"></div>

    <div class="cover-wrap">
        <img src="FB_IMG_1769869953605.jpg" class="cover-photo" alt="Cover">
        <div class="cover-fade"></div>
    </div>

    <nav class="nav-dock">
        <a href="#" class="nav-link active"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-link"><i class="fab fa-whatsapp"></i></a>
        <a href="tel:+923332637235" class="nav-link"><i class="fas fa-phone"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-link"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-link"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <div class="profile-area" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" class="p-pic" alt="Nazim">
            <br>
            <div class="live-badge">🟢 Web-Hub Online</div>
        </div>

        <section class="card" data-aos="fade-up" style="text-align: center;">
            <h1 class="h-title">Web-Hub</h1>
            <p id="greeting" style="font-size: 0.8rem; opacity: 0.7; margin: 10px 0;">Welcome to our official portal</p>
            <div class="tech-hub">
                <div class="tech-pill"><i class="fab fa-react"></i> React</div>
                <div class="tech-pill"><i class="fab fa-wordpress"></i> WP</div>
                <div class="tech-pill"><i class="fas fa-mobile-alt"></i> Apps</div>
                <div class="tech-pill"><i class="fas fa-search-dollar"></i> SEO</div>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px;"><i class="fas fa-th-large"></i> Explore Services</h3>
            <a href="https://wa.me/923332637235?text=I%20want%20to%20order%20a%20Website" class="s-link">
                <span><i class="fas fa-code"></i> &nbsp; Web Development</span>
                <i class="fas fa-chevron-right"></i>
            </a>
            <a href="https://wa.me/923332637235?text=I%20want%20to%20order%20Graphic%20Design" class="s-link">
                <span><i class="fas fa-paint-brush"></i> &nbsp; UI/UX & Graphics</span>
                <i class="fas fa-chevron-right"></i>
            </a>
            <a href="https://wa.me/923332637235?text=I%20want%20SEO%20Services" class="s-link">
                <span><i class="fas fa-bullhorn"></i> &nbsp; Digital Marketing</span>
                <i class="fas fa-chevron-right"></i>
            </a>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-images"></i> Featured Work</h3>
            <div class="work-gallery">
                <img src="https://images.unsplash.com/photo-1547658719-da2b51169166?auto=format&fit=crop&w=300" class="work-item">
                <img src="https://images.unsplash.com/photo-1572044162444-ad60f128bde2?auto=format&fit=crop&w=300" class="work-item">
                <img src="https://images.unsplash.com/photo-1551288049-bbbda536339a?auto=format&fit=crop&w=300" class="work-item">
                <img src="https://images.unsplash.com/photo-1522542550221-31fd19575a2d?auto=format&fit=crop&w=300" class="work-item">
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="border-color: var(--primary);">
            <h3 style="text-align: center; margin-bottom: 20px;">Get a Free Quote</h3>
            <div class="hub-grid">
                <a href="https://wa.me/923332637235" class="hub-btn" style="background: rgba(37, 211, 102, 0.1); border-color: #25d366;"><i class="fab fa-whatsapp"></i> WhatsApp</a>
                <a href="tel:+923332637235" class="hub-btn" style="background: rgba(0, 242, 254, 0.1); border-color: var(--primary);"><i class="fas fa-phone-alt"></i> Direct Call</a>
                <a href="mailto:webhub262@gmail.com" class="hub-btn" style="background: rgba(255, 69, 58, 0.1); border-color: #ff453a;"><i class="fas fa-envelope"></i> Email Us</a>
                <a href="https://www.facebook.com/profile.php?id=100084218946114" class="hub-btn" style="background: rgba(24, 119, 242, 0.1); border-color: #1877f2;"><i class="fab fa-facebook-f"></i> Facebook</a>
            </div>
        </div>

        <footer>© 2026 | WEB-HUB OFFICIAL | FOUNDED BY MUHAMMAD NAZIM</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Smart Greeting Logic
        const hour = new Date().getHours();
        let greetText = hour < 12 ? "Good Morning! Ready to build?" : hour < 18 ? "Good Afternoon! Let's innovate." : "Good Evening! Planning for success?";
        document.getElementById('greeting').innerText = greetText;
    </script>
</body>
</html>
