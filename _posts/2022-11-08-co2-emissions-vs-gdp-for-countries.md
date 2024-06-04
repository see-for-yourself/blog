---
layout: post
title:  "CO2 emissions vs. GDP for countries"
date:   2022-11-08
categories: climate-change
---
_Updated: 2023-11-21, 2024-03-23_

More economically developed countries with higher Gross Domestic Product (GDP) per capita tend to have higher carbon dioxide (CO2) emissions per capita. A regression analysis for the year 2020 is shown in the images below.

Traditional least squares regression with uncertainty bands (see [3]) is shown in Image 1.  The inner bands, displayed as dash lines with longer dashes, are the confidence bands (based on the standard error). The outer bands are the prediction bands (based on +/- 2 standard deviations).

Bayesian inference is used to perform the regression (see [4]) shown in Image 2. This enables visualization of the posterior uncertainty of the regression line (shown by the gray lines in the plot). The uncertainty lines are tight around the regression line and have slopes away from zero, suggesting that there is a high probability of an association between GDP per capita and CO2 emissions.

With the plots in log-log scales, the result can be interpreted as for each 1% increase in GDP, the predicted increase in CO2 emissions is 0.63%.

Since a number of developing countries have large populations (although the birthrate may fall as a country becomes more wealthy), economic development in a sustainable way will be important to meet climate targets.

![Image 1](/blog/assets/images/climate-change/gdp_fit_loglog_country_CO2_GDP_2020_bands_2211v3.png)  
Image 1: Slope: Median = 0.63, Std. Error = 0.03. Residual standard error = 0.44. p-value: < 2.2e-16. Data Sources [1-2]

![Image 2](/blog/assets/images/climate-change/gdp_fit_loglog_country_CO2_GDP_2020_2211v3.png)  
Image 2: Slope: Median = 0.63, MAD_SD = 0.03. Sigma: Median = 0.44, MAD_SD = 0.02 . Data Sources [1-2]

## References

1. Our World in Data. <https://ourworldindata.org/co2-emissions>
2. World Bank. <https://data.worldbank.org>
3. Dalgaard, P. _Introductory Statistics with R_. (2002) Springer-Verlag.
4. Gelman, A., Hill, J., Vehtari, A. _Regression and Other Stories_. (2020) Cambridge University Press.
