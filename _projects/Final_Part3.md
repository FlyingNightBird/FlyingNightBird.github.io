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
# The population growth rate in WY
![growth.PNG](https://github.com/FlyingNightBird/FlyingNightBird.github.io/blob/main/assets/pngs/growth.PNG)  
From the data visualization we can see that the growth rate in WY can only remain the current level or keep going down after 2010.  


# The Unemployment Rate in WY  
![unemployment.PNG](https://github.com/FlyingNightBird/FlyingNightBird.github.io/blob/main/assets/pngs/unemployment.PNG)  
The tend of umemployment is to go down despite the peak in 2016.  
![unemployment.PNG](/assets/pngs/unemployment.PNG)

# See the relationship by cities in WY
This interactive visualization shows the relationship between unemployment and population by cities.
<vegachart schema-url="{{ site.baseurl }}/assets/json/population_employment.json" style="width: 100%"></vegachart>  

### citiation  
1. World Population Review. Wyoming Population 2022 (Demographics, Maps, Graphs). Retrieved Dec 1, 2022, from https://worldpopulationreview.com/states/wyoming-population  
2. FileUnemployment.org 2022. Retrieved Dec 1, 2022, from https://fileunemployment.org/dataview/us-monthly-unemployment-rate. 

---

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/FlyingNightBird/FlyingNightBird.github.io/tree/main/assets/json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/FlyingNightBird/FlyingNightBird.github.io/blob/main/python_notebooks/license_visualization.ipynb" text="The Analysis" %}
</div>

