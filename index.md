---
---

<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }
  
  body { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif; 
         color: #333; line-height: 1.6; }
  
  .header-wrapper { 
    background: linear-gradient(135deg, #0c5456 0%, #0e6e6b 100%);
    color: white;
    padding: 60px 40px;
    position: relative;
    overflow: hidden;
  }
  
  .header-wrapper::after {
    content: '';
    position: absolute;
    bottom: -1px;
    left: 0;
    right: 0;
    height: 40px;
    background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none"><path d="M0,50 Q300,0 600,50 T1200,50 L1200,120 L0,120 Z" fill="%230c5456" opacity="0.3"></path></svg>') repeat-x;
    background-size: 600px 40px;
  }
  
  .header-content { position: relative; z-index: 1; }
  
  .institution { 
    font-size: 0.9rem;
    letter-spacing: 2px;
    text-transform: uppercase;
    font-weight: 600;
    opacity: 0.95;
    margin-bottom: 20px;
  }
  
  .header-content h1 { 
    font-size: 4rem;
    font-weight: 700;
    margin: 10px 0 25px 0;
    letter-spacing: -1px;
  }
  
  .title-section { 
    font-size: 1.1rem;
    line-height: 1.8;
    margin-bottom: 35px;
  }
  
  .title-section strong { font-weight: 600; }
  
  .contact-section {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    font-size: 0.95rem;
    border-top: 1px solid rgba(255,255,255,0.3);
    padding-top: 25px;
  }
  
  .contact-section > div {
    display: flex;
    align-items: center;
    gap: 8px;
  }
  
  .contact-section a { color: white; text-decoration: none; }
  .contact-section a:hover { text-decoration: underline; }
  
  .icon { font-size: 1.2rem; opacity: 0.9; }
  
  .nav-section {
    background: white;
    padding: 0;
    border-bottom: 1px solid #e0e0e0;
  }
  
  .nav-section nav {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 40px;
    display: flex;
    gap: 50px;
  }
  
  .nav-section nav a {
    display: block;
    padding: 25px 0;
    text-decoration: none;
    color: #0a4f4d;
    font-weight: 600;
    font-size: 0.95rem;
    letter-spacing: 1px;
    text-transform: uppercase;
    border-bottom: 3px solid transparent;
    transition: border-color 0.3s;
  }
  
  .nav-section nav a:hover {
    border-bottom-color: #0a4f4d;
  }
  
  .main-content {
    max-width: 1200px;
    margin: 0 auto;
    padding: 60px 40px;
  }
  
  .main-content h1, .main-content h2, .main-content h3 { 
    color: #0a4f4d;
    margin-top: 2.5rem;
    margin-bottom: 1.5rem;
  }
  
  .main-content h1 { font-size: 2.5rem; }
  .main-content h2 { 
    font-size: 1.8rem;
    padding-bottom: 15px;
    border-bottom: 3px solid #0a4f4d;
    display: inline-block;
  }
  .main-content h3 { font-size: 1.2rem; }
  
  .main-content ol, .main-content ul { margin-left: 20px; }
  .main-content ol > li, .main-content ul > li { 
    margin-bottom: 0.8rem;
    line-height: 1.8;
  }
  
  .main-content a { color: #0c5456; text-decoration: none; }
  .main-content a:hover { text-decoration: underline; }
  
  .pill { 
    display: inline-block;
    font-size: 0.8rem;
    font-weight: 600;
    color: #0a4f4d;
    background: #eef5f4;
    border: 1px solid #d8e6e4;
    border-radius: 999px;
    padding: 4px 12px;
    margin: 0 5px 6px 0;
  }
  
  .tag { 
    font-size: 0.7rem;
    font-weight: 600;
    letter-spacing: 0.05em;
    text-transform: uppercase;
    color: #0a4f4d;
    background: #e7f2f1;
    border-radius: 3px;
    padding: 2px 8px;
    margin-left: 8px;
  }
  
  .skills-section {
    margin: 30px 0;
  }
  
  @media (max-width: 768px) {
    .header-wrapper { padding: 40px 20px; }
    .header-content h1 { font-size: 2.5rem; }
    .contact-section { gap: 20px; }
    .nav-section nav { gap: 20px; padding: 0 20px; }
    .nav-section nav a { padding: 15px 0; }
    .main-content { padding: 40px 20px; }
  }
</style>

<div class="header-wrapper">
  <div class="header-content">
    <div class="institution">Zicklin School of Business · Baruch College, CUNY</div>
    <h1>Zeda Li</h1>
    <div class="title-section">
      <strong>Associate Professor of Statistics</strong>, Paul H. Chook Department of Information Systems and Statistics<br>
      Doctoral Faculty, The Graduate Center, CUNY
    </div>
    <div class="contact-section">
      <div><span class="icon">📍</span> <span>One Bernard Baruch Way, New York, NY 10010</span></div>
      <div><span class="icon">✉️</span> <a href="mailto:zeda.li@baruch.cuny.edu">zeda.li@baruch.cuny.edu</a></div>
      <div><span class="icon">📞</span> <span>(646) 312-3379</span></div>
    </div>
  </div>
</div>

<div class="nav-section">
  <nav>
    <a href="#about">About</a>
    <a href="#publications">Publications</a>
    <a href="#software">Software</a>
    <a href="#funding">Funding</a>
    <a href="#teaching">Teaching</a>
  </nav>
</div>

<div class="main-content">

## About {#about}

I am an Associate Professor of Statistics in the Paul H. Chook Department of Information Systems and Statistics, Zicklin School of Business, Baruch College, CUNY, where I have been on the faculty since 2018. I also serve as Doctoral Faculty at the CUNY Graduate Center.

I learned my Ph.D. in Statistics from Temple University in 2018, advised by William W.S. Wei. My research interests include time series analysis, spectral analysis, Bayesian methods, and high-dimensional statistics. I am particularly interested in developing novel statistical methods for analyzing complex, multivariate time series data with applications to physiological signals and other scientific domains.

### Research Interests

<span class="pill">Time series analysis</span>
<span class="pill">Spectral analysis</span>
<span class="pill">Bayesian methods</span>
<span class="pill">Computational statistics</span>
<span class="pill">Dimension reduction</span>
<span class="pill">High-dimensional statistics</span>
<span class="pill">Big data</span>

## Education {#education}

- **Ph.D., Statistics**, Temple University, Philadelphia, PA — 2018

## Publications {#publications}

(*Student co-authors are denoted with *)

1. **Li, Z.** and *Xia, Q. (2026+) "Conditional Graphical Models for Replicated Multivariate Time Series." <span class="tag">Submitted</span>

2. Lee, C. and **Li, Z.** (2026+) "Mean Independent Component Analysis of Multivariate Time Series." *Statistica Sinica*. <span class="tag">To appear</span>

3. **Li, Z.** and Dong, Y. (2025) "[A Cepstral Model for Efficient Spectral Analysis of Replicated Time Series](https://www.tandfonline.com/doi/full/10.1080/10618600.2025.2473936)." *Journal of Computational and Graphical Statistics*, 34, 261–273.

4. **Li, Z.** and Wei, W. (2024) "Measuring the Advantages of Contemporaneous Aggregation in Forecasting." *Journal of Forecasting*, 43, 1308–1320.

5. **Li, Z.**, Yue, Y., and Bruce, S. (2024) "[ANOPOW for Replicated Nonstationary Time Series in Experiments](https://projecteuclid.org/journals/annals-of-applied-statistics/volume-18/issue-1/ANOPOW-for-Replicated-Nonstationary-Time-Series-in-Experiments/10.1214/23-AOAS1757.full)." *Annals of Applied Statistics*, 18, 1–24.

6. Dong, Y. and **Li, Z.** (2024) "[A Note on Marginal Coordinate Test in Sufficient Dimension Reduction](https://www.sciencedirect.com/science/article/pii/S0167715223001712)." *Statistics and Probability Letters*, 205, 110008.

7. *Wang, Y., **Li, Z.**, and Bruce, S. (2023) "[Adaptive Bayesian Sum of Trees Model for Covariate Dependent Spectral Analysis](https://onlinelibrary.wiley.com/doi/10.1111/biom.13763)." *Biometrics*, 79, 2184–2196.

8. **Li, Z.** (2023) "[Robust Conditional Spectral Analysis of Replicated Time Series](https://www.intlpress.com/site/pub/pages/journals/items/sii/content/vols/0016/0001/a007/index.php)." *Statistics and Its Interface*, 16, 1–14.

9. **Li, Z.**, Bruce, S., and *Cai, T. (2022) "[Interpretable Classification of Categorical Time Series Using the Spectral Envelope and Optimal Scalings](https://www.jmlr.org/papers/volume23/21-0369/21-0369.pdf)." *Journal of Machine Learning Research*, 23, 1–32.

10. **Li, Z.**, Rosen, O., Ferrarelli, F., and Krafty, R.T. (2021) "[Adaptive Bayesian Spectral Analysis of High-Dimensional Nonstationary Time Series](https://www.tandfonline.com/doi/full/10.1080/10618600.2020.1819193)." *Journal of Computational and Graphical Statistics*, 30, 1–14.

11. **Li, Z.**, Bruce, S., Wutzke, C., and *Long, Y. (2021) "[Conditional Adaptive Bayesian Spectral Analysis of Replicated Multivariate Time Series](https://onlinelibrary.wiley.com/doi/full/10.1002/bimj.202000076)." *Biometrical Journal*, 63, 1–23.

12. **Li, Z.** and Dong, Y. (2021) "[Model-Free Variable Selection with Matrix-Valued Predictors](https://www.tandfonline.com/doi/full/10.1080/10618600.2020.1806854)." *Journal of Computational and Graphical Statistics*, 29, 1–12.

13. **Li, Z.** and Krafty, R.T. (2019) "[Adaptive Bayesian Time-Frequency Analysis of Multivariate Time Series](https://amstat.tandfonline.com/doi/abs/10.1080/01621459.2017.1415908)." *Journal of the American Statistical Association*, 114, 384–397.

14. Bruce, S., **Li, Z.**, Yang, H.C., and Mukhopadhyay, S. (2019) "[Nonparametric Distributed Learning Architecture for Big Data: Algorithm and Applications](https://ieeexplore.ieee.org/document/8303823)." *IEEE Transactions on Big Data*, 5, 364–376.

15. **Li, Z.** and Bruce, S. (2018) Discussion of "The Statistical Analysis of Acoustic Phonetic Data: Exploring Differences Between Spoken Romance Languages." *Journal of the Royal Statistical Society: Series C*, 67, 1253–1254.

16. Dong, Y. and **Li, Z.** (2018) "[On Sliced Inverse Regression with Response Missing at Random](https://www.tandfonline.com/doi/abs/10.1080/10485252.2018.1508677)." *Journal of Nonparametric Statistics*, 30, 876–900.

17. Dong, Y., Xia, Q., Tang, C.Y., and **Li, Z.** (2018) "[On Sufficient Dimension Reduction with Missing Responses Through Estimating Equations](https://www.sciencedirect.com/science/article/pii/S0167715217302213)." *Statistics and Probability Letters*, 137, 29–37.

18. Esbenshade, A., Sopfe, J., Zhao, Z., **Li, Z.**, Campbell, K., Simmons, J., and Henry, K. (2014) "Overweight Pediatric Cancer Survivors Have a High Risk of Vitamin D Insufficiency." *Pediatric Blood & Cancer*, 61, 1696–1699.

## Software {#software}

- [**CepReg**](https://cran.r-project.org/package=CepReg) — R package on CRAN for "A Cepstral Model for Efficient Spectral Analysis of Replicated Time Series." With Q. Xia.
- [**CepLDA**](https://cran.r-project.org/package=CepLDA) — R package on CRAN for "Discriminant Analysis of Time Series in the Presence of Within-Group Spectral Variability." With R.T. Krafty.
- **MultiSpectMCMC** — MATLAB functions for "Adaptive Bayesian Time–Frequency Analysis of Multivariate Time Series."
- **FactorSpect** — MATLAB functions for "Adaptive Bayesian Spectral Analysis of High-Dimensional Nonstationary Time Series."
- **MultiCABS** — MATLAB functions for "Conditional Adaptive Bayesian Spectral Analysis of Replicated Multivariate Time Series."

## Funding & Grants {#funding}

- **National Science Foundation, DMS-2418850** (Principal Investigator), $225,444, 2024–2027  
  *Covariate-Assisted Analysis of Spectral Matrices with Applications to Physiological Signals*

- **PSC-CUNY Research Award (Traditional A), TRADA-55-179** (Principal Investigator), 2024–2025  
  *Principal Spectral Component Analysis for Replicated Multivariate Time Series*

- **Eugene M. Lang Junior Faculty Research Fellowship**, Baruch College (Principal Investigator), 2020–2021  
  *Evaluating Postural Control and Cognitive Impairment in People with Neurodegenerative Disease: Adaptive Bayesian Time Series Approach*

- **PSC-CUNY Research Award (Traditional A), TRADA-51-94** (Principal Investigator), 2020–2021  
  *Spectral Analysis Framework of High-Dimensional Nonstationary Time Series*

- **Fox School Young Scholar Forum Research Seed Funding**, Temple University (Co-Principal Investigator), 2014–2015  
  *Divide and Conquer Variable Selection*

## Teaching {#teaching}

### Baruch College, City University of New York

- STA 2000: Business Statistics I *(Undergraduate)*
- STA 3000: Statistical Computing *(Undergraduate)*
- STA 3154: Business Statistics II *(Undergraduate)*
- STA 9701: Time Series: Forecasting and Statistical Modeling *(Graduate)*
- STA 9708: Managerial Statistics *(Graduate)*
- STA 9719: Foundations of Statistical Inference *(Graduate)*
- STA 9797: Advanced Data Analysis *(Graduate)*

### Graduate Center, City University of New York

- STA 7050: Multivariate Statistical Analysis *(Doctoral)*

### Temple University

- STAT 1001: Quantitative Methods for Business I *(Undergraduate)*
- STAT 1102: Quantitative Methods for Business II *(Undergraduate)*
- STAT 2103: Business Statistical Analytics *(Undergraduate)*
- Ph.D. Math Camp: intensive two-week mathematics preparation for first-year doctoral students

</div>
