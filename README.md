<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub Infinity | Muhammad Nazim Official</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;900&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #7000ff;
            --success: #00ff88; --bg: #010204; --glass: rgba(255, 255, 255, 0.03);
            --border: rgba(0, 242, 254, 0.2);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Scroll Progress */
        #progress-bar { position: fixed; top: 0; left: 0; height: 3px; background: var(--primary); width: 0%; z-index: 20000; }

        /* Background Visuals */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.1); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 0%, #000 100%); z-index: -1; }

        /* Notifications & Alerts */
        #notif-box { position: fixed; top: 80px; right: -300px; width: 280px; background: var(--glass); backdrop-filter: blur(20px); border: 1px solid var(--primary); color: white; padding: 15px; border-radius: 20px; z-index: 15000; transition: 0.6s; font-size: 0.8rem; }

        /* Navigation */
        nav { position: fixed; top: 0; width: 100%; padding: 20px; display: flex; justify-content: space-between; align-items: center; z-index: 10000; background: rgba(0,0,0,0.5); backdrop-filter: blur(10px); border-bottom: 1px solid var(--border); }
        .nav-logo { font-weight: 900; font-size: 1.5rem; letter-spacing: -1px; background: linear-gradient(45deg, var(--primary), var(--success)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 100px 18px 50px; }

        /* Hero Section */
        .hero-card { background: var(--glass); border: 1px solid var(--border); border-radius: 40px; padding: 40px 30px; text-align: center; margin-bottom: 30px; }
        .brand-name { font-size: 4.2rem; font-weight: 900; letter-spacing: -3px; line-height: 1; margin-bottom: 10px; }
        .live-tag { display: inline-flex; align-items: center; gap: 8px; background: rgba(255,0,0,0.1); color: #ff4444; padding: 5px 15px; border-radius: 50px; font-size: 0.7rem; font-weight: 800; margin-bottom: 20px; }
        .dot { width: 8px; height: 8px; background: #ff4444; border-radius: 50%; animation: pulse 1s infinite; }

        /* Typing Effect */
        .typing-text { color: var(--primary); font-weight: 800; }

        /* Partner Marquee */
        .marquee { overflow: hidden; white-space: nowrap; margin: 30px 0; opacity: 0.4; }
        .marquee-content { display: inline-block; animation: scroll 20s linear infinite; }
        .marquee-content span { margin-right: 50px; font-size: 0.8rem; letter-spacing: 3px; font-weight: 800; }

        /* Services Grid (Ultimate) */
        .service-box { background: var(--glass); border: 1px solid var(--border); border-radius: 30px; padding: 25px; margin-bottom: 15px; cursor: pointer; transition: 0.4s; }
        .service-box:hover { border-color: var(--primary); background: rgba(0,242,254,0.05); }

        /* FAQ Accordion */
        .faq-item { background: rgba(255,255,255,0.02); border-radius: 15px; margin-bottom: 10px; overflow: hidden; border: 1px solid var(--border); }
        .faq-header { padding: 15px 20px; cursor: pointer; display: flex; justify-content: space-between; font-weight: 600; font-size: 0.9rem; }
        .faq-body { padding: 0 20px; max-height: 0; transition: 0.3s; opacity: 0; font-size: 0.8rem; color: #ccc; }

        /* Subscription Box */
        .sub-box { background: linear-gradient(135deg, #0a0a0a 0%, #1a1a1a 100%); padding: 30px; border-radius: 30px; border: 1px solid var(--primary); text-align: center; margin: 40px 0; }
        .sub-input { width: 100%; padding: 15px; border-radius: 15px; border: none; background: #222; color: white; margin: 15px 0; outline: none; }
        
        .main-cta { display: flex; align-items: center; justify-content: center; gap: 10px; width: 100%; padding: 22px; background: linear-gradient(45deg, var(--primary), var(--secondary)); border-radius: 25px; color: #000; font-weight: 900; text-decoration: none; text-transform: uppercase; margin-top: 20px; box-shadow: 0 10px 40px rgba(0, 242, 254, 0.3); }

        /* Footer HQ */
        .footer-hq { background: #000; border: 1px solid var(--border); border-radius: 45px; padding: 45px 30px; margin-top: 50px; }
        
        @keyframes scroll { from { transform: translateX(0); } to { transform: translateX(-50%); } }
        @keyframes pulse { 0% { opacity: 1; } 50% { opacity: 0.3; } 100% { opacity: 1; } }

        footer { text-align: center; padding: 50px; opacity: 0.2; font-size: 0.7rem; letter-spacing: 5px; }
    </style>
</head>
<body>

    <div id="progress-bar"></div>

    <nav>
        <div class="nav-logo">WEB-HUB</div>
        <div id="live-time" style="font-size: 0.7rem; opacity: 0.6; font-weight: 800;">00:00:00</div>
    </nav>

    <div id="notif-box">
        <strong>New Alert:</strong> <span id="notif-text">Incoming client request...</span>
    </div>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        
        <section class="hero-card" data-aos="fade-up">
            <div class="live-tag"><div class="dot"></div> <span id="visitor-count">24</span> ONLINE VISITORS</div>
            <h4 id="greeting" style="color: var(--success); font-weight: 800; margin-bottom: 5px;">Good Day!</h4>
            <h1 class="brand-name">WEB-HUB</h1>
            <p style="font-size: 1.1rem; font-weight: 600;">We Build <span class="typing-text" id="typewriter"></span></p>
        </section>

        <div class="marquee">
            <div class="marquee-content">
                <span>TRUSTED BY 50+ BRANDS</span>
                <span>GLOBAL CLIENTS</span>
                <span>SUPREME QUALITY</span>
                <span>FAST DELIVERY</span>
                <span>TRUSTED BY 50+ BRANDS</span>
                <span>GLOBAL CLIENTS</span>
            </div>
        </div>

        <div data-aos="fade-up">
            <div class="service-box" onclick="toggleDetails('Web Apps', 'Hum custom dashboard aur SaaS applications banate hain jo scalability ke liye optimized hoti hain.')">
                <i class="fas fa-layer-group" style="color: var(--primary); font-size: 1.8rem; margin-bottom: 10px;"></i>
                <h3>Supreme Web Apps</h3>
                <p style="font-size: 0.8rem; opacity: 0.6;">Complex problems, simple solutions.</p>
            </div>

            <div class="service-box" onclick="toggleDetails('AI Integration', 'Aapki website khud sochegi aur jawab degi. AI-powered chatbots aur tools humari speciality hain.')">
                <i class="fas fa-brain" style="color: var(--success); font-size: 1.8rem; margin-bottom: 10px;"></i>
                <h3>AI & Automation</h3>
                <p style="font-size: 0.8rem; opacity: 0.6;">Future-proof your business today.</p>
            </div>
        </div>

        <div style="margin: 40px 0;" data-aos="fade-up">
            <h3 style="margin-bottom: 20px; font-weight: 900; letter-spacing: 1px;">COMMON QUESTIONS</h3>
            <div class="faq-item">
                <div class="faq-header" onclick="toggleFaq(this)">How to start? <i class="fas fa-chevron-down"></i></div>
                <div class="faq-body">Simply click the WhatsApp button, share your idea, and get a custom quote within 30 minutes.</div>
            </div>
            <div class="faq-item">
                <div class="faq-header" onclick="toggleFaq(this)">Project Timelines? <i class="fas fa-chevron-down"></i></div>
                <div class="faq-body">Depending on complexity, we deliver within 3 to 14 business days.</div>
            </div>
        </div>

        <div class="sub-box" data-aos="zoom-in">
            <h3 style="font-weight: 900;">STAY UPDATED</h3>
            <p style="font-size: 0.8rem; opacity: 0.6; margin-top: 5px;">Join our elite newsletter for tech insights.</p>
            <input type="email" class="sub-input" placeholder="Enter your email address">
            <button class="main-cta" style="border: none; cursor: pointer; padding: 15px;">Subscribe Now</button>
        </div>

        <a href="https://wa.me/923332637235" class="main-cta" data-aos="fade-up">
            <i class="fab fa-whatsapp"></i> CONNECT WITH NAZIM
        </a>

        <section class="footer-hq" data-aos="fade-up">
            <div style="border-left: 3px solid var(--primary); padding-left: 20px;">
                <h3 style="font-size: 1.2rem; font-weight: 900;">CORPORATE HQ</h3>
                <p style="font-size: 0.9rem; opacity: 0.7; line-height: 2; margin-top: 15px;">
                    Karachi, Pakistan | Web-Hub Global Solutions<br>
                    Suite 262, Online Excellence Towers<br>
                    Toll Free: <a href="tel:+923332637235" style="color: var(--primary); text-decoration: none;">+92 333 2637235</a>
                </p>
            </div>

            <div style="display: flex; gap: 10px; margin: 30px 0;">
                <a href="#" class="social-link" style="color: white; font-size: 1.5rem;"><i class="fab fa-facebook"></i></a>
                <a href="https://wa.me/923332637235" class="social-link" style="color: white; font-size: 1.5rem;"><i class="fab fa-whatsapp"></i></a>
                <a href="#" class="social-link" style="color: white; font-size: 1.5rem;"><i class="fab fa-linkedin"></i></a>
            </div>

            <div style="text-align: center; border-top: 1px solid var(--border); padding-top: 30px;">
                <h2 style="font-weight: 900; font-size: 2.5rem; letter-spacing: -2px;">Web-Hub</h2>
                <div style="display: flex; justify-content: center; gap: 15px; font-size: 0.75rem; margin-top: 10px; opacity: 0.6;">
                    <span onclick="alert('Privacy Policy: We never share data.')" style="cursor: pointer;">Privacy</span>
                    <span onclick="alert('Terms: 50% advance required.')" style="cursor: pointer;">Terms</span>
                    <span onclick="alert('Security: SSL Encrypted.')" style="cursor: pointer;">Security</span>
                </div>
                <p style="margin-top: 15px; font-size: 0.7rem; opacity: 0.4;">© 2026 WEB-HUB INC. BY MUHAMMAD NAZIM</p>
            </div>
        </section>

        <footer>BEYOND THE LIMITS • 2026</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // 📝 Typewriter Effect
        const words = ["Websites", "Business Apps", "AI Systems", "Brands"];
        let i = 0, j = 0, current = "", isDeleting = false;
        function type() {
            const speed = isDeleting ? 100 : 200;
            if (!isDeleting && j <= words[i].length) {
                current = words[i].substring(0, j++);
            } else if (isDeleting && j >= 0) {
                current = words[i].substring(0, j--);
            }
            document.getElementById("typewriter").textContent = current;
            if (j === words[i].length + 1) isDeleting = true;
            if (j === -1) { isDeleting = false; i = (i + 1) % words.length; }
            setTimeout(type, speed);
        }
        type();

        // 🕒 Live Time & Scroll
        function updateUI() {
            document.getElementById('live-time').innerText = new Date().toLocaleTimeString();
            const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("progress-bar").style.width = (winScroll / height) * 100 + "%";
        }
        setInterval(updateUI, 1000);

        // 🔔 Smart Notifications
        const alerts = ["New Quote Generated 📄", "Nazim is Online 🟢", "Secure Payment Gateway Active 🛡️", "Client from USA joined 🇺🇸"];
        setInterval(() => {
            const box = document.getElementById('notif-box');
            document.getElementById('notif-text').innerText = alerts[Math.floor(Math.random()*alerts.length)];
            box.style.right = "20px";
            setTimeout(() => { box.style.right = "-300px"; }, 4000);
        }, 12000);

        // 👨‍👩‍👧‍👦 Visitor Counter (Fake Real-time)
        setInterval(() => {
            let count = parseInt(document.getElementById('visitor-count').innerText);
            document.getElementById('visitor-count').innerText = count + (Math.random() > 0.5 ? 1 : -1);
        }, 5000);

        // 📂 Accordion Logic
        function toggleFaq(el) {
            const body = el.nextElementSibling;
            body.style.maxHeight = body.style.maxHeight ? null : body.scrollHeight + "px";
            body.style.opacity = body.style.opacity == "1" ? "0" : "1";
        }
    </script>
</body>
</html>
