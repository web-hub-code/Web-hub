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
            --border: rgba(0, 242, 254, 0.25);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; cursor: none; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Advanced Cursor System */
        #cursor { width: 8px; height: 8px; background: var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 100000; box-shadow: 0 0 20px var(--primary); }
        #cursor-aura { width: 35px; height: 35px; border: 1px solid var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 99999; transition: 0.12s ease-out; transform: translate(-50%, -50%); }
        
        /* Scroll Progress Bar */
        #scroll-path { position: fixed; top: 0; left: 0; width: 100%; height: 4px; background: rgba(255,255,255,0.05); z-index: 100001; }
        #scroll-fill { height: 100%; width: 0%; background: linear-gradient(90deg, var(--primary), var(--success)); }

        /* Dynamic Background */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle at 50% 50%, transparent 10%, #000 90%); z-index: -1; }

        nav { position: fixed; top: 0; width: 100%; padding: 20px; display: flex; justify-content: space-between; align-items: center; z-index: 10000; background: rgba(0,0,0,0.85); backdrop-filter: blur(25px); border-bottom: 1px solid var(--border); }
        .nav-logo { font-weight: 900; font-size: 1.5rem; background: linear-gradient(45deg, #fff, var(--primary)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 110px 18px 60px; }

        /* Hero Hub Card */
        .hero-card { background: var(--glass); border: 1.5px solid var(--border); border-radius: 45px; padding: 55px 25px; text-align: center; margin-bottom: 30px; backdrop-filter: blur(20px); box-shadow: 0 30px 60px rgba(0,0,0,0.6); }
        .live-tag { display: inline-flex; align-items: center; gap: 8px; background: rgba(0, 255, 136, 0.1); color: var(--success); padding: 7px 15px; border-radius: 50px; font-size: 0.7rem; font-weight: 900; border: 1px solid var(--success); margin-bottom: 20px; }

        /* Cards & Clickables */
        .card-wrap { background: var(--glass); border: 1.5px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 25px; }
        .section-header { font-size: 1.1rem; font-weight: 900; margin-bottom: 20px; color: var(--primary); display: flex; align-items: center; gap: 10px; border-bottom: 1px solid rgba(255,255,255,0.1); padding-bottom: 15px; }

        /* Real Clickable Social Icons */
        .social-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 15px; margin-top: 10px; }
        .social-box { aspect-ratio: 1/1; background: #0c0c0c; border: 1.5px solid #222; border-radius: 20px; display: flex; align-items: center; justify-content: center; font-size: 1.4rem; color: #fff; text-decoration: none; transition: 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); }
        .social-box:hover { border-color: var(--primary); color: var(--primary); transform: translateY(-8px) rotate(5deg); box-shadow: 0 10px 25px rgba(0,242,254,0.4); }

        .clickable-row { display: flex; justify-content: space-between; align-items: center; padding: 18px 5px; border-bottom: 1px solid rgba(255,255,255,0.05); text-decoration: none; color: #ccc; transition: 0.3s; font-size: 0.95rem; }
        .clickable-row:hover { color: #fff; transform: translateX(10px); background: rgba(255,255,255,0.02); }

        .btn-supreme { background: linear-gradient(90deg, var(--primary), var(--secondary)); border: none; padding: 22px; border-radius: 25px; color: #000; font-weight: 900; width: 100%; text-decoration: none; display: block; text-align: center; margin-top: 25px; box-shadow: 0 10px 30px rgba(0, 242, 254, 0.3); }

        /* Professional Deep Modals */
        .modal { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.98); z-index: 200000; backdrop-filter: blur(40px); overflow-y: auto; }
        .modal-content { position: relative; margin: 60px auto; width: 92%; max-width: 440px; background: #080808; border: 1.5px solid var(--primary); border-radius: 40px; padding: 45px 30px; box-shadow: 0 0 50px rgba(0, 242, 254, 0.1); }
        .modal-content h2 { color: var(--primary); font-size: 1.8rem; margin-bottom: 25px; font-weight: 900; text-align: center; }
        .modal-text { color: #ccc; line-height: 1.8; font-size: 0.95rem; white-space: pre-wrap; margin-bottom: 30px; }

        footer { text-align: center; opacity: 0.3; font-size: 0.7rem; letter-spacing: 4px; margin-top: 60px; padding-bottom: 20px; }

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
                <span id="v-count">156</span> ACTIVE NODES
            </div>
            <h4 id="greeting" style="color: #fff; font-weight: 800; font-size: 0.8rem; letter-spacing: 5px; opacity: 0.5; margin-bottom: 15px;">INITIALIZING...</h4>
            <h1 style="font-size: 3.5rem; font-weight: 900; letter-spacing: -3px; line-height: 1; color: var(--primary);">Web-Hub</h1>
            <p style="color: #aaa; margin: 20px 0 35px; line-height: 1.7; font-size: 0.95rem;">
                Architecting elite digital experiences with <b>Muhammad Nazim</b>. High-performance code meets premium design aesthetics.
            </p>
            <a href="https://wa.me/923332637235" target="_blank" class="btn-supreme"><i class="fab fa-whatsapp"></i> START PROJECT</a>
        </section>

        <div class="card-wrap" data-aos="fade-up">
            <h2 class="section-header"><i class="fas fa-network-wired"></i> Social Ecosystem</h2>
            <div class="social-grid">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-box" title="Facebook">
                    <i class="fab fa-facebook-f"></i>
                </a>
                <a href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank" class="social-box" title="Instagram">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-7401b6310" target="_blank" class="social-box" title="LinkedIn">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="https://wa.me/923332637235" target="_blank" class="social-box" title="WhatsApp">
                    <i class="fab fa-whatsapp"></i>
                </a>
            </div>
        </div>

        <div class="card-wrap" data-aos="fade-up">
            <h2 class="section-header"><i class="fas fa-brain"></i> Intelligence Hub</h2>
            
            <a href="javascript:void(0)" onclick="openInModal('Contact Details', '📞 Direct Line: +92 333 2637235\n✉️ Official Email: info@webhub.com\n📍 Operations: Karachi Tech Zone, Pakistan\n⏰ Support: 24/7 Priority Assistance')" class="clickable-row">
                <span>Contact Protocols</span> <i class="fas fa-chevron-right"></i>
            </a>

            <a href="javascript:void(0)" onclick="openInModal('Security Manifesto', 'Privacy is our priority. Web-Hub Infinity uses end-to-end encryption for all project logic and follows strict non-disclosure protocols (NDA) for all architectural blueprints.')" class="clickable-row">
                <span>Privacy & Security</span> <i class="fas fa-chevron-right"></i>
            </a>

            <a href="javascript:void(0)" onclick="openInModal('Our Roadmap', '1. Discovery: Goal analysis.\n2. Strategy: UI/UX Blueprinting.\n3. Build: High-Performance Coding.\n4. Deploy: Global Optimization.')" class="clickable-row">
                <span>Operational Roadmap</span> <i class="fas fa-chevron-right"></i>
            </a>

            <a href="javascript:void(0)" onclick="openInModal('Pricing Structure', '• Landing Tier: 15k - 25k\n• Corporate Pro: 35k - 60k\n• Full Enterprise: 80k+\n(Note: Prices are flexible based on project scope)')" class="clickable-row">
                <span>Pricing Calculator</span> <i class="fas fa-chevron-right"></i>
            </a>
        </div>

        <div class="card-wrap" data-aos="fade-up">
            <h2 class="section-header"><i class="fas fa-map-marked-alt"></i> Corporate HQ</h2>
            <div style="border-left: 2px solid var(--primary); padding-left: 20px; margin: 15px 0;">
                <p style="font-weight: 800; font-size: 1.1rem; color: #fff;">Muhammad Nazim</p>
                <p style="color: #888; font-size: 0.9rem;">Web-Hub Digital Intelligence Center</p>
                <p style="color: #888; font-size: 0.9rem;">Karachi, PK | 2026 Operations</p>
                <p style="color: var(--primary); font-weight: 900; margin-top: 10px;">HQ: +92 333 2637235</p>
            </div>
        </div>

        <footer>
            © 2026 MUHAMMAD NAZIM • WEB-HUB INFINITY MASTER CORE
        </footer>
    </div>

    <div id="intelModal" class="modal">
        <div class="modal-content">
            <h2 id="modalTitle"></h2>
            <div id="modalText" class="modal-text"></div>
            <button onclick="closeIntelModal()" class="btn-supreme" style="color: #000; margin-top: 0;">DISMISS</button>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Advanced Cursor Tracking
        const cursor = document.getElementById('cursor');
        const aura = document.getElementById('cursor-aura');
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
            aura.style.left = e.clientX + 'px';
            aura.style.top = e.clientY + 'px';
        });

        // Smart Scroll Progress
        window.addEventListener('scroll', () => {
            const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            const scrolled = (winScroll / height) * 100;
            document.getElementById('scroll-fill').style.width = scrolled + "%";
        });

        // Live Clock & Dynamic Greeting
        function runSystemEngine() {
            const now = new Date();
            document.getElementById('live-time').innerText = now.toLocaleTimeString();
            const hr = now.getHours();
            const greet = hr < 12 ? "SUBH BAKHAIR ☀️" : hr < 18 ? "ASSALAM-O-ALAIKUM 🌤️" : "SHAB BAKHAIR 🌙";
            document.getElementById('greeting').innerText = greet;
        }
        setInterval(runSystemEngine, 1000);
        runSystemEngine();

        // Modal Intelligence Engine
        function openInModal(t, b) {
            document.getElementById('modalTitle').innerText = t;
            document.getElementById('modalText').innerText = b;
            document.getElementById('intelModal').style.display = 'block';
            document.body.style.overflow = 'hidden';
        }
        function closeIntelModal() {
            document.getElementById('intelModal').style.display = 'none';
            document.body.style.overflow = 'auto';
        }

        // Live Node Pulse
        setInterval(() => {
            let count = parseInt(document.getElementById('v-count').innerText);
            document.getElementById('v-count').innerText = count + (Math.random() > 0.5 ? 1 : -1);
        }, 3000);
    </script>
</body>
</html>
