<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Zeda Li — Associate Professor of Statistics, Baruch College, CUNY</title>
<meta name="description" content="Zeda Li is Associate Professor of Statistics at the Zicklin School of Business, Baruch College, CUNY. Research in time series analysis, spectral analysis, Bayesian methods, and high-dimensional statistics.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Source+Serif+4:opsz,wght@8..60,400;8..60,600;8..60,700&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#15252e;
    --ink-soft:#42555f;
    --ink-faint:#6b7d86;
    --paper:#ffffff;
    --paper-tint:#f3f6f7;
    --teal:#0e6e6b;
    --teal-deep:#0a4f4d;
    --hairline:#dde5e7;
    --serif:"Source Serif 4", Georgia, serif;
    --sans:"Inter", -apple-system, "Segoe UI", sans-serif;
    --mono:"IBM Plex Mono", ui-monospace, monospace;
  }
  *{margin:0;padding:0;box-sizing:border-box}
  html{scroll-behavior:smooth}
  body{
    font-family:var(--sans);
    color:var(--ink);
    background:var(--paper);
    line-height:1.65;
    font-size:16px;
    -webkit-font-smoothing:antialiased;
  }
  a{color:var(--teal);text-decoration:none;border-bottom:1px solid transparent;transition:border-color .15s, color .15s}
  a:hover{border-bottom-color:var(--teal)}
  a:focus-visible{outline:2px solid var(--teal);outline-offset:2px;border-radius:2px}

  /* ---------- Header ---------- */
  header{
    background:linear-gradient(180deg, #0c3d3b 0%, var(--teal-deep) 100%);
    color:#fff;
    position:relative;
    overflow:hidden;
  }
  .header-inner{
    max-width:880px;
    margin:0 auto;
    padding:72px 28px 56px;
    position:relative;
    z-index:1;
  }
  .eyebrow{
    font-family:var(--mono);
    font-size:.78rem;
    letter-spacing:.14em;
    text-transform:uppercase;
    color:#9fd4cf;
    margin-bottom:14px;
  }
  h1{
    font-family:var(--serif);
    font-weight:700;
    font-size:clamp(2.3rem, 6vw, 3.4rem);
    letter-spacing:-.01em;
    line-height:1.1;
    margin-bottom:14px;
  }
  .title-line{
    font-size:1.05rem;
    color:#d7e8e6;
    max-width:54ch;
    font-weight:400;
  }
  .title-line strong{color:#fff;font-weight:600}
  .header-contact{
    display:flex;
    flex-wrap:wrap;
    gap:10px 26px;
    margin-top:28px;
    font-size:.9rem;
    color:#bcd9d6;
  }
  .header-contact span{display:inline-flex;align-items:center;gap:8px}
  .header-contact svg{flex:none;opacity:.75}
  .header-contact a{color:#eafaf8;border-bottom-color:rgba(255,255,255,.25)}
  .header-contact a:hover{border-bottom-color:#fff}

  /* spectral waveform — nod to spectral analysis of time series */
  .spectra{
    position:absolute;
    inset:auto 0 0 0;
    height:120px;
    width:100%;
    opacity:.5;
    pointer-events:none;
  }
  .spectra path{
    fill:none;
    stroke:#7fc6bf;
    stroke-width:1.4;
    stroke-dasharray:2400;
    stroke-dashoffset:2400;
    animation:draw 2.4s ease-out forwards;
  }
  .spectra path:nth-child(2){stroke:#4fa39c;animation-delay:.25s}
  .spectra path:nth-child(3){stroke:#2c7e78;animation-delay:.5s}
  @keyframes draw{to{stroke-dashoffset:0}}
  @media (prefers-reduced-motion: reduce){
    html{scroll-behavior:auto}
    .spectra path{animation:none;stroke-dashoffset:0}
  }

  /* ---------- Nav ---------- */
  nav{
    position:sticky;
    top:0;
    background:rgba(255,255,255,.92);
    backdrop-filter:blur(8px);
    border-bottom:1px solid var(--hairline);
    z-index:10;
  }
  .nav-inner{
    max-width:880px;
    margin:0 auto;
    padding:0 28px;
    display:flex;
    gap:30px;
    overflow-x:auto;
  }
  nav a{
    font-family:var(--mono);
    font-size:.8rem;
    letter-spacing:.08em;
    text-transform:uppercase;
    color:var(--ink-soft);
    padding:14px 0;
    border-bottom:2px solid transparent;
    white-space:nowrap;
  }
  nav a:hover{color:var(--teal);border-bottom-color:var(--teal)}

  /* ---------- Main ---------- */
  main{max-width:880px;margin:0 auto;padding:24px 28px 80px}
  section{padding-top:56px}
  h2{
    font-family:var(--serif);
    font-weight:600;
    font-size:1.7rem;
    letter-spacing:-.01em;
    margin-bottom:6px;
  }
  .section-rule{
    width:44px;height:3px;background:var(--teal);
    border-radius:2px;margin:10px 0 26px;
  }
  p{color:var(--ink-soft)}

  /* About */
  .about p{max-width:68ch;margin-bottom:16px}
  .interests{
    display:flex;flex-wrap:wrap;gap:8px;margin-top:6px;
  }
  .interests li{
    list-style:none;
    font-size:.83rem;
    font-weight:500;
    color:var(--teal-deep);
    background:var(--paper-tint);
    border:1px solid var(--hairline);
    padding:5px 12px;
    border-radius:999px;
  }

  /* Publications */
  .pub-note{font-size:.85rem;color:var(--ink-faint);margin-bottom:22px}
  .pub-list{list-style:none;counter-reset:pub 0}
  .pub-list li{
    counter-increment:pub;
    position:relative;
    padding:14px 16px 14px 58px;
    margin-bottom:8px;
    border:1px solid transparent;
    border-radius:8px;
    transition:background .15s, border-color .15s;
  }
  .pub-list li::before{
    content:counter(pub, decimal-leading-zero);
    position:absolute;
    left:16px;
    top:17px;
    font-family:var(--mono);
    font-size:.8rem;
    color:var(--ink-faint);
  }
  @media (max-width:560px){
    .pub-list li{padding-left:48px}
    .pub-list li::before{left:10px}
  }
  .pub-list li:hover{background:var(--paper-tint);border-color:var(--hairline)}
  .pub-title{font-family:var(--serif);font-weight:600;font-size:1.04rem;line-height:1.45;color:var(--ink)}
  .pub-title a{color:var(--ink);border-bottom:1px solid var(--hairline)}
  .pub-title a:hover{color:var(--teal);border-bottom-color:var(--teal)}
  .pub-meta{font-size:.9rem;color:var(--ink-soft);margin-top:3px}
  .pub-meta em{color:var(--ink-soft)}
  .me{font-weight:600;color:var(--ink)}
  .student{color:var(--teal-deep)}
  .status{
    font-family:var(--mono);
    font-size:.72rem;
    letter-spacing:.06em;
    text-transform:uppercase;
    color:var(--teal-deep);
    background:#e7f2f1;
    padding:2px 8px;
    border-radius:4px;
    margin-left:6px;
    white-space:nowrap;
  }

  /* About extras */
  .sub-head{
    font-family:var(--serif);font-weight:600;font-size:1.15rem;
    margin:30px 0 12px;color:var(--ink);
  }
  .edu-list{list-style:none;display:grid;gap:6px;max-width:68ch}
  .edu-list li{
    display:flex;gap:14px;align-items:baseline;flex-wrap:wrap;
    padding:8px 0;border-bottom:1px solid var(--hairline);
    font-size:.95rem;
  }
  .edu-deg{font-weight:600;color:var(--ink);flex:none}
  .edu-inst{color:var(--ink-soft);flex:1;min-width:200px}
  .edu-year{font-family:var(--mono);font-size:.8rem;color:var(--teal-deep)}

  /* Software */
  .soft-list{list-style:none;display:grid;gap:10px}
  .soft-list li{
    display:flex;gap:16px;align-items:baseline;flex-wrap:wrap;
    padding:14px 16px;
    background:var(--paper-tint);
    border:1px solid var(--hairline);
    border-radius:8px;
    font-size:.93rem;color:var(--ink-soft);
  }
  .soft-name{font-family:var(--mono);font-size:.85rem;font-weight:500;color:var(--teal-deep);flex:none;min-width:130px}

  /* Level tags */
  .level{
    font-family:var(--mono);font-size:.68rem;letter-spacing:.05em;
    text-transform:uppercase;color:var(--ink-faint);
    border:1px solid var(--hairline);border-radius:4px;
    padding:1px 6px;margin-left:auto;white-space:nowrap;
  }

  /* Grants */
  .grant-list{list-style:none;display:grid;gap:10px}
  .grant-list li{
    display:flex;gap:14px;align-items:baseline;
    padding:14px 16px;
    background:var(--paper-tint);
    border:1px solid var(--hairline);
    border-radius:8px;
  }
  .grant-role{
    font-family:var(--mono);font-size:.72rem;letter-spacing:.06em;
    text-transform:uppercase;color:var(--teal-deep);flex:none;
  }
  .grant-list strong{font-weight:600;color:var(--ink)}
  .grant-list .sub{display:block;font-size:.88rem;color:var(--ink-faint)}

  /* Teaching */
  .teach-inst{
    font-family:var(--serif);font-weight:600;font-size:1.15rem;
    margin:26px 0 12px;color:var(--ink);
  }
  .teach-inst:first-of-type{margin-top:0}
  .course-list{list-style:none;display:grid;gap:6px}
  .course-list li{
    display:flex;gap:14px;align-items:baseline;
    padding:8px 0;
    border-bottom:1px solid var(--hairline);
    font-size:.95rem;color:var(--ink-soft);
  }
  .course-code{
    font-family:var(--mono);font-size:.8rem;color:var(--teal-deep);
    flex:none;min-width:96px;
  }

  /* Footer */
  footer{
    border-top:1px solid var(--hairline);
    padding:28px;
    text-align:center;
    font-size:.83rem;
    color:var(--ink-faint);
  }

  @media (max-width:560px){
    .header-inner{padding:52px 20px 44px}
    .nav-inner, main{padding-left:20px;padding-right:20px}
    .pub-list li{padding:12px 10px}
    .course-code{min-width:84px}
  }
</style>
</head>
<body>

<header>
  <div class="header-inner">
    <p class="eyebrow">Zicklin School of Business · Baruch College, CUNY</p>
    <h1>Zeda Li</h1>
    <p class="title-line"><strong>Associate Professor of Statistics</strong>, Paul H. Chook Department of Information Systems and Statistics<br>Doctoral Faculty, The Graduate Center, CUNY</p>
    <div class="header-contact">
      <span>
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>
        One Bernard Baruch Way, New York, NY 10010
      </span>
      <span>
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-10 6L2 7"/></svg>
        <a href="mailto:zeda.li@baruch.cuny.edu">zeda.li@baruch.cuny.edu</a>
      </span>
      <span>
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
        (646) 312-3379
      </span>
    </div>
  </div>
  <svg class="spectra" viewBox="0 0 1200 120" preserveAspectRatio="none" aria-hidden="true">
    <path d="M0,60 C40,20 80,100 120,60 C160,20 200,100 240,60 C280,20 320,100 360,60 C400,20 440,100 480,60 C520,20 560,100 600,60 C640,20 680,100 720,60 C760,20 800,100 840,60 C880,20 920,100 960,60 C1000,20 1040,100 1080,60 C1120,20 1160,100 1200,60"/>
    <path d="M0,60 C60,35 120,85 180,60 C240,35 300,85 360,60 C420,35 480,85 540,60 C600,35 660,85 720,60 C780,35 840,85 900,60 C960,35 1020,85 1080,60 C1140,35 1200,85 1200,60"/>
    <path d="M0,60 C100,48 200,72 300,60 C400,48 500,72 600,60 C700,48 800,72 900,60 C1000,48 1100,72 1200,60"/>
  </svg>
</header>

<nav aria-label="Section navigation">
  <div class="nav-inner">
    <a href="#about">About</a>
    <a href="#publications">Publications</a>
    <a href="#software">Software</a>
    <a href="#funding">Funding</a>
    <a href="#teaching">Teaching</a>
  </div>
</nav>

<main>

  <section id="about" class="about">
    <h2>About</h2>
    <div class="section-rule"></div>
    <p>I am an Associate Professor of Statistics in the Paul H. Chook Department of Information Systems and Statistics at the Zicklin School of Business, Baruch College, City University of New York, where I have been on the faculty since 2018. I also serve as Doctoral Faculty at the CUNY Graduate Center.</p>
    <p>I earned my Ph.D. in Statistics from Temple University in 2018, advised by <a href="https://sites.temple.edu/wwei/" target="_blank" rel="noopener">William W.S. Wei</a> and <a href="https://sph.emory.edu/faculty/profile/index.php?FID=robert-krafty-10974" target="_blank" rel="noopener">Robert T. Krafty</a>. My research develops statistical methodology with applications to business and biomedical studies, and is supported by the National Science Foundation.</p>
    <ul class="interests" aria-label="Research interests">
      <li>Time series analysis</li>
      <li>Spectral analysis</li>
      <li>Bayesian methods</li>
      <li>Computational statistics</li>
      <li>Dimension reduction</li>
      <li>High-dimensional statistics</li>
      <li>Big data</li>
    </ul>

    <h3 class="sub-head">Education</h3>
    <ul class="edu-list">
      <li><span class="edu-deg">Ph.D., Statistics</span><span class="edu-inst">Temple University, Philadelphia, PA</span><span class="edu-year">2018</span></li>
      <li><span class="edu-deg">M.S., Biostatistics</span><span class="edu-inst">Middle Tennessee State University, Murfreesboro, TN</span><span class="edu-year">2013</span></li>
      <li><span class="edu-deg">B.S., Electrical Engineering</span><span class="edu-inst">Central South University of Forestry and Technology, Changsha, China</span><span class="edu-year">2010</span></li>
    </ul>
  </section>

  <section id="publications">
    <h2>Publications</h2>
    <div class="section-rule"></div>
    <p class="pub-note">An asterisk (<span class="student">*</span>) denotes student co-authors.</p>

    <ol class="pub-list">
      <li>
        <div class="pub-title">Dimension Reduction for Covariate-Dependent Time Series through Conditionally Principal Component Analysis <span class="status">Submitted</span></div>
        <div class="pub-meta"><span class="me">Li, Z.</span>, Lee, C., and Krafty, R. · <em>Journal of the American Statistical Association</em></div>
      </li>
      <li>
        <div class="pub-title">Conditional Graphical Models for Replicated Multivariate Time Series <span class="status">Submitted</span></div>
        <div class="pub-meta"><span class="me">Li, Z.</span> and <span class="student">*</span>Xia, Q. (2026+)</div>
      </li>
      <li>
        <div class="pub-title">Mean Independent Component Analysis of Multivariate Time Series <span class="status">To appear</span></div>
        <div class="pub-meta">Lee, C. and <span class="me">Li, Z.</span> (2026+) · <em>Statistica Sinica</em></div>
      </li>
      <li>
        <div class="pub-title"><a href="https://www.tandfonline.com/doi/full/10.1080/10618600.2025.2473936" target="_blank" rel="noopener">A Cepstral Model for Efficient Spectral Analysis of Replicated Time Series</a></div>
        <div class="pub-meta"><span class="me">Li, Z.</span> and Dong, Y. (2025) · <em>Journal of Computational and Graphical Statistics</em>, 34, 1612–1624</div>
      </li>
      <li>
        <div class="pub-title">Measuring the Advantages of Contemporaneous Aggregation in Forecasting</div>
        <div class="pub-meta"><span class="me">Li, Z.</span> and Wei, W. (2024) · <em>Journal of Forecasting</em>, 43, 1308–1320</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://projecteuclid.org/journals/annals-of-applied-statistics/volume-18/issue-1/ANOPOW-for-replicated-nonstationary-time-series-in-experiments/10.1214/23-AOAS1791.short" target="_blank" rel="noopener">ANOPOW for Replicated Nonstationary Time Series in Experiments</a></div>
        <div class="pub-meta"><span class="me">Li, Z.</span>, Yue, Y., and Bruce, S. (2024) · <em>Annals of Applied Statistics</em>, 18, 328–349</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://www.sciencedirect.com/science/article/pii/S0167715223001712" target="_blank" rel="noopener">A Note on Marginal Coordinate Test in Sufficient Dimension Reduction</a></div>
        <div class="pub-meta">Dong, Y. and <span class="me">Li, Z.</span> (2024) · <em>Statistics and Probability Letters</em>, 204, 109947</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://onlinelibrary.wiley.com/doi/10.1111/biom.13763" target="_blank" rel="noopener">Adaptive Bayesian Sum of Trees Model for Covariate Dependent Spectral Analysis</a></div>
        <div class="pub-meta"><span class="student">*</span>Wang, Y., <span class="me">Li, Z.</span>, and Bruce, S. (2023) · <em>Biometrics</em>, 79, 1826–1839</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://www.intlpress.com/site/pub/pages/journals/items/sii/content/vols/0016/0001/a007/index.php" target="_blank" rel="noopener">Robust Conditional Spectral Analysis of Replicated Time Series</a></div>
        <div class="pub-meta"><span class="me">Li, Z.</span> (2023) · <em>Statistics and Its Interface</em>, 16, 81–96</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://www.jmlr.org/papers/volume23/21-0369/21-0369.pdf" target="_blank" rel="noopener">Interpretable Classification of Categorical Time Series Using the Spectral Envelope and Optimal Scalings</a></div>
        <div class="pub-meta"><span class="me">Li, Z.</span>, Bruce, S., and <span class="student">*</span>Cai, T. (2022) · <em>Journal of Machine Learning Research</em>, 23, 1–31</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://www.tandfonline.com/doi/full/10.1080/10618600.2020.1868305" target="_blank" rel="noopener">Adaptive Bayesian Spectral Analysis of High-Dimensional Nonstationary Time Series</a></div>
        <div class="pub-meta"><span class="me">Li, Z.</span>, Rosen, O., Ferrarelli, F., and Krafty, R.T. (2021) · <em>Journal of Computational and Graphical Statistics</em>, 30, 794–807</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://onlinelibrary.wiley.com/doi/full/10.1002/sim.8884" target="_blank" rel="noopener">Conditional Adaptive Bayesian Spectral Analysis of Replicated Multivariate Time Series</a></div>
        <div class="pub-meta"><span class="me">Li, Z.</span>, Bruce, S., Wutzke, C., and <span class="student">*</span>Long, Y. (2021) · <em>Statistics in Medicine</em>, 40, 1989–2005</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://www.tandfonline.com/doi/full/10.1080/10618600.2020.1806854" target="_blank" rel="noopener">Model-Free Variable Selection with Matrix-Valued Predictors</a></div>
        <div class="pub-meta"><span class="me">Li, Z.</span> and Dong, Y. (2021) · <em>Journal of Computational and Graphical Statistics</em>, 30, 171–178</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://amstat.tandfonline.com/doi/abs/10.1080/01621459.2017.1415908" target="_blank" rel="noopener">Adaptive Bayesian Time-Frequency Analysis of Multivariate Time Series</a></div>
        <div class="pub-meta"><span class="me">Li, Z.</span> and Krafty, R.T. (2019) · <em>Journal of the American Statistical Association</em>, 114, 453–465</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://ieeexplore.ieee.org/document/8303780" target="_blank" rel="noopener">Nonparametric Distributed Learning Architecture for Big Data: Algorithm and Applications</a></div>
        <div class="pub-meta">Bruce, S., <span class="me">Li, Z.</span>, Yang, H.C., and Mukhopadhyay, S. (2019) · <em>IEEE Transactions on Big Data</em>, 5, 166–179</div>
      </li>
      <li>
        <div class="pub-title">Discussion of “The Statistical Analysis of Acoustic Phonetic Data: Exploring Differences Between Spoken Romance Languages”</div>
        <div class="pub-meta"><span class="me">Li, Z.</span> and Bruce, S. (2018) · <em>Journal of the Royal Statistical Society, Series C</em>, 67, 1103–1145</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://www.tandfonline.com/doi/abs/10.1080/10485252.2018.1508677" target="_blank" rel="noopener">On Sliced Inverse Regression with Response Missing at Random</a></div>
        <div class="pub-meta">Dong, Y. and <span class="me">Li, Z.</span> (2018) · <em>Journal of Nonparametric Statistics</em>, 30, 990–1002</div>
      </li>
      <li>
        <div class="pub-title"><a href="https://www.sciencedirect.com/science/article/pii/S0167947318300951" target="_blank" rel="noopener">On Sufficient Dimension Reduction with Missing Responses Through Estimating Equations</a></div>
        <div class="pub-meta">Dong, Y., Xia, Q., Tang, C.Y., and <span class="me">Li, Z.</span> (2018) · <em>Computational Statistics and Data Analysis</em>, 126, 67–77</div>
      </li>
      <li>
        <div class="pub-title">Overweight Pediatric Cancer Survivors Have a High Risk of Vitamin D Insufficiency</div>
        <div class="pub-meta">Esbenshade, A., Sopfe, J., Zhao, Z., <span class="me">Li, Z.</span>, Campbell, K., Simmons, J., and Henry, K. (2014) · <em>Pediatric Blood &amp; Cancer</em>, 61, 723–728</div>
      </li>
    </ol>
  </section>

  <section id="software">
    <h2>Software</h2>
    <div class="section-rule"></div>
    <ul class="soft-list">
      <li>
        <span class="soft-name"><a href="https://cran.r-project.org/package=CepReg" target="_blank" rel="noopener">CepReg</a></span>
        <span>R package on CRAN — cepstral models for efficient spectral analysis of replicated time series. With Q. Xia.</span>
      </li>
      <li>
        <span class="soft-name"><a href="https://cran.r-project.org/package=CepLDA" target="_blank" rel="noopener">CepLDA</a></span>
        <span>R package on CRAN — discriminant analysis of time series in the presence of within-group spectral variability. With R.T. Krafty.</span>
      </li>
      <li>
        <span class="soft-name">MultiSpectMCMC</span>
        <span>MATLAB functions for adaptive Bayesian time–frequency analysis of multivariate time series.</span>
      </li>
      <li>
        <span class="soft-name">FactorSpect</span>
        <span>MATLAB functions for adaptive Bayesian spectral analysis of high-dimensional nonstationary time series.</span>
      </li>
      <li>
        <span class="soft-name">MultiCABS</span>
        <span>MATLAB functions for conditional adaptive Bayesian spectral analysis of replicated multivariate time series.</span>
      </li>
    </ul>
  </section>

  <section id="funding">
    <h2>Funding &amp; Grants</h2>
    <div class="section-rule"></div>
    <ul class="grant-list">
      <li>
        <span class="grant-role">PI</span>
        <span><strong>National Science Foundation, DMS-2418850</strong> · $225,444 · 2024–2027<span class="sub">Covariate-Assisted Analysis of Spectral Matrices with Applications to Physiological Signals</span></span>
      </li>
      <li>
        <span class="grant-role">PI</span>
        <span><strong>PSC-CUNY Research Award (Traditional A), TRADA-55-179</strong> · 2024–2025<span class="sub">Principal Spectral Component Analysis for Replicated Multivariate Time Series</span></span>
      </li>
      <li>
        <span class="grant-role">PI</span>
        <span><strong>Eugene M. Lang Junior Faculty Research Fellowship</strong>, Baruch College · 2020–2021<span class="sub">Evaluating Postural Control and Cognitive Impairment in People with Neurodegenerative Disease: Adaptive Bayesian Time Series Approach</span></span>
      </li>
      <li>
        <span class="grant-role">PI</span>
        <span><strong>PSC-CUNY Research Award (Traditional A), TRADA-51-94</strong> · 2020–2021<span class="sub">Spectral Analysis Framework of High-Dimensional Nonstationary Time Series</span></span>
      </li>
      <li>
        <span class="grant-role">Co-PI</span>
        <span><strong>Fox School Young Scholar Forum Research Seed Funding</strong>, Temple University · 2014–2015<span class="sub">Divide and Conquer Variable Selection</span></span>
      </li>
    </ul>
  </section>
  <section id="teaching">
    <h2>Teaching</h2>
    <div class="section-rule"></div>

    <h3 class="teach-inst">Baruch College, City University of New York</h3>
    <ul class="course-list">
      <li><span class="course-code">STA 2000</span> Business Statistics I <span class="level">Undergraduate</span></li>
      <li><span class="course-code">STA 3000</span> Statistical Computing <span class="level">Undergraduate</span></li>
      <li><span class="course-code">STA 3154</span> Business Statistics II <span class="level">Undergraduate</span></li>
      <li><span class="course-code">STA 9701</span> Time Series: Forecasting and Statistical Modeling <span class="level">Graduate</span></li>
      <li><span class="course-code">STA 9708</span> Managerial Statistics <span class="level">Graduate</span></li>
      <li><span class="course-code">STA 9719</span> Foundations of Statistical Inference <span class="level">Graduate</span></li>
      <li><span class="course-code">STA 9797</span> Advanced Data Analysis <span class="level">Graduate</span></li>
    </ul>

    <h3 class="teach-inst">Graduate Center, City University of New York</h3>
    <ul class="course-list">
      <li><span class="course-code">STA 7050</span> Multivariate Statistical Analysis <span class="level">Doctoral</span></li>
    </ul>

    <h3 class="teach-inst">Temple University</h3>
    <ul class="course-list">
      <li><span class="course-code">STAT 1001</span> Quantitative Methods for Business I <span class="level">Undergraduate</span></li>
      <li><span class="course-code">STAT 1102</span> Quantitative Methods for Business II <span class="level">Undergraduate</span></li>
      <li><span class="course-code">STAT 2103</span> Business Statistical Analytics <span class="level">Undergraduate</span></li>
      <li><span class="course-code">—</span> Ph.D. Math Camp: intensive two-week mathematics preparation for first-year doctoral students <span class="level">Doctoral</span></li>
    </ul>
  </section>

</main>

<footer>
  © 2026 Zeda Li · Baruch College, City University of New York
</footer>

</body>
</html>
