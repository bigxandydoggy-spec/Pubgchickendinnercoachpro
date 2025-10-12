<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>PUBG Coach Pro</title>
<link rel="manifest" href="/manifest.json">
<link rel="apple-touch-icon" sizes="180x180" href="/icons/icon-192.png">
<meta name="theme-color" content="#0d2347">
<link rel="stylesheet" href="/css/style.css">
</head>
<body>
  <div class="app">
    <div class="header">
      <div class="logo"><img src="/icons/icon-192.png" style="width:60px;height:60px;border-radius:8px" alt="logo"></div>
      <div><h1>PUBG Coach Pro</h1><div class="small">Your personal sensitivity & graphics trainer</div></div>
    </div>

    <nav>
      <button class="btn" id="btn-sense">🎯 Sensitivity</button>
      <button class="btn" id="btn-graph">⚙️ Graphics</button>
      <button class="btn" id="btn-strat">🧭 Strategies</button>
      <button class="btn" id="btn-crate">🎁 Crate Luck</button>
      <button class="btn" id="btn-nick">✍️ Nicknames</button>
    </nav>

    <div id="main" class="card">
      <h2 id="title">Welcome</h2>
      <p class="small">Tap "Start Coaching" to enable audio on iOS and view tools.</p>
      <div class="row" style="margin-top:12px">
        <button class="btn" id="start">Start Coaching</button>
      </div>
    </div>

    <div id="winner" class="card" style="display:none;text-align:center;margin-top:12px">
      <img src="/icons/icon-512.png" style="width:160px;height:160px" alt="winner">
      <h2 style="color:#ffd75a">Winner Winner Chicken Dinner!</h2>
    </div>

    <footer>© 2025 LucioDevstudio2025 · PUBG Coach Pro</footer>
  </div>

<script src="/js/app.js"></script>
<script>
if('serviceWorker' in navigator){navigator.serviceWorker.register('/service-worker.js').catch(()=>{});}
</script>
</body>
</html>
{
  "name":"PUBG Coach Pro",
  "short_name":"PUBG Coach Pro",
  "start_url":"/index.html",
  "display":"standalone",
  "background_color":"#071028",
  "theme_color":"#0d2347",
  "icons":[
    {"src":"/icons/icon-192.png","sizes":"192x192","type":"image/png"},
    {"src":"/icons/icon-512.png","sizes":"512x512","type":"image/png"}
  ]
}
const CACHE = 'pubg-coach-pro-v1';
const ASSETS = ['/', '/index.html', '/css/style.css', '/js/app.js', '/manifest.json', '/icons/icon-192.png', '/icons/icon-512.png'];
self.addEventListener('install', e => { e.waitUntil(caches.open(CACHE).then(c => c.addAll(ASSETS))); self.skipWaiting(); });
self.addEventListener('activate', e => e.waitUntil(self.clients.claim()));
self.addEventListener('fetch', e => { e.respondWith(caches.match(e.request).then(r => r || fetch(e.request))); });
:root{--bg:#071028;--accent:#d4af37;--muted:#9fb0d8}
*{box-sizing:border-box}
body{margin:0;font-family:Inter,Arial,Helvetica,sans-serif;background:linear-gradient(180deg,#081a33,#071028);color:#eaf3ff}
.app{max-width:980px;margin:18px auto;padding:18px}
.header{display:flex;gap:12px;align-items:center}
.logo{width:76px;height:76px;border-radius:14px;background:linear-gradient(135deg,#07264d,#08305a);display:flex;align-items:center;justify-content:center;border:3px solid rgba(212,175,55,0.12)}
h1{margin:0;color:var(--accent);font-size:20px}
.small{color:var(--muted);font-size:13px}
.btn{background:linear-gradient(90deg,var(--accent),#f2d878);border:none;padding:10px 14px;border-radius:10px;font-weight:700;color:#06102b;cursor:pointer}
.card{background:rgba(255,255,255,0.02);padding:12px;border-radius:12px;margin-top:12px;border:1px solid rgba(255,255,255,0.03)}
nav{display:flex;gap:8px;flex-wrap:wrap;margin-top:12px}
.row{display:flex;gap:8px;align-items:center}
input.input{padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit;width:100%}
footer{margin-top:18px;text-align:center;color:var(--muted);font-size:13px}
// PUBG Coach Pro - client-side features (no server required for basic tools)
console.log('PUBG Coach Pro loaded');

// iOS audio unlock & victory sound
const victory = new Audio('/assets/sounds/victory_remix.mp3');
victory.preload = 'auto'; victory.volume = 0.9;
let interacted = false;
function unlockAudio() {
  if (interacted) return;
  interacted = true;
  victory.play().then(()=>{ victory.pause(); victory.currentTime = 0; }).catch(()=>{});
  window.removeEventListener('touchstart', unlockAudio);
  window.removeEventListener('click', unlockAudio);
}
window.addEventListener('touchstart', unlockAudio, {passive:true});
window.addEventListener('click', unlockAudio);

// simple UI handlers
document.getElementById('start')?.addEventListener('click', ()=>{ alert('Start Coaching — tap any tool to begin'); interacted=true; });

document.getElementById('btn-sense')?.addEventListener('click', ()=> {
  const main = document.getElementById('main');
  document.getElementById('title').innerText = 'Sensitivity Adjuster';
  main.innerHTML = `
    <h3>Sensitivity Adjuster</h3>
    <p class="small">Enter your base sensitivity (%) and get recommended adjustments per weapon.</p>
    <div class="row"><input class="input" id="base" placeholder="Base sensitivity (%)" type="number"><button class="btn" id="calc">Calculate Adjustments</button></div>
    <div id="out" style="margin-top:10px"></div>
  `;
  document.getElementById('calc').addEventListener('click', ()=> {
    const b = parseFloat(document.getElementById('base').value||0);
    if(!b){ alert('Enter a number'); return; }
    const weapons = {AR:0.95,SMG:0.9,SR:1.05,Shotgun:0.9};
    let html = '<ul>';
    for(const w in weapons){ html += `<li><strong>${w}</strong>: ` + (Math.round(b * weapons[w]*100)/100) + '%</li>'; }
    html += '</ul>';
    document.getElementById('out').innerHTML = html;
  });
});

document.getElementById('btn-graph')?.addEventListener('click', ()=> {
  const main = document.getElementById('main');
  document.getElementById('title').innerText = 'Graphics Optimizer';
  main.innerHTML = `
    <h3>Graphics Optimizer</h3>
    <p class="small">Enter your device name for the suggested graphics preset.</p>
    <div class="row"><input class="input" id="device" placeholder="Device (e.g. iPhone 12)"><button class="btn" id="suggest">Suggest Graphics</button></div>
    <div id="gout" style="margin-top:10px"></div>
  `;
  document.getElementById('suggest').addEventListener('click', ()=>{
    const d = document.getElementById('device').value.toLowerCase();
    let preset = 'Balanced';
    if(d.includes('pro')||d.includes('max')||d.includes('samsung')) preset = 'Ultra';
    if(d.includes('mini')|| (d.includes('iphone') && d.includes('se'))) preset = 'Low-Mid';
    document.getElementById('gout').innerHTML = `<div class="card"><strong>Suggested preset:</strong> ${preset}</div>`;
  });
});

document.getElementById('btn-strat')?.addEventListener('click', ()=> {
  const main = document.getElementById('main');
  document.getElementById('title').innerText = 'Pro Strategies';
  main.innerHTML = `<h3>Pro Strategies</h3><ul><li>Climb buildings using diagonal jumps on corners.</li><li>Use TPP camera to peek safely before exposing your body.</li><li>Throw smoke to fake direction, flank from opposite side.</li><li>Use red-dot on close combat; 3x or 4x for mid range.</li><li>Land in low-traffic areas for full loot before engaging.</li></ul>`;
});

document.getElementById('btn-crate')?.addEventListener('click', ()=> {
  const main = document.getElementById('main');
  document.getElementById('title').innerText = 'Crate Luck Tips';
  main.innerHTML = `<h3>Crate Luck Tips</h3><ul><li>Open crates right after major server maintenance for higher odds.</li><li>Open 10 crates at once instead of single pulls.</li><li>Change your avatar frame or title before opening.</li></ul>`;
});

document.getElementById('btn-nick')?.addEventListener('click', ()=> {
  const main = document.getElementById('main');
  document.getElementById('title').innerText = 'Nickname Generator';
  main.innerHTML = `<h3>Nickname Generator</h3><p class="small">Generate PUBG-compatible nicknames with symbols.</p><div class="row"><select id="theme" class="input"><option value="random">Random</option><option value="sniper">Sniper</option></select><select id="style" class="input" style="width:140px"><option value="symbols">Symbols</option><option value="fancy">Fancy</option></select><button class="btn" id="gen">Generate</button></div><div id="res" style="margin-top:10px"></div><div style="margin-top:8px"><button class="btn" id="copy">Copy</button></div>`;
  const symbols = ['★','☆','✦','✧','✪','✯','❖','⚡','🔥'];
  const fancy = {A:'𝔄',B:'𝔅',C:'𝔇',D:'𝔇',E:'𝔈',F:'𝔉',G:'𝔊',H:'ℌ',I:'𝕀',J:'𝔍',K:'𝔎',L:'𝔏',M:'𝔐',N:'𝔑',O:'𝔒',P:'𝔓',Q:'𝔔',R:'ℜ',S:'𝔖',T:'𝔗',U:'𝔘',V:'𝔙',W:'𝔚',X:'𝔛',Y:'𝔜',Z:'ℨ'};
  function rand(a){return a[Math.floor(Math.random()*a.length)];}
  function stylize(w,s){ if(s==='fancy') return w.split('').map(c=> fancy[c.toUpperCase()]||c).join(''); if(s==='symbols') return w + rand(symbols)+rand(symbols); return w; }
  document.getElementById('gen').addEventListener('click', ()=> {
    const t = document.getElementById('theme').value;
    const s = document.getElementById('style').value;
    const parts = {sniper:['Ghost','Viper','Zero','Shade'], random:['Shadow','Nova','Rift','Falcon']};
    const base = parts[t] ? parts[t][Math.floor(Math.random()*parts[t].length)] : parts['random'][Math.floor(Math.random()*4)];
    const num = Math.random()<0.5 ? '' : String(Math.floor(Math.random()*99));
    const name = stylize(base+num, s);
    document.getElementById('res').innerHTML = '<div style="font-size:18px"><strong>'+name+'</strong></div>';
    document.getElementById('copy').onclick = ()=>{ navigator.clipboard.writeText(name).then(()=>alert('Copied: '+name)); };
  });
});
exports.handler = async function(event, context) {
  return { statusCode: 200, body: JSON.stringify({ ok: true, note: 'netlify function placeholder' }) };
};
[build]
  publish = "."
  command = "npm run build"

[[redirects]]
  from = "/*"
  to = "/index.html"
  status = 200
PUBG Coach Pro — PWA final package
Replace firebase keys in js/app.js if you want to enable Cloud sync and login.
Deploy via Netlify (connect to GitHub or use drag-and-drop).

