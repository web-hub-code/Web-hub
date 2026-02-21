<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub Infinity | Muhammad Nazim - Premium Solutions</title>
    
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

        /* Ultra-Modern Cursor */
        #cursor { width: 8px; height: 8px; background: var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 100000; box-shadow: 0 0 20px var(--primary); }
        #cursor-aura { width: 40px; height: 40px; border: 1px solid var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 99999; transition: 0.1s ease-out; transform: translate(-50%, -50%); }

        /* Dynamic Background */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle at 50% 50%, transparent 10%, #000 90%); z-index: -1; }

        /* Floating Nav & Progress */
        #scroll-path { position: fixed; top: 0; left: 0; width: 100%; height: 4px; background: rgba(255,255,255,0.05); z-index: 100001; }
        #scroll-fill { height: 100%; width: 0%; background: linear-gradient(90deg, var(--primary), var(--success)); transition: 0.1s; }
        
        nav { position: fixed; top: 0; width: 100%; padding: 20px; display: flex; justify-content: space-between; align-items: center; z-index: 10000; background: rgba(0,0,0,0.8); backdrop-filter: blur(30px); border-bottom: 1px solid var(--border); }
        .nav-logo { font-weight: 900; font-size: 1.6rem; letter-spacing: -1px; background: linear-gradient(45deg, #fff, var(--primary)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 110px 15px 60px; }

        /* Hero Hub */
        .hero-card { background: var(--glass); border: 1.5px solid var(--border); border-radius: 45px; padding: 50px 25px; text-align: center; margin-bottom: 35px; backdrop-filter: blur(20px); position: relative; overflow: hidden; }
        .live-tag { display: inline-flex; align-items: center; gap: 8px; background: rgba(0, 255, 136, 0.1); color: var(--success); padding: 7px 15px; border-radius: 50px; font-size: 0.7rem; font-weight: 900; border: 1px solid var(--success); }

        /* Interactive Sections (Screenshot Style) */
        .card-wrap { background: var(--glass); border: 1.5px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 25px; position: relative; }
        .section-header { font-size: 1.1rem; font-weight: 900; margin-bottom: 20px; color: var(--primary); display: flex; align-items: center; gap: 10px; border-bottom: 1px solid rgba(255,255,255,0.1); padding-bottom: 15px; }
        
        .clickable-row { display: flex; justify-content: space-between; align-items: center; padding: 18px 5px; border-bottom: 1px solid rgba(255,255,255,0.05); text-decoration: none; color: #bbb; transition: 0.3s; font-weight: 500; }
        .clickable-row:hover { color: #fff; transform: translateX(8px); background: rgba(255,255,255,0.02); }
        .clickable-row i { font-size: 0.8rem; color: var(--primary); }

        /* Deep Modal Styling */
        .modal { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.98); z-index: 200000; backdrop-filter: blur(40px); overflow-y: auto; }
        .modal-body { position: relative; margin: 50px auto; width: 92%; max-width: 450px; background: #080808; border: 1.5px solid var(--primary); border-radius: 40px; padding: 40px 30px; }
        .modal-body h2 { color: var(--primary); font-size: 1.8rem; margin-bottom: 20px; font-weight: 900; }
        .modal-body p, .modal-body li { font-size: 0.95rem; color: #ccc; line-height: 1.7; margin-bottom: 15px; text-align: left; }
        .close-btn { background: var(--primary); border: none; padding: 15px 40px; border-radius: 50px; color: #000; font-weight: 900; width: 100%; margin-top: 20px; }

        /* Social Connect */
        .social-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 15px; margin-top: 20px; }
        .social-box { aspect-ratio: 1/1; background: #0c0c0c; border: 1.5px solid #222; border-radius: 20px; display: flex; align-items: center; justify-content: center; font-size: 1.4rem; color: #fff; text-decoration: none; transition: 0.4s; }
        .social-box:hover { border-color: var(--primary); color: var(--primary); transform: translateY(-5px); box-shadow: 0 0 15px rgba(0,242,254,0.3); }

        /* Newsletter */
        .newsletter-input { background: #000; border: 1px solid #333; border-radius: 18px; display: flex; overflow: hidden; margin-top: 15px; }
        .newsletter-input input { background: transparent; border: none; padding: 18px; color: #fff; flex: 1; outline: none; }
        .newsletter-input button { background: var(--accent); border: none; padding: 0 22px; color: #fff; font-weight: 800; }

        @keyframes pulse { 0% { transform: scale(1); opacity: 1; } 50% { transform: scale(1.6); opacity: 0; } 100% { transform: scale(1); opacity: 1; } }
    </style>
</head>
<body>

    <div id="cursor"></div>
    <div id="cursor-aura"></div>
    <div id="scroll-path"><div id="scroll-fill"></div></div>

    <nav>
        <div class="nav-logo">WEB-HUB</div>
        <div id="live-time" style="font-size: 0.75rem; font-weight: 800; color: var(--primary);">00:00:00</div>
    </nav>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        
        <section class="hero-card" data-aos="zoom-in">
            <div class="live-tag">
                <div style="width: 8px; height: 8px; background: var(--success); border-radius: 50%; animation: pulse 1.5s infinite;"></div>
                <span id="visitor-count">128</span> ACTIVE NODES
            </div>
            <h4 id="greeting" style="color: #fff; font-weight: 800; font-size: 0.8rem; letter-spacing: 4px; opacity: 0.6; margin: 20px 0 10px;">SUBH BAKHAIR</h4>
            <h1 style="font-size: 3.5rem; font-weight: 900; letter-spacing: -3px; line-height: 1;">Web-Hub</h1>
            <p style="color: #888; font-size: 1rem; line-height: 1.8; margin: 20px 0 30px;">
                Leading the digital era with Muhammad Nazim. We craft high-performance assets tailored to your vision.
            </p>
            <a href="https://wa.me/923332637235" class="close-btn" style="text-decoration: none; display: block; background: linear-gradient(90deg, var(--primary), var(--secondary));">
                <i class="fab fa-whatsapp"></i> INITIATE PROJECT
            </a>
        </section>

        <div class="card-wrap" data-aos="fade-up">
            <h2 class="section-header"><i class="fas fa-layer-group"></i> Professional Info</h2>
            
            <a href="javascript:void(0)" onclick="openDeepModal('About Us', 'Muhammad Nazim is a visionary developer specializing in Enterprise-level Web Solutions and AI Integration. At Web-Hub, we don\'t just build sites; we build digital empires for startups and established brands worldwide.')" class="clickable-row">
                <span>About Our Mission</span> <i class="fas fa-plus"></i>
            </a>

            <a href="javascript:void(0)" onclick="openDeepModal('Privacy Policy', 'Your data is encrypted and secure. We follow GDPR and global data protection standards. No third-party sharing, only transparent business.')" class="clickable-row">
                <span>Privacy & Security</span> <i class="fas fa-plus"></i>
            </a>

            <a href="javascript:void(0)" onclick="openDeepModal('Success Stories', '1. FinTech Dashboard (USA) - 200% Speed Boost\n2. E-com Giant (PK) - 50k+ Daily Users\n3. AI Chatbot System - Automated 80% Support')" class="clickable-row">
                <span>Success Stories</span> <i class="fas fa-plus"></i>
            </a>

            <a href="javascript:void(0)" onclick="openDeepModal('Contact Details', 'Email: info@webhub.com\nPhone: +92 333 2637235\nOffice: Karachi Tech Zone\nHours: 24/7 Global Support')" class="clickable-row">
                <span>Full Contact Info</span> <i class="fas fa-plus"></i>
            </a>
        </div>

        <div class="card-wrap" data-aos="fade-up">
            <h2 class="section-header"><i class="fas fa-map-marker-alt"></i> Corporate HQ</h2>
            <div style="border-left: 2px solid var(--primary); padding-left: 20px; margin: 15px 0;">
                <p style="font-weight: 800; font-size: 1.1rem; color: #fff;">Web-Hub Digital Center</p>
                <p style="color: #888; font-size: 0.9rem;">Karachi, Pakistan | Global Presence</p>
                <p style="color: var(--primary); font-weight: 900; margin-top: 10px;">Direct: +92 333 2637235</p>
            </div>
            
            <div style="margin-top: 30px;">
                <p style="font-size: 0.8rem; color: #555; font-weight: 900; margin-bottom: 10px;">NEWSLETTER SUBSCRIPTION</p>
                <div class="newsletter-input">
                    <input type="email" placeholder="Your work email...">
                    <button onclick="alert('Subscription Confirmed!')">JOIN</button>
                </div>
            </div>
        </div>

        <div class="card-wrap" data-aos="zoom-in">
            <h2 class="section-header"><i class="fas fa-share-nodes"></i> Connect</h2>
            <div class="social-grid">
                <a href="https://facebook.com/share/12E6tH73q6/" class="social-box"><i class="fab fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/itz_nazim_03/" class="social-box"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-0100772bb" class="social-box"><i class="fab fa-linkedin-in"></i></a>
                <a href="https://wa.me/923332637235" class="social-box"><i class="fab fa-whatsapp"></i></a>
            </div>
        </div>

        <footer style="margin-top: 60px; text-align: center; opacity: 0.4;">
            <p style="font-size: 0.7rem; letter-spacing: 5px;">MUHAMMAD NAZIM • EST 2026 • WEB-HUB INFINITY</p>
        </footer>
    </div>

    <div id="deepModal" class="modal">
        <div class="modal-body" data-aos="fade-up">
            <h2 id="modalTitle"></h2>
            <div id="modalContent" style="white-space: pre-wrap; margin-bottom: 20px;"></div>
            <button class="close-btn" onclick="closeDeepModal()">DISMISS</button>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 800, once: true });

        // Cursor & Aura System
        const cursor = document.getElementById('cursor');
        const aura = document.getElementById('cursor-aura');
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
            aura.style.left = e.clientX + 'px';
            aura.style.top = e.clientY + 'px';
        });

        // Scroll Engine
        window.addEventListener('scroll', () => {
            const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            const scrolled = (winScroll / height) * 100;
            document.getElementById('scroll-fill').style.width = scrolled + "%";
        });

        // Live Clock Engine
        function runLiveEngine() {
            const now = new Date();
            document.getElementById('live-time').innerText = now.toLocaleTimeString();
            const hr = now.getHours();
            const greet = hr < 12 ? "SUBH BAKHAIR ☀️" : hr < 18 ? "ASSALAM-O-ALAIKUM 🌤️" : "SHAB BAKHAIR 🌙";
            document.getElementById('greeting').innerText = greet;
        }
        setInterval(runLiveEngine, 1000);
        runLiveEngine();

        // Modal Engine
        function openDeepModal(title, content) {
            document.getElementById('modalTitle').innerText = title;
            document.getElementById('modalContent').innerText = content;
            document.getElementById('deepModal').style.display = 'block';
            document.body.style.overflow = 'hidden';
        }
        function closeDeepModal() {
            document.getElementById('deepModal').style.display = 'none';
            document.body.style.overflow = 'auto';
        }

        // Live Visitor Counter
        setInterval(() => {
            let count = parseInt(document.getElementById('visitor-count').innerText);
            document.getElementById('visitor-count').innerText = count + (Math.random() > 0.5 ? 1 : -1);
        }, 3000);
    </script>
</body>
</html>
