Shachi Shah — Finance & Analytics Portfolio

Selected coursework and independent analysis
Equity valuation · Cash-flow analysis · Portfolio theory · Quantitative coding

Email · LinkedIn · Riverside, CA
Updated July 2026

About this portfolio

I build the model, not just read it.

The four projects below were built through coursework and self-study in corporate finance, valuation, and applied statistics. Each starts with raw data—public filings, market returns, or a case dataset—and works toward a defensible result: an intrinsic value, a cash-flow bridge, a portfolio beta, or a sampling distribution.

Full workbooks and notebooks are available on request.

Core skills

DCF & DDM valuation · CAPM & beta estimation · Cash-flow reconciliation · Python · pandas · NumPy · Matplotlib · Monte Carlo sampling · Sensitivity analysis · Excel financial modeling · Statistical inference

01 — DICK'S Sporting Goods (DKS)

Equity valuation and new-venture appraisal

Built a valuation model from DKS's historical income statement and balance sheet, projecting revenue, margins, and free cash flow. Estimated the cost of equity through CAPM using a five-year beta, the 10-year U.S. Treasury yield as the risk-free rate, and an equity-risk-premium assumption. Estimated the cost of debt from DKS's bond coupons, then calculated WACC using market-value weights of debt and equity.

Cross-checked the DCF result against a dividend discount model. Separately evaluated an in-store sports-equipment service bay as a standalone capital project, including equipment and certification costs, revenue per store, NPV, IRR, and a two-way sensitivity analysis across WACC and EBIT margin.

Methods: CAPM WACC DCF DDM NPV IRR Sensitivity tables

Core valuation outputs

Metric

Result

WACC

8.55%

Cost of equity (CAPM)

9.97%

Five-year beta

1.20

DDM intrinsic value per share

$72.35

New-venture NPV

$6.99M

New-venture IRR

7.64%

Payback period

9 years

<details>
<summary><strong>NPV sensitivity: WACC × EBIT margin ($000s)</strong></summary>

WACC ↓ / EBIT margin →

7%

8%

9%

10%

11%

12%

13%

6%

5,699

6,496

7,293

8,090

8,887

9,684

10,481

7%

5,330

6,075

6,821

7,566

8,311

9,057

9,802

8%

4,994

5,693

6,392

7,090

7,789

8,488

9,186

9%

4,689

5,346

6,002

6,658

7,314

7,970

8,626

10%

4,412

5,029

5,646

6,263

6,881

7,498

8,115

11%

4,158

4,740

5,321

5,903

6,485

7,067

7,649

12%

3,926

4,475

5,024

5,574

6,123

6,673

7,222

</details>

02 — Cash-Flow Reconciliation

Net income to free cash flow

Starting with a two-year income statement and balance sheet, reconstructed the indirect-method cash-flow statement. Added back depreciation; analyzed changes in receivables, inventory, and payables; calculated operating cash flow; and incorporated investing and financing activity to reconcile the ending cash balance.

Used the completed statement to derive free cash flow (after capital expenditures) and free cash flow to equity (after net debt activity), illustrating why net income, EBITDA, and FCF can tell different stories about the same company in the same year.

Methods: Indirect-method cash flow Working capital FCF vs. FCFE Statement tie-out

FY2025 reconciliation ($M)

Item

Amount

Net income

5,220

Depreciation

3,750

Working-capital adjustments

4,000

Cash from operations

12,970

Investing activity

(10,000)

Financing activity

36,000

Net change in cash

38,970

Free cash flow

2,970

Free cash flow to equity

8,970

03 — Student-Managed Fund Stock Screen

Risk, return, and CAPM

Completed a Darden School of Business case exercise involving four candidate holdings for a student-managed equity fund. Estimated each stock's beta by regressing five years of monthly returns against the S&P 500 using ordinary least squares, then compared market-implied risk with historical volatility, dividend yield, credit rating, and valuation multiples.

Used CAPM to estimate required returns and benchmarked the candidates against long-run asset-class risk-and-return data. Evaluated the trade-off between a high-beta cyclical stock and a lower-beta defensive stock in a two-stock portfolio.

Methods: OLS regression Beta estimation CAPM Risk-return analysis Portfolio construction

Candidate screen

Company

Industry

Estimated beta

Delphi

Auto parts

1.29

Groupon

Internet

1.44

Kellogg

Packaged foods

0.54

Kinross Gold

Mining

0.31

Long-run benchmark, 1926–2016

Asset class

Geometric mean return

U.S. Treasury bills

3.4%

Long-term corporate bonds

6.0%

Large-cap equities (S&P)

10.1%

04 — 20-Year Return Simulation

AAPL, MSFT, and TSLA

Pulled monthly price and volume data with yfinance, then used pandas to calculate monthly returns and descriptive statistics for Apple, Microsoft, and Tesla.

Drew repeated 500-observation samples from historical returns and tracked how the distribution of sample means tightened around the population mean as the number of resamples increased—a practical demonstration of the Central Limit Theorem. Repeated the analysis with winsorized returns to study how limiting outliers changes the distribution's shape without substantially shifting its center.

Methods: yfinance pandas NumPy Matplotlib Central Limit Theorem Winsorization Resampling

Monthly return profile, 2010–2024

Security

Mean monthly return

Standard deviation

Apple (AAPL)

2.32%

7.74%

Microsoft (MSFT)

2.02%

6.06%

Tesla (TSLA)

4.70%

18.34%

Sampling experiment

500 observations per sample; 1,000 draws

Metric

Result

AAPL population mean

2.32%

Mean of sample means

2.33%

Standard deviation of sample means

0.34%

Standard deviation of raw returns

7.74%

Toolkit

Area

Capabilities

Financial modeling

Three-statement models, DCF, DDM, comparable-company analysis, NPV/IRR capital budgeting, and scenario and sensitivity tables in Excel

Programming

Data collection, cleaning, analysis, and visualization with Python, pandas, NumPy, Matplotlib, SciPy, and statsmodels

Statistics

OLS regression, beta estimation, hypothesis testing, resampling, the Central Limit Theorem, and winsorization

Corporate finance

CAPM, WACC, capital-structure weighting, cash-flow-statement reconciliation, FCF, and FCFE

Markets

Equity risk premiums, portfolio beta, risk-return trade-offs, and long-run asset-class benchmarking

Communication

Translating detailed financial models into concise, decision-ready recommendations

Every number on this page came from a model I built and can walk through line by line.

Full workbooks and notebooks available on request.
