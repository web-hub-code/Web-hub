<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub | Muhammad Nazim Official</title>
    
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

        /* Background Visuals */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 10%, #000 90%); z-index: -1; }

        /* Header Cover */
        .cover-box { width: 100%; height: 320px; position: relative; overflow: hidden; border-bottom: 3px solid var(--primary); }
        .cover-img { width: 100%; height: 100%; object-fit: cover; filter: brightness(0.5); }
        
        .container { width: 100%; max-width: 600px; margin: -100px auto 0; padding: 0 15px 50px; position: relative; z-index: 10; }

        /* Profile Identity */
        .p-wrap { text-align: center; margin-bottom: 30px; }
        .p-img { width: 160px; height: 160px; border-radius: 50%; border: 4px solid var(--primary); box-shadow: 0 0 40px rgba(0, 242, 254, 0.5); object-fit: cover; background: #000; }
        .badge { display: inline-block; padding: 6px 16px; background: rgba(0, 255, 136, 0.1); border: 1px solid #00ff88; color: #00ff88; border-radius: 50px; font-size: 0.7rem; margin-top: 15px; font-weight: 800; text-transform: uppercase; }

        /* Card Master Style */
        .card { background: var(--glass); backdrop-filter: blur(50px); border: 1px solid var(--border); border-radius: 40px; padding: 35px; margin-bottom: 30px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); transform: translateY(-5px); }

        .logo-main { font-size: 3.8rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--secondary)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-align: center; letter-spacing: -2px; }

        /* Detailed Services (Clickable) */
        .service-link { display: block; text-decoration: none; color: white; background: rgba(255,255,255,0.03); border: 1px solid var(--border); padding: 25px; border-radius: 30px; margin-bottom: 15px; transition: 0.3s; }
        .service-link:hover { border-color: var(--primary); background: rgba(0, 242, 254, 0.08); transform: translateX(10px); }
        .service-link h4 { color: var(--primary); font-size: 1.1rem; margin-bottom: 8px; font-weight: 800; display: flex; align-items: center; gap: 10px; }
        .service-link p { font-size: 0.85rem; opacity: 0.7; line-height: 1.6; }

        /* Custom Quote Section */
        .quote-btn { display: flex; align-items: center; justify-content: center; gap: 10px; width: 100%; padding: 20px; background: linear-gradient(45deg, #25d366, #128c7e); border-radius: 20px; color: white; font-weight: 800; text-decoration: none; text-transform: uppercase; font-size: 1rem; box-shadow: 0 10px 30px rgba(37, 211, 102, 0.2); transition: 0.3s; }
        .quote-btn:hover { transform: scale(1.02); box-shadow: 0 15px 40px rgba(37, 211, 102, 0.4); }

        /* Official Footer (HighLevel Style) */
        .footer-elite { text-align: left; padding: 45px 30px; background: rgba(0,0,0,0.85); border-radius: 45px; border: 1px solid var(--border); }
        .hq-title { color: white; font-weight: 800; font-size: 1.3rem; margin-bottom: 20px; letter-spacing: 2px; text-transform: uppercase; }
        .hq-info { font-size: 1rem; opacity: 0.7; line-height: 2; margin-bottom: 30px; border-left: 3px solid var(--primary); padding-left: 20px; }
        
        .social-grid { display: flex; gap: 15px; margin-bottom: 40px; }
        .social-item { width: 55px; height: 55px; background: var(--glass); border: 1px solid var(--border); display: flex; align-items: center; justify-content: center; border-radius: 50%; color: white; text-decoration: none; font-size: 1.4rem; transition: 0.3s; }
        .social-item:hover { background: var(--primary); color: #000; transform: translateY(-5px) rotate(360deg); }

        /* Legal & Modals */
        .legal-footer { text-align: center; border-top: 1px solid var(--border); padding-top: 40px; }
        .legal-links { display: flex; justify-content: center; gap: 20px; font-size: 0.85rem; margin-top: 20px; flex-wrap: wrap; }
        .legal-links span { color: var(--primary); cursor: pointer; font-weight: 600; text-decoration: underline; transition: 0.3s; }
        .legal-links span:hover { color: white; }

        .modal { display: none; position: fixed; z-index: 9999; left: 0; top: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.95); backdrop-filter: blur(15px); }
        .modal-card { background: #0a0a0a; margin: 15% auto; padding: 40px; border: 1px solid var(--primary); width: 85%; max-width: 500px; border-radius: 40px; position: relative; animation: slideIn 0.4s ease; }
        @keyframes slideIn { from { transform: translateY(50px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
        .close-modal { position: absolute; top: 20px; right: 25px; font-size: 30px; color: var(--primary); cursor: pointer; }

        footer { text-align: center; padding: 50px; opacity: 0.2; font-size: 0.75rem; letter-spacing: 6px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="cover-box">
        <img src="FB_IMG_1769869953605.jpg" class="cover-img" alt="Web-Hub Agency">
    </div>

    <div class="container">
        <div class="p-wrap" data-aos="zoom-in">
            <img src="Snapchat-2096615446.jpg" class="p-img" alt="Muhammad Nazim">
            <br>
            <div class="badge">● Top Rated Digital Agency</div>
        </div>

        <section class="card" data-aos="fade-up">
            <h1 class="logo-main">Web-Hub</h1>
            <p style="text-align: center; opacity: 0.6; letter-spacing: 6px; font-size: 0.7rem; margin-bottom: 25px;">FUTURE OF DIGITAL SOLUTIONS</p>
            <p style="text-align: center; line-height: 1.8; opacity: 0.8; font-size: 0.95rem;">
                Muhammad Nazim ki sarbarahi mein, Web-Hub aapke business ko aik globally recognized brand banata hai. Hum premium design aur advanced coding ke zariye aapka trust jeet-te hain.
            </p>
        </section>

        <div class="card" data-aos="fade-up">
            <h3 style="margin-bottom: 25px; font-weight: 800;"><i class="fas fa-layer-group" style="color: var(--primary);"></i> Our Core Expertise</h3>
            
            <a href="https://wa.me/923332637235?text=I%20want%20to%20discuss%20a%20Web%20Development%20project." class="service-link">
                <h4><i class="fas fa-code"></i> Elite Web Development</h4>
                <p>Custom websites jo fast hon, secure hon, aur har device par perfect dikhein.</p>
            </a>

            <a href="https://wa.me/923332637235?text=I%20want%20to%20discuss%20Graphic%20Designing%20work." class="service-link">
                <h4><i class="fas fa-wand-magic-sparkles"></i> Branding & UI/UX</h4>
                <p>Stunning visuals aur logos jo aapke brand ki identity ko international look dein.</p>
            </a>

            <div style="margin-top: 30px;">
                <a href="https://wa.me/923332637235?text=Hi%20Nazim!%20I%20need%20a%20custom%20price%20quote%20for%20my%20project." class="quote-btn">
                    <i class="fab fa-whatsapp"></i> Get a Custom Quote
                </a>
                <p style="text-align: center; font-size: 0.75rem; opacity: 0.5; margin-top: 10px;">*Prices are flexible based on project scope</p>
            </div>
        </div>

        <section class="footer-elite card" data-aos="fade-up">
            <div class="hq-title">CONTACT US</div>
            <div class="hq-info">
                <strong>Corporate HQ</strong><br>
                Karachi, Pakistan | Web-Hub Center<br>
                Suite 262, Online Digital Solutions<br>
                Toll Free: <a href="tel:+923332637235" style="color: var(--primary); text-decoration: none;">+92 333 2637235</a><br>
                Email: webhub262@gmail.com
            </div>

            <div class="hq-title">SOCIALS</div>
            <div class="social-grid">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-item"><i class="fab fa-facebook-f"></i></a>
                <a href="https://wa.me/923332637235" target="_blank" class="social-item"><i class="fab fa-whatsapp"></i></a>
                <a href="mailto:webhub262@gmail.com" class="social-item"><i class="fas fa-envelope"></i></a>
                <a href="#" class="social-item"><i class="fab fa-instagram"></i></a>
                <a href="#" class="social-item"><i class="fab fa-linkedin-in"></i></a>
            </div>

            <div class="legal-footer">
                <h2 style="font-weight: 900; font-size: 2.2rem; letter-spacing: -1px;">Web-Hub</h2>
                <div style="font-size: 0.75rem; opacity: 0.4; margin-top: 10px;">
                    © 2026 Web-Hub, Inc. | All Rights Reserved<br>
                    Official Portal of Muhammad Nazim
                </div>
                <div class="legal-links">
                    <span onclick="toggleModal('privacy')">Privacy Policy</span>
                    <span onclick="toggleModal('terms')">Terms of Service</span>
                    <span onclick="toggleModal('security')">Security</span>
                </div>
            </div>
        </section>

        <footer>BEYOND THE LIMITS • 2026</footer>
    </div>

    <div id="infoModal" class="modal">
        <div class="modal-card">
            <span class="close-modal" onclick="toggleModal()">&times;</span>
            <h3 id="modalTitle" style="color: var(--primary); margin-bottom: 20px; font-weight: 800;"></h3>
            <div id="modalContent" style="font-size: 0.95rem; line-height: 1.8; opacity: 0.8;"></div>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        function toggleModal(type) {
            const modal = document.getElementById('infoModal');
            const title = document.getElementById('modalTitle');
            const content = document.getElementById('modalContent');
            
            if(!type) {
                modal.style.display = "none";
                return;
            }

            modal.style.display = "block";
            
            if(type === 'privacy') {
                title.innerText = "Privacy Policy";
                content.innerText = "Hum aapka data kabhi kisi ke saath share nahi karte. Web-Hub aapki personal aur project information ko 256-bit encryption ke saath mehfooz rakhta hai.";
            } else if(type === 'terms') {
                title.innerText = "Terms of Service";
                content.innerText = "Har project ka 50% advance lazmi hai. Project completion ke baad 1 month tak free technical support di jati hai. Delivery time requirements ke mutabiq hota hai.";
            } else if(type === 'security') {
                title.innerText = "Security & Trust";
                content.innerText = "Humare banaye gaye codes malware-free aur secure hote hain. Hum premium SSL certificates aur cloud security ka istemal karte hain.";
            }
        }

        window.onclick = function(e) {
            if(e.target == document.getElementById('infoModal')) toggleModal();
        }
    </script>
</body>
</html>
