# TD-INTERIOR-AUTOCARE
“TD Interior Auto Care provides expert interior and exterior auto detailing in the Framingham area. We make every vehicle look and feel like new, delivering high-quality, professional service with attention to detail.”
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TD Interior Auto Care</title>
<style>
  /* -------------------- GENERAL -------------------- */
  body {margin:0; font-family: Arial, Helvetica, sans-serif; background:#0b0b0b; color:#f2f2f2; scroll-behavior:smooth;}
  a{text-decoration:none;color:inherit;}
  section{padding:60px 10%;}
  h2{text-align:center;color:#1e90ff;margin-bottom:40px;font-size:2.2rem;}

  /* -------------------- HERO -------------------- */
  header {
    position: relative; height: 90vh; overflow:hidden; display:flex;
    flex-direction:column; justify-content:center; align-items:center; text-align:center;
    background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)),
                url('https://images.unsplash.com/photo-1603386329225-868f9b1ee6c9') center/cover no-repeat;
    background-size: cover;
    animation: zoomHero 20s infinite alternate;
  }

  @keyframes zoomHero {
    0%{transform:scale(1);}
    50%{transform:scale(1.05);}
    100%{transform:scale(1);}
  }

  header h1, header p, .book-btn {
    animation: floatText 6s ease-in-out infinite alternate;
  }

  @keyframes floatText {
    0%{transform:translateY(0);}
    50%{transform:translateY(-8px);}
    100%{transform:translateY(0);}
  }

  .logo {
    position:absolute; top:20px; left:20px; width:120px; height:120px;
    background:url('A_logo_for_"TD_Interior_Auto_Care"_is_designed_in_.png') center/contain no-repeat;
    background-color:transparent; border-radius:8px;
    animation: floatLogo 8s ease-in-out infinite alternate;
  }

  @keyframes floatLogo {
    0%{transform:translateY(0);}
    50%{transform:translateY(-10px);}
    100%{transform:translateY(0);}
  }

  header h1 {font-size:3.2rem; color:#1e90ff; margin-bottom:10px;}
  header p {font-size:1.2rem; color:#ccc; margin-bottom:20px;}
  .book-btn {background:#00aaff; color:#fff; padding:15px 30px; border-radius:8px; font-size:1.1rem; transition:.3s; cursor:pointer; margin-top:20px;}
  .book-btn:hover{background:#0077aa;}

  /* -------------------- CARDS -------------------- */
  .services, .pricing, .gallery, .reviews{display:grid; grid-template-columns:repeat(auto-fit,minmax(250px,1fr)); gap:25px;}
  .card{background:#121212; padding:30px; border-radius:10px; text-align:center; border:1px solid #1e90ff33;}
  .card h3{color:#1e90ff; margin-bottom:10px;}
  .price{font-size:2rem; color:#00aaff; margin:15px 0;}
  .gallery div, .reviews div{background:#1a1a1a; height:170px; border-radius:8px; display:flex; align-items:center; justify-content:center; color:#666; font-size:0.9rem;}
  .about, .contact{max-width:900px; margin:auto; text-align:center; color:#ccc;}
  footer{background:#000; text-align:center; padding:20px; color:#555; font-size:0.9rem;}

  /* -------------------- SOCIAL ICONS -------------------- */
  .social{text-align:center; margin-top:20px;}
  .social a{display:inline-block; margin:0 10px; color:#1e90ff; font-size:1.5rem; transition:.3s;}
  .social a:hover{color:#00aaff;}

  /* -------------------- POPUP FORM -------------------- */
  .popup-bg{display:none; position:fixed; top:0; left:0; width:100%; height:100%; background: rgba(0,0,0,0.85); justify-content:center; align-items:center; z-index:1000;}
  .popup-content{background:#121212; padding:30px; border-radius:12px; max-width:400px; width:90%; text-align:center; position:relative;}
  .popup-content h3{margin-bottom:15px; color:#1e90ff;}
  .popup-content input, .popup-content textarea{width:100%; padding:10px; margin:8px 0; border-radius:6px; border:none; background:#1a1a1a; color:#fff;}
  .popup-content button{background:#00aaff; color:#fff; padding:12px 25px; border:none; border-radius:6px; cursor:pointer; margin-top:10px;}
  .popup-content button:hover{background:#0077aa;}
  .popup-close{position:absolute; top:15px; right:20px; color:#fff; font-size:1.5rem; cursor:pointer;}

  /* -------------------- PHONE BUTTONS -------------------- */
  .phones{display:flex; justify-content:center; gap:20px; margin-top:20px; flex-wrap:wrap;}
  .phones a{background:#1e90ff; color:#fff; padding:12px 25px; border-radius:6px; transition:.3s;}
  .phones a:hover{background:#00aaff;}

  @media(max-width:600px){
    header h1{font-size:2.2rem;}
    header p{font-size:1rem;}
    .book-btn{font-size:1rem; padding:12px 20px;}
  }
</style>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>

<!-- HERO -->
<header>
  <div class="logo"></div>
  <h1>TD Interior Auto Care</h1>
  <p>Interior & Exterior Auto Detailing</p>
  <p>Serving the Framingham, MA Area</p>
  <button class="book-btn" id="openPopup">Get a Quote</button>
</header>

<!-- SERVICES -->
<section>
<h2>Our Services</h2>
<div class="services">
  <div class="card"><h3>Exterior Auto Care</h3><p>Professional wash, polish, detailing, and exterior enhancement.</p></div>
  <div class="card"><h3>Interior Auto Care</h3><p>Deep interior cleaning, stain removal, and premium finishes.</p></div>
  <div class="card"><h3>Full Auto Package</h3><p>Complete interior and exterior auto transformation.</p></div>
</div>
</section>

<!-- PRICING -->
<section>
<h2>Pricing</h2>
<div class="pricing">
  <div class="card"><h3>Exterior Only</h3><div class="price">$90</div><p>High-quality exterior detail service.</p></div>
  <div class="card"><h3>Interior Only</h3><div class="price">$150</div><p>Complete interior deep clean and refresh.</p></div>
  <div class="card"><h3>Interior + Exterior</h3><div class="price">$210</div><p>Best value full-service auto care package.</p></div>
</div>
</section>

<!-- GALLERY -->
<section>
<h2>Gallery</h2>
<div class="gallery">
  <div>Coming Soon</div>
  <div>Coming Soon</div>
  <div>Coming Soon</div>
  <div>Coming Soon</div>
</div>
</section>

<!-- REVIEWS -->
<section>
<h2>Customer Reviews</h2>
<div class="reviews">
  <div>⭐⭐⭐⭐⭐ “Amazing interior work! Highly recommend.”</div>
  <div>⭐⭐⭐⭐⭐ “My car looks brand new. Great job!”</div>
  <div>⭐⭐⭐⭐⭐ “Professional and fast service.”</div>
</div>
</section>

<!-- ABOUT -->
<section>
<h2>About Us</h2>
<div class="about">
<p>TD Interior Auto Care is dedicated to delivering high-quality interior and exterior auto detailing. We focus on precision, cleanliness, and customer satisfaction while proudly serving the Framingham, Massachusetts area.</p>
</div>
</section>

<!-- CONTACT -->
<section>
<h2>Contact</h2>
<div class="contact">
<p>📍 Framingham, MA</p>
<div class="phones">
  <a href="tel:+18187927569">📞 +1 (818) 792-7569</a>
</div>
<div class="social">
  <a href="#"><i class="fab fa-facebook-f"></i></a>
  <a href="#"><i class="fab fa-instagram"></i></a>
  <a href="#"><i class="fab fa-tiktok"></i></a>
</div>
</div>
</section>

<!-- FOOTER -->
<footer>
© 2026 TD Interior Auto Care. All rights reserved.
</footer>

<!-- POPUP FORM -->
<div class="popup-bg" id="popup">
  <div class="popup-content">
    <span class="popup-close" id="closePopup">&times;</span>
    <h3>Request a Quote</h3>
    <input type="text" placeholder="Full Name">
    <input type="email" placeholder="Email">
    <input type="tel" placeholder="Phone Number">
    <textarea rows="4" placeholder="Your Message / Car Details"></textarea>
    <button>Submit</button>
  </div>
</div>

<script>
  // Pop-up form
  const popup = document.getElementById('popup');
  document.getElementById('openPopup').addEventListener('click', ()=>{popup.style.display='flex';});
  document.getElementById('closePopup').addEventListener('click', ()=>{popup.style.display='none';});
  window.addEventListener('click', e=>{if(e.target==popup){popup.style.display='none';}});
</script>
</body>
</html>
