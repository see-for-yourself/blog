---
layout: post
title:  "Heatwaves in Southwest US and Southern Europe"
date:   2026-10-12
categories: climate-change
---
[_Updated: 2023-08-10, 2026-10-12_]

The Intergovernmental Panel on Climate Change (IPCC) has projected that "future heatwaves will last longer and have higher temperatures" in a report in 2021 [6]. We can make some visualizations of heatwaves to see this phenomenon using temperature data from the National Oceanic and Atmospheric Administration (NOAA) [1], with the available data up to August 2026.

There is no single standard definition of a _heatwave_. One definition that we will use for the visualizations below is attributed to the World Meteorological Organization (WMO) [2-4] and defines a heatwave as 5 or more consecutive days in which the daily max temperature exceeds by 5°C (9°F) the normal max (averaged over a 30-year baseline period such as 1961-1990). This definition is straightforward to compute, and it takes into account the local and seasonal conditions. More sophisticated but harder to formalize definitions may also consider thresholds based on human perceptions of "hot" by the local people, the capacity of the local environment to store and release heat, etc. [4-5].

For the Southwest US, heatwaves for Austin, Las Vegas, and Phoenix are visualized in Image 1. Each heatwave is represented by a circle, with the height indicating its temperature and the size its duration. Looking at these plots, it is noticeable that the top-right area of all three plots contains the higher and larger circles, indicating a trend of hotter and longer heatwaves.

![Image 1](/blog/assets/images/climate-change/plot-3x1_Austin-LasVegas-Phoenix_1933-2026_heatwaves-groups_dark_v02-c.png)  
_Image 1: Baseline period 1961-1990. Data Source: NOAA [1]_

In these visualizations, the NOAA [1] has data for the daily max temperature. We compute the heatwaves by grouping consecutive days that exceed the normal max by 5°C (9°F). For the 30-year baseline, a commonly used period is 1961-1990. For each city, we use a single weather station. Specifically: Austin Camp Mabry (1938-06-01 to 2026-08-31), Las Vegas Harry Reid Airport (1948-09-06 to 2026-08-31), Phoenix Airport (1933-06-01 to 2026-08-31). The gray vertical lines and areas in the plots are dates for which the daily max temperature is unavailable or missing.

More striking visualizations of heatwaves can be seen for Southern Europe. Heatwaves for Athens, Madrid, and Rome are visualized in Image 2:

![Image 2](/blog/assets/images/climate-change/plot-3x1_Athens-Madrid-Rome_1933-2026_heatwaves-groups_dark_v02-c.png)  
_Image 2: Baseline period 1961-1990. Data Source: NOAA [1]_

The wide swaths of gray on the right side of the Athens and Rome visualizations indicate unavailable data for the daily max temperature. There is a moderate amount of missing data for the weather station in Athens (10.0% at Hellinikon station from 1955-01-01 to 2025-08-24) and in Rome (10.5% at Roma Ciampino station from 1951-01-01 to 2025-08-24). However, since almost all of the data in the baseline period (1961-1990) is available, these visualizations are still valid. Furthermore, in the gray swaths on the right side of the Athens and Rome visualizations where we can see more heatwaves than in earlier years, it is possible that there are even more heatwaves that are not detected due to the gaps caused by the unavailable data.

For some other places in the world that are known to be hot, such as Khartoum in Sudan or New Delhi in India, there is a large amount of dates with missing daily max temperature data (70.0% at Khartoum station from 1957-07-01 to 2023-04-15) and (40.6% at New Delhi Safdarjun station from 1944-01-01 to 2025-08-24) in the NOAA data [1], and these would not make accurate visualizations of the heatwaves.

## Hottest 100 Days and Heatwaves

We can also visualize the hottest 100 days for each place using the same data as above, and mark (in red) which of those days belong to heatwaves. See Images 3 and 4. The red circles are concentrated on the right side of the plots, and the pattern is clear that in these cities in the Southwest US and Southern Europe, there are increasingly more hottest-100 days that are part of a heatwave.

![Image 3](/blog/assets/images/climate-change/plot-3x1_Austin-LasVegas-Phoenix_1933-2026_Hottest-100_dark_v02-c.png)  
_Image 3: Baseline period 1961-1990. Data Source: NOAA [1]_

![Image 4](/blog/assets/images/climate-change/plot-3x1_Athens-Madrid-Rome_1933-2026_hottest-100_dark_v02-c.png)  
_Image 4: Baseline period 1961-1990. Data Source: NOAA [1]_

## References

1. NOAA Climate Data Online (CDO). [URL](https://www.ncdc.noaa.gov/cdo-web/)
2. _Wikipedia_. Heat wave definitions. [URL](https://en.wikipedia.org/wiki/Heat_wave#Definitions)
3. "heat wave". _Encyclopædia Britannica_. [URL](https://www.britannica.com/science/heat-wave-meteorology)
4. WMO. "Extreme Heat". [URL](https://wmo.int/themes/extreme-heat)
5. GHHIN. "Understanding Heatwaves: Beyond Extreme Temperatures". [URL](https://heathealth.info/news/understanding-heatwaves-beyond-extreme-temperatures/)
6. IPCC. "Will Unprecedented Extremes Occur As a Result Of Human-Induced Climate Change?"  _IPCC Sixth Assessment Report (AR6), Frequently Asked Questions, FAQ 11.2. (2021)_ [URL](https://www.ipcc.ch/report/ar6/wg1/downloads/faqs/IPCC_AR6_WGI_FAQs_Compiled.pdf)
