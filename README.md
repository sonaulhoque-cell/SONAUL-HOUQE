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
