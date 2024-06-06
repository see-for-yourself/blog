---
layout: post
title:  "A Statistical Paradox: Covid-19 and Census Data for CA Counties"
date:   2024-04-18
categories: covid-19
---
_Updated: 2024-06-06_

A recent news article [1] reported on some differences in death rates of older people and of racial groups in California. This hints at possible reasons for the counterintuitive _downward_ slopes in following plots of Covid-19 cases and deaths per capita against the percentage of people over age 65 for California counties. The _negative_ correlation seems to contradict the established knowledge that older people are at higher risk of Covid-19.

![Image 1](/blog/assets/images/covid-19/Rplot_cases_v_age-65-over_u-bands-c_2x2_850x450_v01-f.png)  
Data Sources: [2], [3].  

Whether or not you have come across this kind of statistical paradox before – also known as Robinson's Paradox – it is interesting to think about what is specifically happening here in CA counties with the demographics and health disparities concerning race and poverty that may be involved. As reported in the news article [1], the Latino population is younger but has higher death rate (early in the pandemic) than Whites. So if a county has a larger percentage of old people and a smaller percentage of Latinos, it may have a _lower_ death per capita than a county with smaller percentage of old people and a larger percentage of Latinos. In order to check this, one would need the breakdown of the number of deaths by race in each county, which is not provided by the Johns Hopkins dataset [2].

---

In any case, it is not hard to construct a simple example to illustrate this statistical paradox with explicit numbers.

Imagine a state S comprising two counties C1 and C2, each with population 100,000. We label some people with characteristic "O" and some with "G" to form groups O and G, respectively.  Some people may belong to both groups. To be less abstract and make things easier to follow, we can think of O as old people with age over 65, and G as people with green skin (so as not to confuse this hypothetical example with a real racial group).

Let the populations of the two counties C1 and C2 be given by the following tables:

| C1 population | in O | not in O | TOTAL  
| --- | --- | --- | ---
| in G | 8,077 | 61,923 | 70,000
| not in G | 6,923 | 23,077 | 30,000
| TOTAL | 15,000 | 85,000 | 100,000

| C2 population | in O | not in O | TOTAL  
| --- | --- | --- | ---
| in G | 1,053 | 8,947 | 10,000
| not in G | 18,947 | 71,053 | 90,000
| TOTAL | 20,000 | 80,000 | 100,000

And with the number of deaths given by:

| C1 deaths | in O | not in O | TOTAL  
| --- | --- | --- | ---
| in G | 187 | 52 | 239
| not in G | 50 | 12 | 62
| TOTAL | 237 | 64 | 301

| C2 deaths | in O | not in O | TOTAL  
| --- | --- | --- | ---
| in G | 35 | 7 | 42
| not in G | 193 | 36 | 229
| TOTAL | 228 | 43 | 271

From the table, county C1 has deaths per capita (per 100,000) of 301, which is _higher than_ county C1's 271, despite C1 having a _lower_ percentage of people over 65 (with 15% in O) than C2 (with 20% in O).

![Image 2](/blog/assets/images/covid-19/Rplot_C1-C2_deaths_v_age-65-over_450x450_v01-f.png)  

Moreover, the parameters are plausible.  In C1 and in C2, the percentages of the population over 65 and of green-skinned are within the wide range of the numbers in California counties for over 65 and for some racial groups.  The ratios of the death rates for over 65 and for not over 65 are approximately 20, which is similar to the ratio in the U.S. based on the numbers on the CDC website [4] (and the fact that about 17% of the U.S. are over 65).  The ratios of the death rates for green skinned and for not green skinned are approximately 5/3, which is similar to the ratio of death rates due to certain racial disparities in California based on the numbers in the news article [1].

## References

1. SJ Mercury News. "Who's dying now? Here's how recent COVID deaths compare to the early months of the pandemic in California", 4/15/2024. [URL](<https://www.mercurynews.com/2024/04/15/whos-dying-now-heres-how-recent-covid-deaths-compare-to-the-early-months-of-the-pandemic-in-california/>)
2. Johns Hopkins Center for Systems Science and Engineering (CSSE). Covid-19 datasets: [URL](<https://coronavirus.jhu.edu/about/how-to-use-our-data>) (data collection stopped 2023-03-10)
3. United States Census Bureau. [URL](<https://data.census.gov>)
4. CDC. Covid-19: People with Certain Medical Conditions. [URL](<https://www.cdc.gov/coronavirus/2019-ncov/need-extra-precautions/people-with-medical-conditions.html>)
