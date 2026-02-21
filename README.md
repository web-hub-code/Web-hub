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
            --primary: #00f2fe; --secondary: #4facfe; --success: #00ff88;
            --bg: #010204; --glass: rgba(255, 255, 255, 0.03); --border: rgba(0, 242, 254, 0.15);
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Outfit', sans-serif; cursor: none; }
        body { background-color: var(--bg); color: white; overflow-x: hidden; scroll-behavior: smooth; }

        /* Next-Gen Cursor */
        #cursor { width: 10px; height: 10px; background: var(--primary); border-radius: 50%; position: fixed; pointer-events: none; z-index: 99999; mix-blend-mode: difference; }
        #cursor-blur { width: 300px; height: 300px; background: radial-gradient(circle, rgba(0, 242, 254, 0.08) 0%, transparent 75%); position: fixed; pointer-events: none; z-index: 99998; border-radius: 50%; transform: translate(-50%, -50%); }

        /* Video Background */
        #bg-video { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; object-fit: cover; filter: brightness(0.12); }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle, transparent 20%, #000 100%); z-index: -1; }

        .container { width: 100%; max-width: 500px; margin: 0 auto; padding: 80px 20px; }

        /* Premium Hub Card (From your Screenshot) */
        .hub-card { background: var(--glass); border: 1.5px solid var(--border); border-radius: 45px; padding: 50px 25px; text-align: center; margin-bottom: 40px; backdrop-filter: blur(20px); box-shadow: 0 30px 60px rgba(0,0,0,0.5); }
        .hub-title { font-size: 3.2rem; font-weight: 900; color: var(--primary); letter-spacing: -2px; margin-bottom: 15px; }
        .hub-desc { color: #aaa; line-height: 1.6; font-size: 0.95rem; margin-bottom: 30px; }
        
        .quote-btn { display: flex; align-items: center; justify-content: center; gap: 12px; width: 100%; padding: 22px; background: linear-gradient(135deg, #00ff88 0%, #00d2ff 100%); border-radius: 25px; color: white; font-weight: 900; text-decoration: none; font-size: 1rem; text-transform: uppercase; box-shadow: 0 10px 25px rgba(0, 255, 136, 0.2); transition: 0.3s; }
        .quote-btn:active { transform: scale(0.96); }

        /* Corporate List Style */
        .corp-section { margin-top: 40px; padding: 20px 0; }
        .corp-header { font-size: 1.3rem; font-weight: 800; color: #fff; margin-bottom: 25px; letter-spacing: 1px; }
        .corp-link { display: block; color: #888; text-decoration: none; padding: 12px 0; font-size: 0.95rem; border-bottom: 1px solid rgba(255,255,255,0.05); transition: 0.3s; }
        .corp-link:hover { color: var(--primary); padding-left: 8px; }

        /* HQ Info Block */
        .hq-block { border-left: 3px solid var(--primary); padding-left: 20px; margin: 25px 0 40px; }
        .hq-block p { font-size: 0.9rem; color: #999; margin-bottom: 8px; line-height: 1.5; }

        /* Social Circles */
        .social-flex { display: flex; gap: 12px; margin-top: 20px; flex-wrap: wrap; }
        .social-item { width: 50px; height: 50px; background: #0c0c0c; border: 1px solid #222; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: #fff; text-decoration: none; font-size: 1.2rem; transition: 0.4s; }
        .social-item:hover { border-color: var(--primary); color: var(--primary); transform: translateY(-5px); }

        /* Get Started Form */
        .start-box { background: #080808; border: 1px solid #1a1a1a; border-radius: 20px; display: flex; overflow: hidden; margin-top: 15px; }
        .start-box input { background: transparent; border: none; padding: 18px; color: #fff; flex: 1; outline: none; font-size: 0.9rem; }
        .start-box button { background: #5f27cd; border: none; padding: 0 25px; color: #fff; font-weight: 700; cursor: none; }

        /* Success Modal */
        .modal { display: none; position: fixed; top:0; left:0; width:100%; height:100%; background:rgba(0,0,0,0.95); z-index: 100000; backdrop-filter: blur(15px); }
        .modal-inner { position: absolute; top:50%; left:50%; transform:translate(-50%, -50%); width: 90%; max-width: 400px; background: #0f0f0f; border: 1px solid var(--primary); padding: 40px 25px; border-radius: 35px; text-align: center; }

        footer { margin-top: 60px; padding: 40px 0; border-top: 1px solid #111; display: flex; justify-content: space-between; align-items: center; font-size: 0.75rem; color: #444; }
        .up-btn { width: 40px; height: 40px; background: #5f27cd; border-radius: 50%; display: flex; align-items: center; justify-content: center; color: #fff; }

        @keyframes pulse { 0% { transform: scale(1); opacity: 1; } 50% { transform: scale(1.4); opacity: 0; } 100% { transform: scale(1); opacity: 1; } }
    </style>
</head>
<body>

    <div id="cursor"></div>
    <div id="cursor-blur"></div>

    <video autoplay muted loop playsinline id="bg-video">
        <source src="https://assets.mixkit.co/videos/preview/mixkit-abstract-technology-connection-lines-render-animation-2807-large.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>

    <div class="container">
        
        <section class="hub-card" data-aos="fade-down">
            <h1 class="hub-title">Web-Hub</h1>
            <p class="hub-desc">
                Expert digital solutions tailored for your business. We specialize in high-performance web apps and creative branding.
            </p>
            <a href="https://wa.me/923332637235" class="quote-btn">
                <i class="fab fa-whatsapp"></i> GET A CUSTOM QUOTE
            </a>
        </section>

        <div class="corp-section" data-aos="fade-up">
            <h2 class="corp-header">Company</h2>
            <a href="javascript:void(0)" onclick="openModal('Success Stories', 'Hamne 50+ international clients ke liye high-end websites aur AI bots banaye hain jo unki sales ko 200% tak increase kar chuke hain.')" class="corp-link">Success Stories</a>
            <a href="javascript:void(0)" onclick="openModal('Affiliate Program', 'Join our 30% commission program. Aap client layein, hum kaam karenge aur aapko har deal par 30% profit milega.')" class="corp-link">30% Affiliate Program</a>
            <a href="javascript:void(0)" onclick="openModal('Pricing Calculator', 'Pricing fix nahi hy. Ye depend karta hy ke aapko landing page chahiye ya full e-commerce system. WhatsApp par rate list mil jayegi.')" class="corp-link">Pricing Calculator</a>
            <a href="#" class="corp-link">Our Network</a>
            <a href="#" class="corp-link">Privacy Policy</a>
            <a href="#" class="corp-link">Terms of Service</a>
        </div>

        <div class="corp-section" data-aos="fade-up">
            <h2 class="corp-header">Corporate HQ</h2>
            <div class="hq-block">
                <p>Karachi, Pakistan | Web-Hub Center</p>
                <p>Suite 262, Online Excellence</p>
                <p style="color: var(--primary); font-weight: 800; font-size: 1rem;">Direct: +92 333 2637235</p>
            </div>

            <h2 class="corp-header">Social Connect</h2>
            <div class="social-flex">
                <a href="https://facebook.com/share/12E6tH73q6/" class="social-item"><i class="fab fa-facebook-f"></i></a>
                <a href="https://wa.me/923332637235" class="social-item"><i class="fab fa-whatsapp"></i></a>
                <a href="mailto:info@webhub.com" class="social-item"><i class="far fa-envelope"></i></a>
                <a href="https://www.instagram.com/itz_nazim_03/" class="social-item"><i class="fab fa-instagram"></i></a>
                <a href="https://www.linkedin.com/in/muhammad-nazim-0100772bb" class="social-item"><i class="fab fa-linkedin-in"></i></a>
            </div>
        </div>

        <div class="corp-section" data-aos="fade-up">
            <h2 class="corp-header">Get Started</h2>
            <p style="font-size: 0.85rem; color: #666; margin-bottom: 5px;">Start Free 30 Day Trial</p>
            <div class="start-box">
                <input type="email" id="userEmail" placeholder="Enter your email address">
                <button type="button" onclick="alert('Subscription Successful! We will contact you soon.')">Submit</button>
            </div>
        </div>

        <footer>
            <span>© 2026 Web-Hub. All rights reserved.</span>
            <a href="#" class="up-btn"><i class="fas fa-chevron-up"></i></a>
        </footer>
    </div>

    <div id="bizModal" class="modal">
        <div class="modal-inner">
            <h3 id="modalTitle" style="color:var(--primary); margin-bottom:15px; font-size:1.6rem;"></h3>
            <p id="modalBody" style="font-size:0.95rem; color:#ccc; line-height:1.7; margin-bottom:25px;"></p>
            <button onclick="closeModal()" style="background:var(--primary); border:none; padding:12px 30px; border-radius:50px; color:#000; font-weight:900; cursor:none;">CLOSE</button>
        </div>
    </div>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({ duration: 1000, once: true });

        // Cursor Logic
        const cursor = document.getElementById('cursor');
        const blur = document.getElementById('cursor-blur');
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
            blur.style.left = e.clientX + 'px';
            blur.style.top = e.clientY + 'px';
        });

        // Modal Controls
        function openModal(title, body) {
            document.getElementById('modalTitle').innerText = title;
            document.getElementById('modalBody').innerText = body;
            document.getElementById('bizModal').style.display = 'block';
        }
        function closeModal() {
            document.getElementById('bizModal').style.display = 'none';
        }
    </script>
</body>
</html>
