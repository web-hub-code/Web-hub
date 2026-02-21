<html lang="da">
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

        /* Scroll Progress Bar */
        #scroll-path { position: fixed; top: 0; left: 0; height: 4px; background: linear-gradient(to right, var(--primary), var(--success)); z-index: 20000; width: 0%; transition: 0.2s; }

        /* Baggrundseffekter */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.1); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 0%, #000 100%); z-index: -1; }

        /* Flydende Notifikationer */
        .toast { position: fixed; bottom: 30px; left: -400px; width: 300px; background: var(--glass); backdrop-filter: blur(20px); border: 1px solid var(--primary); padding: 15px; border-radius: 20px; z-index: 10005; transition: 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275); display: flex; align-items: center; gap: 12px; box-shadow: 0 10px 30px rgba(0,0,0,0.5); }

        /* Glas Navigation */
        nav { position: fixed; top: 0; width: 100%; padding: 20px; display: flex; justify-content: space-between; align-items: center; z-index: 10000; background: rgba(0,0,0,0.4); backdrop-filter: blur(15px); border-bottom: 1px solid var(--border); }
        .nav-logo { font-weight: 900; font-size: 1.4rem; background: linear-gradient(45deg, var(--primary), var(--success)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 100px 18px 50px; }

        /* Hero Card med Smart Greeting */
        .hero-card { background: var(--glass); border: 1px solid var(--border); border-radius: 40px; padding: 40px 30px; text-align: center; margin-bottom: 30px; }
        .status-tag { display: inline-flex; align-items: center; gap: 8px; background: rgba(0,255,136,0.1); color: var(--success); padding: 6px 16px; border-radius: 50px; font-size: 0.7rem; font-weight: 800; margin-bottom: 20px; text-transform: uppercase; }
        .pulse { width: 8px; height: 8px; background: var(--success); border-radius: 50%; animation: pulse-green 1.5s infinite; }

        /* Service Cards */
        .service-card { background: var(--glass); border: 1px solid var(--border); border-radius: 30px; padding: 25px; margin-bottom: 20px; transition: 0.4s; cursor: pointer; position: relative; overflow: hidden; }
        .service-card:hover { border-color: var(--primary); transform: translateY(-5px); background: rgba(0, 242, 254, 0.05); }
        
        /* FAQ System */
        .faq-box { background: rgba(255,255,255,0.02); border-radius: 20px; margin-bottom: 12px; border: 1px solid var(--border); }
        .faq-trigger { padding: 18px; cursor: pointer; display: flex; justify-content: space-between; font-weight: 600; font-size: 0.9rem; }
        .faq-content { padding: 0 18px; max-height: 0; overflow: hidden; transition: 0.3s; opacity: 0; font-size: 0.85rem; color: #aaa; }

        /* Premium Knapper */
        .btn-infinity { display: flex; align-items: center; justify-content: center; gap: 12px; width: 100%; padding: 22px; background: linear-gradient(45deg, var(--primary), var(--secondary)); border-radius: 25px; color: #000; font-weight: 900; text-decoration: none; text-transform: uppercase; box-shadow: 0 15px 40px rgba(0, 242, 254, 0.3); transition: 0.4s; margin-top: 20px; }
        .btn-infinity:hover { transform: scale(1.02); box-shadow: 0 20px 50px rgba(0, 242, 254, 0.5); }

        /* Corporate Footer */
        .footer-elite { background: #000; border: 1px solid var(--border); border-radius: 45px; padding: 45px 30px; margin-top: 60px; }
        
        @keyframes pulse-green { 0% { box-shadow: 0 0 0 0 rgba(0, 255, 136, 0.7); } 70% { box-shadow: 0 0 0 10px rgba(0, 255, 136, 0); } 100% { box-shadow: 0 0 0 0 rgba(0, 255, 136, 0); } }

        footer { text-align: center; padding: 60px; opacity: 0.2; font-size: 0.7rem; letter-spacing: 6px; }
    </style>
</head>
<body>

    <div id="scroll-path"></div>

    <nav>
        <div class="nav-logo">WEB-HUB</div>
        <div id="live-clock" style="font-size: 0.75rem; font-weight: 800; color: var(--primary);">00:00:00</div>
    </nav>

    <div id="toast-notif" class="toast">
        <i class="fas fa-check-circle" style="color: var(--success); font-size: 1.5rem;"></i>
        <div>
            <div style="font-weight: 900; font-size: 0.8rem;">NY BESKED</div>
            <div id="toast-msg" style="font-size: 0.75rem; opacity: 0.8;">Nazim er nu online</div>
        </div>
    </div>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        
        <section class="hero-card" data-aos="zoom-in">
            <div class="status-tag"><div class="pulse"></div> <span id="user-count">42</span> Aktive Besøgende</div>
            <h3 id="greeting" style="color: var(--primary); font-weight: 600; margin-bottom: 10px;">Goddag</h3>
            <h1 style="font-size: 4rem; font-weight: 900; letter-spacing: -3px; line-height: 1;">WEB-HUB</h1>
            <p style="margin-top: 20px; font-size: 1rem; opacity: 0.7; line-height: 1.8;">
                Vi forvandler komplekse idéer til intelligente digitale økosystemer. Oplev fremtidens webudvikling med Muhammad Nazim.
            </p>
        </section>

        <div data-aos="fade-up">
            <h2 style="margin-bottom: 25px; font-weight: 900; letter-spacing: 1px;">EKSKLUSIVE LØSNINGER</h2>
            
            <div class="service-card" onclick="openInfo('Enterprise Apps', 'Vi bygger skalerbare SaaS-platforme med avancerede dashboard-funktioner og realtids-data.')">
                <i class="fas fa-rocket" style="color: var(--primary); font-size: 2rem; margin-bottom: 15px;"></i>
                <h3>Supreme Web Apps</h3>
                <p style="font-size: 0.85rem; opacity: 0.6;">Specialbyggede applikationer til store virksomheder.</p>
            </div>

            <div class="service-card" onclick="openInfo('AI Integration', 'Vi implementerer maskinlæring og smarte chatbots, der automatiserer din kundeservice 24/7.')">
                <i class="fas fa-brain" style="color: var(--success); font-size: 2rem; margin-bottom: 15px;"></i>
                <h3>AI & Automatisering</h3>
                <p style="font-size: 0.85rem; opacity: 0.6;">Gør din forretning klogere med kunstig intelligens.</p>
            </div>
        </div>

        <div style="margin: 50px 0;" data-aos="fade-up">
            <h2 style="margin-bottom: 25px; font-weight: 900;">OFTE STILLEDE SPØRGSMÅL</h2>
            <div class="faq-box">
                <div class="faq-trigger" onclick="toggleFaq(this)">Hvor hurtigt leverer I? <i class="fas fa-plus"></i></div>
                <div class="faq-content">Små projekter tager 3-5 dage, mens store enterprise-løsninger tager 2-4 uger.</div>
            </div>
            <div class="faq-box">
                <div class="faq-trigger" onclick="toggleFaq(this)">Er support inkluderet? <i class="fas fa-plus"></i></div>
                <div class="faq-content">Ja, vi tilbyder 30 dages gratis teknisk support efter hver lancering.</div>
            </div>
        </div>

        <a href="https://wa.me/923332637235" class="btn-infinity" data-aos="flip-up">
            <i class="fab fa-whatsapp"></i> START DIT PROJEKT NU
        </a>

        <section class="footer-elite" data-aos="fade-up">
            <div style="border-left: 4px solid var(--primary); padding-left: 20px;">
                <h3 style="font-weight: 900; letter-spacing: 2px;">HOVEDKONTOR</h3>
                <p style="opacity: 0.7; font-size: 0.95rem; margin-top: 15px; line-height: 2;">
                    Web-Hub Global | Suite 262<br>
                    Karachi, Pakistan<br>
                    Tlf: +92 333 2637235<br>
                    Email: webhub262@gmail.com
                </p>
            </div>

            <div style="display: flex; gap: 15px; margin: 40px 0;">
                <a href="https://wa.me/923332637235" target="_blank" style="color: white; font-size: 1.8rem;"><i class="fab fa-whatsapp"></i></a>
                <a href="#" style="color: white; font-size: 1.8rem;"><i class="fab fa-facebook"></i></a>
                <a href="#" style="color: white; font-size: 1.8rem;"><i class="fab fa-linkedin"></i></a>
            </div>

            <div style="text-align: center; border-top: 1px solid var(--border); padding-top: 40px;">
                <h2 style="font-weight: 900; font-size: 3rem; letter-spacing: -3px;">Web-Hub</h2>
                <p style="font-size: 0.7rem; opacity: 0.4; letter-spacing: 2px; margin-top: 10px;">
                    © 2026 WEB-HUB INC. | DESIGNED BY MUHAMMAD NAZIM
                </p>
                <div style="margin-top: 20px; font-size: 0.8rem; color: var(--primary);">
                    <span style="cursor:pointer" onclick="alert('Privatlivspolitik: Vi beskytter dine data.')">Privacy</span> | 
                    <span style="cursor:pointer" onclick="alert('Vilkår: 50% forudbetaling påkrævet.')">Terms</span>
                </div>
            </div>
        </section>

        <footer>BEYOND THE LIMITS • 2026</footer>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // 🕒 Realtids Ur & Scroll Progress
        window.onscroll = function() {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            document.getElementById("scroll-path").style.width = (winScroll / height) * 100 + "%";
        };

        function updateClock() {
            const now = new Date();
            document.getElementById('live-clock').innerText = now.toLocaleTimeString();
            
            let hr = now.getHours();
            let greet = hr < 12 ? "Godmorgen ☀️" : hr < 18 ? "Goddag 🌤️" : "Godaften 🌙";
            document.getElementById('greeting').innerText = greet;
        }
        setInterval(updateClock, 1000);
        updateClock();

        // 🔔 Smart Toast Notifikationer
        const messages = [
            "Nyt projekt startet i Dubai! 🇦🇪",
            "5 stjernet anmeldelse modtaget! ⭐",
            "Nazim er ledig til konsultation! 📞",
            "Sikkerheds-update fuldført! 🛡️"
        ];
        
        function showToast() {
            const toast = document.getElementById('toast-notif');
            document.getElementById('toast-msg').innerText = messages[Math.floor(Math.random()*messages.length)];
            toast.style.left = "20px";
            setTimeout(() => { toast.style.left = "-400px"; }, 5000);
        }
        setTimeout(showToast, 3000);
        setInterval(showToast, 15000);

        // 📂 FAQ & Info System
        function toggleFaq(el) {
            const content = el.nextElementSibling;
            content.style.maxHeight = content.style.maxHeight ? null : content.scrollHeight + "px";
            content.style.opacity = content.style.opacity == "1" ? "0" : "1";
            el.querySelector('i').classList.toggle('fa-minus');
        }

        function openInfo(t, m) {
            alert(t + ":\n" + m);
        }

        // 👥 Live Visitor Counter
        setInterval(() => {
            let count = parseInt(document.getElementById('user-count').innerText);
            document.getElementById('user-count').innerText = count + (Math.random() > 0.5 ? 1 : -1);
        }, 4000);
    </script>
</body>
</html>
