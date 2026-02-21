<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub Official | Digital Solutions</title>
    
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

        /* Background Video */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }

        /* Cover Section */
        .cover-container { width: 100%; height: 250px; position: relative; overflow: hidden; }
        .cover-photo { width: 100%; height: 100%; object-fit: cover; filter: brightness(0.6); }
        .cover-overlay { position: absolute; bottom: 0; left: 0; width: 100%; height: 60%; background: linear-gradient(to top, var(--bg), transparent); }

        .container { width: 100%; max-width: 550px; margin: -70px auto 0; padding: 0 15px 120px; position: relative; z-index: 5; }

        /* Profile Photo */
        .profile-pic-wrapper { text-align: center; margin-bottom: 10px; }
        .profile-pic { width: 140px; height: 140px; border-radius: 50%; border: 4px solid var(--primary); box-shadow: 0 0 30px var(--primary); object-fit: cover; background: var(--bg); }

        /* Card System */
        .card { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 25px; }
        .hero-info { text-align: center; }
        .logo-main { font-size: 3rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-transform: uppercase; }

        /* Image Gallery */
        .gallery-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-top: 15px; }
        .gallery-img { width: 100%; height: 130px; border-radius: 20px; object-fit: cover; border: 1px solid var(--border); transition: 0.3s; }
        .gallery-img:hover { transform: scale(1.05); border-color: var(--primary); }

        /* Tech Badges */
        .tech-icons { display: flex; justify-content: center; gap: 20px; font-size: 1.5rem; margin-top: 15px; color: var(--secondary); }

        /* Buttons */
        .btn-action { display: flex; align-items: center; justify-content: center; gap: 10px; background: linear-gradient(45deg, var(--primary), var(--secondary)); border: none; color: white; padding: 18px; width: 100%; border-radius: 22px; font-weight: 800; cursor: pointer; text-decoration: none; font-size: 1rem; margin-bottom: 15px; transition: 0.3s; }
        .btn-action:hover { box-shadow: 0 10px 30px rgba(0, 242, 254, 0.4); transform: translateY(-3px); }

        /* Bottom Nav */
        .bottom-nav { position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); width: 90%; background: rgba(0,0,0,0.8); backdrop-filter: blur(30px); border-radius: 40px; border: 1px solid var(--border); display: flex; justify-content: space-around; padding: 16px; z-index: 1000; }
        .nav-item { color: white; font-size: 1.4rem; opacity: 0.6; }
        .nav-item:hover { opacity: 1; color: var(--primary); }

        footer { text-align: center; font-size: 0.75rem; opacity: 0.3; letter-spacing: 5px; padding: 20px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>

    <div class="cover-container">
        <img src="FB_IMG_1769869953605.jpg" class="cover-photo" alt="Cover">
        <div class="cover-overlay"></div>
    </div>

    <nav class="bottom-nav">
        <a href="#" class="nav-item"><i class="fas fa-home"></i></a>
        <a href="https://wa.me/923332637235" target="_blank" class="nav-item"><i class="fab fa-whatsapp"></i></a>
        <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="nav-item"><i class="fab fa-facebook-f"></i></a>
        <a href="mailto:webhub262@gmail.com" class="nav-item"><i class="fas fa-envelope"></i></a>
    </nav>

    <div class="container">
        <div class="profile-pic-wrapper" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" class="profile-pic" alt="Nazim">
        </div>

        <section class="card hero-info" data-aos="fade-up">
            <h1 class="logo-main">Web-Hub</h1>
            <p style="letter-spacing: 6px; font-size: 0.7rem; opacity: 0.8; margin-top: 5px;">THE FUTURE OF CODE</p>
            
            <div class="tech-icons">
                <i class="fab fa-html5"></i>
                <i class="fab fa-css3-alt"></i>
                <i class="fab fa-js-square"></i>
                <i class="fab fa-react"></i>
                <i class="fab fa-wordpress"></i>
            </div>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 15px;"><i class="fas fa-project-diagram" style="color: var(--primary);"></i> Our Digital Space</h3>
            <div class="gallery-grid">
                <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=400&q=80" class="gallery-img" alt="Coding">
                <img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?auto=format&fit=crop&w=400&q=80" class="gallery-img" alt="Software">
                <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&w=400&q=80" class="gallery-img" alt="Marketing">
                <img src="https://images.unsplash.com/photo-1504639725590-34d0984388bd?auto=format&fit=crop&w=400&q=80" class="gallery-img" alt="Hacking">
            </div>
        </div>

        <div class="card" data-aos="fade-up">
            <h3><i class="fas fa-award"></i> Why Choose Web-Hub?</h3>
            <p style="font-size: 0.85rem; margin-top: 10px; line-height: 1.6; opacity: 0.9;">
                Web-Hub sirf aik website nahi, ye aapke business ka digital ghar hai. Hum modern tech use karte hain taake aapki site super fast aur secure rahe. 
            </p>
        </div>

        <div class="card" data-aos="fade-up" style="text-align: center;">
            <h3 style="margin-bottom: 20px;">Ready for the Next Level?</h3>
            <a href="https://wa.me/923332637235" class="btn-action"><i class="fab fa-whatsapp"></i> START WHATSAPP CHAT</a>
            <a href="tel:+923332637235" class="btn-action" style="background: rgba(255,255,255,0.05); border: 1px solid var(--border); box-shadow: none;"><i class="fas fa-phone"></i> CALL OFFICIAL LINE</a>
        </div>

        <footer>© 2026 | WEB-HUB | MUHAMMAD NAZIM</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>AOS.init({ duration: 1000, once: true });</script>
</body>
</html>
