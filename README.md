# aruaradhna26.github.io
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Priyanka 🎂</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Cormorant+Garamond:ital,wght@0,300;0,400;1,300;1,400&family=Dancing+Script:wght@400;700&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

  :root {
    --rose: #f4a7b9;
    --blush: #fce4ec;
    --gold: #f9c74f;
    --deep-rose: #c2185b;
    --cream: #fff8f0;
    --peach: #ffb347;
    --lavender: #ce93d8;
    --text: #4a1942;
  }

  html { scroll-behavior: smooth; }

  body {
    background: linear-gradient(135deg, #1a0a2e 0%, #2d0a4e 30%, #1a0a2e 60%, #0d0620 100%);
    min-height: 100vh;
    font-family: 'Cormorant Garamond', serif;
    overflow-x: hidden;
    color: #fff;
  }

  /* ── FIREWORKS CANVAS ── */
  #fireworks-canvas {
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    pointer-events: none;
    z-index: 0;
  }

  /* ── FLOATING HEARTS ── */
  .hearts-layer {
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    pointer-events: none;
    z-index: 1;
    overflow: hidden;
  }
  .heart {
    position: absolute;
    bottom: -60px;
    font-size: 1.4rem;
    opacity: 0;
    animation: floatHeart linear infinite;
  }
  @keyframes floatHeart {
    0%   { opacity: 0; transform: translateY(0) rotate(-10deg) scale(0.8); }
    10%  { opacity: 0.9; }
    80%  { opacity: 0.6; }
    100% { opacity: 0; transform: translateY(-110vh) rotate(20deg) scale(1.2); }
  }

  /* ── SPARKLING STARS ── */
  .star {
    position: fixed;
    width: 3px; height: 3px;
    border-radius: 50%;
    background: #fff;
    pointer-events: none;
    z-index: 1;
    animation: twinkle ease-in-out infinite;
  }
  @keyframes twinkle {
    0%, 100% { opacity: 0; transform: scale(0.5); }
    50%       { opacity: 1; transform: scale(1.4); }
  }

  /* ── MAIN WRAPPER ── */
  .wrapper {
    position: relative;
    z-index: 2;
    max-width: 860px;
    margin: 0 auto;
    padding: 60px 24px 80px;
  }

  /* ── HERO HEADER ── */
  .hero {
    text-align: center;
    margin-bottom: 60px;
    animation: fadeDown 1.2s ease both;
  }
  @keyframes fadeDown {
    from { opacity: 0; transform: translateY(-40px); }
    to   { opacity: 1; transform: translateY(0); }
  }
  .hero-sub {
    font-family: 'Dancing Script', cursive;
    font-size: clamp(1.2rem, 3vw, 1.6rem);
    color: var(--rose);
    letter-spacing: 0.12em;
    margin-bottom: 10px;
    animation: fadeDown 1s ease 0.2s both;
  }
  .hero-title {
    font-family: 'Playfair Display', serif;
    font-size: clamp(3rem, 10vw, 6.5rem);
    font-weight: 700;
    line-height: 1;
    background: linear-gradient(135deg, #f9c74f, #f4a7b9, #ce93d8, #f9c74f);
    background-size: 300% 300%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: gradientShift 4s ease-in-out infinite, fadeDown 1s ease 0.4s both;
  }
  @keyframes gradientShift {
    0%,100% { background-position: 0% 50%; }
    50%      { background-position: 100% 50%; }
  }
  .hero-name {
    font-family: 'Dancing Script', cursive;
    font-size: clamp(2.8rem, 9vw, 5.5rem);
    color: #fff;
    text-shadow: 0 0 40px rgba(244,167,185,0.8), 0 0 80px rgba(244,167,185,0.4);
    animation: fadeDown 1s ease 0.6s both, namePulse 3s ease-in-out 2s infinite;
  }
  @keyframes namePulse {
    0%,100% { text-shadow: 0 0 40px rgba(244,167,185,0.8), 0 0 80px rgba(244,167,185,0.4); }
    50%      { text-shadow: 0 0 60px rgba(244,167,185,1), 0 0 120px rgba(249,199,79,0.6); }
  }
  .hero-decor {
    font-size: 2rem;
    margin-top: 16px;
    animation: fadeDown 1s ease 0.8s both;
    filter: drop-shadow(0 0 8px rgba(249,199,79,0.7));
  }

  /* ── GLASS CARD ── */
  .glass-card {
    background: rgba(255,255,255,0.06);
    backdrop-filter: blur(18px);
    -webkit-backdrop-filter: blur(18px);
    border: 1px solid rgba(255,255,255,0.15);
    border-radius: 28px;
    padding: 42px 48px;
    margin-bottom: 36px;
    box-shadow: 0 8px 60px rgba(0,0,0,0.4), inset 0 1px 0 rgba(255,255,255,0.12);
    animation: fadeUp 0.9s ease both;
  }
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(40px); }
    to   { opacity: 1; transform: translateY(0); }
  }
  .glass-card:nth-child(2) { animation-delay: 0.2s; }
  .glass-card:nth-child(3) { animation-delay: 0.4s; }
  .glass-card:nth-child(4) { animation-delay: 0.6s; }

  /* ── LETTER ── */
  .letter-label {
    font-family: 'Dancing Script', cursive;
    font-size: 1.4rem;
    color: var(--gold);
    margin-bottom: 20px;
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .letter-label::after {
    content: '';
    flex: 1;
    height: 1px;
    background: linear-gradient(90deg, rgba(249,199,79,0.4), transparent);
  }
  .letter-body {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.18rem;
    line-height: 1.9;
    color: rgba(255,255,255,0.88);
    font-style: italic;
  }
  .letter-body p { margin-bottom: 18px; }
  .letter-body p:last-child { margin-bottom: 0; }
  .letter-signature {
    text-align: right;
    margin-top: 28px;
    font-family: 'Dancing Script', cursive;
    font-size: 1.6rem;
    color: var(--rose);
    text-shadow: 0 0 20px rgba(244,167,185,0.5);
  }

  /* ── BIRTHDAY CAKE ── */
  .cake-section {
    text-align: center;
  }
  .cake-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.5rem;
    color: var(--gold);
    margin-bottom: 28px;
    font-style: italic;
  }
  .cake-container {
    display: inline-block;
    position: relative;
    margin-bottom: 28px;
  }
  .candles-row {
    display: flex;
    justify-content: center;
    gap: 22px;
    margin-bottom: 0;
    position: relative;
    z-index: 3;
  }
  .candle {
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
  }
  .flame {
    width: 12px;
    height: 20px;
    background: radial-gradient(ellipse at 50% 80%, #fff700, #ff9800 40%, #ff4500 80%, transparent);
    border-radius: 50% 50% 30% 30%;
    animation: flicker 0.3s ease-in-out infinite alternate;
    filter: drop-shadow(0 0 6px #ff9800) drop-shadow(0 0 14px #ff4500);
    transform-origin: bottom center;
    transition: opacity 0.4s;
  }
  @keyframes flicker {
    0%   { transform: scaleX(1) scaleY(1) rotate(-3deg); }
    100% { transform: scaleX(0.85) scaleY(1.1) rotate(3deg); }
  }
  .flame.out {
    animation: blowOut 0.5s ease forwards;
  }
  @keyframes blowOut {
    0%   { opacity: 1; transform: scaleY(1.4) scaleX(0.6) translateY(-8px); }
    60%  { opacity: 0.4; transform: scaleY(0.3) scaleX(2) translateY(4px); }
    100% { opacity: 0; transform: scaleY(0); }
  }
  .candle-stick {
    width: 10px;
    height: 44px;
    background: linear-gradient(180deg, #fff, #fce4ec 40%, #f48fb1);
    border-radius: 5px 5px 3px 3px;
    position: relative;
  }
  .candle-stick::after {
    content: '';
    position: absolute;
    top: 0; left: 50%;
    transform: translateX(-50%);
    width: 3px; height: 8px;
    background: #555;
    border-radius: 2px;
  }
  /* CAKE SVG */
  .cake-svg {
    display: block;
    margin: 0 auto;
    filter: drop-shadow(0 10px 30px rgba(244,167,185,0.4));
  }

  /* ── COUNTDOWN ── */
  .countdown-area { margin-top: 24px; }
  .countdown-display {
    font-family: 'Playfair Display', serif;
    font-size: 5rem;
    font-weight: 700;
    color: #fff;
    text-shadow: 0 0 40px rgba(249,199,79,0.8);
    min-height: 80px;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: all 0.2s;
  }
  .blow-btn {
    margin-top: 20px;
    padding: 16px 48px;
    font-family: 'Dancing Script', cursive;
    font-size: 1.4rem;
    color: var(--text);
    background: linear-gradient(135deg, var(--gold), var(--peach));
    border: none;
    border-radius: 50px;
    cursor: pointer;
    box-shadow: 0 4px 20px rgba(249,199,79,0.4);
    transition: transform 0.2s, box-shadow 0.2s;
    letter-spacing: 0.05em;
  }
  .blow-btn:hover { transform: scale(1.06); box-shadow: 0 6px 30px rgba(249,199,79,0.6); }
  .blow-btn:active { transform: scale(0.97); }
  .wish-message {
    font-family: 'Dancing Script', cursive;
    font-size: 2rem;
    color: var(--rose);
    margin-top: 20px;
    opacity: 0;
    transition: opacity 0.8s;
    text-shadow: 0 0 20px rgba(244,167,185,0.7);
  }
  .wish-message.show { opacity: 1; }

  /* ── PHOTO FRAME EMOJIS ── */
  .deco-row {
    display: flex;
    justify-content: center;
    gap: 14px;
    font-size: 2rem;
    margin: 10px 0 0;
    filter: drop-shadow(0 2px 8px rgba(0,0,0,0.3));
  }

  /* ── FOOTER ── */
  .footer {
    text-align: center;
    padding-top: 20px;
    font-family: 'Dancing Script', cursive;
    font-size: 1.1rem;
    color: rgba(255,255,255,0.35);
  }

  @media (max-width: 600px) {
    .glass-card { padding: 28px 22px; }
    .letter-body { font-size: 1rem; }
  }
</style>
</head>
<body>

<canvas id="fireworks-canvas"></canvas>
<div class="hearts-layer" id="hearts-layer"></div>

<div class="wrapper">

  <!-- HERO -->
  <div class="hero">
    <div class="hero-sub">✨ Wishing you the most magical day ✨</div>
    <div class="hero-title">Happy Birthday</div>
    <div class="hero-name">Priyanka</div>
    <div class="hero-decor">🌸 🌟 🎉 🌸</div>
  </div>

  <!-- CAKE SECTION -->
  <div class="glass-card cake-section" style="animation-delay:0.1s">
    <div class="cake-title">Make a wish & blow out the candles 🕯️</div>
    <div class="cake-container">
      <div class="candles-row" id="candles-row">
        <div class="candle"><div class="flame" id="f1"></div><div class="candle-stick"></div></div>
        <div class="candle"><div class="flame" id="f2"></div><div class="candle-stick"></div></div>
        <div class="candle"><div class="flame" id="f3"></div><div class="candle-stick"></div></div>
        <div class="candle"><div class="flame" id="f4"></div><div class="candle-stick"></div></div>
        <div class="candle"><div class="flame" id="f5"></div><div class="candle-stick"></div></div>
      </div>
      <!-- Birthday cake SVG -->
      <svg class="cake-svg" width="320" height="200" viewBox="0 0 320 200" fill="none" xmlns="http://www.w3.org/2000/svg">
        <!-- Plate -->
        <ellipse cx="160" cy="188" rx="145" ry="12" fill="rgba(255,255,255,0.08)"/>
        <!-- Bottom tier -->
        <rect x="30" y="130" width="260" height="60" rx="8" fill="url(#cakeBottom)"/>
        <ellipse cx="160" cy="130" rx="130" ry="14" fill="url(#topEllipseB)"/>
        <!-- Bottom tier frosting drip -->
        <path d="M50 130 Q60 115 70 130 Q80 115 90 130 Q100 115 110 130 Q120 115 130 130 Q140 115 150 130 Q160 115 170 130 Q180 115 190 130 Q200 115 210 130 Q220 115 230 130 Q240 115 250 130 Q260 115 270 130" stroke="#fff" stroke-width="3" fill="none" opacity="0.6"/>
        <!-- Bottom tier decorations -->
        <circle cx="80" cy="155" r="6" fill="#f48fb1" opacity="0.9"/>
        <circle cx="120" cy="162" r="5" fill="#ce93d8" opacity="0.9"/>
        <circle cx="160" cy="155" r="6" fill="#f48fb1" opacity="0.9"/>
        <circle cx="200" cy="162" r="5" fill="#ce93d8" opacity="0.9"/>
        <circle cx="240" cy="155" r="6" fill="#f48fb1" opacity="0.9"/>
        <!-- Mid tier -->
        <rect x="65" y="75" width="190" height="58" rx="8" fill="url(#cakeMid)"/>
        <ellipse cx="160" cy="75" rx="95" ry="12" fill="url(#topEllipseM)"/>
        <!-- Mid drip -->
        <path d="M80 75 Q90 62 100 75 Q110 62 120 75 Q130 62 140 75 Q150 62 160 75 Q170 62 180 75 Q190 62 200 75 Q210 62 220 75 Q230 62 240 75" stroke="#fff" stroke-width="2.5" fill="none" opacity="0.55"/>
        <!-- Mid decorations -->
        <text x="100" y="110" font-size="22" text-anchor="middle">🌸</text>
        <text x="160" y="110" font-size="22" text-anchor="middle">🌸</text>
        <text x="220" y="110" font-size="22" text-anchor="middle">🌸</text>
        <!-- Top tier -->
        <rect x="105" y="28" width="110" height="50" rx="8" fill="url(#cakeTop)"/>
        <ellipse cx="160" cy="28" rx="55" ry="10" fill="url(#topEllipseT)"/>
        <!-- Top drip -->
        <path d="M118 28 Q126 17 134 28 Q142 17 150 28 Q158 17 166 28 Q174 17 182 28 Q190 17 198 28 Q206 17 202 28" stroke="#fff" stroke-width="2" fill="none" opacity="0.5"/>
        <!-- Star decorations on top -->
        <text x="130" y="58" font-size="14">⭐</text>
        <text x="158" y="58" font-size="14">⭐</text>
        <text x="186" y="56" font-size="14">⭐</text>
        <!-- Bottom writing -->
        <text x="160" y="167" font-family="Georgia, serif" font-size="13" fill="white" text-anchor="middle" opacity="0.85" font-style="italic">Happy Birthday Priyanka 🎂</text>
        <defs>
          <linearGradient id="cakeBottom" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0%" stop-color="#f8bbd9"/>
            <stop offset="100%" stop-color="#e91e8c"/>
          </linearGradient>
          <linearGradient id="topEllipseB" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0%" stop-color="#fff" stop-opacity="0.85"/>
            <stop offset="100%" stop-color="#f8bbd9" stop-opacity="0.7"/>
          </linearGradient>
          <linearGradient id="cakeMid" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0%" stop-color="#ce93d8"/>
            <stop offset="100%" stop-color="#7b1fa2"/>
          </linearGradient>
          <linearGradient id="topEllipseM" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0%" stop-color="#fff" stop-opacity="0.85"/>
            <stop offset="100%" stop-color="#ce93d8" stop-opacity="0.7"/>
          </linearGradient>
          <linearGradient id="cakeTop" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0%" stop-color="#f9c74f"/>
            <stop offset="100%" stop-color="#f77f00"/>
          </linearGradient>
          <linearGradient id="topEllipseT" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0%" stop-color="#fff" stop-opacity="0.9"/>
            <stop offset="100%" stop-color="#f9c74f" stop-opacity="0.7"/>
          </linearGradient>
        </defs>
      </svg>
    </div>

    <div class="countdown-area">
      <div class="countdown-display" id="countdown-display">🕯️</div>
      <button class="blow-btn" id="blow-btn" onclick="startCountdown()">Blow the Candles!</button>
      <div class="wish-message" id="wish-msg">🎉 May all your wishes come true, Priyanka! 🎉</div>
    </div>
  </div>

  <!-- HEARTFELT LETTER -->
  <div class="glass-card" style="animation-delay:0.3s">
    <div class="letter-label">💌 A Letter from your Aradhna</div>
    <div class="letter-body">
      <p>Happy Birthday Priyanka,</p>
      <p>Where do I even begin? You have been one of the most important person in my life the kind of person whose one call or text lights my day i have missed you soo much  . Today, on your birthday,  the day you were born, i would love to say that althogh i dont give much time to you m,i m happy to have you as my friend</p>
      <p>happy birthday love<3 .</p>
      <p>Thank you for being my friend even when i m rude sometimes even when we dont talk for months even when we dont meet regularly,   I am lucky to have  crossed paths with you.</p>
      <p>On this special day, I hope you feel surrounded by every ounce of joy you have ever given others. I hope the universe shows up for you the same way you show up for everyone you love. I hope today is nothing short of absolutely magical because you deserve nothing less.
      although im not there i hope all your wishes come true 
      happy bithday to my lovely friend</p>
      <p>i hope that you have a great life ahead and you become a great doctor ,dont stress youtrself to much take care love you ,and if you ever feel lonely remember youll always have me.</p>
      <p>Happy Birthday Sweetheart 🌸</p>
    </div>
    <div class="letter-signature">Lots of love, Aradhna 💕</div>
  </div>

  <!-- DECORATIVE FOOTER EMOJIS -->
  <div class="deco-row">🌸 💫 🎂 🎉 ✨ 🌟 💖 🌸</div>

  <div class="footer" style="margin-top:40px">
    Made with all the love in the world for Priyanka 💗
  </div>

</div>

<script>
/* ─── FLOATING HEARTS ─── */
const heartsLayer = document.getElementById('hearts-layer');
const heartEmojis = ['💖','💕','💗','💓','💞','🌸','✨','💫','💝','❤️'];
for (let i = 0; i < 30; i++) {
  const h = document.createElement('div');
  h.className = 'heart';
  h.textContent = heartEmojis[Math.floor(Math.random() * heartEmojis.length)];
  h.style.left = Math.random() * 100 + 'vw';
  h.style.fontSize = (0.9 + Math.random() * 1.6) + 'rem';
  h.style.animationDuration = (6 + Math.random() * 10) + 's';
  h.style.animationDelay = (Math.random() * 10) + 's';
  heartsLayer.appendChild(h);
}

/* ─── TWINKLING STARS ─── */
for (let i = 0; i < 80; i++) {
  const s = document.createElement('div');
  s.className = 'star';
  s.style.left = Math.random() * 100 + 'vw';
  s.style.top = Math.random() * 100 + 'vh';
  const sz = 1 + Math.random() * 3;
  s.style.width = sz + 'px';
  s.style.height = sz + 'px';
  s.style.animationDuration = (1.5 + Math.random() * 3) + 's';
  s.style.animationDelay = (Math.random() * 4) + 's';
  s.style.opacity = Math.random() * 0.8;
  document.body.appendChild(s);
}

/* ─── FIREWORKS ─── */
const canvas = document.getElementById('fireworks-canvas');
const ctx = canvas.getContext('2d');

function resize() {
  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;
}
resize();
window.addEventListener('resize', resize);

class Particle {
  constructor(x, y, color) {
    this.x = x; this.y = y;
    const angle = Math.random() * Math.PI * 2;
    const speed = 1.5 + Math.random() * 5;
    this.vx = Math.cos(angle) * speed;
    this.vy = Math.sin(angle) * speed;
    this.alpha = 1;
    this.decay = 0.012 + Math.random() * 0.018;
    this.color = color;
    this.radius = 1.5 + Math.random() * 2.5;
    this.gravity = 0.08;
    this.trail = [];
  }
  update() {
    this.trail.push({ x: this.x, y: this.y, alpha: this.alpha });
    if (this.trail.length > 6) this.trail.shift();
    this.vy += this.gravity;
    this.vx *= 0.98;
    this.x += this.vx;
    this.y += this.vy;
    this.alpha -= this.decay;
  }
  draw(ctx) {
    for (let i = 0; i < this.trail.length; i++) {
      const t = this.trail[i];
      ctx.beginPath();
      ctx.arc(t.x, t.y, this.radius * (i / this.trail.length), 0, Math.PI * 2);
      ctx.fillStyle = this.color.replace('1)', `${t.alpha * 0.3})`);
      ctx.fill();
    }
    ctx.beginPath();
    ctx.arc(this.x, this.y, this.radius, 0, Math.PI * 2);
    ctx.fillStyle = this.color.replace('1)', `${this.alpha})`);
    ctx.fill();
  }
}

const particles = [];
const fwColors = [
  'rgba(249,199,79,1)', 'rgba(244,167,185,1)', 'rgba(206,147,216,1)',
  'rgba(255,179,71,1)', 'rgba(255,255,255,1)', 'rgba(100,220,255,1)',
  'rgba(180,255,100,1)', 'rgba(255,100,160,1)'
];

function burst(x, y) {
  const color = fwColors[Math.floor(Math.random() * fwColors.length)];
  const count = 70 + Math.floor(Math.random() * 50);
  for (let i = 0; i < count; i++) particles.push(new Particle(x, y, color));
}

function randomBurst() {
  const x = 60 + Math.random() * (canvas.width - 120);
  const y = 60 + Math.random() * (canvas.height * 0.6);
  burst(x, y);
}

let fwInterval = setInterval(randomBurst, 1200);

function animateFireworks() {
  ctx.fillStyle = 'rgba(0,0,0,0.18)';
  ctx.fillRect(0, 0, canvas.width, canvas.height);
  for (let i = particles.length - 1; i >= 0; i--) {
    particles[i].update();
    particles[i].draw(ctx);
    if (particles[i].alpha <= 0) particles.splice(i, 1);
  }
  requestAnimationFrame(animateFireworks);
}
animateFireworks();

/* ─── BIRTHDAY COUNTDOWN & CANDLE BLOW ─── */
let counting = false;

function startCountdown() {
  if (counting) return;
  counting = true;
  const btn = document.getElementById('blow-btn');
  btn.disabled = true;
  btn.style.opacity = '0.5';

  const display = document.getElementById('countdown-display');
  const nums = ['3', '2', '1', '🎉'];
  let i = 0;

  display.textContent = nums[i];
  display.style.transform = 'scale(1.3)';
  setTimeout(() => display.style.transform = 'scale(1)', 200);

  const tick = setInterval(() => {
    i++;
    if (i < nums.length) {
      display.textContent = nums[i];
      display.style.transform = 'scale(1.4)';
      setTimeout(() => display.style.transform = 'scale(1)', 200);

      if (nums[i] === '🎉') {
        blowAllCandles();
        document.getElementById('wish-msg').classList.add('show');
        // extra burst of fireworks
        for (let k = 0; k < 8; k++) {
          setTimeout(() => randomBurst(), k * 200);
        }
        clearInterval(tick);
      }
    }
  }, 900);
}

function blowAllCandles() {
  for (let i = 1; i <= 5; i++) {
    setTimeout(() => {
      const f = document.getElementById('f' + i);
      if (f) f.classList.add('out');
    }, (i - 1) * 120);
  }
}
</script>
</body>
</html>
