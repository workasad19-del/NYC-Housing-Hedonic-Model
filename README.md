# Hedonic Pricing Model: NYC Real Estate Valuation

## Abstract
This project applies **Multivariate Linear Regression (OLS)** to quantify the impact of structural and locational attributes on rental prices in New York City. Specifically, it isolates the "Manhattan Premium" and the marginal cost of distance from subway transit hubs.

## Methodology
The study utilizes a **Hedonic Pricing Framework** (Rosen, 1974) to decompose the value of a property into its constituent characteristics.

### Econometric Specification
The primary estimating equation is defined as:

$$Price = \beta_0 + \beta_1(Size) + \beta_2(Distance) + \beta_3(Manhattan) + u$$

### Key Challenges Addressed
* **Omitted Variable Bias (OVB):** Controlled for *Distance to Subway* to correct the bias on the *Size* coefficient, addressing the correlation between outer-borough location and square footage.
* **Distributional Analysis:** Analyzed Skewness and Kurtosis to quantify the fat-tailed distribution of luxury real estate prices in the CBD.

## Results
* **Manhattan Premium:** The model identified a statistically significant premium for CBD location, holding structural quality constant.
* **Distance Decay:** Verified a negative non-linear relationship between rent prices and walking distance to transit.

## Tools Used
* **Econometrics:** Stata / Python (Pandas, Statsmodels)
* **Data Source:** Zillow (Random Sample, n=100)

---
*Author: Asad Khan*
*[Link to Full Research Paper (PDF)](Determinants%20of%20Housing%20Prices%20in%20New%20York%20%20ASAD.pdf)*

