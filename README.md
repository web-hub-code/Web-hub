<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub Intelligence | Muhammad Nazim</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;900&display=swap" rel="stylesheet">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />

    <style>
        :root {
            --primary: #00f2fe; --secondary: #4facfe; --accent: #7000ff;
            --success: #00ff88; --bg: #010204; --glass: rgba(255, 255, 255, 0.03);
            --border: rgba(0, 242, 254, 0.25);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Background */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 0%, #000 100%); z-index: -1; }

        /* Notification Slider */
        #notification-box {
            position: fixed; top: 20px; right: -300px; width: 280px; 
            background: linear-gradient(135deg, var(--primary), var(--accent));
            color: #000; padding: 15px; border-radius: 15px; z-index: 10001;
            font-weight: 800; font-size: 0.85rem; box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            transition: 0.8s cubic-bezier(0.68, -0.55, 0.27, 1.55);
            display: flex; align-items: center; gap: 10px;
        }

        .container { width: 100%; max-width: 550px; margin: 0 auto; padding: 20px 18px 100px; }

        /* Smart Header */
        .smart-header { text-align: right; font-size: 0.7rem; opacity: 0.6; letter-spacing: 2px; margin-bottom: 10px; }

        /* Hero Card */
        .glass-card { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 40px; padding: 35px; margin-bottom: 25px; transition: 0.4s; position: relative; }
        
        .welcome-msg { font-size: 1.1rem; color: var(--success); font-weight: 600; margin-bottom: 5px; display: block; }
        .brand-logo { font-size: 3.5rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--success)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; letter-spacing: -2px; }

        /* Slider */
        .swiper { width: 100%; border-radius: 25px; margin: 20px 0; border: 1px solid var(--border); }
        .swiper-slide img { width: 100%; height: 220px; object-fit: cover; filter: brightness(0.7); }

        /* Buttons & Features */
        .feat-item { display: flex; align-items: center; gap: 15px; padding: 20px; background: rgba(255,255,255,0.02); border: 1px solid var(--border); border-radius: 20px; margin-bottom: 15px; cursor: pointer; transition: 0.3s; }
        .main-btn { display: flex; align-items: center; justify-content: center; gap: 12px; width: 100%; padding: 22px; background: linear-gradient(45deg, var(--primary), var(--secondary)); border-radius: 25px; color: #000; font-weight: 900; text-decoration: none; text-transform: uppercase; box-shadow: 0 10px 30px rgba(0, 242, 254, 0.3); transition: 0.4s; }

        /* Corporate Footer */
        .footer-hq { background: rgba(0,0,0,0.85); border: 1px solid var(--border); border-radius: 45px; padding: 40px 25px; margin-top: 40px; }
        .social-wrap { display: flex; gap: 10px; margin: 25px 0; justify-content: center; }
        .social-btn { width: 45px; height: 45px; background: var(--glass); border: 1px solid var(--border); border-radius: 50%; display: flex; align-items: center; justify-content: center; color: white; text-decoration: none; transition: 0.3s; }

        /* Modal */
        .modal { display: none; position: fixed; z-index: 10000; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.95); backdrop-filter: blur(15px); }
        .modal-card { background: #0a0a0a; margin: 20% auto; padding: 40px; border: 1px solid var(--primary); width: 90%; max-width: 400px; border-radius: 40px; text-align: center; position: relative; }

        footer { text-align: center; padding: 40px; opacity: 0.3; font-size: 0.65rem; letter-spacing: 4px; }
    </style>
</head>
<body>

    <div id="notification-box">
        <i class="fas fa-bell"></i>
        <span id="notif-text">New Client Inquiry Received!</span>
    </div>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        <div class="smart-header" id="digital-clock">00:00:00 AM</div>
        
        <section class="glass-card" data-aos="fade-down">
            <span class="welcome-msg" id="greeting">Loading...</span>
            <h1 class="brand-logo" data-aos="slide-right">Web-Hub</h1>
            <p style="font-size: 0.85rem; opacity: 0.7; line-height: 1.6; margin-top: 15px;">
                Welcome to Web-Hub. Muhammad Nazim's official agency for modern business scaling and digital transformation.
            </p>
        </section>

        <div class="swiper mySwiper" data-aos="zoom-in">
            <div class="swiper-wrapper">
                <div class="swiper-slide"><img src="FB_IMG_1769869953605.jpg" alt="Portfolio 1"></div>
                <div class="swiper-slide"><img src="Snapchat-2096615446.jpg" alt="Portfolio 2"></div>
                <div class="swiper-slide"><img src="FB_IMG_1769869953605.jpg" alt="Portfolio 3"></div>
            </div>
        </div>

        <div data-aos="fade-up">
            <div class="feat-item" onclick="openDetails('Smart Automation', 'Hum aapke business mein AI aur bots lagate hain jo kaam ko 10x fast kar dete hain.')">
                <i class="fas fa-robot"></i>
                <div>
                    <h4 style="color: var(--primary);">Smart Automation</h4>
                    <p style="font-size: 0.7rem; opacity: 0.5;">Work smart, grow fast.</p>
                </div>
            </div>

            <a href="https://wa.me/923332637235?text=Hello%20Nazim!%20I%20am%20coming%20from%20your%20Web-Hub%20Intelligence%20Portal." class="main-btn">
                <i class="fab fa-whatsapp"></i> Start Modern Project
            </a>
        </div>

        <section class="footer-hq" data-aos="fade-up">
            <div style="border-left: 3px solid var(--primary); padding-left: 15px;">
                <h3 style="font-size: 1rem; letter-spacing: 2px;">GLOBAL OPERATIONS</h3>
                <p style="font-size: 0.85rem; opacity: 0.6; margin-top: 10px;">
                    Web-Hub Center, Karachi, Pakistan<br>
                    Official Support: webhub262@gmail.com
                </p>
            </div>

            <div class="social-wrap">
                <a href="https://wa.me/923332637235" class="social-btn"><i class="fab fa-whatsapp"></i></a>
                <a href="#" class="social-btn"><i class="fab fa-facebook-f"></i></a>
                <a href="#" class="social-btn"><i class="fab fa-instagram"></i></a>
                <a href="#" class="social-btn"><i class="fab fa-linkedin-in"></i></a>
            </div>

            <div style="text-align: center; border-top: 1px solid rgba(255,255,255,0.1); padding-top: 25px;">
                <h2 style="font-weight: 900; font-size: 2.2rem; letter-spacing: -1px;">Web-Hub</h2>
                <div style="display: flex; justify-content: center; gap: 15px; font-size: 0.75rem; margin-top: 10px;">
                    <span style="color: var(--primary); cursor: pointer;" onclick="openDetails('Privacy Policy', 'Full data encryption guaranteed.')">Privacy</span>
                    <span style="color: var(--primary); cursor: pointer;" onclick="openDetails('Terms', 'Standard agency agreements apply.')">Terms</span>
                </div>
            </div>
        </section>

        <footer>BEYOND THE LIMITS • 2026</footer>
    </div>

    <div id="infoModal" class="modal">
        <div class="modal-card">
            <span style="position:absolute; top:15px; right:20px; font-size:25px; cursor:pointer; color:var(--primary);" onclick="closeDetails()">&times;</span>
            <h3 id="modalTitle" style="color: var(--primary); margin-bottom: 15px;"></h3>
            <p id="modalBody" style="font-size: 0.9rem; line-height: 1.6; opacity: 0.8;"></p>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        new Swiper(".mySwiper", { loop: true, autoplay: { delay: 3000 } });

        // 🕒 Digital Clock & Smart Greeting
        function updateClock() {
            const now = new Date();
            const hours = now.getHours();
            document.getElementById('digital-clock').innerText = now.toLocaleTimeString();

            let greet = "";
            if (hours < 12) greet = "Good Morning ☀️";
            else if (hours < 17) greet = "Good Afternoon 🌤️";
            else greet = "Good Evening 🌙";
            
            document.getElementById('greeting').innerText = greet + " | Welcome to Web-Hub";
        }
        setInterval(updateClock, 1000);
        updateClock();

        // 🔔 Slide-in Notifications
        const messages = [
            "Project 'Elite-Site' Completed! ✅",
            "New Client from Dubai Joined! 🌍",
            "Nazim is now Live for Consultations! 📞",
            "Web-Hub reached 150+ Projects! 🚀"
        ];
        
        function showNotification() {
            const box = document.getElementById('notification-box');
            const text = document.getElementById('notif-text');
            text.innerText = messages[Math.floor(Math.random() * messages.length)];
            
            box.style.right = "20px";
            setTimeout(() => { box.style.right = "-300px"; }, 4000);
        }
        setTimeout(() => { setInterval(showNotification, 10000); showNotification(); }, 3000);

        // Modal Functions
        function openDetails(t, b) {
            document.getElementById('modalTitle').innerText = t;
            document.getElementById('modalBody').innerText = b;
            document.getElementById('infoModal').style.display = "block";
        }
        function closeDetails() { document.getElementById('infoModal').style.display = "none"; }
    </script>
</body>
</html>
