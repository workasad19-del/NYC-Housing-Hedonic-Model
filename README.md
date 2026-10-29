# Hedonic Pricing Model: NYC Real Estate Valuation

OLS hedonic pricing model of New York City rents: the effect of apartment size, subway distance and a Manhattan location on monthly rent.

*Research Methods project, MSc Economics and Political Science, University of Milan (December 2025).*

## Abstract

This project applies **multiple linear regression (OLS)** to quantify how structural and locational attributes affect rental prices in New York City. It asks whether the "Manhattan Premium" outweighs apartment size and subway convenience as a driver of rent.

## Methodology

The study uses the **hedonic pricing framework** (Rosen, 1974) to break an apartment's price into its characteristics, following Diewert and Shimizu (2016).

### Estimating equation

```
Price = β0 + β1(Size) + β2(Distance) + β3(Manhattan) + u
```

| Variable | Definition |
|---|---|
| Price | Monthly rent (USD) |
| Size | Floor area (sq ft) |
| Distance | Walking time to nearest subway station (minutes) |
| Manhattan | Dummy: 1 if in Manhattan, 0 if in Brooklyn, Queens or the Bronx |

### Data

Cross-sectional sample of 100 listings (2023) drawn at random from Zillow: 48 in Manhattan and 52 in the outer boroughs.

### Key issues addressed

- **Omitted variable bias (OVB):** Derives the bias formula and compares a naive model (Price on Size only) with the full model, to show how the size coefficient changes once location and convenience are controlled for.
- **Distribution of prices:** Rent is right-skewed (skewness about 1.68, kurtosis about 5.6), with a small number of luxury listings pulling the mean (about $4,605) above the median ($3,575).
- **Multicollinearity:** Manhattan and subway distance are correlated (about -0.59), and this is taken into account when interpreting the coefficients.

## Preliminary findings (correlations with rent)

- Size: 0.85
- Manhattan: 0.64
- Distance to subway: -0.36

Rent rises with size and in Manhattan, and falls as the walk to the subway gets longer. Regression results and diagnostics are in the paper.

## Full paper

[Determinants of Housing Prices in New York City (PDF)](./Determinants%20of%20Housing%20Prices%20in%20New%20York%20City%20By%20Asad%20khan.pdf)

## Tools

- Stata (OLS, correlation and summary statistics)
- Data source: Zillow (random sample, n = 100)

---

*Author: Asad Khan*
