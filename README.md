# empirical-capm-analysis

Empirical analysis of CAPM model in Python using historical stock data 

---

## Motivation
The Capital Asset Pricing Model (CAPM) is a foundational model in financial economics, widely used to describe the relationship between expected return and systematic risk. Despite its theoretical elegance, CAPM is known to face challenges when applied to real-world data. This project investigates how well CAPM performs empirically using historical stock market data.

## Research Questions
This project seeks to answer the following questions:
- How can CAPM be estimated empirically using historical data?
- How stable is the estimated beta over time?
- Under what conditions does CAPM appear to break down?

## Methodology
- Historical price data is collected using the `yfinance` library.
- Returns are computed from adjusted closing prices when available.
- CAPM parameters (alpha and beta) are estimated using linear regression.
- Rolling-window regressions are used to analyze time variation in beta.

## Key Concepts
- Systematic risk (beta)
- Market returns
- Linear regression
- Rolling estimation

## Results and Discussion
The analysis shows that while CAPM provides a reasonable first-order approximation of risk, beta is not stable over time. Rolling estimates reveal significant variation, highlighting one of the main motivations behind multi-factor asset pricing models.

## Limitations
- CAPM relies on strong assumptions such as a single risk factor and frictionless markets.
- Results are sensitive to the choice of time period and market proxy.
- This project focuses on a single stock and does not generalize across assets.

## Conclusion
CAPM remains a useful pedagogical and baseline empirical model, but its empirical limitations become evident when beta instability is examined. These findings motivate the use of more advanced multi-factor models in applied finance.

## Technologies Used
- Python
- NumPy
- Pandas
- yfinance
- Matplotlib

## How to Run
1. Clone the repository.
2. Install required dependencies.
3. Run the Jupyter notebook or Python script to reproduce the analysis.
