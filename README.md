<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Finance &amp; Analytics Portfolio — Selected Work</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,500;0,9..144,600;1,9..144,500&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --paper:#F4F1E8;
    --paper-deep:#ECE7D8;
    --ink:#1B2B3A;
    --ink-soft:#5B6B77;
    --brass:#9C7A3C;
    --brass-light:#C9A868;
    --forest:#2E5A4C;
    --rust:#8B4332;
    --line:#D6CFB9;
    --line-strong:#B9AF92;
    --card:#FFFDF7;
  }
  *{box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    margin:0;
    background:var(--paper);
    color:var(--ink);
    font-family:'Inter',sans-serif;
    -webkit-font-smoothing:antialiased;
  }
  ::selection{background:var(--brass-light);color:var(--ink);}

  a{color:inherit;}

  .wrap{max-width:1080px;margin:0 auto;padding:0 32px;}

  /* ---------- MASTHEAD ---------- */
  .masthead{
    border-bottom:2px solid var(--ink);
    padding-top:28px;
  }
  .masthead-top{
    display:flex;justify-content:space-between;align-items:baseline;
    font-family:'IBM Plex Mono',monospace;
    font-size:11px;letter-spacing:.12em;text-transform:uppercase;
    color:var(--ink-soft);
    padding-bottom:18px;
    border-bottom:1px solid var(--line);
  }
  .masthead-date{color:var(--brass);}
  .masthead-main{
    display:flex;justify-content:space-between;align-items:flex-end;
    gap:24px;padding:26px 0 22px;
    flex-wrap:wrap;
  }
  .eyebrow{
    font-family:'IBM Plex Mono',monospace;
    font-size:12px;letter-spacing:.18em;text-transform:uppercase;
    color:var(--brass);margin:0 0 8px;
  }
  h1{
    font-family:'Fraunces',serif;
    font-weight:600;
    font-size:clamp(38px,6vw,58px);
    line-height:1.02;
    margin:0;
    letter-spacing:-0.01em;
  }
  .name-placeholder{border-bottom:2px dashed var(--brass-light);}
  .masthead-blurb{
    max-width:340px;font-size:14.5px;line-height:1.55;color:var(--ink-soft);
    padding-bottom:4px;
  }
  .contact-row{
    font-family:'IBM Plex Mono',monospace;font-size:12px;color:var(--ink-soft);
    display:flex;gap:18px;flex-wrap:wrap;padding-bottom:22px;
  }
  .contact-row span::before{content:"— ";color:var(--brass);}

  /* ---------- TICKER STRIP ---------- */
  .ticker{
    background:var(--ink);
    color:var(--paper);
    overflow:hidden;
    white-space:nowrap;
    position:relative;
    border-bottom:2px solid var(--ink);
  }
  .ticker-track{
    display:inline-flex;
    animation:scroll 34s linear infinite;
    padding:13px 0;
  }
  .ticker:hover .ticker-track{animation-play-state:paused;}
  @keyframes scroll{
    from{transform:translateX(0);}
    to{transform:translateX(-50%);}
  }
  .tick{
    font-family:'IBM Plex Mono',monospace;
    font-size:12.5px;
    padding:0 28px;
    border-right:1px solid rgba(244,241,232,.2);
    display:inline-flex;align-items:center;gap:8px;
  }
  .tick b{color:var(--brass-light);font-weight:600;}
  .tick .up{color:#7FBE9C;}

  @media (prefers-reduced-motion: reduce){
    .ticker-track{animation:none;}
  }

  /* ---------- INTRO NOTE ---------- */
  .note{
    padding:36px 0 8px;
    max-width:700px;
  }
  .note p{
    font-size:16px;line-height:1.7;color:var(--ink);
    margin:0 0 14px;
  }
  .note .lede{
    font-family:'Fraunces',serif;font-style:italic;font-weight:500;
    font-size:20px;color:var(--forest);
  }

  /* ---------- SKILLS ROW ---------- */
  .skills{
    display:flex;flex-wrap:wrap;gap:10px;
    padding:22px 0 44px;
    border-bottom:1px solid var(--line);
  }
  .skill-pill{
    font-family:'IBM Plex Mono',monospace;
    font-size:11.5px;letter-spacing:.03em;
    border:1px solid var(--line-strong);
    padding:6px 12px;
    color:var(--ink-soft);
    background:var(--card);
  }

  /* ---------- EXHIBITS ---------- */
  .exhibits{padding-top:8px;}
  .exhibit{
    display:grid;
    grid-template-columns:96px 1fr;
    gap:0 28px;
    padding:52px 0;
    border-bottom:1px solid var(--line);
    position:relative;
  }
  .exhibit:last-child{border-bottom:none;}
  .ex-num{
    font-family:'Fraunces',serif;font-weight:300;
    font-size:56px;color:var(--line-strong);
    line-height:1;
  }
  .ex-label{
    font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.1em;
    color:var(--brass);text-transform:uppercase;margin-top:8px;
  }
  .ex-body h2{
    font-family:'Fraunces',serif;font-weight:600;font-size:27px;
    margin:0 0 6px;letter-spacing:-.01em;
  }
  .ex-sub{
    font-size:13.5px;color:var(--ink-soft);margin:0 0 18px;
    font-style:italic;
  }
  .ex-grid{
    display:grid;grid-template-columns:1.3fr 1fr;gap:32px;
    align-items:start;
  }
  .ex-text p{font-size:14.5px;line-height:1.7;margin:0 0 14px;color:var(--ink);}
  .ex-text strong{color:var(--ink);}
  .ex-tags{display:flex;flex-wrap:wrap;gap:7px;margin-top:16px;}
  .ex-tag{
    font-family:'IBM Plex Mono',monospace;font-size:10.5px;
    background:var(--paper-deep);border:1px solid var(--line-strong);
    padding:4px 9px;color:var(--ink-soft);
  }

  .stat-card{
    background:var(--card);border:1px solid var(--line-strong);
    padding:18px 20px;margin-bottom:14px;
  }
  .stat-card h3{
    font-family:'IBM Plex Mono',monospace;font-size:10.5px;letter-spacing:.08em;
    text-transform:uppercase;color:var(--ink-soft);margin:0 0 12px;
    border-bottom:1px solid var(--line);padding-bottom:8px;
  }
  .stat-row{display:flex;justify-content:space-between;align-items:baseline;padding:5px 0;}
  .stat-row .k{font-size:12.5px;color:var(--ink-soft);}
  .stat-row .v{font-family:'IBM Plex Mono',monospace;font-size:13.5px;font-weight:600;color:var(--forest);}
  .stat-row .v.rust{color:var(--rust);}

  /* mini bar chart */
  .barviz{margin-top:4px;}
  .bar-item{margin-bottom:11px;}
  .bar-item .lbl{
    display:flex;justify-content:space-between;
    font-family:'IBM Plex Mono',monospace;font-size:11px;color:var(--ink-soft);
    margin-bottom:4px;
  }
  .bar-track{height:7px;background:var(--paper-deep);border:1px solid var(--line-strong);}
  .bar-fill{height:100%;background:linear-gradient(90deg,var(--forest),var(--brass-light));}

  /* heatmap */
  .heat-wrap{overflow-x:auto;}
  .heatmap{border-collapse:collapse;font-family:'IBM Plex Mono',monospace;font-size:10.5px;width:100%;}
  .heatmap th,.heatmap td{padding:6px 7px;text-align:center;border:1px solid var(--paper);}
  .heatmap th{background:var(--ink);color:var(--paper);font-weight:500;font-size:10px;}
  .heatmap td{color:#0f2a20;}
  .heatmap .rowhead{background:var(--ink);color:var(--paper);font-weight:500;}

  /* cashflow ladder */
  .ladder{font-family:'IBM Plex Mono',monospace;font-size:12px;}
  .ladder-row{
    display:flex;justify-content:space-between;padding:7px 0;
    border-bottom:1px dotted var(--line-strong);
  }
  .ladder-row.total{font-weight:600;border-bottom:1px solid var(--ink);}
  .ladder-row .k{color:var(--ink-soft);}
  .ladder-row .v{color:var(--ink);}
  .ladder-row .v.neg{color:var(--rust);}
  .ladder-row .v.pos{color:var(--forest);}

  /* ---------- TOOLKIT ---------- */
  .toolkit{padding:56px 0;border-bottom:1px solid var(--line);}
  .toolkit h2{
    font-family:'Fraunces',serif;font-weight:600;font-size:26px;margin:0 0 24px;
  }
  .tool-grid{
    display:grid;grid-template-columns:repeat(3,1fr);gap:1px;
    background:var(--line-strong);border:1px solid var(--line-strong);
  }
  .tool-cell{background:var(--card);padding:20px 18px;}
  .tool-cell h4{
    font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.06em;
    text-transform:uppercase;color:var(--brass);margin:0 0 8px;
  }
  .tool-cell p{font-size:13px;color:var(--ink-soft);line-height:1.55;margin:0;}

  /* ---------- FOOTER ---------- */
  footer{padding:44px 0 60px;}
  footer .close{
    font-family:'Fraunces',serif;font-style:italic;font-size:19px;color:var(--forest);
    max-width:560px;line-height:1.5;margin:0 0 22px;
  }
  .footer-meta{
    display:flex;justify-content:space-between;flex-wrap:wrap;gap:12px;
    font-family:'IBM Plex Mono',monospace;font-size:11px;color:var(--ink-soft);
    padding-top:18px;border-top:1px solid var(--line);
  }
  .stamp{
    display:inline-block;border:1.5px solid var(--rust);color:var(--rust);
    font-family:'IBM Plex Mono',monospace;font-size:10px;letter-spacing:.1em;
    padding:4px 10px;transform:rotate(-3deg);text-transform:uppercase;
  }

  @media(max-width:760px){
    .wrap{padding:0 18px;}
    .exhibit{grid-template-columns:1fr;}
    .ex-num{font-size:34px;}
    .ex-grid{grid-template-columns:1fr;}
    .tool-grid{grid-template-columns:1fr;}
    .masthead-main{flex-direction:column;align-items:flex-start;}
  }
</style>
</head>
<body>

<header class="masthead">
  <div class="wrap">
    <div class="masthead-top">
      <span>Selected Coursework &amp; Independent Analysis</span>
      <span class="masthead-date">Updated July 2026</span>
    </div>
    <div class="masthead-main">
      <div>
        <p class="eyebrow">Analyst Portfolio</p>
        <h1><span class="name-placeholder">Shachi Shah</span></h1>
      </div>
      <p class="masthead-blurb">Four projects spanning equity valuation, cash-flow analysis, portfolio theory, and quantitative coding — built from scratch, own methodology, own numbers.</p>
    </div>
    <div class="contact-row">
      <span>shachi261190@gmail.com</span>
      <span>linkedin.com/in/shachi-suketu-kavita/</span>
      <span>Riverside, CA</span>
    </div>
  </div>
</header>

<div class="ticker">
  <div class="ticker-track" id="tickerTrack"></div>
</div>

<main class="wrap">

  <section class="note">
    <p class="lede">I build the model, not just read it.</p>
    <p>The four projects below were built for coursework and self-study in corporate finance, valuation, and applied statistics. Each one starts from raw data — public filings, market returns, or a case dataset — and works through to a defensible number: an intrinsic value, a cash-flow bridge, a portfolio beta, a sampling distribution. I've summarized the approach and the output of each here; happy to walk through the full workbook or notebook on request.</p>
  </section>

  <div class="skills">
    <span class="skill-pill">DCF &amp; DDM Valuation</span>
    <span class="skill-pill">CAPM / Beta Estimation</span>
    <span class="skill-pill">Cash Flow Reconciliation</span>
    <span class="skill-pill">Python — pandas / numpy / matplotlib</span>
    <span class="skill-pill">Monte Carlo Sampling</span>
    <span class="skill-pill">Sensitivity &amp; Scenario Analysis</span>
    <span class="skill-pill">Excel Financial Modeling</span>
    <span class="skill-pill">Statistical Inference</span>
  </div>

  <section class="exhibits">

    <!-- EXHIBIT 01 : DKS -->
    <article class="exhibit">
      <div>
        <div class="ex-num">01</div>
        <div class="ex-label">Valuation</div>
      </div>
      <div class="ex-body">
        <h2>DICK'S Sporting Goods (DKS) — Equity Valuation &amp; New-Venture Appraisal</h2>
        <p class="ex-sub">Full three-statement build, DCF/DDM intrinsic value, and a standalone NPV/IRR case for a proposed in-store service line.</p>
        <div class="ex-grid">
          <div class="ex-text">
            <p>Built a valuation model for DKS from its historical income statement and balance sheet, projecting revenue, margins, and free cash flow forward. Estimated the cost of equity via CAPM (5-year beta, 10-year Treasury as the risk-free rate, an equity risk premium assumption) and the cost of debt from DKS's actual bond coupons, then blended them into a WACC using market-value weights of debt and equity.</p>
            <p>Cross-checked the DCF output against a dividend discount model, and separately underwrote a new business idea — an in-store sports-equipment service bay — as its own capital project: built a unit-economics model (equipment cost, certification cost, revenue per store), then ran it through an NPV/IRR framework with a two-way sensitivity table across WACC and EBIT margin.</p>
            <div class="ex-tags">
              <span class="ex-tag">CAPM</span><span class="ex-tag">WACC</span><span class="ex-tag">DCF</span><span class="ex-tag">DDM</span><span class="ex-tag">NPV / IRR</span><span class="ex-tag">Sensitivity Tables</span>
            </div>
          </div>
          <div>
            <div class="stat-card">
              <h3>Core Valuation Outputs</h3>
              <div class="stat-row"><span class="k">WACC</span><span class="v">8.55%</span></div>
              <div class="stat-row"><span class="k">Cost of equity (CAPM)</span><span class="v">9.97%</span></div>
              <div class="stat-row"><span class="k">Beta (5-yr)</span><span class="v">1.20</span></div>
              <div class="stat-row"><span class="k">DDM intrinsic value / sh</span><span class="v">$72.35</span></div>
              <div class="stat-row"><span class="k">New venture NPV</span><span class="v">$6.99M</span></div>
              <div class="stat-row"><span class="k">New venture IRR</span><span class="v">7.64%</span></div>
              <div class="stat-row"><span class="k">Payback period</span><span class="v rust">9 years</span></div>
            </div>
            <div class="stat-card">
              <h3>NPV Sensitivity — WACC × EBIT Margin ($000s)</h3>
              <div class="heat-wrap" id="heatmap"></div>
            </div>
          </div>
        </div>
      </div>
    </article>

    <!-- EXHIBIT 02 : Cash Flow -->
    <article class="exhibit">
      <div>
        <div class="ex-num">02</div>
        <div class="ex-label">Financial Statement Analysis</div>
      </div>
      <div class="ex-body">
        <h2>Cash Flow Reconciliation — Net Income to Free Cash Flow</h2>
        <p class="ex-sub">Built the bridge from the income statement through working-capital changes to CFO, FCF, and FCFE.</p>
        <div class="ex-grid">
          <div class="ex-text">
            <p>Starting from a two-year income statement and balance sheet, reconstructed the indirect-method cash flow statement: added back depreciation, worked through the changes in receivables, inventory, and payables to get operating cash flow, then layered in investing (capex) and financing (debt and equity issuance) activity to tie out to the ending cash balance exactly.</p>
            <p>Used the reconciled statement to derive two different definitions of "cash the business actually generated" — Free Cash Flow (after capex) and Free Cash Flow to Equity (after net debt activity) — and showed why net income, EBITDA, and FCF told three different stories for the same company in the same year.</p>
            <div class="ex-tags">
              <span class="ex-tag">Indirect Method CF</span><span class="ex-tag">Working Capital</span><span class="ex-tag">FCF vs FCFE</span><span class="ex-tag">Statement Tie-Out</span>
            </div>
          </div>
          <div>
            <div class="stat-card">
              <h3>Reconciliation, FY2025 ($M)</h3>
              <div class="ladder">
                <div class="ladder-row"><span class="k">Net income</span><span class="v pos">5,220</span></div>
                <div class="ladder-row"><span class="k">+ Depreciation</span><span class="v">3,750</span></div>
                <div class="ladder-row"><span class="k">± Working capital</span><span class="v">4,000</span></div>
                <div class="ladder-row total"><span class="k">Cash from operations</span><span class="v pos">12,970</span></div>
                <div class="ladder-row"><span class="k">Investing activity</span><span class="v neg">(10,000)</span></div>
                <div class="ladder-row"><span class="k">Financing activity</span><span class="v pos">36,000</span></div>
                <div class="ladder-row total"><span class="k">Net change in cash</span><span class="v pos">38,970</span></div>
                <div class="ladder-row"><span class="k">Free Cash Flow</span><span class="v pos">2,970</span></div>
                <div class="ladder-row"><span class="k">Free Cash Flow to Equity</span><span class="v pos">8,970</span></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </article>

    <!-- EXHIBIT 03 : Cavalier Fund -->
    <article class="exhibit">
      <div>
        <div class="ex-num">03</div>
        <div class="ex-label">Portfolio &amp; Risk</div>
      </div>
      <div class="ex-body">
        <h2>Student-Managed Fund Stock Screen — Risk, Return &amp; CAPM</h2>
        <p class="ex-sub">A case-based portfolio exercise (Darden School of Business): evaluating four candidate holdings for a student-managed equity fund.</p>
        <div class="ex-grid">
          <div class="ex-text">
            <p>Worked through a real capital-allocation decision for a student-managed fund choosing between four candidate stocks across different industries. For each, estimated beta by regressing five years of monthly stock returns against the S&amp;P 500 (OLS), and compared that market-implied risk against each stock's historical volatility, dividend yield, credit rating, and valuation multiple.</p>
            <p>Used those inputs to reason through CAPM-implied required returns and to benchmark each candidate against long-run asset-class return and risk data (bills, bonds, and large-cap equities since 1926), then weighed the trade-off between a high-beta cyclical name and a lower-beta defensive one for a two-stock portfolio.</p>
            <div class="ex-tags">
              <span class="ex-tag">OLS Regression</span><span class="ex-tag">Beta Estimation</span><span class="ex-tag">CAPM</span><span class="ex-tag">Risk-Return Tradeoff</span><span class="ex-tag">Portfolio Construction</span>
            </div>
          </div>
          <div>
            <div class="stat-card">
              <h3>Candidate Screen — Estimated Beta Range</h3>
              <div class="barviz" id="betaBars"></div>
            </div>
            <div class="stat-card">
              <h3>Long-Run Benchmark (1926–2016)</h3>
              <div class="stat-row"><span class="k">T-bills, geometric mean</span><span class="v">3.4%</span></div>
              <div class="stat-row"><span class="k">Long-term corp. bonds</span><span class="v">6.0%</span></div>
              <div class="stat-row"><span class="k">Large-cap equities (S&amp;P)</span><span class="v">10.1%</span></div>
            </div>
          </div>
        </div>
      </div>
    </article>

    <!-- EXHIBIT 04 : Python -->
    <article class="exhibit">
      <div>
        <div class="ex-num">04</div>
        <div class="ex-label">Applied Statistics / Python</div>
      </div>
      <div class="ex-body">
        <h2>20-Year Return Simulation — AAPL, MSFT, TSLA</h2>
        <p class="ex-sub">Independent Python project: pulling market data, computing returns, and demonstrating the Central Limit Theorem by simulation.</p>
        <div class="ex-grid">
          <div class="ex-text">
            <p>Pulled 20 years of monthly price and volume data for Apple, Microsoft, and Tesla with <code>yfinance</code>, then computed monthly returns and summary statistics (mean, standard deviation, quartiles) for each stock in <code>pandas</code>.</p>
            <p>Drew repeated 500-observation samples from a stock's return history and tracked how the distribution of sample means tightened around the population mean as the number of resamples grew — a working demonstration of the Central Limit Theorem — then repeated the exercise on winsorized returns to show how capping outliers changes the shape of the distribution without moving its center much.</p>
            <div class="ex-tags">
              <span class="ex-tag">yfinance</span><span class="ex-tag">pandas / numpy</span><span class="ex-tag">matplotlib</span><span class="ex-tag">Central Limit Theorem</span><span class="ex-tag">Winsorization</span><span class="ex-tag">Resampling</span>
            </div>
          </div>
          <div>
            <div class="stat-card">
              <h3>Monthly Return Profile (2010–2024)</h3>
              <div class="barviz" id="retBars"></div>
            </div>
            <div class="stat-card">
              <h3>Sampling Experiment (n=500, 1,000 draws)</h3>
              <div class="stat-row"><span class="k">Population mean (AAPL)</span><span class="v">2.32%</span></div>
              <div class="stat-row"><span class="k">Mean of sample means</span><span class="v">2.33%</span></div>
              <div class="stat-row"><span class="k">Std. dev. of sample means</span><span class="v">0.34%</span></div>
              <div class="stat-row"><span class="k">Std. dev. of raw returns</span><span class="v rust">7.74%</span></div>
            </div>
          </div>
        </div>
      </div>
    </article>

  </section>

  <section class="toolkit">
    <h2>Toolkit</h2>
    <div class="tool-grid">
      <div class="tool-cell"><h4>Modeling</h4><p>Three-statement builds, DCF, DDM, comparable-company setup, NPV/IRR capital budgeting, scenario &amp; sensitivity tables in Excel.</p></div>
      <div class="tool-cell"><h4>Programming</h4><p>Python for data pull, cleaning, and analysis — pandas, numpy, matplotlib, scipy.stats, statsmodels.</p></div>
      <div class="tool-cell"><h4>Statistics</h4><p>Regression (OLS/beta), hypothesis testing, resampling, the Central Limit Theorem, outlier treatment (winsorization).</p></div>
      <div class="tool-cell"><h4>Corporate Finance</h4><p>Cost of capital (CAPM, WACC), capital structure weighting, cash-flow statement reconciliation, FCF/FCFE.</p></div>
      <div class="tool-cell"><h4>Markets</h4><p>Equity risk premiums, portfolio beta, risk-return tradeoffs, long-run asset-class benchmarking.</p></div>
      <div class="tool-cell"><h4>Communication</h4><p>Translating a model into a one-page recommendation — the same discipline behind this page.</p></div>
    </div>
  </section>

  <footer>
    <p class="close">Every number on this page came out of a model I built and can walk through line by line — that's the pitch.</p>
    <div class="footer-meta">
      <span>Full workbooks &amp; notebook available on request</span>
      <span class="stamp">Draft — for interview use</span>
    </div>
  </footer>

</main>

<script>
  // Ticker content
  const stats = [
    "WACC 8.55%", "DDM VALUE $72.35/SH", "BETA 1.20", "NEW VENTURE NPV $6.99M",
    "IRR 7.64%", "FCFE FY25 $8.97M", "AAPL μ 2.32% σ 7.74%", "TSLA μ 4.70% σ 18.34%",
    "MSFT μ 2.02% σ 6.06%", "1000-DRAW CLT SIM", "4-STOCK CAPM SCREEN", "20-YR MONTHLY DATASET"
  ];
  const track = document.getElementById('tickerTrack');
  const build = () => stats.map(s => {
    const [label, ...rest] = s.split(' ');
    return `<span class="tick"><b>${label}</b> ${rest.join(' ')}</span>`;
  }).join('');
  track.innerHTML = build() + build(); // duplicate for seamless loop

  // Beta bars (Exhibit 03)
  const betas = [
    {name:'Delphi (Auto Parts)', v:1.29},
    {name:'Groupon (Internet)', v:1.44},
    {name:'Kellogg (Packaged Foods)', v:0.54},
    {name:'Kinross Gold (Mining)', v:0.31},
  ];
  const maxBeta = 1.6;
  document.getElementById('betaBars').innerHTML = betas.map(b => `
    <div class="bar-item">
      <div class="lbl"><span>${b.name}</span><span>β ${b.v.toFixed(2)}</span></div>
      <div class="bar-track"><div class="bar-fill" style="width:${(b.v/maxBeta*100).toFixed(0)}%"></div></div>
    </div>`).join('');

  // Return volatility bars (Exhibit 04)
  const rets = [
    {name:'AAPL — mean 2.32%', v:7.74},
    {name:'MSFT — mean 2.02%', v:6.06},
    {name:'TSLA — mean 4.70%', v:18.34},
  ];
  const maxStd = 20;
  document.getElementById('retBars').innerHTML = rets.map(r => `
    <div class="bar-item">
      <div class="lbl"><span>${r.name}</span><span>σ ${r.v.toFixed(2)}%</span></div>
      <div class="bar-track"><div class="bar-fill" style="width:${(r.v/maxStd*100).toFixed(0)}%"></div></div>
    </div>`).join('');

  // NPV sensitivity heatmap (Exhibit 01) — WACC (rows) x EBIT margin (cols), $000s
  const margins = [0.07,0.08,0.09,0.10,0.11,0.12,0.13];
  const waccs = [0.06,0.07,0.08,0.09,0.10,0.11,0.12];
  const grid = [
    [5698844,6495834,7292824,8089814,8886804,9683793,10480783],
    [5329640,6075082,6820523,7565964,8311406,9056847,9802288],
    [4994433,5693072,6391711,7090351,7788990,8487629,9186268],
    [4689497,5345561,6001625,6657689,7313752,7969816,8625880],
    [4411567,5028826,5646085,6263344,6880603,7497862,8115121],
    [4157773,4739597,5321421,5903245,6485069,7066893,7648717],
    [3925588,4474994,5024400,5573806,6123213,6672619,7222025],
  ];
  let flat = grid.flat();
  let min = Math.min(...flat), max = Math.max(...flat);
  function cellColor(v){
    const t = (v-min)/(max-min);
    // interpolate paper -> forest
    const c1=[236,231,216], c2=[47,90,76];
    const c = c1.map((c0,i)=>Math.round(c0+(c2[i]-c0)*t));
    return `rgb(${c[0]},${c[1]},${c[2]})`;
  }
  let html = '<table class="heatmap"><tr><th>WACC ↓ / EBIT ％→</th>' +
    margins.map(m=>`<th>${(m*100).toFixed(0)}%</th>`).join('') + '</tr>';
  waccs.forEach((w,i)=>{
    html += `<tr><td class="rowhead">${(w*100).toFixed(0)}%</td>` +
      grid[i].map(v=>`<td style="background:${cellColor(v)}">${(v/1000).toFixed(0)}</td>`).join('') + '</tr>';
  });
  html += '</table>';
  document.getElementById('heatmap').innerHTML = html;
</script>

</body>
</html>
