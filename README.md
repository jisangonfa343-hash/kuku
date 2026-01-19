# kuku
make new enegy
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Business Website Starter</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header class="header">
    <div class="container">
      <h1>My Business</h1>
      <nav>
        <a href="#home">Home</a>
        <a href="#services">Services</a>
        <a href="#products">Products</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <section id="home" class="hero">
    <div class="container">
      <h2>Grow Your Business With Us</h2>
      <p>Professional solutions for your company.</p>
      <button onclick="openWhatsApp()">Chat on WhatsApp</button>
    </div>
  </section>

  <section id="services" class="section">
    <div class="container">
      <h2>Our Services</h2>
      <div class="grid">
        <div class="card">Web Development</div>
        <div class="card">Digital Marketing</div>
        <div class="card">IT Support</div>
      </div>
    </div>
  </section>

  <section id="products" class="section">
    <div class="container">
      <h2>Our Products</h2>
      <div class="grid">
        <div class="card">Product A</div>
        <div class="card">Product B</div>
        <div class="card">Product C</div>
      </div>
    </div>
  </section>

  <section id="contact" class="section">
    <div class="container">
      <h2>Contact Us</h2>
      <form id="contactForm">
        <input type="text" placeholder="Your Name" required />
        <input type="email" placeholder="Your Email" required />
        <textarea placeholder="Your Message" required></textarea>
        <button type="submit">Send Message</button>
      </form>
    </div>
  </section>

  <footer class="footer">
    <div class="container">
      <p>© 2026 My Business. All rights reserved.</p>
    </div>
  </footer>

  <script src="script.js"></script>
</body>
</html>

<!-- style.css -->
<style>
body{margin:0;font-family:Arial;background:#f4f4f4}
.container{width:90%;margin:auto}
.header{background:#222;color:#fff;padding:15px}
nav a{color:#fff;margin:0 10px;text-decoration:none}
.hero{background:#0077cc;color:#fff;padding:80px 0;text-align:center}
.section{padding:50px 0}
.grid{display:flex;gap:20px;flex-wrap:wrap}
.card{background:#fff;padding:20px;border-radius:8px;flex:1;min-width:200px;text-align:center}
.footer{background:#222;color:#fff;text-align:center;padding:20px}
input,textarea,button{width:100%;padding:10px;margin:10px 0}
button{background:#0077cc;color:#fff;border:none;border-radius:5px;cursor:pointer}
</style>

<!-- script.js -->
<script>
function openWhatsApp(){
  window.open("https://wa.me/251900000000","_blank");
}

document.getElementById("contactForm").addEventListener("submit",function(e){
  e.preventDefault();
  alert("Message sent successfully!");
});
</script>
