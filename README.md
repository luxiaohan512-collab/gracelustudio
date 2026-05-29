<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Danli Lu</title>

  <!-- Google Font -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
    }

    body{
      font-family:'Inter',sans-serif;
      background:#0f0f0f;
      color:white;
      line-height:1.6;
    }

    a{
      color:white;
      text-decoration:none;
    }

    img{
      width:100%;
      display:block;
      object-fit:cover;
    }

    /* NAV */

    nav{
      position:fixed;
      top:0;
      width:100%;
      padding:24px 60px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      background:rgba(15,15,15,0.7);
      backdrop-filter:blur(10px);
      z-index:1000;
    }

    nav h1{
      font-size:18px;
      letter-spacing:2px;
      font-weight:600;
    }

    nav ul{
      display:flex;
      gap:32px;
      list-style:none;
    }

    nav ul li a{
      font-size:14px;
      opacity:0.8;
      transition:0.3s;
    }

    nav ul li a:hover{
      opacity:1;
    }

    /* HERO */

    .hero{
      height:100vh;
      display:flex;
      flex-direction:column;
      justify-content:center;
      align-items:center;
      text-align:center;
      padding:0 20px;
      background:url('https://images.unsplash.com/photo-1492691527719-9d1e07e534b4?q=80&w=1600&auto=format&fit=crop') center/cover;
      position:relative;
    }

    .hero::after{
      content:'';
      position:absolute;
      inset:0;
      background:rgba(0,0,0,0.45);
    }

    .hero-content{
      position:relative;
      z-index:2;
    }

    .hero h2{
      font-size:72px;
      font-weight:600;
      letter-spacing:3px;
      margin-bottom:16px;
    }

    .hero p{
      font-size:18px;
      opacity:0.9;
    }

    /* SECTION */

    section{
      padding:120px 80px;
    }

    .section-title{
      font-size:42px;
      margin-bottom:50px;
      font-weight:600;
    }

    /* RESUME */

    .resume-grid{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:40px;
    }

    .resume-card{
      border:1px solid rgba(255,255,255,0.1);
      padding:32px;
      border-radius:20px;
      background:#161616;
    }

    .resume-card h3{
      margin-bottom:12px;
      font-size:22px;
    }

    .resume-card p{
      opacity:0.75;
      margin-bottom:10px;
    }

    /* PORTFOLIO */

    .portfolio-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:24px;
    }

    .portfolio-item{
      position:relative;
      overflow:hidden;
      border-radius:24px;
    }

    .portfolio-item img{
      height:400px;
      transition:0.4s ease;
    }

    .portfolio-item:hover img{
      transform:scale(1.05);
    }

    .portfolio-overlay{
      position:absolute;
      inset:0;
      background:linear-gradient(to top, rgba(0,0,0,0.8), transparent);
      display:flex;
      align-items:flex-end;
      padding:24px;
    }

    .portfolio-overlay h4{
      font-size:20px;
    }

    /* SOCIAL */

    .social-links{
      display:flex;
      gap:24px;
      flex-wrap:wrap;
    }

    .social-links a{
      padding:16px 28px;
      border:1px solid rgba(255,255,255,0.15);
      border-radius:999px;
      transition:0.3s;
      background:#161616;
    }

    .social-links a:hover{
      background:white;
      color:black;
    }

    /* FOOTER */

    footer{
      padding:40px;
      text-align:center;
      opacity:0.5;
      font-size:14px;
    }

    /* MOBILE */

    @media(max-width:768px){

      nav{
        padding:20px;
      }

      nav ul{
        gap:16px;
      }

      .hero h2{
        font-size:42px;
      }

      section{
        padding:80px 24px;
      }

      .resume-grid{
        grid-template-columns:1fr;
      }

      .section-title{
        font-size:32px;
      }
    }

  </style>
</head>

<body>

  <!-- NAVIGATION -->

  <nav>
    <h1>DANLI LU</h1>

    <ul>
      <li><a href="#resume">Resume</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#social">Social Media</a></li>
    </ul>
  </nav>

  <!-- HERO -->

  <div class="hero">

    <div class="hero-content">
      <h2>DANLI LU</h2>

      <p>
        NYC Photographer & Marketing Specialist
      </p>
    </div>

  </div>

  <!-- RESUME -->

  <section id="resume">

    <h2 class="section-title">Resume</h2>

    <div class="resume-grid">

      <div class="resume-card">
        <h3>Experience</h3>

        <p>
          Marketing Specialist — HungryPanda
        </p>

        <p>
          Freelance Photographer — NYC
        </p>

        <p>
          Brand Campaign & Event Production
        </p>
      </div>

      <div class="resume-card">
        <h3>Education & Awards</h3>

        <p>
          School of Visual Arts — Digital Photography
        </p>

        <p>
          MBA — Trine University
        </p>

        <p>
          Urban Photo Awards Official Visual
        </p>
      </div>

    </div>

  </section>

  <!-- PORTFOLIO -->

  <section id="portfolio">

    <h2 class="section-title">Portfolio</h2>

    <div class="portfolio-grid">

      <div class="portfolio-item">

        <img src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?q=80&w=1200&auto=format&fit=crop">

        <div class="portfolio-overlay">
          <h4>Fashion Photography</h4>
        </div>

      </div>

      <div class="portfolio-item">

        <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?q=80&w=1200&auto=format&fit=crop">

        <div class="portfolio-overlay">
          <h4>Food Photography</h4>
        </div>

      </div>

      <div class="portfolio-item">

        <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?q=80&w=1200&auto=format&fit=crop">

        <div class="portfolio-overlay">
          <h4>Portrait Photography</h4>
        </div>

      </div>

    </div>

  </section>

  <!-- SOCIAL -->

  <section id="social">

    <h2 class="section-title">Social Media</h2>

    <div class="social-links">

      <a href="https://instagram.com" target="_blank">
        Instagram
      </a>

      <a href="https://tiktok.com" target="_blank">
        TikTok
      </a>

      <a href="https://linkedin.com" target="_blank">
        LinkedIn
      </a>

      <a href="mailto:your@email.com">
        Email
      </a>

    </div>

  </section>

  <!-- FOOTER -->

  <footer>
    © 2026 Danli Lu. All Rights Reserved.
  </footer>

</body>
</html>
