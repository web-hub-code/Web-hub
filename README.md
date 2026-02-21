<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub | Unlimited Innovation</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #7000ff;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.04); --border: rgba(255, 255, 255, 0.08);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Animated Particles Background */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15) contrast(1.2); }
        .vignette { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 30%, #000 100%); z-index: -1; }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 120px; }

        /* VVIP Card Styling */
        .card { background: var(--glass); backdrop-filter: blur(45px); border: 1px solid var(--border); border-radius: 40px; padding: 30px; margin-bottom: 25px; transition: 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275); }
        .card:hover { border-color: var(--primary); transform: scale(1.02); box-shadow: 0 20px 40px rgba(0,0,0,0.4); }

        /* Hero Hub */
        .hero { text-align: center; border: 1px solid var(--primary); }
        .logo-main { font-size: 3.5rem; font-weight: 900; background: linear-gradient(to right, var(--primary), var(--accent), var(--secondary)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -2px; }
        
        /* Skills/Features Tags */
        .tag-cloud { display: flex; flex-wrap: wrap; gap: 10px; justify-content: center; margin-top: 15px; }
        .tag { padding: 6px 15px; background: rgba(0, 242, 254, 0.1); border-radius: 50px; border: 1px solid var(--primary); font-size: 0.7rem; color: var(--primary); font-weight: 600; }

        /* Glass Form */
        input, textarea { width: 100%; padding: 15px; margin-bottom: 15px; background: rgba(255,255,255,0.03); border: 1px solid var(--border); border-radius: 18px; color: white; outline: none; transition: 0.3s; }
        input:focus { border-color: var(--primary); background: rgba(255,255,255,0.07); }
        
        .btn-mega { background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 20px; width: 100%; border-radius: 20px; font-weight: 800; cursor: pointer; font-size: 1.1rem; box-shadow: 0 15px 35px rgba(0, 242, 254, 0.3); text-transform: uppercase; transition: 0.3s; text-decoration: none; display: block; text-align: center; }
        .btn-mega:active { transform: scale(0.95); }

        /* Bottom Menu */
        .bottom-nav { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 90%; background: rgba(0,0,0,0.8); backdrop-filter: blur(30px); border-radius: 40px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 18px; z-index: 1000; }
        .nav-item { color: white; font-size: 1.4rem; position: relative; transition: 0.3s; }
        .nav-item:hover { color: var(--primary); }
        .nav-item.active::after { content: ''; position: absolute; bottom: -8px; left: 50%; transform: translateX(-50%); width: 5px; height: 5px; background: var(--primary); border-radius: 50%; box-shadow: 0 0 10px var(--primary); }

        /* Testimonials Scroll */
        .testimonial-box { border-left: 3px solid var(--accent); padding-left: 15px; margin-top: 15px; }
        .testimonial-box p { font-size: 0.85rem; font-style: italic; opacity: 0.8; }
        .client-name { color: var(--primary); font-weight: 600; font-size: 0.75rem; margin-top: 5px; }

        footer { text-align: center; font-size: 0.7rem; opacity: 0.3; letter-spacing: 5px; padding-bottom: 20px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="vignette"></div>

    <nav class="bottom-nav">
        <a href="#" class="nav-item active"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="fade-down">
            <h1 class="logo-main">Web-Hub</h1>
            <p style="font-size: 0.8rem; letter-spacing: 6px; opacity: 0.8; margin-top: 5px;">BEYOND DIGITAL LIMITS</p>
            <div class="tag-cloud">
                <span class="tag">AI WEBSITES</span>
                <span class="tag">BRANDING</span>
                <span class="tag">SEO MAX</span>
                <span class="tag">24/7 VIP</span>
            </div>
        </section>

        <div class="card" data-aos="fade-up" style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; text-align: center;">
            <div><h2 style="color: var(--primary);">500+</h2><p style="font-size: 0.6rem; opacity: 0.6;">PROJECTS DONE</p></div>
            <div><h2 style="color: var(--primary);">200+</h2><p style="font-size: 0.6rem; opacity: 0.6;">GLOBAL CLIENTS</p></div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 20px; font-size: 1.2rem;"><i class="fas fa-star" style="color: gold;"></i> Unlimited Solutions</h3>
            <div style="display: flex; align-items: center; gap: 15px; margin-bottom: 15px;">
                <i class="fas fa-rocket" style="font-size: 1.5rem; color: var(--primary);"></i>
                <div><h4 style="font-size: 0.9rem;">Ultra Fast Deployment</h4><p style="font-size: 0.7rem; opacity: 0.6;">Websites that load in milliseconds.</p></div>
            </div>
            <div style="display: flex; align-items: center; gap: 15px; margin-bottom: 15px;">
                <i class="fas fa-fingerprint" style="font-size: 1.5rem; color: var(--accent);"></i>
                <div><h4 style="font-size: 0.9rem;">Unique Brand Identity</h4><p style="font-size: 0.7rem; opacity: 0.6;">Stand out from your competitors.</p></div>
            </div>
        </div>

        <div class="card" data-aos="fade-left">
            <h3><i class="fas fa-quote-right"></i> Clients Voice</h3>
            <div class="testimonial-box">
                <p>"Nazim is a magician! Web-Hub is the best decision for my brand."</p>
                <div class="client-name">— Rashid Khan (Dubai)</div>
            </div>
        </div>

        <div class="card" data-aos="fade-up" style="text-align: center;">
            <img src="Snapchat-2096615446.jpg" style="width: 90px; height: 90px; border-radius: 50%; border: 3px solid var(--primary); margin-bottom: 15px; box-shadow: 0 0 20px var(--primary);">
            <h3>Let's Dominate the Web</h3>
            <p style="font-size: 0.8rem; margin: 15px 0; opacity: 0.7;">Ready to scale? Connect with our expert team now.</p>
            <a href="https://wa.me/923332637235" class="btn-mega">START YOUR PROJECT</a>
            <div style="margin-top: 20px; display: flex; justify-content: center; gap: 20px; opacity: 0.7;">
                <a href="tel:+923332637235" style="color: white;"><i class="fas fa-phone"></i></a>
                <a href="mailto:webhub262@gmail.com" style="color: white;"><i class="fas fa-envelope"></i></a>
                <a href="https://www.facebook.com/profile.php?id=100084218946114" style="color: white;"><i class="fab fa-facebook"></i></a>
            </div>
        </div>

        <footer>© 2026 | WEB-HUB UNLIMITED | MUHAMMAD NAZIM</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 1000, once: true });</script>
</body>
</html>
