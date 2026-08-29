<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>NCRC — North Coast Run Crew</title>
<meta name="description" content="Your Social Run Crew on the North Coast.
Every Thursday, 7:30pm at Babushka Portrush. 5k, your pace, with a halfway
rest. No sign-ups, no commitments." />
<style>
:root {
--purple: #4a2c8a;
--purple-dark: #3a1f6e;
--purple-deep: #2d1758;
--purple-light: #6b4bb5;
--white: #ffffff;
--off-white: #f8f6fc;
--sand: #f5f3f9;
--muted: #6b6580;
--text: #1a122e;
--accent: #e8d5ff;
}
  * {
margin: 0;
padding: 0;
box-sizing: border-box;
}
  html {
scroll-behavior: smooth;
}
  body {
font-family: "Segoe UI", system-ui, -apple-system, BlinkMacSystemFont,
sans-serif;    color: var(--text);
background: var(--sand);
line-height: 1.6;
}
a {
color: inherit;
text-decoration:}
none;
/* Header */
header {
position: fixed;
top: 0;
left: 0;
right: 0;
z-index: 100;
background: rgba(45, 23, 88, 0.95);
backdrop-filter: blur(12px);
border-bottom: 1px solid rgba(255, 255, 255, 0.08);
}
.nav {
max-width: 1080px;
margin: 0 auto;
padding: 0.7rem 1.4rem;
display: flex;
align-items: center;
justify-content: space-between;
}
.logo {
display: flex;
align-items: center;
gap: 0.65rem;
color: var(--white);      }
.logo img {
height: 42px;
width: auto;
border-radius: 6px;
display: block;
}
.logo-text {
font-weight: 700;
font-size: 0.95rem;
letter-spacing: 0.04em;
text-transform: uppercase;
line-height: 1.15;
}
.nav-links {
display: flex;
gap: 1.5rem;
list-style: none;
align-items: center;
}
.nav-links a {
color: rgba(255, 255, 255, 0.85);
font-size: 0.92rem;
font-weight: 500;
transition: color 0.2s;
}
.nav-links a:hover {
color: var(--accent);
}
.nav-cta {background: var(--white) !important;
color: var(--purple) !important;
padding: 0.42rem 1.1rem;
border-radius: 999px;
font-weight: 700;
}
  .nav-cta:hover {
background: var(--accent) !important;
color: var(--purple-deep) !important;
}
  /* Hero */
.hero {
min-height: 100vh;
background: linear-gradient(160deg, var(--purple-deep) 0%, var(--purple)
55%, var(--purple-light) 100%);
color: white;
display: flex;
align-items: center;
padding: 7.5rem 1.4rem 5rem;
position: relative;
overflow: hidden;
}
  .hero::before {
content: "";
position: absolute;
inset: 0;
background: radial-gradient(ellipse at 80% 20%, rgba(255,255,255,0.08),
transparent 50%);
pointer-events: none;
}
  .hero::after {
content: "";   position: absolute;
bottom: -1px;
left: 0;
right: 0;
height: 70px;
background: var(--sand);
clip-path: ellipse(65% 100% at 50% 100%);
}
.hero-inner {
max-width: 1080px;
margin: 0 auto;
width: 100%;
position: relative;
z-index: 1;
}
.hero-logo {
width: 140px;
height: auto;
border-radius: 12px;
margin-bottom: 1.5rem;
box-shadow: 0 12px 40px rgba(0,0,0,0.25);
}
.hero-badge {
display: inline-flex;
align-items: center;
gap: 0.4rem;
background: rgba(255, 255, 255, 0.12);
border: 1px solid rgba(255, 255, 255, 0.2);
padding: 0.35rem 0.95rem;
border-radius: 999px;
font-size: 0.84rem;
font-weight: 500;
margin-bottom: 1.2rem;     letter-spacing:}
0.02em;
.hero h1 {
font-size: clamp(2.5rem, 6.5vw, 3.9rem);
font-weight: 800;
line-height: 1.08;
margin-bottom: 1rem;
letter-spacing: -0.025em;
text-transform: uppercase;
}
.hero h1 span {
display: block;
color: var(--accent);
}
.hero-lead {
font-size: 1.18rem;
max-width: 32rem;
opacity: 0.95;
margin-bottom: 1.85rem;
}
.hero-actions {
display: flex;
flex-wrap: wrap;
gap: 0.8rem;
}
.btn {
display: inline-flex;
align-items: center;
justify-content: center;
padding: 0.82rem 1.55rem;
border-radius: 999px;      font-weight: 600;
font-size: 0.98rem;
transition: transform 0.15s, background 0.2s, box-shadow 0.2s;
border: none;
cursor: pointer;
}
.btn:hover {
transform: translateY(-2px);
}
.btn-primary {
background: var(--white);
color: var(--purple);
box-shadow: 0 8px 28px rgba(0,0,0,0.2);
font-weight: 700;
}
.btn-primary:hover {
background: var(--accent);
color: var(--purple-deep);
}
.btn-ghost {
background: transparent;
color: white;
border: 1.5px solid rgba(255, 255, 255, 0.45);
}
.btn-ghost:hover {
background: rgba(255, 255, 255, 0.12);
border-color: white;
}
/* Sections */
section {     padding: 4.25rem 1.4rem;
}
.container {
max-width: 1080px;
margin: 0 auto;
}
.section-label {
font-size: 0.78rem;
font-weight: 700;
letter-spacing: 0.13em;
text-transform: uppercase;
color: var(--purple);
margin-bottom: 0.5rem;
}
.section-title {
font-size: clamp(1.75rem, 3.4vw, 2.3rem);
font-weight: 800;
letter-spacing: -0.02em;
margin-bottom: 0.85rem;
color: var(--text);
}
.section-lead {
font-size: 1.08rem;
color: var(--muted);
max-width: 36rem;
margin-bottom: 2.25rem;
}
/* About */
.about-grid {
display: grid;
grid-template-columns: 1.15fr 0.85fr;     gap: 2rem;
align-items:}
start;
.about-card {
background: white;
border-radius: 1.15rem;
padding: 1.6rem 1.5rem;
box-shadow: 0 4px 22px rgba(45, 23, 88, 0.06);
border: 1px solid rgba(74, 44, 138, 0.08);
margin-bottom: 1rem;
}
.about-card:last-childmargin-bottom: 0;
}
{
.about-card h3 {
font-size: 1.1rem;
margin-bottom: 0.4rem;
color: var(--purple-dark);
}
.about-card p {
color: var(--muted);
font-size: 0.97rem;
}
.highlight-box {
background: var(--purple);
color: white;
border-radius: 1.2rem;
padding: 1.85rem 1.6rem;
height: 100%;
}
     .highlight-box h3 {
font-size: 1.2rem;
margin-bottom: 0.75rem;
}
.highlight-box ul {
list-style: none;
}
.highlight-box li {
display: flex;
gap: 0.65rem;
margin-bottom: 0.7rem;
font-size: 0.97rem;
opacity: 0.95;
}
.highlight-box li::before {
content: "→";
color: var(--accent);
font-weight: 700;
flex-shrink: 0;
}
/* When & Where */
#run {
background: white;
}
.run-card {
background: var(--off-white);
border-radius: 1.25rem;
padding: 2rem 1.75rem;
border: 1px solid rgba(74, 44, 138, 0.08);
display: grid;
grid-template-columns: 1fr 1fr;      gap: 2rem;
align-items:}
center;
.run-details h3 {
font-size: 1.35rem;
margin-bottom: 0.85rem;
color: var(--text);
}
.detail-row {
display: flex;
gap: 0.75rem;
margin-bottom: 0.65rem;
font-size: 1.02rem;
}
.detail-row strong {
min-width: 5.5rem;
color: var(--purple);
font-weight: 600;
}
.detail-row span {
color: var(--text);
}
.run-cta {
text-align: center;
background: white;
border-radius: 1rem;
padding: 1.75rem 1.5rem;
border: 1px solid rgba(74, 44, 138, 0.08);
}
.run-cta p {color: var(--muted);
font-size: 0.95rem;
margin-bottom: 1.15rem;
}
  .run-cta .btn-primary {
width: 100%;
background: var(--purple);
color: white;
box-shadow: 0 8px 24px rgba(74, 44, 138, 0.3);
}
  .run-cta .btn-primary:hover {
background: var(--purple-dark);
color: white;
}
  /* Join */
#join {
background: linear-gradient(160deg, var(--purple-deep) 0%, var(--purple)
100%);
color: white;
}
  #join .section-label {
color: var(--accent);
}
  #join .section-title {
color: white;
}
  #join .section-lead {
color: rgba(255, 255, 255, 0.85);
}
    .join-points {
list-style: none;
margin-bottom:}
1.75rem;
.join-points li {
display: flex;
gap: 0.7rem;
margin-bottom: 0.7rem;
font-size: 1.02rem;
opacity: 0.95;
}
.join-points li::before {
content: "✓";
color: var(--accent);
font-weight: 800;
flex-shrink: 0;
}
.ig-link {
display: inline-flex;
align-items: center;
gap: 0.5rem;
background: rgba(255, 255, 255, 0.12);
border: 1px solid rgba(255, 255, 255, 0.25);
padding: 0.85rem 1.5rem;
border-radius: 999px;
font-weight: 600;
transition: background 0.2s, transform 0.15s;
}
.ig-link:hover {
background: rgba(255, 255, 255, 0.2);
transform: translateY(-2px);
}     /* Contact */
.contact-grid {
display: grid;
grid-template-columns: repeat(3, 1fr);
gap: 1.15rem;
}
.contact-card {
background: white;
border-radius: 1.1rem;
padding: 1.6rem 1.25rem;
text-align: center;
border: 1px solid rgba(74, 44, 138, 0.08);
box-shadow: 0 4px 18px rgba(45, 23, 88, 0.05);
}
.contact-icon {
width: 46px;
height: 46px;
margin: 0 auto 0.9rem;
border-radius: 50%;
background: rgba(74, 44, 138, 0.1);
color: var(--purple);
display: grid;
place-items: center;
font-size: 1.15rem;
font-weight: 700;
}
.contact-card h3 {
font-size: 1.02rem;
margin-bottom: 0.3rem;
}
.contact-card p,      .contact-card a {
font-size: 0.93rem;
color: var(--muted);
}
.contact-card a:hover {
color: var(--purple);
}
/* Footer */
footer {
background: var(--purple-deep);
color: rgba(255, 255, 255, 0.75);
padding: 2.5rem 1.4rem;
text-align: center;
font-size: 0.88rem;
}
footer .footer-logo {
height: 56px;
width: auto;
border-radius: 8px;
margin-bottom: 1rem;
}
footer p {
margin-top: 0.4rem;
}
/* Mobile */
@media (max-width: 780px) {
.nav-links {
display: none;
}
.logo-text {display: none;
}
  .about-grid,
.run-card {
grid-template-columns: 1fr;
}
  .contact-grid {
grid-template-columns: 1fr;
}
  .detail-row {
flex-direction: column;
gap: 0.15rem;
}
  .detail-row strong {
min-width: auto;
}
  .hero-logo {
width: 110px;
}
}
</style>
</head>
<body>
<header>
<nav class="nav">
<a href="#" class="logo">
<img src="ncrc-logo.png" alt="North Coast Run Crew" />
<span class="logo-text">North Coast<br />Run Crew</span>
</a>
<ul class="nav-links">
<li><a href="#about">About</a></li><li><a href="#run">The Run</a></li>
<li><a href="#join">Join</a></li>
<li><a href="#contact">Contact</a></li>
<li><a href="https://www.instagram.com/northcoastruncrew/"
target="_blank" rel="noopener" class="nav-cta">Instagram</a></li>
</ul>
</nav>
</header>
  <section class="hero">
<div class="hero-inner">
<img src="ncrc-logo.png" alt="North Coast Run Crew" class="hero-logo" />
<div class="hero-badge">Your Social Run Crew on the North Coast 💙</div>
<h1>Every Thursday.<span>Your pace.</span></h1>
<p class="hero-lead">
5k with a halfway rest. No sign-ups. No commitments. Just show up and
run with the crew in Portrush.
</p>
<div class="hero-actions">
<a href="#run" class="btn btn-primary">When & where</a>
<a href="https://www.instagram.com/northcoastruncrew/" target="_blank"
rel="noopener" class="btn btn-ghost">Follow on Instagram</a>
</div>
</div>
</section>
  <section id="about">
<div class="container">
<p class="section-label">Who we are</p>
<h2 class="section-title">NCRC — North Coast Run Crew</h2>
<p class="section-lead">
A friendly social run crew based on Northern Ireland’s North Coast. We
meet every Thursday evening for an easy, inclusive 5k.
</p>
  <div class="about-grid"><div>
<div class="about-card">
<h3>All paces welcome</h3>
<p>
Whether you’re brand new or a regular, we run at your pace. There’s a
halfway rest so everyone can stick together and enjoy the craic.
</p>
</div>
<div class="about-card">
<h3>No pressure, no commitment</h3>
<p>
No sign-ups. No fees. Just turn up when you can. It’s a local social run
crew — come once or come every week.
</p>
</div>
<div class="about-card">
<h3>Coastal community</h3>
<p>
We meet by the sea in Portrush and keep things simple, welcoming and
social. Blue-heart energy only.
</p>
</div>
</div>
<div class="highlight-box">
<h3>The vibe</h3>
<ul>
<li>Social first, pace second</li>
<li>Halfway break built in</li>
<li>Locals & visitors welcome</li>
<li>Post-run chat encouraged</li>
<li>Just show up</li>
</ul>
</div>
</div>
</div>
</section>  <section id="run">
<div class="container">
<p class="section-label">Weekly session</p>
<h2 class="section-title">Thursday evening 5k</h2>
<p class="section-lead">
Same time, same place every week. Meet early for a chat, then head out
together.
</p>
  <div class="run-card">
<div class="run-details">
<h3>Thursday social run</h3>
<div class="detail-row">
<strong>Meet</strong>
<span>7:30pm at Babushka, Portrush</span>
</div>
<div class="detail-row">
<strong>Run starts</strong>
<span>7:45pm</span>
</div>
<div class="detail-row">
<strong>Distance</strong>
<span>5k (with a halfway rest)</span>
</div>
<div class="detail-row">
<strong>Pace</strong>
<span>Your pace — all abilities welcome</span>
</div>
<div class="detail-row">
<strong>Where</strong>
<span>Babushka Kitchen Café, South Pier, Portrush</span>
</div>
</div>
<div class="run-cta">
<p>No need to message ahead.<br />Just lace up and come along.</p><a href="https://www.instagram.com/northcoastruncrew/"
target="_blank" rel="noopener" class="btn btn-primary">
Check Instagram for updates
</a>
</div>
</div>
</div>
</section>
  <section id="join">
<div class="container">
<p class="section-label">Get involved</p>
<h2 class="section-title">Come run with us</h2>
<p class="section-lead">
The easiest way to stay in the loop is Instagram. That’s where we post any
changes and share the crew vibe.
</p>
<ul class="join-points">
<li>Free — no membership, no sign-up</li>
<li>Show up on Thursday at 7:30pm</li>
<li>Follow @northcoastruncrew for updates</li>
<li>Bring a friend or come solo</li>
</ul>
<a href="https://www.instagram.com/northcoastruncrew/" target="_blank"
rel="noopener" class="ig-link">
@northcoastruncrew on Instagram →
</a>
</div>
</section>
  <section id="contact">
<div class="container">
<p class="section-label">Find us</p>
<h2 class="section-title">Questions or first time?</h2>
<p class="section-lead">
Drop us a message on Instagram or just come along — we’ll look after you.</p>
  <div class="contact-grid">
<div class="contact-card">
<div class="contact-icon">IG</div>
<h3>Instagram</h3>
<a href="https://www.instagram.com/northcoastruncrew/"
target="_blank" rel="noopener">@northcoastruncrew</a>
</div>
<div class="contact-card">
<div class="contact-icon">📍</div>
<h3>Meet point</h3>
<p>Babushka<br />South Pier, Portrush</p>
</div>
<div class="contact-card">
<div class="contact-icon">🕐</div>
<h3>Every Thursday</h3>
<p>Meet 7:30pm<br />Run 7:45pm</p>
</div>
</div>
</div>
</section>
  <footer>
<img src="ncrc-logo.png" alt="North Coast Run Crew" class="footer-logo" />
<p>Your Social Run Crew on the North Coast 💙</p>
<p style="margin-top: 0.85rem; opacity: 0.55;">Portrush · Northern Ireland ·
All paces welcome</p>
</footer>
</body>
</html>
