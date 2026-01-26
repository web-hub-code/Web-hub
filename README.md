<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MrKhan PRO Services</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap');

        body {
            margin: 0;
            padding: 0;
            font-family: 'Orbitron', sans-serif;
            background: #000;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow: hidden;
        }

        .container {
            background: #0d0d0d;
            border-radius: 20px;
            padding: 40px 30px;
            text-align: center;
            max-width: 500px;
            box-shadow: 0 0 30px rgba(0,0,0,0.7);
            animation: glow 2s infinite alternate;
        }

        @keyframes glow {
            0% { box-shadow: 0 0 20px #00f, 0 0 30px #f00; }
            50% { box-shadow: 0 0 40px #00f, 0 0 60px #f00; }
            100% { box-shadow: 0 0 20px #00f, 0 0 30px #f00; }
        }

        h1 {
            font-size: 28px;
            color: #00ffff;
            text-shadow: 0 0 10px #00ffff, 0 0 20px #ff00ff;
            margin-bottom: 20px;
            animation: neon 1.5s infinite alternate;
        }

        @keyframes neon {
            0% { text-shadow: 0 0 5px #00ffff, 0 0 10px #ff00ff; }
            50% { text-shadow: 0 0 20px #00ffff, 0 0 30px #ff00ff; }
            100% { text-shadow: 0 0 5px #00ffff, 0 0 10px #ff00ff; }
        }

        p, .services li {
            color: #fff;
            text-shadow: 0 0 5px #00f, 0 0 10px #f00;
        }

        ul.services {
            list-style: none;
            padding: 0;
            margin: 20px 0;
        }

        ul.services li {
            margin: 15px 0;
            font-size: 16px;
        }

        .contact {
            margin-top: 25px;
        }

        .btn {
            display: block;
            width: 85%;
            margin: 12px auto;
            padding: 15px;
            border-radius: 12px;
            background: linear-gradient(45deg, #00f, #ff0044);
            color: #fff;
            font-weight: bold;
            font-size: 16px;
            text-decoration: none;
            text-shadow: 0 0 5px #fff;
            transition: all 0.3s ease;
            animation: pulse 2s infinite;
        }

        .btn:hover {
            transform: scale(1.05);
            background: linear-gradient(45deg, #ff0044, #00ffff);
            color: #000;
            text-shadow: 0 0 10px #fff;
        }

        @keyframes pulse {
            0% { box-shadow: 0 0 10px #00f, 0 0 20px #ff0044; }
            50% { box-shadow: 0 0 20px #00f, 0 0 40px #ff0044; }
            100% { box-shadow: 0 0 10px #00f, 0 0 20px #ff0044; }
        }

        .note {
            margin-top: 20px;
            font-size: 14px;
            color: #aaa;
            text-shadow: 0 0 5px #f00;
        }

        /* Animate background flicker effect */
        body::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle, rgba(255,0,68,0.1) 0%, transparent 80%);
            animation: flicker 3s infinite;
        }

        @keyframes flicker {
            0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% { opacity: 0.1; }
            20%, 22%, 24%, 55% { opacity: 0.3; }
        }

    </style>
</head>
<body>
    <div class="container">
        <h1>PRO Online Services by MrKhan 🚀</h1>
        <p>Apni website ya online service banwani hai? Check my services below:</p>
        <ul class="services">
            <li>💻 Professional Websites & Bio-Link Pages</li>
            <li>🔐 Firebase Login / Signup</li>
            <li>🎬 Viral Video Editing (Reels, Shorts, YouTube)</li>
            <li>🖼 Eye-Catching Thumbnails</li>
        </ul>
        <div class="contact">
            <a class="btn" href="https://www.instagram.com/mr_nazim073?igsh=MXd4d2hmcWNvNjVsdQ==" target="_blank">Instagram</a>
            <a class="btn" href="https://www.facebook.com/share/184Khe9iZu/" target="_blank">Facebook</a>
            <a class="btn" href="mailto:nazimkhan01123@gmail.com">Email</a>
        </div>
        <p class="note">Fast Delivery • Low Budget • Clean & Modern Work</p>
    </div>
</body>
</html>
