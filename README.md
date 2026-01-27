<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Web‑Hub | Digital Services</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body{
    margin:0;
    font-family:Arial, sans-serif;
    background:#050914;
    color:#fff;
}
.hero{
    background:url('https://images.unsplash.com/photo-1521737604893-d14cc237f11d') center/cover no-repeat;
    height:90vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
}
.hero h1{
    font-size:48px;
    background:rgba(0,0,0,0.6);
    padding:20px;
    border-radius:20px;
}
.section{
    padding:60px 8%;
}
.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}
.card{
    background:#0b1020;
    border:1px solid #1e90ff;
    border-radius:20px;
    padding:20px;
    box-shadow:0 0 20px rgba(30,144,255,0.4);
}
.card img{
    width:100%;
    border-radius:15px;
}
.card h3{
    margin-top:15px;
}
</style>
</head>

<body>

<!-- HERO -->
<div class="hero">
    <h1>WEB‑HUB <br> Professional Digital Services</h1>
</div>

<!-- SERVICES -->
<div class="section">
<h2>Our Services</h2>

<div class="cards">

<div class="card">
<img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085">
<h3>Website Development</h3>
<p>Modern, fast & responsive websites.</p>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1552664730-d307ca884978">
<h3>SEO Optimization</h3>
<p>Rank your website on Google.</p>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1533750349088-cd871a92f312">
<h3>Digital Marketing</h3>
<p>Grow your business online.</p>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1517245386807-bb43f82c33c4">
<h3>UI / UX Design</h3>
<p>Attractive & user‑friendly designs.</p>
</div>

</div>
</div>

</body>
</html>
