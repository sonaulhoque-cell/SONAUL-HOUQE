/* Basic reset */
* { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }
body { font-family: Arial, Helvetica, sans-serif; color: #172033; line-height: 1.65; background: #fff; }
a { color: inherit; text-decoration: none; }
.container { width: min(1120px, 90%); margin: 0 auto; }

.site-header { position: sticky; top: 0; z-index: 20; background: rgba(255,255,255,.96); border-bottom: 1px solid #e9edf3; }
.navbar { min-height: 76px; display: flex; align-items: center; justify-content: space-between; }
.logo { font-size: 1.35rem; font-weight: 800; letter-spacing: -.5px; }
.logo span { color: #0d9488; }
.nav-links { display: flex; gap: 30px; list-style: none; font-weight: 600; color: #465166; }
.nav-links a:hover, .text-link:hover { color: #0d9488; }
.menu-toggle { display: none; border: 0; background: transparent; font-size: 1.8rem; cursor: pointer; color: #172033; }

.hero { position: relative; width: 100%; overflow: hidden; aspect-ratio: 16 / 9; min-height: 520px; max-height: min(860px, calc(100vh - 76px)); display: flex; align-items: flex-end; color: white; background: linear-gradient(115deg, rgba(10,25,48,.96), rgba(10,90,91,.82)), linear-gradient(45deg, #13243c, #0d9488); }
.eyebrow { color: #0d9488; font-size: .78rem; font-weight: 800; letter-spacing: 2px; margin-bottom: 14px; }
.hero-bg { position: absolute; inset: 0; width: 100%; height: 100%; object-fit: cover; object-position: center 30%; }
.hero-shade { position: absolute; inset: 0; background: radial-gradient(ellipse 70% 85% at 0% 100%, rgba(10,25,48,.92) 0%, rgba(10,25,48,.6) 45%, rgba(10,25,48,0) 100%), linear-gradient(to top, rgba(10,25,48,.75) 0%, rgba(10,25,48,0) 45%); }
.hero-content { position: relative; z-index: 1; padding-top: 60px; padding-bottom: 44px; }
.hero-text { max-width: 560px; }
.hero h1.founder-name { font-family: Georgia, "Times New Roman", serif; font-size: clamp(2.1rem, 4.4vw, 3.6rem); font-weight: 700; letter-spacing: 2px; white-space: nowrap; line-height: 1.08; color: #fff; max-width: none; text-shadow: 0 2px 14px rgba(10,25,48,.55); }
.hero-tagline { color: #8ee2d4; font-weight: 700; font-size: 1.1rem; margin-top: 10px; }
.hero .eyebrow { color: #9ce7dc; text-shadow: 0 1px 8px rgba(10,25,48,.9); }
h1 { font-size: clamp(2.8rem, 7vw, 5.2rem); line-height: 1.06; letter-spacing: -2px; max-width: 750px; }
h1 span { color: #8ee2d4; }
.hero-copy { max-width: 470px; color: #e8eff5; font-size: .98rem; margin: 12px 0 22px; }
.hero-actions { display: flex; gap: 14px; flex-wrap: wrap; }
.btn { display: inline-block; padding: 13px 23px; border-radius: 7px; border: 2px solid transparent; font-weight: 700; font-size: .95rem; cursor: pointer; transition: transform .2s, background .2s; }
.btn:hover { transform: translateY(-2px); }
.btn-primary { background: #0d9488; color: white; }
.btn-primary:hover { background: #08786f; }
.btn-outline { border-color: rgba(255,255,255,.7); color: white; }
.btn-outline:hover { background: white; color: #172033; }

.section { padding: 92px 0; }
h2 { font-size: clamp(2rem, 4vw, 3rem); line-height: 1.15; letter-spacing: -1px; margin-bottom: 18px; }
.two-column { display: grid; grid-template-columns: .85fr 1.15fr; gap: 70px; align-items: start; }
.two-column p { color: #596579; margin-bottom: 17px; }
.lead { font-size: 1.2rem; color: #26364c !important; }
.text-link { color: #0d9488; font-weight: 700; }
.services-section { background: #f5f8fa; }
.section-heading { text-align: center; max-width: 650px; margin: 0 auto 42px; }
.section-heading > p:last-child { color: #687487; }
.service-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 22px; }
.service-card { background: white; border: 1px solid #e7edf1; border-radius: 12px; padding: 30px; box-shadow: 0 10px 30px rgba(23,32,51,.04); }
.service-icon { width: 48px; height: 48px; display: grid; place-items: center; border-radius: 10px; background: #e1f5f1; color: #08786f; font-weight: 800; margin-bottom: 22px; }
.service-card h3 { font-size: 1.25rem; margin-bottom: 10px; }
.service-card p { color: #687487; }

.contact-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 70px; align-items: start; }
.contact-intro > p:not(.eyebrow) { color: #687487; max-width: 440px; }
.contact-details { margin: 26px 0; color: #536075; }
.contact-details p { margin: 8px 0; }
.contact-details a { color: #0d9488; }
.social-links { display: flex; gap: 18px; flex-wrap: wrap; color: #0d9488; font-weight: 700; }
.contact-form { padding: 30px; border: 1px solid #e6ebf0; border-radius: 12px; box-shadow: 0 12px 35px rgba(23,32,51,.06); }
.contact-form label { display: block; font-weight: 700; font-size: .9rem; margin: 14px 0 6px; }
.contact-form input, .contact-form textarea { width: 100%; padding: 12px 13px; border: 1px solid #d8e0e8; border-radius: 6px; font: inherit; color: #172033; background: #fff; }
.contact-form input:focus, .contact-form textarea:focus { outline: 2px solid #9ce7dc; border-color: #0d9488; }
.contact-form textarea { resize: vertical; }
.submit-btn { width: 100%; margin-top: 20px; }
.form-note, .form-status { font-size: .82rem; color: #687487; margin-top: 12px; }
.form-status { color: #08786f; font-weight: 700; }

.site-footer { background: #101d30; color: #cbd5e1; padding: 24px 0; font-size: .9rem; }
.footer-inner { display: flex; justify-content: space-between; gap: 20px; flex-wrap: wrap; }
.footer-inner a { color: #8ee2d4; }
.whatsapp-float { position: fixed; right: 22px; bottom: 22px; z-index: 30; background: #20b95a; color: white; border-radius: 30px; padding: 12px 18px; font-weight: 700; box-shadow: 0 5px 18px rgba(0,0,0,.2); }
.whatsapp-float span { font-size: 1.1rem; margin-right: 5px; }

@media (max-width: 900px) {
  .hero { display: block; aspect-ratio: auto; min-height: 0; max-height: none; }
  .hero-bg { position: relative; display: block; height: auto; object-fit: initial; }
  .hero-shade { background: linear-gradient(to bottom, rgba(10,25,48,0) 0, rgba(10,25,48,0) 38vw, rgba(10,25,48,1) 56.25vw, rgba(10,25,48,1) 100%); }
  .hero-content { margin-top: -15vw; padding-top: 0; padding-bottom: 44px; }
  .hero-text { max-width: 640px; }
  .hero { max-height: none; }
}

@media (max-width: 760px) {
  .menu-toggle { display: block; }
  .nav-links { display: none; position: absolute; top: 76px; left: 0; right: 0; padding: 18px 5%; background: white; border-bottom: 1px solid #e9edf3; flex-direction: column; gap: 14px; }
  .nav-links.open { display: flex; }
  .two-column, .contact-grid { grid-template-columns: 1fr; gap: 32px; }
  .section { padding: 68px 0; }
  .service-grid { grid-template-columns: 1fr; }
  .contact-form { padding: 22px; }
}
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MY BUSINESS PLATFORM</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@700;800&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:'Inter',sans-serif;background:#0A1F44;min-height:100vh;overflow:hidden}
.scene{position:absolute;inset:0;width:100%;height:100%;transition:opacity .8s ease, transform .8s ease}
/* INTRO SCENE */
#intro{
  background:linear-gradient(135deg,#0A1F44 0%, #0F2F5A 25%, #0E7C7B 55%, #14B8A6 75%, #E0F2FF 100%);
  display:flex;align-items:center;justify-content:center;text-align:center;z-index:10;
}
#intro.hide{opacity:0;transform:scale(1.05);pointer-events:none}
.blob{position:absolute;border-radius:50%;background:radial-gradient(circle at 30% 30%, rgba(255,255,255,.9), rgba(255,255,255,.2) 60%);animation:float 10s ease-in-out infinite}
.blob1{width:480px;height:480px;left:-10%;top:5%;opacity:.6}
.blob2{width:380px;height:380px;right:-8%;top:20%;opacity:.5;animation-delay:-3s}
.blob3{width:700px;height:280px;left:20%;bottom:-5%;opacity:.4;filter:blur(25px);animation-delay:-6s}
@keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-20px)}}
.cloud{position:absolute;background:white;border-radius:50px;opacity:.35}
.cloud1{width:140px;height:40px;left:12%;top:18%;animation:drift 40s linear infinite}
.cloud1::before{content:'';position:absolute;width:60px;height:60px;background:white;border-radius:50%;left:20px;top:-20px}
.cloud1::after{content:'';position:absolute;width:70px;height:45px;background:white;border-radius:50%;left:60px;top:-15px}
.cloud2{width:100px;height:30px;right:18%;top:68%;opacity:.25;animation:drift 55s linear infinite reverse}
.cloud2::before{content:'';position:absolute;width:45px;height:45px;background:white;border-radius:50%;left:15px;top:-15px}
.cloud2::after{content:'';position:absolute;width:55px;height:35px;background:white;border-radius:50%;left:45px;top:-10px}
@keyframes drift{from{transform:translateX(0)}to{transform:translateX(15vw)}}
.intro-center{position:relative;z-index:2;padding:20px;perspective:1400px}
.welcome{font-size:13px;letter-spacing:.45em;color:rgba(255,255,255,.95);text-transform:uppercase;margin-bottom:20px;opacity:0;animation:fadeUp 1s ease .2s forwards}
.line{font-family:'Syne',sans-serif;color:white;text-shadow:0 10px 30px rgba(0,60,120,.25);display:flex;justify-content:center;line-height:.92}
.line-welcome{font-size:clamp(2.2rem,6vw,4rem);font-weight:800;letter-spacing:.02em}
.line-business{font-size:clamp(2.8rem,8.5vw,6rem);font-weight:800;letter-spacing:-.01em;margin-top:6px}
.line-platform{font-size:clamp(2.8rem,8.5vw,6rem);font-weight:800;letter-spacing:.06em}
.letter{display:inline-block;opacity:0;transform:translateZ(-2500px) scale(.1) translateY(80px);filter:blur(20px);animation:letterIn 1.1s cubic-bezier(.16,1,.3,1) forwards}
@keyframes letterIn{0%{opacity:0;transform:translateZ(-2500px) scale(.1) translateY(80px);filter:blur(25px)}40%{opacity:.6;filter:blur(8px)}100%{opacity:1;transform:translateZ(0) scale(1) translateY(0);filter:blur(0)}}
@keyframes fadeUp{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:translateY(0)}}
.progress-wrap{width:200px;height:4px;background:rgba(255,255,255,.35);border-radius:100px;margin:35px auto 0;overflow:hidden;opacity:0;animation:fadeUp .8s ease .8s forwards}
.progress{height:100%;width:0%;background:white;border-radius:100px;animation:load 4s linear forwards}
@keyframes load{from{width:0%}to{width:100%}}
.loading-text{margin-top:12px;font-size:11px;letter-spacing:.2em;text-transform:uppercase;color:rgba(255,255,255,.7);opacity:0;animation:fadeUp .8s ease 1s forwards}
.skip{margin-top:20px;background:rgba(255,255,255,.15);border:1px solid rgba(255,255,255,.6);color:white;padding:8px 18px;border-radius:100px;font-size:12px;cursor:pointer}
/* LOGIN SCENE */
#login{
  background:linear-gradient(135deg,#0A1F44 0%, #0F2F5A 30%, #0E7C7B 60%, #14B8A6 85%, #E0F2FF 100%);
  display:flex;align-items:center;justify-content:center;padding:20px;
  opacity:0;transform:translateY(20px);pointer-events:none;z-index:5;
}
#login.show{opacity:1;transform:translateY(0);pointer-events:auto}
.login-card{
  width:100%;max-width:400px;background:white;border-radius:24px;padding:32px 28px;
  box-shadow:0 20px 60px rgba(10,31,68,.35);
  text-align:center;
}
.login-logo{width:56px;height:56px;background:#E0F2FF;border-radius:16px;display:flex;align-items:center;justify-content:center;font-size:26px;margin:0 auto 12px}
.login-card h2{font-family:'Syne',sans-serif;font-size:24px;color:#0F2A44;line-height:1.1}
.login-card p{font-size:13px;color:#6A829A;margin:8px 0 22px;line-height:1.5}
.field{text-align:left;margin-bottom:14px}
.field label{font-size:12px;font-weight:600;color:#33475F;letter-spacing:.02em;display:block;margin-bottom:6px}
.field input{
  width:100%;padding:13px 14px;border:1.5px solid #DCE8F5;border-radius:12px;
  font-size:14px;outline:none;background:#F8FBFF;color:#0F2A44;transition:.2s;
}
.field input:focus{border-color:#0E7C7B;background:white;box-shadow:0 0 0 4px rgba(20,184,166,.15)}
.row{display:flex;justify-content:space-between;align-items:center;font-size:12px;margin:4px 0 18px}
.row a{color:#0E7C7B;text-decoration:none;font-weight:600}
.check{display:flex;gap:6px;align-items:center;color:#6A829A}
.login-btn{
  width:100%;padding:14px;border:none;border-radius:12px;background:#0A1F44;color:white;
  font-size:14px;font-weight:700;cursor:pointer;box-shadow:0 8px 20px rgba(10,31,68,.35);
}
.login-btn:active{transform:scale(.98)}
.divider{display:flex;align-items:center;gap:12px;margin:20px 0;color:#8AA0B5;font-size:11px;letter-spacing:.08em;text-transform:uppercase}
.divider::before,.divider::after{content:'';flex:1;height:1px;background:#E2EAF3}
.social{display:flex;flex-direction:column;gap:10px}
.social button{
  width:100%;padding:12px;border:1.5px solid #E2EAF3;background:white;border-radius:12px;
  display:flex;align-items:center;justify-content:center;gap:10px;font-size:13.5px;font-weight:600;color:#1A2B3D;cursor:pointer;
}
.social button:hover{border-color:#C5D9EF;background:#F8FBFF}
.g-icon{width:18px;height:18px;background:conic-gradient(from 0deg,#EA4335 0 25%,#4285F4 0 50%,#34A853 0 75%,#FBBC05 0 100%);border-radius:50%;display:inline-block}
.fb-icon{width:18px;height:18px;background:#1877F2;color:white;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:800}
.signup{margin-top:18px;font-size:12.5px;color:#6A829A}
.signup a{color:#0E7C7B;font-weight:700;text-decoration:none}
.back{margin-top:14px;background:none;border:none;color:#8AA0B5;font-size:12px;cursor:pointer;text-decoration:underline}
@media(max-width:480px){.login-card{padding:26px 20px}}

.logo-top{display:flex;flex-direction:column;align-items:center;margin-bottom:14px}
.logo-top img{width:220px;max-width:85%;background:white;padding:10px 14px;border-radius:14px;box-shadow:0 8px 25px rgba(0,0,0,.12);object-fit:contain}
</style>
</head>
<body>

<!-- SCENE 1: INTRO -->
<div id="intro" class="scene">
  <div class="blob blob1"></div><div class="blob blob2"></div><div class="blob blob3"></div>
  <div class="cloud cloud1"></div><div class="cloud cloud2"></div>
  <div class="intro-center">
    <div class="welcome">WELCOME TO</div>
    <div class="line line-welcome" id="line-welcome"></div>
    <div class="line line-business" id="line-business"></div>
    <div class="line line-platform" id="line-platform"></div>
    <div class="progress-wrap"><div class="progress"></div></div>
    <div class="loading-text">Loading your business platform...</div>
    <button class="skip" onclick="goLogin()">Skip Intro →</button>
  </div>
</div>

<!-- SCENE 2: LOGIN -->
<div id="login" class="scene">
  <div class="login-card">
    <div class="logo-top"><img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/4gHYSUNDX1BST0ZJTEUAAQEAAAHIbGNtcwIQAABtbnRyUkdCIFhZWiAH4gADABQACQAOAB1hY3NwTVNGVAAAAABzYXdzY3RybAAAAAAAAAAAAAAAAAAA9tYAAQAAAADTLWhhbmSdkQA9QICwPUB0LIGepSKOAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAlkZXNjAAAA8AAAABxjcHJ0AAABDAAAAAx3dHB0AAABGAAAABRyWFlaAAABLAAAABRnWFlaAAABQAAAABRiWFlaAAABVAAAABRyVFJDAAABaAAAAGBnVFJDAAABaAAAAGBiVFJDAAABaAAAAGBkZXNjAAAAAAAAAAV1UkdCAAAAAAAAAAAAAAAAdGV4dAAAAABDQzAAWFlaIAAAAAAAAPNUAAEAAAABFslYWVogAAAAAAAAb6AAADjyAAADj1hZWiAAAAAAAABilgAAt4kAABjaWFlaIAAAAAAAACSgAAAPhQAAtsRjdXJ2AAAAAAAAACoAAAB8APgBnAJ1A4MEyQZOCBIKGAxiDvQRzxT2GGocLiBDJKwpai5+M+s5sz/WRldNNlR2XBdkHWyGdVZ+jYgskjacq6eMstu+mcrH12Xkd/H5////2wBDAAMCAgMCAgMDAwMEAwMEBQgFBQQEBQoHBwYIDAoMDAsKCwsNDhIQDQ4RDgsLEBYQERMUFRUVDA8XGBYUGBIUFRT/2wBDAQMEBAUEBQkFBQkUDQsNFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBT/wAARCACRAuEDASIAAhEBAxEB/8QAHgABAAICAwEBAQAAAAAAAAAAAAYHBQgDBAkBAgr/xABXEAABAwQBAgMFAwUICw0JAAABAAIDBAUGEQcSIRMxQQgUIlFhFXGBCRYjMpEXNkJidZOhshgZNzhSVFV0sbPTJTNWV3JzdpKUtNHU8CQ0Q4KDlaKlwf/EABwBAQEAAgMBAQAAAAAAAAAAAAABBAUCAwYHCP/EADQRAAIBBAECAwUHAwUAAAAAAAABAgMEBREhEjEGQVETFGFxgRUiMpGhsfEH0fAzNEJSkv/aAAwDAQACEQMRAD8A9U0REAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBVrz/wA/4v7OGBuyrKnVMlK+dtLT0lExr56iZwc4MYHOaPJriSSAAFZS86vyxGRiDGeNbCCSaqsrK5wHkPCZExu/v8Z37CsihTVWooM6a03Tg5IlP9t64x/4IZb/ADVL/tly0n5XXiyaqhjmxbLKeF7w18xgpnBgJ7uIE2zrz7LyWVp+y9xK7m7nnD8SdE6Sgqqxs1foEhtLEDJNsjy2xpaD83BbuVlQjFyfkamN1Vk0ke+ltuNPd7dS11JJ4tLVRNnikAI6mOALT3+YIXZX4iiZDG2ONoYxgDWtaNAAeQAX7XnDeBEVc88884t7O2A1GVZVUPbTteIaajpwHVFZMQSI42kgE6BJJIAAJKqTk9IjaitssXa+ryXzj8rbyVdbpIcXx2wWC2AkRx1kclZUEb7Fz+pjfLXYM+fcrO8WfldMqo7xFDyFilsudpe4NfVWIPp6mEeruh73tk/5O2fes52NZLejEV3Sb1s9S0UPxrlCxcgcaDNMSuMF4tM9HJU01Q3fSS1p217exaQ4EOadEEEdloB7PX5S/k/lnmzD8Pu9ixKmtl4r20tRLRUdUyZrSCdsLqlwB7eoKx4UJzTaXbud0q0INJ+Z6XoiLoO4Ii6N8rZLbZq6riDXSQQvkaHjYJDSRtdc5qnFzl2RyinJqK8zvItav7JHKP8AE7X/ADMn+0T+yRyf/E7X/Myf7RfO3/UDBp66pf8Alnql4YyT/wCK/NGyqKmOLuZb3mmVx2yvp6GOndE95dBG9rtjy7l5H9CudevxWWtczQ95tG3HeuVo0V7Y1rCr7GutPW/UIiLcmAEREAREQHxfUWOyK8Mx+x11ykjdKylhdMWNOi4Ab0F11KkaUHUm9Jcs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
