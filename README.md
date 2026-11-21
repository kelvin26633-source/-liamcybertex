# -liamcybertex
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Liamcybertex | Cyber Security, Cloud Setup &amp; IT Shop</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Sora:wght@500;700;800&family=DM+Sans:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#05080f; --surface:#0d1524; --ink:#eaf2ff; --muted:#9fb0cc; --line:#1c2c4a;
  --blue:#2f8cff; --blue-ink:#ffffff; --glow:rgba(47,140,255,.28);
  --head:"Sora","Trebuchet MS",system-ui,sans-serif;
  --body:"DM Sans","Segoe UI",system-ui,sans-serif;
  box-sizing:border-box; padding-top:env(safe-area-inset-top,0px); padding-bottom:env(safe-area-inset-bottom,0px);
  color-scheme:dark;
}
@media (prefers-color-scheme:light){
  :root:not([data-theme="dark"]){--bg:#eef4ff;--surface:#ffffff;--ink:#07101f;--muted:#44566f;--line:#c9d8f2;--blue:#0a5fd1;--glow:rgba(10,95,209,.18);color-scheme:light}
}
:root[data-theme="light"]{--bg:#eef4ff;--surface:#ffffff;--ink:#07101f;--muted:#44566f;--line:#c9d8f2;--blue:#0a5fd1;--glow:rgba(10,95,209,.18);color-scheme:light}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*,*::before,*::after{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font:400 1.05rem/1.6 var(--body);min-height:100vh}
a{color:inherit}
:focus-visible{outline:3px solid var(--blue);outline-offset:3px}
.wrap{max-width:1040px;margin:0 auto;padding:0 1.25rem}
header.nav{position:sticky;top:env(safe-area-inset-top,0px);background:var(--bg);border-bottom:1px solid var(--line);z-index:5}
.nav .wrap{display:flex;justify-content:space-between;align-items:center;gap:1rem;flex-wrap:wrap;padding-top:.7rem;padding-bottom:.7rem}
.brand{display:flex;align-items:center;gap:.6rem;text-decoration:none;font-family:var(--head);font-weight:800;font-size:1.2rem}
.brand svg{width:34px;height:34px}
.brand span{color:var(--blue)}
nav.links{display:flex;gap:.3rem;flex-wrap:wrap}
nav.links a{text-decoration:none;color:var(--muted);font-weight:500;padding:.4rem .8rem;border-radius:6px}
nav.links a:hover{color:var(--ink)}
nav.links a.on{background:var(--blue);color:var(--blue-ink)}
.page{display:none;padding-bottom:3rem}
.page.show{display:block}
.hero{padding:4.5rem 0 3rem;background:radial-gradient(60rem 22rem at 80% -10%,var(--glow),transparent)}
.tag{display:inline-block;border:1px solid var(--blue);color:var(--blue);border-radius:99px;padding:.25rem .9rem;font-size:.9rem;font-weight:600;margin-bottom:1rem}
h1{font-family:var(--head);font-weight:800;font-size:clamp(2.3rem,7vw,4.4rem);line-height:1.02;letter-spacing:-.03em;margin:0 0 1rem}
h1 em{font-style:normal;color:var(--blue)}
h2{font-family:var(--head);font-size:clamp(1.6rem,4vw,2.2rem);margin:0 0 1rem;letter-spacing:-.02em}
.lead{max-width:58ch;color:var(--muted);margin:0 0 1.6rem}
.btns{display:flex;gap:.8rem;flex-wrap:wrap}
.btn{display:inline-block;padding:.75rem 1.3rem;border-radius:6px;text-decoration:none;border:2px solid var(--blue);background:none;color:var(--blue);font:600 1rem var(--body)}
.btn.fill{background:var(--blue);color:var(--blue-ink)}
.btn:hover{filter:brightness(1.12)}
.pagehead{padding:3rem 0 1rem}
section.blk{padding:2.2rem 0;border-top:1px solid var(--line)}
.grid{display:grid;gap:1rem;grid-template-columns:repeat(auto-fit,minmax(240px,1fr))}
.card{background:var(--surface);border:1px solid var(--line);border-radius:10px;padding:1.4rem}
.card h3{font-family:var(--head);font-size:1.15rem;margin:0 0 .5rem}
.card p{margin:0 0 .8rem;color:var(--muted)}
.card ul{margin:0;padding-left:1.1rem;color:var(--muted)}
.card .btn{padding:.5rem 1rem;font-size:.95rem;margin-top:.4rem}
.ico{width:42px;height:42px;border-radius:8px;background:var(--glow);display:grid;place-items:center;font-size:1.3rem;margin-bottom:.8rem}
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:1rem;margin-top:2rem}
.stats div{border-left:3px solid var(--blue);padding-left:.8rem}
.stats b{display:block;font-family:var(--head);font-size:1.3rem}
.stats span{color:var(--muted);font-size:.95rem}
.steps{counter-reset:s;list-style:none;margin:0;padding:0;display:grid;gap:.8rem}
.steps li{counter-increment:s;background:var(--surface);border:1px solid var(--line);border-radius:10px;padding:1rem 1.2rem 1rem 3.4rem;position:relative}
.steps li::before{content:counter(s);position:absolute;left:1rem;top:.9rem;width:1.7rem;height:1.7rem;border-radius:50%;background:var(--blue);color:var(--blue-ink);display:grid;place-items:center;font-weight:700}
.contact{list-style:none;margin:0;padding:0;display:grid;gap:.8rem;grid-template-columns:repeat(auto-fit,minmax(250px,1fr))}
.contact li{background:var(--surface);border:1px solid var(--line);border-radius:10px;padding:1rem 1.2rem}
.contact small{display:block;color:var(--muted)}
.contact a{font-weight:600;color:var(--blue);word-break:break-word}
.cta{background:var(--surface);border:1px solid var(--blue);border-radius:12px;padding:1.8rem;text-align:center;margin-top:2rem;box-shadow:0 0 30px var(--glow)}
footer{border-top:1px solid var(--line);padding:1.6rem 0;text-align:center;color:var(--muted);font-size:.95rem}
</style>
</head>
<body>
<svg width="0" height="0" style="position:absolute" aria-hidden="true"><symbol id="logo" viewBox="0 0 48 48"><path d="M24 3 6 10v13c0 11 7.6 18.6 18 22 10.4-3.4 18-11 18-22V10z" fill="#0a2a5c" stroke="#2f8cff" stroke-width="2.5"/><path d="M17 15v16h13" fill="none" stroke="#eaf2ff" stroke-width="4" stroke-linecap="round" stroke-linejoin="round"/><circle cx="31" cy="19" r="3" fill="#2f8cff"/></symbol></svg>

<header class="nav"><div class="wrap">
  <a class="brand" href="#home" aria-label="Liamcybertex home"><svg><use href="#logo"/></svg>Liam<span>cybertex</span></a>
  <nav class="links" aria-label="Main">
    <a href="#home" data-p="home">Home</a><a href="#services" data-p="services">Services</a><a href="#shop" data-p="shop">IT Shop</a><a href="#about" data-p="about">About</a><a href="#contact" data-p="contact">Contact</a>
  </nav>
</div></header>

<main>
<div class="page" id="home">
  <div class="hero"><div class="wrap">
    <span class="tag">Cyber security · Cloud · IT hardware</span>
    <h1>Secure systems. <em>Smarter cloud.</em> Reliable IT.</h1>
    <p class="lead">Liamcybertex protects your business from cyber threats, sets up your cloud, and supplies the IT equipment you need, all in one place.</p>
    <div class="btns"><a class="btn fill" href="#services">Our services</a><a class="btn" href="https://wa.me/254769560407">Chat on WhatsApp</a></div>
    <div class="stats"><div><b>Security</b><span>Protection and checks</span></div><div><b>Cloud</b><span>Setup and migration</span></div><div><b>IT Shop</b><span>Hardware and accessories</span></div></div>
  </div></div>
  <section class="blk"><div class="wrap">
    <h2>What we do</h2>
    <div class="grid">
      <div class="card"><div class="ico">🛡️</div><h3>Cyber security services</h3><p>Keep your data, staff and customers safe from attacks.</p><a class="btn" href="#services">Learn more</a></div>
      <div class="card"><div class="ico">☁️</div><h3>Cloud setup</h3><p>Get your business running on the cloud, safely and correctly.</p><a class="btn" href="#services">Learn more</a></div>
      <div class="card"><div class="ico">💻</div><h3>IT shop</h3><p>Computers, networking gear and accessories for work and home.</p><a class="btn" href="#shop">Visit shop</a></div>
    </div>
  </div></section>
</div>

<div class="page" id="services">
  <div class="wrap">
    <div class="pagehead"><h1>Our <em>services</em></h1><p class="lead">Practical protection and cloud solutions for small businesses, schools and individuals.</p></div>
    <div class="grid">
      <div class="card"><div class="ico">🛡️</div><h3>Cyber security</h3><ul><li>Security checks and risk assessment</li><li>Network and Wi-Fi protection</li><li>Account and password security</li><li>Malware cleanup and prevention</li><li>Staff security awareness</li></ul></div>
      <div class="card"><div class="ico">☁️</div><h3>Cloud setup</h3><ul><li>Cloud account setup and configuration</li><li>Moving files and systems to the cloud</li><li>Secure access and permissions</li><li>Backups and recovery</li><li>Website and app hosting</li></ul></div>
      <div class="card"><div class="ico">🔧</div><h3>IT support</h3><ul><li>Computer and network troubleshooting</li><li>Software installation</li><li>System setup for offices</li><li>Advice on the right equipment</li></ul></div>
    </div>
    <section class="blk" style="margin-top:2rem"><h2>How it works</h2>
      <ol class="steps"><li><b>Contact us.</b> Tell us what you need on WhatsApp, phone or email.</li><li><b>We assess.</b> We review your setup and agree a clear plan and price.</li><li><b>We deliver.</b> We set up, secure and test everything.</li><li><b>We support.</b> We stay available if you need help afterwards.</li></ol>
    </section>
    <div class="cta"><h2>Need a quote?</h2><p class="lead" style="margin-inline:auto">Tell us about your business and we’ll recommend the right service.</p><a class="btn fill" href="https://wa.me/254769560407?text=Hello%20Liamcybertex%2C%20I%20would%20like%20a%20quote%20for%20your%20services.">Request a quote</a></div>
  </div>
</div>

<div class="page" id="shop">
  <div class="wrap">
    <div class="pagehead"><h1>IT <em>shop</em></h1><p class="lead">Quality IT equipment with advice from people who understand security. Message us for stock and prices.</p></div>
    <div class="grid">
      <div class="card"><div class="ico">💻</div><h3>Laptops and desktops</h3><p>New and refurbished computers for work, school and business.</p><a class="btn" href="https://wa.me/254769560407?text=Hello%2C%20I%20am%20interested%20in%20laptops%20and%20desktops.">Ask for prices</a></div>
      <div class="card"><div class="ico">📡</div><h3>Networking</h3><p>Routers, switches, cables and Wi-Fi equipment.</p><a class="btn" href="https://wa.me/254769560407?text=Hello%2C%20I%20am%20interested%20in%20networking%20equipment.">Ask for prices</a></div>
      <div class="card"><div class="ico">🔐</div><h3>Security devices</h3><p>Security keys, CCTV and other protection hardware.</p><a class="btn" href="https://wa.me/254769560407?text=Hello%2C%20I%20am%20interested%20in%20security%20devices.">Ask for prices</a></div>
      <div class="card"><div class="ico">🖱️</div><h3>Accessories</h3><p>Keyboards, mice, chargers, flash drives and storage.</p><a class="btn" href="https://wa.me/254769560407?text=Hello%2C%20I%20am%20interested%20in%20accessories.">Ask for prices</a></div>
      <div class="card"><div class="ico">🖨️</div><h3>Printers and office</h3><p>Printers, toner and office IT essentials.</p><a class="btn" href="https://wa.me/254769560407?text=Hello%2C%20I%20am%20interested%20in%20printers.">Ask for prices</a></div>
      <div class="card"><div class="ico">🔧</div><h3>Parts and repairs</h3><p>Batteries, screens, memory and repair services.</p><a class="btn" href="https://wa.me/254769560407?text=Hello%2C%20I%20need%20a%20repair%20or%20parts.">Ask for prices</a></div>
    </div>
  </div>
</div>

<div class="page" id="about">
  <div class="wrap">
    <div class="pagehead"><h1>About <em>Liamcybertex</em></h1></div>
    <p class="lead">Liamcybertex was founded by Kelvin Kipkoech, a computer science student at KYU and a skilled cyber security and cloud engineer. We help businesses and individuals stay safe online and make the most of technology.</p>
    <div class="grid" style="margin-top:1.5rem">
      <div class="card"><h3>Security first</h3><p>Every setup we do is built with protection in mind.</p></div>
      <div class="card"><h3>Clear and honest</h3><p>Plain language, fair advice and no unnecessary upsells.</p></div>
      <div class="card"><h3>Always learning</h3><p>We keep up with new threats and tools, including AI. Kelvin is also building an AI detector project.</p></div>
    </div>
  </div>
</div>

<div class="page" id="contact">
  <div class="wrap">
    <div class="pagehead"><h1>Contact <em>us</em></h1><p class="lead">The fastest way to reach us is WhatsApp.</p></div>
    <ul class="contact">
      <li><small>Phone</small><a href="tel:+254769560407">0769 560 407</a></li>
      <li><small>WhatsApp</small><a href="https://wa.me/254769560407">Message 0769 560 407</a></li>
      <li><small>Email</small><a href="mailto:nizzyliam@gmail.com">nizzyliam@gmail.com</a></li>
      <li><small>Instagram</small><a href="https://instagram.com/Nizzyliam">@Nizzyliam</a></li>
      <li><small>X (Twitter)</small><a href="https://x.com/Nizzyliam">@Nizzyliam</a></li>
      <li><small>TikTok</small><a href="https://tiktok.com/@Nizzyliam">@Nizzyliam</a></li>
      <li><small>Facebook</small><a href="https://facebook.com/Nizzyliam">@Nizzyliam</a></li>
      <li><small>GitHub</small><a href="https://github.com/Nizzyliam">@Nizzyliam</a></li>
    </ul>
  </div>
</div>
</main>

<footer><div class="wrap">© 2026 Liamcybertex. All rights reserved.</div></footer>

<script>
(function(){
  var pages=["home","services","shop","about","contact"];
  function show(){
    var h=(location.hash||"").replace("#","");
    if(pages.indexOf(h)<0)h="home";
    pages.forEach(function(p){document.getElementById(p).classList.toggle("show",p===h)});
    document.querySelectorAll("nav.links a").forEach(function(a){a.classList.toggle("on",a.getAttribute("data-p")===h)});
    window.scrollTo(0,0);
  }
  window.addEventListener("hashchange",show);
  show();
})();
</script>
</body>
</html>
