<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub | Muhammad Nazim</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #f093fb;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.05); --border: rgba(255, 255, 255, 0.1);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; -webkit-tap-highlight-color: transparent; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; }

        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.2); }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 15px 120px; }

        .card { background: var(--glass); backdrop-filter: blur(30px); border: 1px solid var(--border); border-radius: 30px; padding: 25px; margin-bottom: 25px; transition: 0.3s; }
        .hero { text-align: center; padding: 50px 20px; }
        .profile-pic { width: 130px; height: 130px; border-radius: 50%; border: 3px solid var(--primary); box-shadow: 0 0 25px var(--primary); margin-bottom: 15px; }
        
        .gradient-text { background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; font-size: 2.2rem; }

        .service-list { list-style: none; margin-top: 15px; }
        .service-list li { padding: 10px 0; border-bottom: 1px solid rgba(255,255,255,0.05); font-size: 0.9rem; display: flex; align-items: center; gap: 10px; }
        .service-list i { color: var(--primary); }

        .bottom-nav { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 92%; background: rgba(0,0,0,0.85); backdrop-filter: blur(20px); border-radius: 40px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 15px; z-index: 1000; }
        .nav-item { color: white; font-size: 1.25rem; }

        .cta-btn { background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 18px; width: 100%; border-radius: 18px; font-weight: 800; cursor: pointer; display: block; text-align: center; text-decoration: none; margin-top: 10px; box-shadow: 0 10px 20px rgba(0, 242, 254, 0.2); }

        footer { text-align: center; font-size: 0.75rem; opacity: 0.4; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <section class="card hero" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" alt="Muhammad Nazim" class="profile-pic">
            <h1 class="gradient-text">Web Hub</h1>
            <p style="opacity: 0.8; letter-spacing: 2px;">BY MUHAMMAD NAZIM</p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-tools"></i> Expert Services</h3>
            <ul class="service-list">
                <li><i class="fas fa-check-circle"></i> Custom Web Development</li>
                <li><i class="fas fa-check-circle"></i> UI/UX Modern Interface</li>
                <li><i class="fas fa-check-circle"></i> SEO & Digital Marketing</li>
                <li><i class="fas fa-check-circle"></i> 24/7 Technical Support</li>
            </ul>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-info-circle"></i> Why Web-Hub?</h3>
            <p style="font-size: 0.85rem; line-height: 1.6; opacity: 0.8; margin-top: 10px;">
                Hum technology aur creativity ko mila kar aapke business ko ek naya muqam dete hain. Web-Hub sirf ek website nahi, aapke digital sapno ki tabeer hai.
            </p>
        </div>

        <div class="card" data-aos="fade-up" style="text-align: center;">
            <h3>Start Your Project</h3>
            <p style="font-size: 0.8rem; margin: 10px 0 20px; opacity: 0.7;">Let's build something extraordinary together.</p>
            <a href="https://wa.me/923332637235" class="cta-btn">HIRE ME NOW</a>
        </div>

        <footer>© 2026 | WEB HUB | POWERED BY MUHAMMAD NAZIM</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 800, once: true });</script>
</body>
</html>
