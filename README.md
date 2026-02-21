<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Web-Hub Official | Muhammad Nazim</title>
    
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
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.15); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 20%, #000 100%); z-index: -1; }

        .container { width: 100%; max-width: 600px; margin: 20px auto; padding: 0 15px 80px; position: relative; z-index: 10; }

        /* Elite Card Style */
        .card { background: var(--glass); backdrop-filter: blur(50px); border: 1px solid var(--border); border-radius: 40px; padding: 35px; margin-bottom: 30px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); }

        .logo-main { font-size: 3.5rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-align: center; letter-spacing: -2px; }

        /* Custom Quote Section (Pricing Ki Jagah) */
        .quote-box { text-align: center; padding: 20px; background: rgba(0, 242, 254, 0.05); border-radius: 30px; border: 1px dashed var(--primary); }
        .btn-wa { display: inline-block; width: 100%; padding: 18px; background: linear-gradient(45deg, #25d366, #128c7e); border-radius: 20px; color: white; font-weight: 800; text-decoration: none; text-transform: uppercase; margin-top: 20px; transition: 0.3s; border: none; cursor: pointer; }
        .btn-wa:hover { transform: scale(1.02); box-shadow: 0 0 20px rgba(37, 211, 102, 0.4); }

        /* Footer (HighLevel Screenshot Style) */
        .footer-elite { text-align: left; padding: 40px 25px; background: rgba(0,0,0,0.8); border-radius: 40px; border: 1px solid var(--border); }
        .hq-title { color: white; font-weight: 800; font-size: 1.3rem; margin-bottom: 20px; letter-spacing: 2px; border-bottom: 2px solid var(--primary); display: inline-block; padding-bottom: 5px; }
        .hq-info { font-size: 0.95rem; opacity: 0.7; line-height: 2; margin-bottom: 30px; }
        
        .social-row { display: flex; gap: 15px; margin-top: 20px; }
        .social-link { width: 50px; height: 50px; background: var(--glass); border: 1px solid var(--border); display: flex; align-items: center; justify-content: center; border-radius: 50%; color: white; text-decoration: none; font-size: 1.3rem; transition: 0.3s; }
        .social-link:hover { background: var(--primary); color: #000; transform: scale(1.1); }

        /* Modal / Privacy Policy Popup */
        .modal { display: none; position: fixed; z-index: 2000; left: 0; top: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.9); backdrop-filter: blur(10px); }
        .modal-content { background: #111; margin: 15% auto; padding: 30px; border: 1px solid var(--primary); width: 85%; max-width: 500px; border-radius: 30px; position: relative; }
        .close-btn { position: absolute; top: 15px; right: 20px; font-size: 25px; color: var(--primary); cursor: pointer; }
        .modal-text { font-size: 0.9rem; line-height: 1.6; opacity: 0.8; }

        .legal-links { display: flex; justify-content: center; gap: 20px; font-size: 0.8rem; margin-top: 20px; }
        .legal-links span { color: var(--primary); cursor: pointer; text-decoration: underline; }

        footer { text-align: center; padding: 40px; opacity: 0.2; font-size: 0.75rem; letter-spacing: 4px; }
    </style>
</head>
<body>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        <section class="card" data-aos="fade-up">
            <h1 class="logo-main">Web-Hub</h1>
            <p style="text-align: center; opacity: 0.6; letter-spacing: 8px; font-size: 0.7rem; margin-bottom: 25px;">GLOBAL DIGITAL AGENCY</p>
            
            <div class="quote-box">
                <h3 style="color: white; margin-bottom: 10px;">Get a Custom Quote</h3>
                <p style="font-size: 0.85rem; opacity: 0.7;">Prices depend on your project requirements. Share your idea with us!</p>
                <a href="https://wa.me/923332637235?text=Hi%20Nazim!%20I%20want%20to%20discuss%20a%20project%20and%20get%20a%20price%20quote." class="btn-wa">
                    <i class="fab fa-whatsapp"></i> Chat for Pricing
                </a>
            </div>
        </section>

        <section class="footer-elite card" data-aos="fade-up">
            <div class="hq-title">CORPORATE HQ</div>
            <div class="hq-info">
                Karachi, Pakistan | Web-Hub Center<br>
                Suite 262, Online Excellence Towers<br>
                Toll Free: <a href="tel:+923332637235" style="color: var(--primary); text-decoration: none;">+92 333 2637235</a><br>
                Support: webhub262@gmail.com
            </div>

            <div class="hq-title">GLOBAL CONNECT</div>
            <div class="social-row">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-link"><i class="fab fa-facebook-f"></i></a>
                <a href="https://wa.me/923332637235" target="_blank" class="social-link"><i class="fab fa-whatsapp"></i></a>
                <a href="mailto:webhub262@gmail.com" class="social-link"><i class="fas fa-envelope"></i></a>
                <a href="#" class="social-link"><i class="fab fa-linkedin-in"></i></a>
                <a href="#" class="social-link"><i class="fab fa-instagram"></i></a>
            </div>

            <div style="text-align: center; margin-top: 40px; border-top: 1px solid var(--border); padding-top: 30px;">
                <h2 style="font-weight: 900; letter-spacing: -1px; font-size: 2.2rem;">Web-Hub</h2>
                <div style="font-size: 0.75rem; opacity: 0.5; margin: 15px 0;">
                    © 2026 Web-Hub, Inc. • A Muhammad Nazim Signature Project
                </div>
                <div class="legal-links">
                    <span onclick="openModal('privacy')">Privacy Policy</span>
                    <span onclick="openModal('terms')">Terms</span>
                    <span onclick="openModal('security')">Security</span>
                </div>
            </div>
        </section>

        <footer>BEYOND THE LIMITS • 2026</footer>
    </div>

    <div id="legalModal" class="modal">
        <div class="modal-content">
            <span class="close-btn" onclick="closeModal()">&times;</span>
            <h3 id="modalTitle" style="color: var(--primary); margin-bottom: 15px;"></h3>
            <div id="modalBody" class="modal-text"></div>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        function openModal(type) {
            const modal = document.getElementById('legalModal');
            const title = document.getElementById('modalTitle');
            const body = document.getElementById('modalBody');
            
            modal.style.display = "block";
            
            if(type === 'privacy') {
                title.innerText = "Privacy Policy";
                body.innerHTML = "Web-Hub respects your privacy. We never share your project data or personal contact info with third parties. Your information is encrypted and used only for project communication.";
            } else if(type === 'terms') {
                title.innerText = "Terms of Service";
                body.innerHTML = "All projects require a 50% advance. Delivery time depends on project complexity. Web-Hub provides 1 month free support after project completion.";
            } else if(type === 'security') {
                title.innerText = "Security";
                body.innerHTML = "Our servers are protected with SSL encryption. We ensure that every website we build is safe from cyber attacks and data breaches.";
            }
        }

        function closeModal() {
            document.getElementById('legalModal').style.display = "none";
        }

        window.onclick = function(event) {
            if (event.target == document.getElementById('legalModal')) {
                closeModal();
            }
        }
    </script>
</body>
</html>
