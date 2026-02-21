<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    
    <title>Web-Hub Infinity | Muhammad Nazim - Premium Web Solutions</title>
    <meta name="description" content="Custom Web Development, AI Automation, and UI/UX Design by Muhammad Nazim. Next-level digital solutions with flexible pricing.">
    <meta name="keywords" content="Muhammad Nazim, Web-Hub, Web Developer Pakistan, AI Automation, Custom Website Pricing">
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;900&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #7000ff;
            --success: #00ff88; --bg: #010204; --glass: rgba(255, 255, 255, 0.05);
            --border: rgba(0, 242, 254, 0.2);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; cursor: none; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Custom Cursor Experience */
        #cursor { width: 12px; height: 12px; background: var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 99999; mix-blend-mode: difference; transition: transform 0.1s; }
        #cursor-blur { width: 300px; height: 300px; background: radial-gradient(circle, rgba(0, 242, 254, 0.1) 0%, transparent 70%); position: fixed; pointer-events: none; z-index: 99998; border-radius: 50%; transform: translate(-50%, -50%); transition: 0.15s ease-out; }

        /* Smooth Progress Bar */
        #progress-bar { position: fixed; top: 0; left: 0; height: 4px; background: linear-gradient(to right, var(--primary), var(--success)); z-index: 100000; width: 0%; transition: 0.2s; }

        /* Background Visuals */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.18); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 0%, #000 100%); z-index: -1; }

        /* Premium Nav */
        nav { position: fixed; top: 0; width: 100%; padding: 18px 25px; display: flex; justify-content: space-between; align-items: center; z-index: 10000; background: rgba(0,0,0,0.7); backdrop-filter: blur(25px); border-bottom: 1px solid var(--border); }
        .nav-logo { font-weight: 900; font-size: 1.6rem; background: linear-gradient(45deg, var(--primary), var(--success)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -1px; }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 110px 20px 60px; }

        /* Hero Hub */
        .hero { background: var(--glass); border: 1px solid var(--border); border-radius: 45px; padding: 50px 30px; text-align: center; margin-bottom: 35px; backdrop-filter: blur(15px); position: relative; overflow: hidden; }
        .live-status { display: inline-flex; align-items: center; gap: 8px; background: rgba(0, 255, 136, 0.1); color: var(--success); padding: 7px 15px; border-radius: 50px; font-size: 0.75rem; font-weight: 800; margin-bottom: 25px; border: 1px solid var(--success); }
        .pulse-dot { width: 8px; height: 8px; background: var(--success); border-radius: 50%; animation: pulse 1.5s infinite; }

        /* Service Cards - Clickable */
        .s-card { background: var(--glass); border: 1px solid var(--border); border-radius: 35px; padding: 30px; margin-bottom: 22px; transition: 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275); position: relative; overflow: hidden; }
        .s-card:hover { border-color: var(--primary); transform: translateY(-10px); background: rgba(0, 242, 254, 0.1); box-shadow: 0 25px 50px rgba(0,0,0,0.6); }
        .s-card i { font-size: 2.5rem; color: var(--primary); margin-bottom: 15px; display: block; }
        .price-badge { position: absolute; top: 25px; right: 25px; font-size: 0.65rem; background: var(--primary); color: #000; padding: 5px 12px; border-radius: 50px; font-weight: 900; letter-spacing: 1px; }

        /* Review Section */
        .review-card { background: rgba(255,255,255,0.02); padding: 30px; border-radius: 30px; border: 1px solid var(--border); margin: 45px 0; text-align: center; }
        .stars { color: #ffcc00; margin-bottom: 15px; font-size: 1.1rem; }

        /* FAQ System */
        details { background: var(--glass); padding: 20px; border-radius: 25px; border: 1px solid var(--border); margin-bottom: 15px; transition: 0.3s; }
        summary { font-weight: 600; font-size: 0.95rem; cursor: none; outline: none; }
        details p { padding-top: 15px; font-size: 0.85rem; opacity: 0.7; line-height: 1.6; }

        /* Supreme CTA */
        .btn-supreme { display: flex; align-items: center; justify-content: center; gap: 12px; width: 100%; padding: 22px; background: linear-gradient(45deg, var(--primary), var(--secondary)); border-radius: 25px; color: #000; font-weight: 900; text-decoration: none; text-transform: uppercase; box-shadow: 0 15px 45px rgba(0, 242, 254, 0.4); margin-top: 20px; transition: 0.3s; }
        .btn-supreme:active { transform: scale(0.95); }

        /* Modal Overlay */
        .modal { display: none; position: fixed; z-index: 200000; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.98); backdrop-filter: blur(30px); }
        .modal-inner { background: #0a0a0a; margin: 18% auto; padding: 45px; border: 1px solid var(--primary); width: 92%; max-width: 480px; border-radius: 45px; text-align: center; position: relative; box-shadow: 0 0 100px rgba(0, 242, 254, 0.1); }

        /* Floating WA */
        .wa-float { position: fixed; bottom: 35px; right: 25px; width: 65px; height: 65px; background: #25d366; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 32px; color: white; z-index: 15000; box-shadow: 0 15px 35px rgba(37, 211, 102, 0.4); text-decoration: none; transition: 0.3s; }

        footer { text-align: center; padding: 70px 20px; opacity: 0.4; font-size: 0.7rem; letter-spacing: 5px; border-top: 1px solid var(--border); margin-top: 50px; }

        @keyframes pulse { 0% { transform: scale(1); opacity: 1; } 50% { transform: scale(1.6); opacity: 0; } 100% { transform: scale(1); opacity: 1; } }
    </style>
</head>
<body>

    <div id="cursor"></div>
    <div id="cursor-blur"></div>
    <div id="progress-bar"></div>

    <nav>
        <div class="nav-logo">WEB-HUB</div>
        <div id="live-clock" style="font-size: 0.8rem; font-weight: 900; color: var(--primary);">00:00:00</div>
    </nav>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        
        <section class="hero" data-aos="zoom-out">
            <div class="live-status"><div class="pulse-dot"></div> <span id="v-count">64</span> ACTIVE USERS</div>
            <h4 id="greet-text" style="color: var(--success); font-weight: 800; font-size: 0.85rem; letter-spacing: 3px; margin-bottom: 10px;">WELCOME</h4>
            <h1 style="font-size: 3.8rem; font-weight: 900; letter-spacing: -3px; line-height: 0.9; margin: 15px 0;">WEB-HUB INFINITY</h1>
            <p style="opacity: 0.7; font-size: 1rem; line-height: 1.8; margin-top: 20px;">
                Leading the digital era with Muhammad Nazim. We craft high-performance assets tailored to your vision.
            </p>
        </section>

        <div data-aos="fade-up">
            <h2 style="margin-bottom: 25px; font-weight: 900; letter-spacing: -1px;">PREMIUM ECOSYSTEM</h2>
            
            <div class="s-card" onclick="openDetails('Elite Web Apps', 'Pricing: Custom (Depends on Features) \n\n Hum modern frameworks (React/Next.js) use karke ultra-fast apps banate hain. Final pricing aapki complex requirements aur design ke mutabiq decide hogi.')">
                <span class="price-badge">VARIABLE</span>
                <i class="fas fa-code-branch"></i>
                <h3>Supreme Development</h3>
                <p style="font-size: 0.85rem; opacity: 0.6;">Scalable SaaS & Corporate Platforms.</p>
            </div>

            <div class="s-card" onclick="openDetails('AI Automation', 'Pricing: Flexible Budget \n\n Aapke business ke liye intelligent AI bots aur automated systems. Pricing aapke workflow ki depth par depend karti hy.')">
                <span class="price-badge">FLEXIBLE</span>
                <i class="fas fa-brain"></i>
                <h3>AI & Intelligence</h3>
                <p style="font-size: 0.85rem; opacity: 0.6;">Smart automation for modern growth.</p>
            </div>

            <div class="s-card" onclick="openDetails('Next-Gen UI/UX', 'Pricing: Per Scope \n\n Visually stunning aur conversion-focused designs. Pricing aapki branding requirements ke mutabiq customize hogi.')">
                <span class="price-badge">CUSTOM</span>
                <i class="fas fa-wand-magic-sparkles"></i>
                <h3>Visual Design</h3>
                <p style="font-size: 0.85rem; opacity: 0.6;">Futuristic UI that drives results.</p>
            </div>
        </div>

        <div class="review-card" data-aos="flip-up">
            <div class="stars">★★★★★</div>
            <p id="r-text" style="font-style: italic; font-size: 0.95rem; opacity: 0.8; line-height: 1.6;">"Web-Hub transformed our workflow. Nazim provided the best price and quality."</p>
            <h5 id="r-author" style="margin-top: 15px; color: var(--primary); letter-spacing: 1px;">— David, Germany</h5>
        </div>

        <div style="margin: 45px 0;" data-aos="fade-up">
            <h3 style="margin-bottom: 20px; font-weight: 900;">BUSINESS QUERIES</h3>
            <details>
                <summary>Pricing fix hoti hy ya kam ho sakti hy?</summary>
                <p>Hamari koi bhi price fix nahi hy. Hum hamesha customer ki requirements aur unke budget ko dekh kar best custom quote tayyar karte hain.</p>
            </details>
            <details>
                <summary>Project delivery ka kya process hy?</summary>
                <p>Simple! Click on WhatsApp, tell your needs, get a quote, and we start. Delivery time depends on features (Usually 1 week).</p>
            </details>
        </div>

        <a href="https://wa.me/923332637235" class="btn-supreme" data-aos="zoom-in">
            <i class="fab fa-whatsapp"></i> GET YOUR CUSTOM QUOTE
        </a>

        <footer>
            <h2 style="font-weight: 900; letter-spacing: -2px; font-size: 3rem; margin-bottom: 15px; opacity: 1; color: white;">Web-Hub</h2>
            <div style="display: flex; justify-content: center; gap: 25px; margin: 30px 0; font-size: 1.8rem;">
                <a href="https://wa.me/923332637235" style="color: white; transition: 0.3s;"><i class="fab fa-whatsapp"></i></a>
                <a href="#" style="color: white; transition: 0.3s;"><i class="fab fa-linkedin-in"></i></a>
                <a href="#" style="color: white; transition: 0.3s;"><i class="fab fa-instagram"></i></a>
            </div>
            <p style="font-size: 0.65rem; opacity: 0.5;">MUHAMMAD NAZIM • GLOBAL DIGITAL SOLUTIONS • EST 2026</p>
        </footer>
    </div>

    <div id="infoModal" class="modal">
        <div class="modal-inner">
            <span style="position:absolute; top:20px; right:30px; font-size:40px; cursor:none; color:var(--primary);" onclick="closeDetails()">&times;</span>
            <h3 id="m-title" style="color: var(--primary); margin-bottom: 20px; font-size: 1.8rem; font-weight: 900;"></h3>
            <p id="m-body" style="font-size: 1rem; line-height: 1.8; opacity: 0.85; white-space: pre-wrap; text-align: left;"></p>
            <a href="https://wa.me/923332637235" class="btn-supreme" style="padding: 16px; font-size: 0.8rem; margin-top: 35px;">Discuss Budget on WhatsApp</a>
        </div>
    </div>

    <a href="https://wa.me/923332637235" class="wa-float">
        <i class="fab fa-whatsapp"></i>
    </a>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Cursor Movement
        const cursor = document.getElementById('cursor');
        const blur = document.getElementById('cursor-blur');
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
            blur.style.left = e.clientX + 'px';
            blur.style.top = e.clientY + 'px';
        });

        // Scroll Progress Line
        window.onscroll = () => {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("progress-bar").style.width = (winScroll / height) * 100 + "%";
        };

        // Live Clock & Time-based Greeting
        function runLiveEngine() {
            const now = new Date();
            document.getElementById('live-clock').innerText = now.toLocaleTimeString();
            let hr = now.getHours();
            let greeting = hr < 12 ? "SUBH BAKHAIR ☀️" : hr < 18 ? "ASSALAM-O-ALAIKUM 🌤️" : "SHAB BAKHAIR 🌙";
            document.getElementById('greet-text').innerText = greeting;
        }
        setInterval(runLiveEngine, 1000);
        runLiveEngine();

        // Modal System
        function openDetails(t, b) {
            document.getElementById('m-title').innerText = t;
            document.getElementById('m-body').innerText = b;
            document.getElementById('infoModal').style.display = "block";
        }
        function closeDetails() { document.getElementById('infoModal').style.display = "none"; }

        // Testimonial Engine
        const feeds = [
            {t: "Nazim delivered exactly what we needed. Pricing was very fair.", n: "— Ahmed, Dubai"},
            {t: "The design quality is on another level. Very modern vibe.", n: "— Liam, USA"},
            {t: "Best developer for custom business automation.", n: "— Zeeshan, PK"}
        ];
        let fIdx = 0;
        setInterval(() => {
            fIdx = (fIdx + 1) % feeds.length;
            document.getElementById('r-text').innerText = `"${feeds[fIdx].t}"`;
            document.getElementById('r-author').innerText = feeds[fIdx].n;
        }, 5000);

        // Fake Live Visitor Counter
        setInterval(() => {
            let count = parseInt(document.getElementById('v-count').innerText);
            document.getElementById('v-count').innerText = count + (Math.random() > 0.5 ? 1 : -1);
        }, 4000);
    </script>
</body>
</html>
