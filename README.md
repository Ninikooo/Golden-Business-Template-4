<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>LuxGold — Premium Business Website</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    /* ========== CORE STYLES ========== */
    :root {
      --black: #0b0d12;
      --gold-dark: #7a5c20;
      --gold: #f2c451;
      --gold-light: #ffe29f;
      --yellow: #ffd36a;
      --surface: #14161d;
      --ink: #f8f8f8;
      --muted: #b3b3b3;
      --border: rgba(255,255,255,.15);
      --radius: 20px;
      --shadow: 0 20px 60px rgba(0,0,0,.5);
      --grad-gold: linear-gradient(135deg, var(--gold-dark), var(--gold), var(--gold-light));
    }
    *{box-sizing:border-box;margin:0;padding:0}
    body{font-family:'Poppins',sans-serif;background:var(--black);color:var(--ink);overflow-x:hidden}
    a{text-decoration:none;color:inherit}

    /* ========== NAVIGATION ========== */
    header {
      position:sticky;top:0;z-index:1000;
      display:flex;justify-content:space-between;align-items:center;
      padding:15px 30px;background:rgba(11,13,18,.9);
      backdrop-filter:blur(12px);border-bottom:1px solid var(--border);
    }
    header h1{font-size:24px;font-weight:700;background:var(--grad-gold);-webkit-background-clip:text;color:transparent}
    nav{display:flex;gap:20px}
    nav a{padding:8px 14px;border-radius:999px;transition:.3s}
    nav a:hover{background:var(--grad-gold);color:#111}
    .btn{padding:12px 22px;border-radius:30px;font-weight:600;border:none;cursor:pointer;box-shadow:var(--shadow)}
    .btn-primary{background:var(--grad-gold);color:#111}
    .btn-ghost{background:transparent;border:1px solid var(--gold);color:var(--gold)}

    /* ========== HERO ========== */
    .hero{
      display:grid;grid-template-columns:1fr 1fr;align-items:center;
      padding:100px 40px;background:radial-gradient(1200px 600px at 80% -20%,rgba(255,211,106,.15),transparent 70%);
    }
    .hero h2{font-size:clamp(36px,5vw,64px);font-weight:800;line-height:1.1}
    .hero h2 span{background:var(--grad-gold);-webkit-background-clip:text;color:transparent}
    .hero p{max-width:500px;color:var(--muted);margin:20px 0}
    .hero img{width:100%;max-width:400px;border-radius:50%;box-shadow:0 0 50px rgba(242,196,81,.4);animation:float 6s ease-in-out infinite}
    @keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-12px)}}

    /* ========== SECTIONS ========== */
    section{padding:80px 20px;max-width:1200px;margin:auto}
    h2.section-title{font-size:clamp(28px,4vw,40px);margin-bottom:10px}
    p.section-sub{color:var(--muted);margin-bottom:40px;max-width:700px}

    /* ========== CARDS ========== */
    .grid{display:grid;gap:20px}
    .grid-3{grid-template-columns:repeat(auto-fit,minmax(280px,1fr))}
    .card{
      background:rgba(255,255,255,.05);padding:24px;border-radius:var(--radius);
      border:1px solid var(--border);transition:.3s;position:relative;overflow:hidden
    }
    .card:hover{transform:translateY(-6px);box-shadow:var(--shadow)}
    .card h3{margin:10px 0;color:var(--gold)}
    .card p{color:var(--muted)}

    /* ========== FOOTER ========== */
    footer{background:#111;padding:40px 20px;text-align:center;color:var(--muted);font-size:14px}

    /* ========== REVEAL ANIMATION ========== */
    .fade{opacity:0;transform:translateY(30px);transition:all .7s ease}
    .fade.visible{opacity:1;transform:none}

    @media(max-width:768px){
      .hero{grid-template-columns:1fr;text-align:center}
      .hero img{margin:auto;margin-top:30px}
    }
  </style>
</head>
<body>

<header>
  <h1>LuxGold</h1>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#showcase">Showcase</a>
    <a href="#pricing">Pricing</a>
    <a href="#contact">Contact</a>
  </nav>
  <button class="btn btn-primary">Get a Quote</button>
</header>

<!-- HERO -->
<section class="hero" id="home">
  <div>
    <h2 class="fade">A <span>Luxurious</span> Website Template</h2>
    <p class="fade">Metallic gradients, glass surfaces, smooth animations and unique graphics — built for premium businesses.</p>
    <button class="btn btn-primary fade">Explore Now</button>
    <button class="btn btn-ghost fade">Learn More</button>
  </div>
  <img src="https://picsum.photos/400" alt="Luxury emblem" class="fade">
</section>

<!-- ABOUT -->
<section id="about">
  <h2 class="section-title fade">About Us</h2>
  <p class="section-sub fade">LuxGold is designed as a multifunctional template for boutiques, real estate, finance, beauty, and luxury brands.</p>
</section>

<!-- SERVICES -->
<section id="services">
  <h2 class="section-title fade">Our Services</h2>
  <div class="grid grid-3">
    <div class="card fade"><h3>Branding</h3><p>Identity, strategy and luxury design systems.</p></div>
    <div class="card fade"><h3>Web Design</h3><p>Responsive, animated, premium websites.</p></div>
    <div class="card fade"><h3>E-Commerce</h3><p>Elegant shopping experiences with trust.</p></div>
  </div>
</section>

<!-- SHOWCASE -->
<section id="showcase">
  <h2 class="section-title fade">Showcase</h2>
  <p class="section-sub fade">A gallery of luxurious projects.</p>
  <div class="grid grid-3">
    <div class="card fade"><h3>Project One</h3><p>Golden gradient UI.</p></div>
    <div class="card fade"><h3>Project Two</h3><p>Luxury e-commerce layout.</p></div>
    <div class="card fade"><h3>Project Three</h3><p>Premium business landing.</p></div>
  </div>
</section>

<!-- PRICING -->
<section id="pricing">
  <h2 class="section-title fade">Pricing</h2>
  <div class="grid grid-3">
    <div class="card fade"><h3>Basic</h3><p>$499</p></div>
    <div class="card fade"><h3>Premium</h3><p>$999</p></div>
    <div class="card fade"><h3>Enterprise</h3><p>$1999</p></div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <h2 class="section-title fade">Contact Us</h2>
  <form class="fade">
    <input type="text" placeholder="Your Name" required>
    <input type="email" placeholder="Your Email" required>
    <textarea placeholder="Message" rows="5"></textarea>
    <button class="btn btn-primary">Send</button>
  </form>
</section>

<footer>
  <p>© 2025 LuxGold. All rights reserved.</p>
</footer>

<script>
  // Fade-in scroll animation
  const observer=new IntersectionObserver(entries=>{
    entries.forEach(e=>{if(e.isIntersecting)e.target.classList.add('visible')});
  },{threshold:.2});
  document.querySelectorAll('.fade').forEach(el=>observer.observe(el));
</script>
</body>
</html>
