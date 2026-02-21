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

        /* Tech Background */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 10%, #000 90%); z-index: -1; }

        /* Hero Header */
        .cover-box { width: 100%; height: 280px; position: relative; overflow: hidden; border-bottom: 3px solid var(--primary); }
        .cover-img { width: 100%; height: 100%; object-fit: cover; filter: brightness(0.5); }
        .container { width: 100%; max-width: 580px; margin: -80px auto 0; padding: 0 15px 50px; position: relative; z-index: 10; }

        /* Profile Hub */
        .p-wrap { text-align: center; margin-bottom: 25px; }
        .p-img { width: 150px; height: 150px; border-radius: 50%; border: 4px solid var(--primary); box-shadow: 0 0 30px rgba(0, 242, 254, 0.4); object-fit: cover; background: #000; }
        .badge { display: inline-block; padding: 5px 15px; background: rgba(0, 255, 136, 0.1); border: 1px solid #00ff88; color: #00ff88; border-radius: 50px; font-size: 0.7rem; margin-top: 12px; font-weight: 800; }

        /* Card Master */
        .card { background: var(--glass); backdrop-filter: blur(40px); border: 1px solid var(--border); border-radius: 35px; padding: 30px; margin-bottom: 25px; transition: 0.4s; }
        .card:hover { border-color: var(--primary); }
        .logo-main { font-size: 3.2rem; font-weight: 900; background: linear-gradient(45deg, var(--primary), var(--secondary)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-align: center; letter-spacing: -1px; }

        /* Dynamic Quote Button */
        .quote-btn { display: flex; align-items: center; justify-content: center; gap: 10px; width: 100%; padding: 18px; background: linear-gradient(45deg, #25d366, #128c7e); border-radius: 20px; color: white; font-weight: 800; text-decoration: none; text-transform: uppercase; margin-top: 10px; transition: 0.3s; }
        .quote-btn:hover { transform: translateY(-3px); box-shadow: 0 10px 25px rgba(37, 211, 102, 0.3); }

        /* Corporate Footer (HighLevel Based) */
        .footer-elite { text-align: left; padding: 40px 25px; background: rgba(0,0,0,0.8); border-radius: 40px; border: 1px solid var(--border); }
        .hq-title { color: white; font-weight: 800; font-size: 1.2rem; margin-bottom: 15px; letter-spacing: 1px; }
        .hq-info { font-size: 0.9rem; opacity: 0.7; line-height: 1.8; margin-bottom: 25px; padding-left: 15px; border-left: 2px solid var(--primary); }
        
        .social-grid { display: flex; gap: 12px; margin-bottom: 30px; }
        .social-item { width: 48px; height: 48px; background: var(--glass); border: 1px solid var(--border); display: flex; align-items: center; justify-content: center; border-radius: 50%; color: white; text-decoration: none; font-size: 1.2rem; transition: 0.3s; }
        .social-item:hover { background: var(--primary); color: #000; transform: scale(1.1); }

        /* Interaction Elements */
        .legal-links { display: flex; justify-content: center; gap: 15px; font-size: 0.8rem; margin-top: 20px; }
        .legal-links span { color: var(--primary); cursor: pointer; text-decoration: underline; }

        .modal { display: none; position: fixed; z-index: 999; left: 0; top: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.9); backdrop-filter: blur(10px); }
        .modal-content { background: #111; margin: 20% auto; padding: 30px; border: 1px solid var(--primary); width: 85%; max-width: 450px; border-radius: 30px; position: relative; text-align: center; }
        .close { position: absolute; top: 15px; right: 20px; font-size: 24px; color: var(--primary); cursor: pointer; }

        footer { text-align: center; padding: 30px; opacity: 0.2; font-size: 0.7rem; letter-spacing: 4px; }
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
            <br><div class="badge">Verified Agency Owner</div>
        </div>

        <section class="card" data-aos="fade-up">
            <h1 class="logo-main">Web-Hub</h1>
            <p style="text-align: center; opacity: 0.7; font-size: 0.9rem; line-height: 1.6;">
                Expert digital solutions tailored for your business. We specialize in high-performance web apps and creative branding.
            </p>
            <div style="margin-top: 25px;">
                <a href="https://wa.me/923332637235?text=Hi%20Nazim!%20I%20want%20to%20get%20a%20price%20quote%20for%20my%20project." class="quote-btn">
                    <i class="fab fa-whatsapp"></i> Get A Custom Quote
                </a>
            </div>
        </section>

        <section class="footer-elite card" data-aos="fade-up">
            <div class="hq-title">CORPORATE HQ</div>
            <div class="hq-info">
                Karachi, Pakistan | Web-Hub Center<br>
                Suite 262, Online Excellence<br>
                Toll Free: <a href="tel:+923332637235" style="color: var(--primary); text-decoration: none;">+92 333 2637235</a>
            </div>

            <div class="hq-title">SOCIAL CONNECT</div>
            <div class="social-grid">
                <a href="https://www.facebook.com/profile.php?id=100084218946114" target="_blank" class="social-item"><i class="fab fa-facebook-f"></i></a>
                <a href="https://wa.me/923332637235" target="_blank" class="social-item"><i class="fab fa-whatsapp"></i></a>
                <a href="mailto:webhub262@gmail.com" class="social-item"><i class="fas fa-envelope"></i></a>
                <a href="#" class="social-item"><i class="fab fa-instagram"></i></a>
                <a href="#" class="social-item"><i class="fab fa-linkedin-in"></i></a>
            </div>

            <div style="text-align: center; border-top: 1px solid var(--border); padding-top: 25px;">
                <h2 style="font-size: 2rem; font-weight: 900;">Web-Hub</h2>
                <div style="font-size: 0.7rem; opacity: 0.5; margin: 10px 0;">
                    © 2026 Web-Hub, Inc. • Muhammad Nazim Signature Project
                </div>
                <div class="legal-links">
                    <span onclick="showModal('Privacy Policy', 'Your data is encrypted and never shared with third parties.')">Privacy Policy</span>
                    <span onclick="showModal('Terms of Service', '50% upfront payment is required. Delivery time varies by project.')">Terms</span>
                    <span onclick="showModal('Security', 'Our sites use SSL encryption to ensure maximum protection.')">Security</span>
                </div>
            </div>
        </section>

        <footer>BEYOND THE LIMITS • 2026</footer>
    </div>

    <div id="infoModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="hideModal()">&times;</span>
            <h3 id="mTitle" style="color: var(--primary); margin-bottom: 15px;"></h3>
            <p id="mText" style="font-size: 0.9rem; opacity: 0.8; line-height: 1.5;"></p>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });
        function showModal(t, txt) {
            document.getElementById('mTitle').innerText = t;
            document.getElementById('mText').innerText = txt;
            document.getElementById('infoModal').style.display = "block";
        }
        function hideModal() { document.getElementById('infoModal').style.display = "none"; }
        window.onclick = function(e) { if(e.target.className == 'modal') hideModal(); }
    </script>
</body>
</html>
