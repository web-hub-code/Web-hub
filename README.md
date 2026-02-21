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
            --success: #00ff88; --bg: #010204; --glass: rgba(255, 255, 255, 0.03);
            --border: rgba(0, 242, 254, 0.15);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; cursor: none; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Next-Gen Interactive Background */
        #canvas-bg { position: fixed; top: 0; left: 0; z-index: -1; pointer-events: none; }
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.1); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle at 50% 50%, transparent 10%, #000 90%); z-index: -1; }

        /* Futuristic Cursor */
        #cursor { width: 8px; height: 8px; background: var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 100000; box-shadow: 0 0 15px var(--primary); transition: transform 0.1s ease; }
        #cursor-aura { width: 40px; height: 40px; border: 1px solid var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 99999; transition: 0.15s ease-out; transform: translate(-50%, -50%); }

        /* Nav & Progress */
        #scroll-path { position: fixed; top: 0; left: 0; width: 100%; height: 3px; background: rgba(255,255,255,0.05); z-index: 100001; }
        #scroll-fill { height: 100%; width: 0%; background: linear-gradient(90deg, var(--primary), var(--success)); }
        
        nav { position: fixed; top: 0; width: 100%; padding: 20px; display: flex; justify-content: space-between; align-items: center; z-index: 10000; background: rgba(0,0,0,0.85); backdrop-filter: blur(25px); border-bottom: 1px solid var(--border); }
        .nav-logo { font-weight: 900; font-size: 1.5rem; letter-spacing: -1px; background: linear-gradient(45deg, #fff, var(--primary)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 110px 18px 60px; }

        /* Hero Glass Card */
        .hero-card { background: var(--glass); border: 1px solid var(--border); border-radius: 40px; padding: 50px 25px; text-align: center; margin-bottom: 30px; backdrop-filter: blur(20px); position: relative; overflow: hidden; box-shadow: 0 40px 100px rgba(0,0,0,0.6); }
        .hero-card::before { content: ''; position: absolute; top: -50%; left: -50%; width: 200%; height: 200%; background: conic-gradient(transparent, var(--primary), transparent 30%); animation: rotate 10s linear infinite; z-index: -1; opacity: 0.1; }

        /* Modern Lists (As per your Screenshot) */
        .corp-wrap { background: var(--glass); border: 1px solid var(--border); border-radius: 35px; padding: 25px; margin-bottom: 25px; }
        .section-header { font-size: 1.1rem; font-weight: 900; margin-bottom: 20px; color: var(--primary); display: flex; align-items: center; gap: 10px; }
        .link-row { display: flex; justify-content: space-between; align-items: center; padding: 18px 0; border-bottom: 1px solid rgba(255,255,255,0.05); text-decoration: none; color: #ccc; transition: 0.3s; }
        .link-row:hover { color: #fff; transform: translateX(5px); }
        .link-row i { font-size: 0.8rem; opacity: 0.5; }

        /* Floating WA Button */
        .floating-action { position: fixed; bottom: 30px; right: 25px; z-index: 10000; }
        .wa-btn { width: 65px; height: 65px; background: #25d366; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1.8rem; color: #fff; box-shadow: 0 15px 35px rgba(37, 211, 102, 0.4); text-decoration: none; animation: float 3s ease-in-out infinite; }

        /* HQ Block */
        .hq-box { padding: 20px; border-left: 2px solid var(--primary); background: rgba(0, 242, 254, 0.02); margin-top: 15px; border-radius: 0 20px 20px 0; }
        .hq-box p { font-size: 0.9rem; color: #888; margin-bottom: 5px; }

        /* Success Popups */
        .modal { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.98); z-index: 200000; backdrop-filter: blur(30px); }
        .modal-body { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); width: 85%; max-width: 400px; background: #0a0a0a; border: 1px solid var(--primary); border-radius: 40px; padding: 40px; text-align: center; }

        @keyframes rotate { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
        @keyframes float { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-10px); } }
        @keyframes pulse { 0% { transform: scale(1); opacity: 1; } 50% { transform: scale(1.6); opacity: 0; } 100% { transform: scale(1); opacity: 1; } }

        /* Mobile specific adjustments */
        @media (max-width: 480px) { .hero-card { padding: 40px 15px; } .hub-title { font-size: 2.5rem; } }
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
            <div style="display: inline-flex; align-items: center; gap: 8px; background: rgba(0, 255, 136, 0.1); color: var(--success); padding: 8px 16px; border-radius: 50px; font-size: 0.7rem; font-weight: 900; margin-bottom: 20px; border: 1px solid var(--success);">
                <div style="width: 8px; height: 8px; background: var(--success); border-radius: 50%; animation: pulse 1.5s infinite;"></div>
                <span id="visitor-count">104</span> ONLINE NOW
            </div>
            <h4 id="greeting" style="color: #fff; font-weight: 800; font-size: 0.8rem; letter-spacing: 4px; opacity: 0.6;">SUBH BAKHAIR</h4>
            <h1 style="font-size: 3.5rem; font-weight: 900; letter-spacing: -3px; line-height: 1; margin: 15px 0;">Web-Hub</h1>
            <p style="color: #888; font-size: 0.95rem; line-height: 1.7; margin-bottom: 30px;">
                Muhammad Nazim's premium ecosystem for web development and AI automation. Building the future, one pixel at a time.
            </p>
            <a href="https://wa.me/923332637235" class="wa-btn" style="width: 100%; border-radius: 20px; font-size: 1rem; font-weight: 900; gap: 10px;">
                <i class="fab fa-whatsapp"></i> START YOUR PROJECT
            </a>
        </section>

        <div class="corp-wrap" data-aos="fade-up">
            <h2 class="section-header"><i class="fas fa-building"></i> Company</h2>
            <a href="javascript:void(0)" onclick="showModal('Success Stories', 'Hamne last 12 months mein 150% growth achieve ki hy aur 40+ international startups ko digitalize kiya hy.')" class="link-row">
                <span>Success Stories</span> <i class="fas fa-chevron-right"></i>
            </a>
            <a href="javascript:void(0)" onclick="showModal('30% Affiliate', 'Sirf ek referral dein aur jab project finalize hoga, 30% commission aapke bank account mein hoga.')" class="link-row">
                <span>30% Affiliate Program</span> <i class="fas fa-chevron-right"></i>
            </a>
            <a href="javascript:void(0)" onclick="showModal('Flexible Pricing', 'Websites start from 15k and go up to 500k. Final price hum hamesha customer ki requirement dekh kar decide karte hain.')" class="link-row">
                <span>Pricing Calculator</span> <i class="fas fa-chevron-right"></i>
            </a>
            <a href="#" class="link-row"><span>Our Network</span> <i class="fas fa-chevron-right"></i></a>
            <a href="#" class="link-row"><span>Privacy Policy</span> <i class="fas fa-chevron-right"></i></a>
        </div>

        <div class="corp-wrap" data-aos="fade-up">
            <h2 class="section-header"><i class="fas fa-map-marker-alt"></i> Corporate HQ</h2>
            <div class="hq-box">
                <p><strong>Muhammad Nazim</strong></p>
                <p>Web-Hub Digital Center, Karachi</p>
                <p>Pakistan | Global Reach</p>
                <p style="color: var(--primary); margin-top: 10px; font-weight: 900;">Direct: +92 333 2637235</p>
            </div>
            
            <div style="margin-top: 30px;">
                <p style="font-size: 0.8rem; color: #666; margin-bottom: 10px;">Start Free 30 Day Trial</p>
                <div style="background: #000; border: 1px solid #222; border-radius: 15px; display: flex; overflow: hidden;">
                    <input type="email" placeholder="Enter email" style="background: transparent; border: none; padding: 15px; color: #fff; flex: 1; outline: none;">
                    <button style="background: var(--accent); border: none; padding: 0 20px; color: #fff; font-weight: 700;">Submit</button>
                </div>
            </div>
        </div>

        <div style="display: flex; gap: 12px; justify-content: center; margin-top: 30px;" data-aos="zoom-in">
            <a href="https://facebook.com/share/12E6tH73q6/" class="social-item" style="width: 50px; height: 50px; background: #0c0c0c; border: 1px solid #222; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: #fff; text-decoration: none;"><i class="fab fa-facebook-f"></i></a>
            <a href="https://www.instagram.com/itz_nazim_03/" class="social-item" style="width: 50px; height: 50px; background: #0c0c0c; border: 1px solid #222; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: #fff; text-decoration: none;"><i class="fab fa-instagram"></i></a>
            <a href="https://www.linkedin.com/in/muhammad-nazim-0100772bb" class="social-item" style="width: 50px; height: 50px; background: #0c0c0c; border: 1px solid #222; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: #fff; text-decoration: none;"><i class="fab fa-linkedin-in"></i></a>
        </div>

        <footer style="margin-top: 60px; text-align: center; border-top: 1px solid #111; padding-top: 30px;">
            <p style="font-size: 0.7rem; color: #444; letter-spacing: 5px;">© 2026 WEB-HUB | ALL RIGHTS RESERVED</p>
        </footer>
    </div>

    <div class="floating-action">
        <a href="https://wa.me/923332637235" class="wa-btn"><i class="fab fa-whatsapp"></i></a>
    </div>

    <div id="infoModal" class="modal">
        <div class="modal-body">
            <h3 id="modalTitle" style="color: var(--primary); margin-bottom: 20px; font-size: 1.5rem;"></h3>
            <p id="modalText" style="color: #ccc; line-height: 1.6; margin-bottom: 30px;"></p>
            <button onclick="hideModal()" style="background: var(--primary); border: none; padding: 12px 40px; border-radius: 50px; color: #000; font-weight: 900;">GOT IT</button>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Advanced Cursor
        const cursor = document.getElementById('cursor');
        const aura = document.getElementById('cursor-aura');
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
            aura.style.left = e.clientX + 'px';
            aura.style.top = e.clientY + 'px';
        });

        // Scroll Progress
        window.addEventListener('scroll', () => {
            const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            const scrolled = (winScroll / height) * 100;
            document.getElementById('scroll-fill').style.width = scrolled + "%";
        });

        // Live Clock & Greeting Engine
        function runLive() {
            const now = new Date();
            document.getElementById('live-time').innerText = now.toLocaleTimeString();
            const hr = now.getHours();
            const greet = hr < 12 ? "SUBH BAKHAIR ☀️" : hr < 18 ? "ASSALAM-O-ALAIKUM 🌤️" : "SHAB BAKHAIR 🌙";
            document.getElementById('greeting').innerText = greet;
        }
        setInterval(runLive, 1000);
        runLive();

        // Modal Engine
        function showModal(title, text) {
            document.getElementById('modalTitle').innerText = title;
            document.getElementById('modalText').innerText = text;
            document.getElementById('infoModal').style.display = 'block';
        }
        function hideModal() { document.getElementById('infoModal').style.display = 'none'; }

        // Live Visitors Pulse
        setInterval(() => {
            let count = parseInt(document.getElementById('visitor-count').innerText);
            document.getElementById('visitor-count').innerText = count + (Math.random() > 0.5 ? 1 : -1);
        }, 3000);
    </script>
</body>
</html>
