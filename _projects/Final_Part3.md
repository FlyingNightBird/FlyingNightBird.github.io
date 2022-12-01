---
name: How unemployment rate has effects on population in WY
tools: [Python, HTML, vega-lite]
image: assets/pngs/final.PNG
description: final project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

Group member: Jiahao Tian/Zhuokun He  
The population growth rates in Wyoming is one of the highest. Wyoming also has an unemployment rate below average.
These elements may make the relationship between unemployment and population more clear in Wyoming.
First, Let's check the population growth rate in Wyoming by a glance.
# The population growth rate in WY
![growth.PNG](/assets/pngs/growth.PNG) 
Due to the data visualization, the population growth rate keeps going down in the history.
If we focus on the performance of growth rate in recent years, we can see that the growth rate in WY can only remain the current level or keep going down after 2010.  
But the population growth rate is still positive even through it has shrunk to 0.2%.  
So what happens to the unemployment rate in recent years? 
# The Unemployment Rate in WY  
![unemployment.PNG](/assets/pngs/unemployment.PNG)  
Through there is a peak in 2016, the tend of umemployment rate keeps going down until Covid-19 comes.
The average rate from 2014 to 2020 should be about 4.5%.
It seems that low unemployment can't stop the population growth rate from dropping, but notice that we can't say low unemployment rate doesn't have postive effect on population growth. There is possibility that it has positive effect but not has enough effect. So Let's see the population growth in a more specific way.
# See the relationship by cities in WY
This interactive visualization shows the relationship between unemployment and population by cities.
<vegachart schema-url="{{ site.baseurl }}/assets/json/population_employment.json" style="width: 100%"></vegachart>  

<center>Citiation</center>
1. World Population Review. Wyoming Population 2022 (Demographics, Maps, Graphs). Retrieved Dec 1, 2022, from https://worldpopulationreview.com/states/wyoming-population  
2. FileUnemployment.org 2022. Retrieved Dec 1, 2022, from https://fileunemployment.org/dataview/us-monthly-unemployment-rate  
3. DATA.GOV 2022. Retrieved Dec 1, 2022, from https://catalog.data.gov/dataset/atlas-of-rural-and-small-town-america  
---

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/FlyingNightBird/FlyingNightBird.github.io/tree/main/assets/json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/FlyingNightBird/FlyingNightBird.github.io/blob/main/python_notebooks/license_visualization.ipynb" text="The Analysis" %}
</div>

