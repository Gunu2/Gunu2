<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>M Gunawan — Lecturer · AI · Engineer</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;600;800&family=Orbitron:wght@600;800&display=swap" rel="stylesheet">
<style>
:root{--bg:#070b12;--panel:#0d1522;--line:#1c2b40;--text:#d6e4f5;--muted:#7f95b1;--cyan:#22d3ee;--teal:#0c7c8a;--amber:#fbbf24;--green:#34d399;color-scheme:dark;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:light){:root:not([data-theme="dark"]){--bg:#eef5fa;--panel:#ffffff;--line:#c5d5e4;--text:#10243a;--muted:#4b6580;--cyan:#0a7f93;--teal:#0c7c8a;--amber:#a16207;--green:#047857;color-scheme:light}}
:root[data-theme="light"]{--bg:#eef5fa;--panel:#ffffff;--line:#c5d5e4;--text:#10243a;--muted:#4b6580;--cyan:#0a7f93;--amber:#a16207;--green:#047857;color-scheme:light}
*,*::before,*::after{box-sizing:border-box}
html{scroll-behavior:smooth;scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--text);font:15px/1.65 "JetBrains Mono",ui-monospace,Consolas,monospace;overflow-x:hidden}
#bg{position:fixed;inset:0;width:100%;height:100%;z-index:0}
body::after{content:"";position:fixed;inset:0;pointer-events:none;z-index:5;background:repeating-linear-gradient(0deg,transparent 0 2px,rgba(34,211,238,.035) 2px 3px);animation:scan 8s linear infinite}
@keyframes scan{to{background-position:0 60px}}
main{position:relative;z-index:2;max-width:980px;margin:0 auto;padding:0 20px 80px}
section{padding:56px 0 0}
h2{font:800 14px "Orbitron",sans-serif;letter-spacing:.2em;color:var(--cyan);text-transform:uppercase;margin:0 0 22px}
h2::before{content:"> ";color:var(--amber)}
.hero{min-height:92vh;display:flex;flex-direction:column;justify-content:center;gap:18px}
.badge{display:inline-flex;gap:8px;align-items:center;font-size:12px;color:var(--green);border:1px solid var(--green);padding:4px 12px;border-radius:99px;width:max-content;background:color-mix(in srgb,var(--green) 10%,transparent)}
.dot{width:8px;height:8px;border-radius:50%;background:var(--green);animation:pulse 1.4s infinite}
@keyframes pulse{0%{box-shadow:0 0 0 0 var(--green)}100%{box-shadow:0 0 0 10px transparent}}
.name{font:800 clamp(38px,9vw,84px)/1.05 "Orbitron",sans-serif;margin:0;color:var(--cyan);position:relative;text-shadow:0 0 24px color-mix(in srgb,var(--cyan) 55%,transparent);animation:glitch 6s infinite}
.name::before,.name::after{content:attr(data-t);position:absolute;inset:0;opacity:.0}
.name::before{color:var(--amber);animation:g1 6s infinite}
.name::after{color:#f43f5e;animation:g2 6s infinite}
@keyframes g1{0%,92%,100%{opacity:0;transform:none}93%{opacity:.8;transform:translate(-4px,1px);clip-path:inset(10% 0 55% 0)}96%{opacity:.8;transform:translate(3px,-1px);clip-path:inset(60% 0 8% 0)}}
@keyframes g2{0%,92%,100%{opacity:0;transform:none}94%{opacity:.7;transform:translate(4px,-1px);clip-path:inset(40% 0 30% 0)}97%{opacity:.7;transform:translate(-3px,1px);clip-path:inset(5% 0 70% 0)}}
.type{font-size:clamp(15px,2.6vw,21px);min-height:1.8em;color:var(--text)}
.type::after{content:"▌";color:var(--cyan);animation:blink 1s steps(1) infinite}
@keyframes blink{50%{opacity:0}}
.chips{display:flex;flex-wrap:wrap;gap:8px}
.chip{font-size:12px;padding:4px 11px;border:1px solid var(--line);background:var(--panel);border-radius:6px;color:var(--muted);transition:.25s}
.chip:hover{color:var(--cyan);border-color:var(--cyan);transform:translateY(-3px);box-shadow:0 6px 18px -6px var(--cyan)}
.cta{display:flex;gap:12px;flex-wrap:wrap;margin-top:8px}
.btn{color:var(--bg);background:var(--cyan);padding:10px 20px;border-radius:6px;text-decoration:none;font-weight:600;font-size:13px;transition:.25s;position:relative;overflow:hidden}
.btn.alt{background:transparent;color:var(--cyan);border:1px solid var(--cyan)}
.btn:hover{transform:translateY(-3px);box-shadow:0 10px 26px -8px var(--cyan)}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:14px}
.card{background:var(--panel);border:1px solid var(--line);border-radius:10px;padding:20px;position:relative;overflow:hidden;transition:.3s}
.card::before{content:"";position:absolute;top:0;left:-100%;width:60%;height:2px;background:linear-gradient(90deg,transparent,var(--cyan),transparent);animation:sweep 3.5s infinite}
@keyframes sweep{to{left:140%}}
.card:hover{border-color:var(--cyan);transform:translateY(-4px)}
.num{font:800 34px "Orbitron",sans-serif;color:var(--amber)}
.lbl{font-size:12px;color:var(--muted)}
.skills{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:14px}
.skills h3{margin:0 0 12px;font-size:13px;color:var(--text)}
.tl{position:relative;padding-left:26px;border-left:1px dashed var(--line)}
.tl details{position:relative;margin:0 0 14px;background:var(--panel);border:1px solid var(--line);border-radius:8px;padding:12px 16px;transition:.25s}
.tl details::before{content:"";position:absolute;left:-33px;top:18px;width:11px;height:11px;border-radius:50%;background:var(--bg);border:2px solid var(--cyan)}
.tl details[open]{border-color:var(--cyan)}
.tl details[open]::before{background:var(--cyan);box-shadow:0 0 12px var(--cyan)}
summary{cursor:pointer;list-style:none;font-size:13px}
summary::-webkit-details-marker{display:none}
summary b{color:var(--amber)}
.tl ul{margin:10px 0 2px;padding-left:18px;color:var(--muted);font-size:13px}
.tl li{margin:3px 0}
.term{background:var(--panel);border:1px solid var(--line);border-radius:10px;padding:18px 20px;font-size:13px;white-space:pre-wrap;overflow-x:auto}
.term .k{color:var(--cyan)}.term .v{color:var(--text)}
.rv{opacity:0;transform:translateY(28px);transition:opacity .8s,transform .8s}
.rv.in{opacity:1;transform:none}
footer{text-align:center;color:var(--muted);font-size:12px;padding:40px 0 10px}
@media (prefers-reduced-motion:reduce){*,*::before,*::after{animation:none!important;transition:none!important}.rv{opacity:1;transform:none}}
</style>
</head>
<body>
<canvas id="bg" aria-hidden="true"></canvas>
<main>
<header class="hero">
  <span class="badge"><i class="dot"></i>SYSTEM ONLINE · AVAILABLE</span>
  <h1 class="name" data-t="M GUNAWAN">M GUNAWAN</h1>
  <div class="type" id="type" aria-live="polite"></div>
  <div class="chips"><span class="chip">7+ years</span><span class="chip">Indonesia · remote</span><span class="chip">English (fluent)</span><span class="chip">German (B1)</span><span class="chip">Indonesian · Acehnese (native)</span></div>
  <div class="cta">
    <a class="btn" href="mailto:gunawn94@gmail.com">Email me</a>
    <a class="btn alt" href="https://linkedin.com/in/m-gunawan-174101144" target="_blank" rel="noopener">LinkedIn</a>
    <a class="btn alt" href="https://github.com/Gunu2" target="_blank" rel="noopener">GitHub</a>
  </div>
</header>

<section class="rv"><h2>unit.status</h2>
<div class="term"><span class="k">UNIT        </span>: <span class="v">M GUNAWAN</span>
<span class="k">ROLE        </span>: <span class="v">Lecturer (IoT &amp; Image Processing) / AI Data Trainer / Maintenance Planner</span>
<span class="k">EXPERIENCE  </span>: <span class="v">7+ years, industrial manufacturing, utilities, AI &amp; academia</span>
<span class="k">DEPLOYMENT  </span>: <span class="v">any project site / remote</span>
<span class="k">STATUS      </span>: <span class="v" style="color:var(--green)">AVAILABLE</span></div>
<p style="color:var(--muted);margin-top:18px">University lecturer in Image Processing and Embedded Systems/IoT, AI Data Trainer &amp; Quality Rater, and Maintenance Planner / Electrical Technician. I bridge industrial engineering with AI and computer vision, teach applied IoT and image processing, train AI models, and build practical tools that make teams faster.</p></section>

<section class="rv"><h2>impact.log</h2>
<div class="grid">
  <div class="card"><div class="num"><span data-c="5" data-pre="-" data-suf="%">0</span></div><div class="lbl">Annual energy consumption, through power quality analysis</div></div>
  <div class="card"><div class="num"><span data-c="16" data-suf=" KL">0</span></div><div class="lbl">Boiler fuel saved every two months</div></div>
  <div class="card"><div class="num"><span data-c="80" data-pre="~" data-suf=" t">0</span></div><div class="lbl">CO₂ per year targeted by optimization initiatives</div></div>
  <div class="card"><div class="num"><span data-c="7" data-suf="+ yrs">0</span></div><div class="lbl">Industry, utilities, AI and academia</div></div>
</div></section>

<section class="rv"><h2>modules.loaded</h2>
<div class="skills">
  <div class="card"><h3>AI, Computer Vision &amp; IoT</h3><div class="chips"><span class="chip">Image Processing</span><span class="chip">Embedded Systems &amp; IoT</span><span class="chip">AI Data Training</span><span class="chip">Video &amp; Image Annotation</span><span class="chip">Quality Rating</span></div></div>
  <div class="card"><h3>Planning &amp; coordination</h3><div class="chips"><span class="chip">Maintenance Planning</span><span class="chip">Scheduling</span><span class="chip">Progress Reporting</span><span class="chip">Vendor Coordination</span></div></div>
  <div class="card"><h3>Electrical &amp; utilities</h3><div class="chips"><span class="chip">LV/MV Panels</span><span class="chip">Boiler</span><span class="chip">Compressor</span><span class="chip">Piping &amp; Tanks</span><span class="chip">Power Quality</span></div></div>
  <div class="card"><h3>Reliability &amp; safety</h3><div class="chips"><span class="chip">Preventive Maintenance</span><span class="chip">Predictive Maintenance</span><span class="chip">Root Cause Analysis</span><span class="chip">Fire Protection</span></div></div>
  <div class="card"><h3>Documentation &amp; tools</h3><div class="chips"><span class="chip">SOP Development</span><span class="chip">Technical Documentation</span><span class="chip">No-code Chatbot</span></div></div>
</div></section>

<section class="rv"><h2>mission.log</h2>
<div class="tl">
<details open><summary><b>2026 – present</b> · Lecturer (Image Processing &amp; Embedded Systems / IoT), Almuslim University</summary><ul><li>Teaching undergraduate courses in Image Processing and Embedded Systems &amp; IoT</li><li>Designing hands-on laboratory practicums, simulations, and applied deep learning / IoT projects</li></ul></details>
<details open><summary><b>2025 – present</b> · AI Data Trainer, Data Annotator &amp; Quality Rater (Mercor, CrowdGen, OneForma, Freelancer)</summary><ul><li>Generalist and specialist AI data trainer for model evaluation, prompt/response grading, and RLHF workflows</li><li>Video and image annotation for computer vision and multimodal AI datasets</li><li>Quality rating and guideline compliance auditing across international AI projects</li></ul></details>
<details><summary><b>2024 – present</b> · Maintenance Planner / Technical Consultation, PT Juang Aceh Teknologi</summary><ul><li>Administrative and engineering technical support, including international clients</li><li>Communication, scheduling and documentation tasks; customer inquiries</li></ul></details>
<details><summary><b>Mar – May 2024</b> · Procurement, Idemitsu Lube Techno Indonesia (Karawang)</summary><ul><li>Managed supplier documentation and purchase records; analysed procurement data for planning</li><li>Prepared reports and communicated with vendors and internal teams</li></ul></details>
<details><summary><b>2019 – 2024</b> · Maintenance Planner, Idemitsu Lube Techno Indonesia (Cikarang)</summary><ul><li>Planned and executed preventive and predictive maintenance for industrial systems and utilities</li><li>Reduced breakdowns through schedule optimization and autonomous maintenance</li><li>Cut annual energy use by 5% and boiler fuel by 16 KL every two months</li><li>Supervised safety improvements; managed hydrants, alarms, sprinklers and extinguishers</li><li>Built an internal engineering documentation tool (no-code chatbot)</li></ul></details>
<details><summary><b>Jan – Jun 2018</b> · Project Superintendent, Delta-I Second Plant Project</summary><ul><li>Supervised installation of tanks, piping and static equipment</li><li>Coordinated utility installation (boilers, compressors); oversaw LV/MV panel installation and commissioning</li><li>Wrote operational SOPs for maintenance systems</li></ul></details>
<details><summary><b>Aug 2017 – Jan 2018</b> · Production Operator, Idemitsu Lube Techno Indonesia (Karawang)</summary><ul><li>Lubricant filling, packaging and blending per SOP; quality and process monitoring</li></ul></details>
</div></section>

<section class="rv"><h2>education.db</h2>
<div class="grid">
  <div class="card"><div class="lbl">2023 – 2025</div><b>MSc, Information Technology</b><div class="lbl">President University</div></div>
  <div class="card"><div class="lbl">2019 – 2021</div><b>B.Eng, Electrical Power Systems</b><div class="lbl">University of Jaya Baya, Jakarta</div></div>
</div></section>

<section class="rv"><h2>open.channel</h2>
<div class="cta"><a class="btn" href="mailto:gunawn94@gmail.com">gunawn94@gmail.com</a><a class="btn alt" href="https://linkedin.com/in/m-gunawan-174101144" target="_blank" rel="noopener">linkedin.com/in/m-gunawan</a></div></section>
<footer>© M Gunawan · built with ⚡ and caffeine</footer>
</main>
<script>
(function(){
var reduce=matchMedia("(prefers-reduced-motion: reduce)").matches;
// typing
var roles=["> initializing profile…","Lecturer | Image Processing & IoT","AI Data Trainer & Quality Rater","Maintenance Planner & Electrical Technician","Reliability & Energy Efficiency"];
var el=document.getElementById("type"),ri=0,ci=0,del=false;
function tick(){var s=roles[ri];
 if(reduce){el.textContent=roles[1];return}
 el.textContent=s.slice(0,ci);
 if(!del&&ci<s.length){ci++;setTimeout(tick,55)}
 else if(!del){del=true;setTimeout(tick,1300)}
 else if(ci>0){ci--;setTimeout(tick,25)}
 else{del=false;ri=(ri+1)%roles.length;setTimeout(tick,300)}}
tick();
// reveal + counters
function count(n){var t=+n.dataset.c,pre=n.dataset.pre||"",suf=n.dataset.suf||"",s=null;
 function f(ts){if(!s)s=ts;var k=Math.min((ts-s)/1400,1);n.textContent=pre+Math.round(t*(1-Math.pow(1-k,3)))+suf;if(k<1)requestAnimationFrame(f)}
 if(reduce){n.textContent=pre+t+suf}else requestAnimationFrame(f)}
var io=new IntersectionObserver(function(es){es.forEach(function(e){if(e.isIntersecting){e.target.classList.add("in");e.target.querySelectorAll("[data-c]").forEach(count);io.unobserve(e.target)}})},{threshold:.15});
document.querySelectorAll(".rv").forEach(function(x){io.observe(x)});
// network canvas
var c=document.getElementById("bg"),x=c.getContext("2d"),W,H,P=[],m={x:-999,y:-999};
function rs(){W=c.width=innerWidth;H=c.height=innerHeight;P=[];var n=Math.min(90,Math.floor(W*H/16000));for(var i=0;i<n;i++)P.push({x:Math.random()*W,y:Math.random()*H,vx:(Math.random()-.5)*.4,vy:(Math.random()-.5)*.4})}
addEventListener("resize",rs);rs();
addEventListener("pointermove",function(e){m.x=e.clientX;m.y=e.clientY});
function col(){return getComputedStyle(document.documentElement).getPropertyValue("--cyan").trim()||"#22d3ee"}
var cc=col();matchMedia("(prefers-color-scheme: light)").addEventListener("change",function(){cc=col()});
function draw(){x.clearRect(0,0,W,H);x.fillStyle=cc;x.strokeStyle=cc;
 for(var i=0;i<P.length;i++){var a=P[i];a.x+=a.vx;a.y+=a.vy;if(a.x<0||a.x>W)a.vx*=-1;if(a.y<0||a.y>H)a.vy*=-1;
  x.globalAlpha=.7;x.beginPath();x.arc(a.x,a.y,1.6,0,6.3);x.fill();
  for(var j=i+1;j<P.length;j++){var b=P[j],d=Math.hypot(a.x-b.x,a.y-b.y);if(d<130){x.globalAlpha=(1-d/130)*.35;x.beginPath();x.moveTo(a.x,a.y);x.lineTo(b.x,b.y);x.stroke()}}
  var dm=Math.hypot(a.x-m.x,a.y-m.y);if(dm<170){x.globalAlpha=(1-dm/170)*.7;x.beginPath();x.moveTo(a.x,a.y);x.lineTo(m.x,m.y);x.stroke()}}
 x.globalAlpha=1;if(!reduce)requestAnimationFrame(draw)}
draw();
})();
</script>
</body>
</html>
