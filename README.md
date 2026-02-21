<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    
    <title>Web-Hub Infinity | Muhammad Nazim - Professional Web Solutions</title>
    <meta name="description" content="Premium Web Development, AI Automation, and UI/UX by Muhammad Nazim. Custom pricing for global businesses.">
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;900&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --success: #00ff88;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(0, 242, 254, 0.15);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; cursor: none; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Custom Neon Cursor */
        #cursor { width: 10px; height: 10px; background: var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 99999; mix-blend-mode: difference; transition: transform 0.1s; }
        #cursor-blur { width: 280px; height: 280px; background: radial-gradient(circle, rgba(0, 242, 254, 0.1) 0%, transparent 70%); position: fixed; pointer-events: none; z-index: 99998; border-radius: 50%; transform: translate(-50%, -50%); }

        /* Background Visuals */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 20%, #000 100%); z-index: -1; }

        /* Navigation */
        nav { position: fixed; top: 0; width: 100%; padding: 18px 25px; display: flex; justify-content: space-between; align-items: center; z-index: 10000; background: rgba(0,0,0,0.8); backdrop-filter: blur(20px); border-bottom: 1px solid var(--border); }
        .nav-logo { font-weight: 900; font-size: 1.6rem; background: linear-gradient(45deg, var(--primary), var(--success)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        .container { width: 100%; max-width: 520px; margin: 0 auto; padding: 100px 20px 60px; }

        /* Hero Card (From Screenshot) */
        .hub-card { background: var(--glass); border: 1.5px solid var(--border); border-radius: 45px; padding: 50px 30px; text-align: center; margin-bottom: 40px; backdrop-filter: blur(15px); }
        .live-tag { display: inline-flex; align-items: center; gap: 8px; background: rgba(0, 255, 136, 0.1); color: var(--success); padding: 6px 14px; border-radius: 50px; font-size: 0.75rem; font-weight: 800; margin-bottom: 20px; border: 1px solid var(--success); }
        .dot { width: 8px; height: 8px; background: var(--success); border-radius: 50%; animation: pulse 1.5s infinite; }

        /* Supreme Button */
        .quote-btn { display: flex; align-items: center; justify-content: center; gap: 12px; width: 100%; padding: 22px; background: linear-gradient(135deg, #00ff88 0%, #00d2ff 100%); border-radius: 25px; color: white; font-weight: 900; text-decoration: none; font-size: 1rem; text-transform: uppercase; margin-top: 30px; box-shadow: 0 10px 25px rgba(0, 255, 136, 0.2); transition: 0.3s; }

        /* Corporate List Styling */
        .section-title { font-size: 1.4rem; font-weight: 900; margin: 40px 0 20px; letter-spacing: 1px; text-transform: uppercase; }
        .corp-link { display: block; color: #888; text-decoration: none; padding: 15px 0; font-size: 1rem; border-bottom: 1px solid rgba(255,255,255,0.05); transition: 0.3s; }
        .corp-link:hover { color: var(--primary); padding-left: 10px; }

        /* HQ Block */
        .hq-info { border-left: 3px solid var(--primary); padding-left: 20px; margin: 25px 0 40px; }
        .hq-info p { font-size: 0.95rem; color: #999; margin-bottom: 8px; line-height: 1.6; }

        /* Social Circles */
        .social-row { display: flex; gap: 15px; margin-top: 25px; flex-wrap: wrap; }
        .social-circle { width: 55px; height: 55px; background: #0c0c0c; border: 1px solid #222; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: white; text-decoration: none; font-size: 1.3rem; transition: 0.4s; }
        .social-circle:hover { border-color: var(--primary); color: var(--primary); transform: translateY(-5px); box-shadow: 0 0 20px rgba(0, 242, 254, 0.2); }

        /* Newsletter Box */
        .start-box { background: #0a0a0a; border: 1px solid #222; border-radius: 20px; display: flex; overflow: hidden; margin-top: 20px; }
        .start-box input { background: transparent; border: none; padding: 18px; color: white; flex: 1; outline: none; }
        .start-box button { background: #6c5ce7; border: none; padding: 0 25px; color: white; font-weight: 700; cursor: none; }

        /* Modal Overlay */
        .modal { display: none; position: fixed; z-index: 100000; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.95); backdrop-filter: blur(20px); }
        .modal-content { background: #0f0f0f; margin: 20% auto; padding: 40px; border: 1px solid var(--primary); width: 90%; max-width: 420px; border-radius: 40px; text-align: center; }

        footer { text-align: left; padding: 60px 0 20px; border-top: 1px solid #111; margin-top: 50px; color: #444; font-size: 0.8rem; }

        @keyframes pulse { 0% { transform: scale(1); opacity: 1; } 50% { transform: scale(1.5); opacity: 0; } 100% { transform: scale(1); opacity: 1; } }
    </style>
</head>
<body>

    <div id="cursor"></div>
    <div id="cursor-blur"></div>

    <nav>
        <div class="nav-logo">WEB-HUB</div>
        <div id="live-timer" style="font-size: 0.8rem; font-weight: 800; color: var(--primary);">00:00:00</div>
    </nav>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        
        <section class="hub-card" data-aos="zoom-in">
            <div class="live-tag"><div class="dot"></div> <span id="v-count">74</span> USERS LIVE</div>
            <h4 id="greet" style="color: var(--success); font-weight: 800; font-size: 0.85rem; letter-spacing: 3px; margin-bottom: 10px;">LOADING...</h4>
            <h1 style="font-size: 3.5rem; font-weight: 900; color: var(--primary); letter-spacing: -2px;">Web-Hub</h1>
            <p style="margin-top: 20px; color: #ddd; line-height: 1.8; font-size: 1rem;">
                Expert digital solutions tailored for your business. We specialize in high-performance web apps and creative branding with flexible pricing.
            </p>
            <a href="https://wa.me/923332637235" class="quote-btn">
                <i class="fab fa-whatsapp"></i> GET A CUSTOM QUOTE
            </a>
        </section>

        <div class="corp-section" data-aos="fade-up">
            <h2 class="section-title">Company</h2>
            <a href="javascript:void(0)" onclick="pop('Success Stories', 'Hamne 50+ clients ke liye custom portals banaye hain. Hum har project ko zero se build karte hain takay result 100% mile.')" class="corp-link">Success Stories</a>
            <a href="javascript:void(0)" onclick="pop('Affiliate Program', 'Humare sath partner banein. Har referral par 30% commission payein. No questions asked.')" class="corp-link">30% Affiliate Program</a>
            <a href="javascript:void(0)" onclick="pop('Pricing Calculator', 'Pricing fix nahi hoti. Ye aapki requirements (Design, Pages, Features) par depend karti hy. WhatsApp karein quote ke liye.')" class="corp-link">Pricing Calculator</a>
            <a href="#" class="corp-link">Our Network</a>
            <a href="#" class="corp-link">Privacy Policy</a>
            <a href="#" class="corp-link">Uptime Status</a>
        </div>

        <div class="corp-section" data-aos="fade-up">
            <h2 class="section-title">Corporate HQ</h2>
            <div class="hq-info">
                <p>Karachi, Pakistan | Web-Hub Center</p>
                <p>Suite 262, Online Excellence</p>
                <p style="color: var(--primary); font-weight: 800;">Toll Free: +92 333 2637235</p>
            </div>

            <h2 class="section-title">Social Connect</h2>
            <div class="social-row">
                <a href="https://facebook.com/share/12E6tH73q6/" class="social-circle"><i class="fab fa-facebook-f"></i></a>
                <a href="https://wa.me/923332637235" class="social-circle"><i class="fab fa-whatsapp"></i></a>
                <a href="mailto:info@webhub.com" class="social-circle"><i class="far fa-envelope"></i></a>
                <a href="https://www.instagram.com/itz_nazim_03/" class="social-circle"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-0100772bb" class="social-circle"><i class="fab fa-linkedin-in"></i></a>
            </div>
        </div>

        <div class="corp-section" data-aos="fade-up">
            <h2 class="section-title">Get Started</h2>
            <p style="font-size: 0.9rem; color: #888;">Start Free 30 Day Trial</p>
            <div class="start-box">
                <input type="email" placeholder="Enter your email address">
                <button type="button" onclick="alert('Thank you! Our team will contact you.')">Submit</button>
            </div>
        </div>

        <footer>
            <div style="display:flex; justify-content:space-between; align-items:center;">
                <span>© 2026 Web-Hub Infinity. All rights reserved.</span>
                <div style="width:40px; height:40px; background:#6c5ce7; border-radius:50%; display:flex; align-items:center; justify-content:center; color:white;">
                    <i class="fas fa-chevron-up"></i>
                </div>
            </div>
        </footer>
    </div>

    <div id="popModal" class="modal">
        <div class="modal-content">
            <h3 id="popTitle" style="color:var(--primary); margin-bottom:20px; font-size:1.8rem;"></h3>
            <p id="popBody" style="font-size:1rem; color:#ccc; line-height:1.7; margin-bottom:30px;"></p>
            <button onclick="closePop()" style="background:var(--primary); border:none; padding:12px 35px; border-radius:50px; color:#000; font-weight:900;">CLOSE</button>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Custom Cursor Movement
        const cursor = document.getElementById('cursor');
        const blur = document.getElementById('cursor-blur');
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
            blur.style.left = e.clientX + 'px';
            blur.style.top = e.clientY + 'px';
        });

        // Live Engine (Clock & Greeting)
        function updateUI() {
            const now = new Date();
            document.getElementById('live-timer').innerText = now.toLocaleTimeString();
            let hr = now.getHours();
            let greeting = hr < 12 ? "SUBH BAKHAIR ☀️" : hr < 18 ? "ASSALAM-O-ALAIKUM 🌤️" : "SHAB BAKHAIR 🌙";
            document.getElementById('greet').innerText = greeting;
        }
        setInterval(updateUI, 1000);
        updateUI();

        // Visitor Counter Pulse
        setInterval(() => {
            let count = parseInt(document.getElementById('v-count').innerText);
            document.getElementById('v-count').innerText = count + (Math.random() > 0.5 ? 1 : -1);
        }, 4000);

        // Modal Logic
        function pop(t, b) {
            document.getElementById('popTitle').innerText = t;
            document.getElementById('popBody').innerText = b;
            document.getElementById('popModal').style.display = 'block';
        }
        function closePop() {
            document.getElementById('popModal').style.display = 'none';
        }
    </script>
</body>
</html>
