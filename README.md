<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub Infinity | Muhammad Nazim</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;900&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #7000ff;
            --success: #00ff88; --bg: #010204; --glass: rgba(255, 255, 255, 0.04);
            --border: rgba(0, 242, 254, 0.2);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; cursor: none; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Custom Neon Cursor */
        #cursor { width: 8px; height: 8px; background: var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 100000; box-shadow: 0 0 20px var(--primary); }
        #cursor-aura { width: 35px; height: 35px; border: 1px solid var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 99999; transition: 0.1s ease-out; transform: translate(-50%, -50%); }

        /* Background Video Overlay */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle at 50% 50%, transparent 10%, #000 90%); z-index: -1; }

        nav { position: fixed; top: 0; width: 100%; padding: 20px; display: flex; justify-content: space-between; align-items: center; z-index: 10000; background: rgba(0,0,0,0.85); backdrop-filter: blur(25px); border-bottom: 1px solid var(--border); }
        .nav-logo { font-weight: 900; font-size: 1.5rem; background: linear-gradient(45deg, #fff, var(--primary)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 110px 18px 60px; }

        /* Main Glass Card */
        .card-wrap { background: var(--glass); border: 1.5px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 25px; backdrop-filter: blur(20px); box-shadow: 0 20px 50px rgba(0,0,0,0.5); }
        .section-header { font-size: 1.1rem; font-weight: 900; margin-bottom: 20px; color: var(--primary); display: flex; align-items: center; gap: 10px; border-bottom: 1px solid rgba(255,255,255,0.1); padding-bottom: 12px; }

        /* SOCIAL GRID: YE SAB CLICKABLE HAIN */
        .social-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 15px; margin-top: 10px; }
        .social-box { aspect-ratio: 1/1; background: #0c0c0c; border: 1.5px solid #222; border-radius: 20px; display: flex; align-items: center; justify-content: center; font-size: 1.4rem; color: #fff; text-decoration: none; transition: 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); }
        .social-box:hover { border-color: var(--primary); color: var(--primary); transform: translateY(-8px) scale(1.1); box-shadow: 0 10px 25px rgba(0,242,254,0.4); }

        /* Business Rows */
        .clickable-row { display: flex; justify-content: space-between; align-items: center; padding: 18px 5px; border-bottom: 1px solid rgba(255,255,255,0.05); text-decoration: none; color: #ccc; transition: 0.3s; font-size: 0.95rem; }
        .clickable-row:hover { color: #fff; transform: translateX(8px); background: rgba(255,255,255,0.03); }

        /* Action Button */
        .btn-main { background: linear-gradient(90deg, var(--primary), var(--secondary)); border: none; padding: 20px; border-radius: 25px; color: #000; font-weight: 900; width: 100%; text-decoration: none; display: block; text-align: center; margin-top: 25px; box-shadow: 0 10px 30px rgba(0, 242, 254, 0.3); transition: 0.3s; }
        .btn-main:active { transform: scale(0.95); }

        /* Deep Modal */
        .modal { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.98); z-index: 200000; backdrop-filter: blur(40px); }
        .modal-body { position: relative; margin: 80px auto; width: 90%; max-width: 420px; background: #080808; border: 1.5px solid var(--primary); border-radius: 40px; padding: 40px; text-align: left; }
        .modal-body h2 { color: var(--primary); margin-bottom: 20px; font-weight: 900; }
        .modal-body p { color: #ccc; line-height: 1.8; white-space: pre-wrap; margin-bottom: 25px; }

        footer { text-align: center; opacity: 0.3; font-size: 0.75rem; letter-spacing: 3px; margin-top: 50px; }
    </style>
</head>
<body>

    <div id="cursor"></div>
    <div id="cursor-aura"></div>

    <nav>
        <div class="nav-logo">WEB-HUB</div>
        <div id="live-time" style="font-size: 0.75rem; font-weight: 800; color: var(--primary);">00:00:00</div>
    </nav>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        
        <section class="card-wrap" style="text-align: center;" data-aos="zoom-in">
            <h1 style="font-size: 3.5rem; font-weight: 900; letter-spacing: -3px; color: var(--primary);">Web-Hub</h1>
            <p style="color: #aaa; margin: 15px 0 25px; font-size: 1rem; line-height: 1.6;">Precision engineered web solutions by <b>Muhammad Nazim</b>. Elevate your brand to the digital elite.</p>
            <a href="https://wa.me/923332637235" target="_blank" class="btn-main"><i class="fab fa-whatsapp"></i> INITIATE CONNECTION</a>
        </section>

        <div class="card-wrap" data-aos="fade-up">
            <h2 class="section-header"><i class="fas fa-link"></i> Social Ecosystem</h2>
            <div class="social-grid">
                <a href="https://facebook.com/share/12E6tH73q6/" target="_blank" class="social-box" title="Facebook">
                    <i class="fab fa-facebook-f"></i>
                </a>
                <a href="https://www.instagram.com/itz_nazim_03/" target="_blank" class="social-box" title="Instagram">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-0100772bb" target="_blank" class="social-box" title="LinkedIn">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="https://wa.me/923332637235" target="_blank" class="social-box" title="WhatsApp">
                    <i class="fab fa-whatsapp"></i>
                </a>
            </div>
        </div>

        <div class="card-wrap" data-aos="fade-up">
            <h2 class="section-header"><i class="fas fa-shield-alt"></i> Intelligence Hub</h2>
            
            <a href="javascript:void(0)" onclick="openModal('Contact Center', '📞 Phone: +92 333 2637235\n✉️ Email: info@webhub.com\n📍 HQ: Karachi Tech District, Pakistan\n⏰ Support: 24/7 Global Intelligence')" class="clickable-row">
                <span>Contact Protocols</span> <i class="fas fa-chevron-right"></i>
            </a>

            <a href="javascript:void(0)" onclick="openModal('Privacy & Security', 'All architectural data is encrypted via 256-bit protocols. Web-Hub Infinity prioritizes client confidentiality and intellectual property protection above all.')" class="clickable-row">
                <span>Security Manifesto</span> <i class="fas fa-chevron-right"></i>
            </a>

            <a href="javascript:void(0)" onclick="openModal('Success Stories', '• 50+ Custom Deployments\n• 100% Client Retention Rate\n• Specialized in AI-driven E-commerce & SaaS architectures.')" class="clickable-row">
                <span>Mission Success</span> <i class="fas fa-chevron-right"></i>
            </a>
        </div>

        <footer>
            © 2026 MUHAMMAD NAZIM • WEB-HUB INFINITY CORE
        </footer>
    </div>

    <div id="infoModal" class="modal">
        <div class="modal-body">
            <h2 id="modalTitle"></h2>
            <p id="modalText"></p>
            <button onclick="closeModal()" class="btn-main" style="color: #000;">CLOSE INTERFACE</button>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Cursor System
        const cursor = document.getElementById('cursor');
        const aura = document.getElementById('cursor-aura');
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
            aura.style.left = e.clientX + 'px';
            aura.style.top = e.clientY + 'px';
        });

        // Live Clock Engine
        setInterval(() => {
            document.getElementById('live-time').innerText = new Date().toLocaleTimeString();
        }, 1000);

        // Modal Engine
        function openModal(t, b) {
            document.getElementById('modalTitle').innerText = t;
            document.getElementById('modalText').innerText = b;
            document.getElementById('infoModal').style.display = 'block';
            document.body.style.overflow = 'hidden';
        }
        function closeModal() {
            document.getElementById('infoModal').style.display = 'none';
            document.body.style.overflow = 'auto';
        }
    </script>
</body>
</html>
