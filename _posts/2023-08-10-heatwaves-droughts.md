---
layout: post
title:  "Looking for Heatwaves and Droughts"
date:   2023-08-10
categories: climate-change
---
_Updated: 2023-09-05, 2024-06-21_

This post concerns extreme weather events, in particular heatwaves and droughts.

Extreme events are by definition rare. And they are not easy to define precisely. Even for the related concept of "outlier", in general there is no statistical or mathematical definition that works well in all applications.

One notable kind of extreme weather event is a **heatwave**. There is no single standard definition of a heatwave. One definition attributed to the World Meteorological Organization is 5 or more consecutive days with daily max exceeding the normal max (for a 30-year baseline period) by 5°C (9°F). See [H2-H4].

It is interesting to see which very hot days are or are not actually heatwave days. We can take the top 1% hot days over a dataset's period, and highlight those that are within a heatwave by the above definition. Note that this filters out moderately warm days in the winter which might be categorized as a heatwave by the above definition, but subjectively would not feel like a heatwave.

Image 1 shows the results for various cities in the vicinity of Southwest U.S., and Image 2 for cities in Southern Europe. There appears to be more extreme weather events in the more recent years in the case of heatwaves during days with the highest temperatures.

![Image 1](/blog/assets/images/climate-change/ehe_Cities_1951-2023_TMAX_4_06-a_LPAA_2308v1.png)  

![Image 2](/blog/assets/images/climate-change/ehe_Cities_1955-2023_TMAX_4_06-a_MMRA_2308v1.png)  
Images 1-2: Data Sources [H1]

---

**Droughts**, unlike heatwaves, are persistent and can last an extended period of time. A drought is broadly defined as drier than normal, and it depends on the local conditions of a place (see [D3]).

We can visualize droughts by using level curves based on drought length. A day is counted as belonging to level k if the closest day with rain is at least k days.

Image 3 shows the results for cities in vicinity of Southwest U.S., and Image 4 for the cities in Southern Europe.

According to the IPCC report in 2021 [D3], in the Southwest U.S. and in Southern Europe (and in a number of regions around the world), drought is expected to increase under future warming, as precipitation is expected to decline as the world warms. In our level curve visualizations from the 1950s to 2022, this is not yet clearly noticeable (except for Marseilles and perhaps Las Vegas).

![Image 3](/blog/assets/images/climate-change/dl_Cities_1951-2022_drought-levels_03-d_LPAA_2308v1.png)  

![Image 4](/blog/assets/images/climate-change/dl_Cities_1955-2022_drought-levels_03-d_MMRA_2308v1.png)  
Images 3-4: Data Sources [D1]

## References

H. Heatwaves

1. NOAA Climate Data Online (CDO). [URL](https://www.ncdc.noaa.gov/cdo-web/)
2. Wikipedia. Heat wave definitions. [URL](https://en.wikipedia.org/wiki/Heat_wave#Definitions)
3. "heat wave". Encyclopaedia Britannica. [URL](https://www.britannica.com/science/heat-wave-meteorology)
4. WMO. New Two-Tier approach on "climate normals". 2015. [URL](https://public.wmo.int/en/media/news/new-two-tier-approach-%E2%80%9Cclimate-normals%E2%80%9D)
5. IPCC. "Why Are Cities Hotspots of Global Warming?"  IPCC Sixth Assessment Report (AR6). Frequently Asked Questions, FAQ 10.2. 2021. [URL](https://www.ipcc.ch/report/ar6/wg1/downloads/faqs/IPCC_AR6_WGI_FAQs_Compiled.pdf)

D. Droughts

1. NOAA Climate Data Online (CDO). [URL](https://www.ncdc.noaa.gov/cdo-web/)
2. AMETSOC. "rain day". [URL](https://glossary.ametsoc.org/wiki/Rain_day)
3. IPCC. " What Causes Droughts, and Will Climate Change Make Them Worse?"  IPCC Sixth Assessment Report (AR6). Frequently Asked Questions, FAQ 8.3. 2021. [URL](https://www.ipcc.ch/report/ar6/wg1/downloads/faqs/IPCC_AR6_WGI_FAQs_Compiled.pdf)
