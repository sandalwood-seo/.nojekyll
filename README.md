<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Chandan | Web Developer & Digital Marketer</title>

<!-- Google Font -->
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600&family=Poppins&display=swap" rel="stylesheet">

<style>
:root{
  --bg:#0b0f1a;
  --panel:#111827;
  --neon:#00f7ff;
  --text:#e5e7eb;
}
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}
body{
  font-family:'Poppins',sans-serif;
  background:var(--bg);
  color:var(--text);
  display:flex;
}

/* Sidebar */
.sidebar{
  width:260px;
  background:linear-gradient(180deg,#0f172a,#020617);
  padding:25px;
  height:100vh;
  position:fixed;
}
.logo{
  font-family:'Orbitron',sans-serif;
  color:var(--neon);
  font-size:22px;
  margin-bottom:30px;
  text-align:center;
}
.search-box input{
  width:100%;
  padding:10px;
  border:none;
  outline:none;
  border-radius:6px;
  background:#020617;
  color:#fff;
  margin-bottom:25px;
}
.nav a{
  display:block;
  padding:12px;
  margin-bottom:10px;
  text-decoration:none;
  color:#cbd5f5;
  border-radius:6px;
  transition:.3s;
}
.nav a:hover{
  background:var(--neon);
  color:#000;
}

/* Main Content */
.main{
  margin-left:260px;
  padding:40px;
  width:100%;
}
.section{
  margin-bottom:80px;
}
.hero h1{
  font-size:42px;
  font-family:'Orbitron',sans-serif;
}
.hero span{
  color:var(--neon);
}
.hero p{
  max-width:600px;
  margin-top:15px;
  opacity:.9;
}
.btn{
  margin-top:25px;
  display:inline-block;
  padding:12px 24px;
  border:1px solid var(--neon);
  color:var(--neon);
  text-decoration:none;
  border-radius:30px;
  transition:.3s;
}
.btn:hover{
  background:var(--neon);
  color:#000;
}

/* Cards */
.grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:25px;
}
.card{
  background:var(--panel);
  padding:25px;
  border-radius:15px;
  border:1px solid rgba(0,247,255,.2);
}
.card h3{
  color:var(--neon);
  margin-bottom:10px;
}

/* Footer */
footer{
  text-align:center;
  opacity:.6;
  padding:20px;
}
</style>
</head>

<body>

<!-- Sidebar -->
<div class="sidebar">
  <div class="logo">CHANDAN.dev</div>

  <div class="search-box">
    <input type="text" placeholder="Search..." onkeyup="searchSection(this.value)">
  </div>

  <div class="nav">
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </div>
</div>

<!-- Main Content -->
<div class="main">

<section id="home" class="section hero">
  <h1>Hi, I'm <span>Chandan</span></h1>
  <p>Web Developer & Digital Marketer crafting high-performance websites, SEO strategies and futuristic digital experiences.</p>
  <a href="#contact" class="btn">Hire Me</a>
</section>

<section id="about" class="section">
  <h2>About Me</h2>
  <p>I specialise in building responsive websites and driving organic growth using SEO, analytics, and performance marketing strategies.</p>
</section>

<section id="skills" class="section">
  <h2>Skills</h2>
  <div class="grid">
    <div class="card"><h3>Web Development</h3><p>HTML, CSS, JavaScript, WordPress</p></div>
    <div class="card"><h3>SEO</h3><p>On-Page, Off-Page, Technical SEO</p></div>
    <div class="card"><h3>Marketing</h3><p>Google Analytics, Ads, Branding</p></div>
    <div class="card"><h3>Tools</h3><p>Search Console, Canva, AI Tools</p></div>
  </div>
</section>

<section id="projects" class="section">
  <h2>Projects</h2>
  <div class="grid">
    <div class="card"><h3>Portfolio Website</h3><p>Modern responsive personal website</p></div>
    <div class="card"><h3>SEO Campaign</h3><p>Ranked keywords on Google SERP</p></div>
  </div>
</section>

<section id="contact" class="section">
  <h2>Contact</h2>
  <p>Email: yourname@email.com</p>
  <p>Location: India</p>
</section>

<footer>
  © 2026 Chandan | Digital Portfolio
</footer>

</div>

<script>
function searchSection(value){
  value=value.toLowerCase();
  document.querySelectorAll('.section').forEach(sec=>{
    sec.style.display = sec.innerText.toLowerCase().includes(value)
    ? 'block':'none';
  });
}
</script>

</body>
</html>
