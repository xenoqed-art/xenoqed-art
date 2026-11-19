<!-- HEADER -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:231a3a,100:0d1117&height=180&section=header&text=Xeno_QED&fontSize=80&fontColor=a371f7&animation=twinkling&fontAlignY=50" width="100%" alt="Xeno_QED banner" />
</p>

<p align="center"><b>Actuarial Science × Quantitative Finance</b></p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&pause=1200&color=A371F7&center=true&vCenter=true&width=400&height=50&lines=Aspiring+Quantitative+Analyst;Actuarial+Science+Student;Python+for+Financial+Engineering;Derivatives+Pricing+%26+Risk+Models;Monte+Carlo+%26+Stochastic+Modeling;Fedora+Linux+Enthusiast;Obsidian+Zettelkasten+User" alt="Typing animation: Aspiring Quantitative Analyst, Actuarial Science Student, Python for Financial Engineering, Derivatives Pricing and Risk Models, Monte Carlo and Stochastic Modeling, Fedora Linux Enthusiast, Obsidian Zettelkasten User" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=xenoqed-art&label=PROFILE+VIEWS&color=3fb950&style=flat-square&labelColor=161b22" alt="Profile views" />
  <img src="https://img.shields.io/github/followers/xenoqed-art?style=flat-square&logo=github&logoColor=white&color=a371f7&labelColor=161b22" alt="GitHub followers" />
  <a href="https://www.linkedin.com/in/arturo-vega-5951643a9">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-a371f7?style=flat-square&logo=linkedin&logoColor=white&labelColor=161b22" alt="LinkedIn" />
  </a>
</p>

---

<!-- PROFILE -->
<h2 align="center">⚡ Quant Profile</h2>

```python
class QuantProfile:
    alias       = "Xeno_QED"
    background  = "Actuarial Science"
    school      = "UAEMéx"
    target      = "Quantitative Analyst"
    languages   = ["Python", "C++"]
    math        = ["Probability",
                   "Statistics",
                   "Stochastic Processes"]
    typesetting = "LaTeX"
    os          = "Fedora Linux"
    brain       = "Obsidian · 3,400+ notes"
    offline     = ["Taekwondo",
                   "Basketball",
                   "Guitar"]
```

---

<!-- FOCUS -->
<h2 align="center">🎯 Quant Focus</h2>

- 📈 **Quantitative finance** — building my path toward becoming a Quant.
- 🛡️ **Actuarial science** — financial modeling and risk analysis.
- 🐍 **Python for financial engineering** — data, models and numerical methods.
- 🧠 **Knowledge systems** — a STEM & Feynman-style Zettelkasten in Obsidian.

<p align="center">
  <img src="https://img.shields.io/badge/Stochastic%20Calculus-a371f7?style=flat-square&labelColor=161b22&label=%CE%A3" alt="Stochastic Calculus" />
  <img src="https://img.shields.io/badge/Derivatives%20Pricing-a371f7?style=flat-square&labelColor=161b22&label=%CE%94" alt="Derivatives Pricing" />
  <img src="https://img.shields.io/badge/Monte%20Carlo-3fb950?style=flat-square&labelColor=161b22&label=%E2%88%AB" alt="Monte Carlo" />
  <img src="https://img.shields.io/badge/Time%20Series-a371f7?style=flat-square&labelColor=161b22&label=%CE%BB" alt="Time Series" />
  <img src="https://img.shields.io/badge/Risk%20%26%20VaR-a371f7?style=flat-square&labelColor=161b22&label=%CF%83" alt="Risk and VaR" />
  <img src="https://img.shields.io/badge/Portfolio%20Theory-a371f7?style=flat-square&labelColor=161b22&label=%CE%B2" alt="Portfolio Theory" />
</p>

---

<!-- MATH -->
<h2 align="center">📐 Core Mathematics</h2>

<p align="center"><b>Geometric Brownian Motion</b> — the standard model for asset prices</p>

$$dS_t = \mu S_t \, dt + \sigma S_t \, dW_t$$

<p align="center"><b>Black–Scholes</b> — European call option price</p>

$$C = S_0 \, N(d_1) - K e^{-rT} N(d_2)$$

$$d_1 = \frac{\ln(S_0/K) + (r + \sigma^2/2)T}{\sigma \sqrt{T}}$$

$$d_2 = d_1 - \sigma\sqrt{T}$$

<p align="center"><b>Sharpe Ratio</b> — risk-adjusted performance</p>

$$S = \frac{E[R_p - R_f]}{\sigma_p}$$

---

<!-- MONTE CARLO -->
<h2 align="center">🎲 Monte Carlo in Action</h2>

<p align="center">Simulating asset price paths (purple) to price a European call. Green bars are the outcomes that finish in the money.</p>

<p align="center">
  <img src="montecarlo.svg" width="640" alt="Animated Monte Carlo simulation: GBM price paths, their expected value and the distribution of terminal prices, giving a call price of about 8.01" />
</p>

```python
import numpy as np

def mc_call(S0, K, r, vol, T, n=10**5):
    z = np.random.standard_normal(n)
    drift = (r - 0.5 * vol**2) * T
    diff = vol * np.sqrt(T) * z
    ST = S0 * np.exp(drift + diff)
    payoff = np.maximum(ST - K, 0)
    return np.exp(-r * T) * payoff.mean()

print(mc_call(100, 105, 0.05, 0.2, 1))
# ≈ 8.0 (Black–Scholes: 8.02)
```

---

<!-- ROADMAP -->
<h2 align="center">🧭 Path to Quant</h2>

```mermaid
flowchart TD
    A["Actuarial Science"] --> B["Stochastic Calculus"]
    B --> C["Derivatives Pricing"]
    C --> D["Python Quant Models"]
    D --> E["Quant Analyst"]
    classDef quant fill:#161b22,stroke:#a371f7,stroke-width:2px,color:#e0e0e0
    class A,B,C,D,E quant
    linkStyle default stroke:#3fb950,stroke-width:2px
```

---

<!-- TECH -->
<h2 align="center">🧰 Tech Arsenal</h2>

<h3 align="center">Programming &amp; Data</h3>
<p align="center">
  <img src="https://skillicons.dev/icons?i=py,cpp,numpy,pandas&theme=dark" alt="Python, C++, NumPy, Pandas" />
</p>

<h3 align="center">Math &amp; Documentation</h3>
<p align="center">
  <img src="https://skillicons.dev/icons?i=latex,md,obsidian&theme=dark" alt="LaTeX, Markdown, Obsidian" />
</p>

<h3 align="center">Environment &amp; Tools</h3>
<p align="center">
  <img src="https://skillicons.dev/icons?i=fedora,linux,git,github,vscode&theme=dark" alt="Fedora, Linux, Git, GitHub, VS Code" />
</p>

---

<!-- ANALYTICS -->
<h2 align="center">📡 GitHub Analytics</h2>

<p align="center">
  <a href="https://github.com/xenoqed-art">
    <img width="400" alt="xenoqed-art GitHub stats" src="https://github-readme-stats.vercel.app/api?username=xenoqed-art&include_all_commits=true&count_private=true&show_icons=true&line_height=20&card_width=400&title_color=a371f7&icon_color=3fb950&text_color=e0e0e0&bg_color=0d1117&border_color=333333&border_radius=12" />
  </a>
  <a href="https://github.com/xenoqed-art">
    <img width="400" alt="xenoqed-art top languages" src="https://github-readme-stats.vercel.app/api/top-langs?username=xenoqed-art&layout=compact&locale=en&card_width=400&title_color=a371f7&text_color=e0e0e0&bg_color=0d1117&border_color=333333&border_radius=12" />
  </a>
</p>

<p align="center">
  <img width="480" alt="xenoqed-art streak stats" src="https://streak-stats.demolab.com?user=xenoqed-art&border_radius=12&background=0d1117&border=333333&stroke=444444&ring=a371f7&fire=3fb950&currStreakNum=e0e0e0&sideNums=e0e0e0&currStreakLabel=a371f7&sideLabels=a371f7&dates=8b949e" />
</p>

<p align="center">
  <img width="100%" alt="xenoqed-art contribution graph" src="https://github-readme-activity-graph.vercel.app/graph?username=xenoqed-art&bg_color=0d1117&color=a371f7&line=a371f7&point=3fb950&area=true&area_color=a371f7&hide_border=true&custom_title=Contribution%20Graph" />
</p>

---

<!-- CONNECT -->
<h2 align="center">🌐 Let's Connect</h2>

<p align="center">
  <a href="https://www.linkedin.com/in/arturo-vega-5951643a9">
    <img src="https://img.shields.io/badge/LinkedIn-a371f7?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=161b22" alt="LinkedIn" />
  </a>
</p>

<!-- QUOTE -->
<p align="center">
  <em>"What I cannot create, I do not understand."</em><br />
  — Richard Feynman
</p>

<!-- FOOTER -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:231a3a,100:0d1117&height=100&section=footer" width="100%" alt="" />
</p>
