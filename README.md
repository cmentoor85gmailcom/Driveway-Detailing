<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Driveway Detailing — Mobile Car Wash</title>
  <meta name="description" content="Driveway Detailing - Mobile car wash & detailing. Professional packages, add-ons, and mobile service.">
  <style>
    :root{
      --bg:#0b0b0b;
      --muted:#9aa0a6;
      --accent:#00c853;
      --card:#0f0f0f;
      --glass: rgba(255,255,255,0.03);
      --container: 1100px;
      --radius:8px;
      --shadow: 0 6px 20px rgba(0,0,0,0.6);
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0;background:var(--bg);color:#e9ecef;line-height:1.45}
    .container{max-width:var(--container);margin:0 auto;padding:24px}
    .site-header{position:sticky;top:0;background:linear-gradient(180deg, rgba(0,0,0,0.6), rgba(0,0,0,0.9));z-index:40;border-bottom:1px solid rgba(255,255,255,0.03)}
    .header-inner{display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:64px;height:64px;object-fit:contain}
    .brand-text h1{margin:0;font-size:18px;letter-spacing:1px}
    .sub{margin:0;color:var(--muted);font-size:12px}
    .main-nav a{color:#fff;margin:0 10px;text-decoration:none;font-weight:600;font-size:14px}
    .main-nav a:hover{text-decoration:underline}
    .contact-quick .btn-whatsapp{background:var(--accent);color:#000;padding:8px 12px;border-radius:6px;text-decoration:none;font-weight:700}
    .hero{background-image: url('assets/hero-bg.jpg'); background-size:cover;background-position:center;height:420px;display:flex;align-items:center;justify-content:center;position:relative}
    .hero-overlay{background:linear-gradient(180deg, rgba(0,0,0,0.6), rgba(0,0,0,0.6));width:100%;height:100%;display:flex;align-items:center}
    .hero-content{padding:40px;color:#fff;text-align:center}
    .hero h2{font-size:36px;margin:0 0 12px;color:var(--accent);letter-spacing:1px}
    .lead{color:var(--muted);max-width:720px;margin:0 auto 18px}
    .cta-row{display:flex;gap:12px;justify-content:center}
    .btn-primary{background:var(--accent);color:#000;padding:12px 18px;border-radius:8px;text-decoration:none;font-weight:700}
    .btn-outline{background:transparent;color:#fff;padding:12px 18px;border-radius:8px;border:1px solid rgba(255,255,255,0.07);text-decoration:none}
    .section{padding:54px 0}
    .section-title{font-size:22px;margin-bottom:6px;color:#fff}
    .section-sub{color:var(--muted);margin-bottom:18px}
    .cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:20px;margin-top:18px}
    .card{background:var(--card);border-radius:10px;overflow:hidden;box-shadow:var(--shadow);display:flex;flex-direction:column}
    .card img{width:100%;height:180px;object-fit:cover;display:block}
    .card-body{padding:18px;flex:1;display:flex;flex-direction:column}
    .pkg-title{margin:0 0 8px;color:var(--accent);font-weight:800}
    .pkg-list{list-style:none;padding:0;margin:0 0 14px;color:var(--muted)}
    .pkg-list li{padding:6px 0;border-bottom:1px dashed rgba(255,255,255,0.02)}
    .card-foot{margin-top:auto}
    .select-pkg{background:transparent;border:2px solid var(--accent);color:var(--accent);padding:10px 14px;border-radius:6px;cursor:pointer;font-weight:800}
    .note{margin-top:18px;color:var(--muted);background:var(--glass);padding:12px;border-radius:8px;border:1px solid rgba(255,255,255,0.02)}
    .work-grid{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:start}
    .panel{background:var(--card);padding:16px;border-radius:10px;box-shadow:var(--shadow);margin-bottom:16px}
    .selected-box{padding:12px;background:rgba(255,255,255,0.02);border-radius:6px;color:var(--muted)}
    .addons-list label{display:block;padding:8px 6px;border-bottom:1px solid rgba(255,255,255,0.02);cursor:pointer}
    .summary{padding:10px;background:rgba(0,0,0,0.35);border-radius:6px}
    .summary .total{margin-top:8px;font-size:18px;color:var(--accent);font-weight:800}
    .booking-actions{display:flex;gap:10px;margin-top:10px}
    .work-right .booking-form label{display:block;color:var(--muted);margin-bottom:8px}
    .booking-form input, .booking-form textarea{width:100%;padding:10px;margin-top:6px;border-radius:6px;border:1px solid rgba(255,255,255,0.06);background:transparent;color:#fff}
    .form-row{display:flex;gap:8px;margin-top:10px}
    .gallery-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:10px}
    .gallery-grid img{width:100%;height:160px;object-fit:cover;border-radius:6px;box-shadow:var(--shadow)}
    .location-inner{display:grid;grid-template-columns:1fr 420px;gap:24px;align-items:center}
    .loc-right iframe{width:100%;height:260px;border-radius:8px;border:0;box-shadow:var(--shadow)}
    .site-footer{background:#050505;color:var(--muted);padding:28px 0;border-top:1px solid rgba(255,255,255,0.03)}
    .footer-inner{display:flex;justify-content:space-between;gap:24px;align-items:flex-start}
    .footer-bottom{background:#020202;padding:12px 0;margin-top:18px}
    .small{font-size:12px;color:var(--muted)}
    @media (max-width:980px){
      .work-grid{grid-template-columns:1fr}
      .location-inner{grid-template-columns:1fr}
      .header-inner{flex-direction:column;gap:10px;align-items:flex-start}
      .main-nav{display:none}
    }
  </style>
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <div class="brand">
        <img src="assets/logo.png" alt="Driveway Detailing logo" class="logo"/>
        <div class="brand-text">
          <h1>Driveway Detailing</h1>
          <p class="sub">Mobile Car Wash • Detailing est 2024</p>
        </div>
      </div>
      <nav class="main-nav">
        <a href="#packages">Packages</a>
        <a href="#work">Book</a>
        <a href="#gallery">Gallery</a>
        <a href="#contact">Contact</a>
        <a href="#location">Location</a>
      </nav>
      <div class="contact-quick">
        <a class="btn-whatsapp" href="https://wa.me/27660642112" target="_blank">WhatsApp</a>
      </div>
    </div>
  </header>

  <section class="hero">
    <div class="hero-overlay">
      <div class="container hero-content">
        <h2>Professional Mobile Car Detailing</h2>
        <p class="lead">Detailing with purpose: serving you with grace. We come to you — full exterior wash, interior detailing, paint protection & more.</p>
        <div class="cta-row">
          <a href="#work" class="btn-primary">Book Now</a>
          <a href="#packages" class="btn-outline">See Packages</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Packages -->
  <section id="packages" class="section">
    <div class="container">
      <h3 class="section-title">Packages Available</h3>
      <p class="section-sub">Choose a package that suits your car — add-ons at R100 each.</p>
      <div class="cards">
        <article class="card">
          <img src="assets/pkg-exterior.jpg" alt="The Ark">
          <div class="card-body">
            <h4 class="pkg-title">THE ARK — R250</h4>
            <ul class="pkg-list">
              <li>Basic exterior wash</li><li>Interior vacuuming</li><li>Window cleaning</li><li>Paint protection</li><li>Tire shine</li>
            </ul>
            <div class="card-foot"><button class="select-pkg" data-name="The Ark" data-price="250">Select</button></div>
          </div>
        </article>
        <article class="card">
          <img src="assets/pkg-full.jpg" alt="The Mountain Top">
          <div class="card-body">
            <h4 class="pkg-title">THE MOUNTAIN TOP — R300</h4>
            <ul class="pkg-list">
              <li>Complete wash</li><li>Full interior detailing</li><li>Tire shine & leather conditioning</li><li>Paint/wax protection</li>
            </ul>
            <div class="card-foot"><button class="select-pkg" data-name="The Mountain Top" data-price="300">Select</button></div>
          </div>
        </article>
        <article class="card">
          <img src="assets/pkg-engine.jpg" alt="Engine detailing">
          <div class="card-body">
            <h4 class="pkg-title">ENGINE DETAILING — R150</h4>
            <ul class="pkg-list">
              <li>Removes dirt & grease</li><li>Enhances performance & aesthetics</li>
            </ul>
            <div class="card-foot"><button class="select-pkg" data-name="Engine Detailing" data-price="150">Select</button></div>
          </div>
        </article>
      </div>
      <div class="note"><strong>Detailing add-ons</strong> at <strong>R100 per add-on</strong> — Pet hair & odour removal, Subscription packages, Express steam cleaning, Motorcycle cleaning, Full body buff, Boat cleaning, Wash/Dry exterior R150, Interior cleaning R150.</div>
    </div>
  </section>

  <!-- Booking -->
  <section id="work" class="section">
    <div class="container work-grid">
      <div class="work-left">
        <h3 class="section-title">Book / Select Services</h3>
        <div class="panel"><h4>Selected package</h4><div id="selected-package" class="selected-box">None selected</div></div>
        <div class="panel"><h4>Add-ons</h4>
          <div class="addons-list">
            <label><input type="checkbox" class="addon-checkbox" data-name="Pet hair & odour removal" data-price="100"> Pet hair & odour removal</label>
            <label><input type="checkbox" class="addon-checkbox" data-name="Express steam cleaning" data-price="100"> Express steam cleaning</label>
            <label><input type="checkbox" class="addon-checkbox" data-name="Full body buff" data-price="100"> Full body buff</label>
            <label><input type="checkbox" class="addon-checkbox" data-name="Motorcycle cleaning" data-price="100"> Motorcycle cleaning</label>
            <label><input type="checkbox" class="addon-checkbox" data-name="Boat cleaning" data-price="100"> Boat cleaning</label>
            <label><input type="checkbox" class="addon-checkbox" data-name="Wash/Dry exterior" data-price="150"> Wash/Dry exterior (R150)</label>
            <label><input type="checkbox" class="addon-checkbox" data-name="Interior cleaning" data-price="150"> Interior cleaning (R150)</label>
          </div>
        </div>
        <div class="panel">
          <h4>Summary</h4>
          <div class="summary"><div>Package: <span id="summary-package">—</span></div><div>Add-ons: <span id="summary-addons">—</span></div><div class="total">Total: R<span id="summary-total">0</span></div></div>
          <div class="booking-actions"><a id="whatsapp-book" class="btn-primary" href="#" target="_blank">Message on WhatsApp</a><button id="clear-selection" class="btn-outline">Clear</button></div>
        </div>
      </div>
    </div>
  </section>

  <!-- Gallery -->
  <section id="gallery" class="section">
    <div class="container">
      <h3 class="section-title">Gallery</h3>
      <div class="gallery-grid"><img src="assets/gallery1.jpg"><img src="assets/gallery2.jpg"><img src="assets/gallery3.jpg"><img src="assets/gallery4.jpg"></div>
    </div>
  </section>

  <!-- Location -->
  <section id="location" class="section">
    <div class="container location-inner">
      <div><h3 class="section-title">Our Service Area</h3><p>We are a mobile service. We'll come to you.</p></div>
      <div><iframe src="https://www.google.com/maps/embed?pb=!1m18..." loading="lazy"></iframe></div>
    </div>
  </section>

  <footer id="contact" class="site-footer">
    <div class="container footer-inner"><div><p>© <span id="year"></span> Driveway Detailing</p></div></div>
  </footer>

  <script>
    document.addEventListener('DOMContentLoaded',()=>{
      const selectPkgBtns=document.querySelectorAll('.select-pkg');
      const selectedPackageEl=document.getElementById('selected-package');
      const summaryPackage=document.getElementById('summary-package');
      const summaryAddons=document.getElementById('summary-addons');
      const summaryTotal=document.getElementById('summary-total');
      const addonCheckboxes=document.querySelectorAll('.addon-checkbox');
      const whatsappBook=document.getElementById('whatsapp-book');
      const clearBtn=document.getElementById('clear-selection');
      let selectedPackage=null;let selectedAddons=[];
      function renderSummary(){
        if(selectedPackage){selectedPackageEl.textContent=${selectedPackage.name} — R${selectedPackage.price};summaryPackage.textContent=${selectedPackage.name} (R${selectedPackage.price});}else{selectedPackageEl.textContent='None selected';summaryPackage.textContent='—';}
        if(selectedAddons.length){summaryAddons.textContent=selectedAddons.map(a=>${a.name} (R${a.price})).join(', ');}else{summaryAddons.textContent='—';}
        const total=(selectedPackage?selectedPackage.price:0)+selectedAddons.reduce((s,a)=>s+a.price,0);summaryTotal.textContent=total;
        const phone='27660642112';const message=Hello! I would like to book:%0APackage: ${selectedPackage?selectedPackage.name+' - R'+selectedPackage.price:'None'}%0AAdd-ons: ${selectedAddons.length?selectedAddons.map(a=>a.name).join(', '):'None'}%0ATotal: R${total};whatsappBook.href=https://wa.me/${phone}?text=${message};
      }
      selectPkgBtns.forEach(btn=>{btn.addEventListener('click',()=>{const name=btn.dataset.name;const price=Number(btn.dataset.price);selectedPackage={name,price};selectPkgBtns.forEach(b=>b.classList.remove('active'));btn.classList.add('active');renderSummary();});});
      addonCheckboxes.forEach(chk=>{chk.addEventListener('change',()=>{const name=chk.dataset.name;const price=Number(chk.dataset.price);if(chk.checked){selectedAddons.push({name,price});}else{selectedAddons=selectedAddons.filter(a=>a.name!==name||a.price!==price);}renderSummary();});});
      clearBtn.addEventListener('click',()=>{selectedPackage=null;selectedAddons=[];summaryTotal.textContent=0;summaryAddons.textContent='—';summaryPackage.textContent='—';selectedPackageEl.textContent='None selected';addonCheckboxes.forEach(c=>c.checked=false);selectPkgBtns.forEach(b=>b.classList.remove('active'));});
      document.getElementById('year').textContent=new Date().getFullYear();
      renderSummary();
    });
  </script>
</body>
</html>
