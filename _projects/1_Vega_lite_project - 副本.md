---
name: Vega Lite Example Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/visualization.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# 1. Number of License Type
 This data visualization shows the number of different License Types, and we can see that about three kinds of licenses occupy most of the whole.

The data of the x-axis is License Type, and the data type is Nominal. The y-axis and the interactive count line are the number of License Type, and the data type is quantitative. In this chart, the original color of the bar is orange, if not checked, the bar will be gray. Although I did not use python to process the raw data, in the chart I aggregated the License Type.

Inside this char, the interactivity I added is an auxiliary line. This line will display the total number of selected License Types, which can help users better analyze the number of specific License Types.


<vegachart schema-url="{{ site.baseurl }}/assets/json/number_of_license.json" style="width: 100%"></vegachart>

---
# 2. Scatter for Effective Time and Expiration Time of License
This data visualization shows the relationship between the License's Effective Time and Expiration Time. As can be seen from the figure, the validity period of most licenses after 1980 is similar.

In this chart, Effective Time and Expiration Time are both temporal data, and License Status is nominal data. I color the points in the figure based on License Status. This can help users understand the status characteristics of licenses in different time periods and help them analyze data. Since the expiraiton times of some of the data points are anomalous, I limited the time range to 1975 to 2050.

The interactivity of this chart is tooltip and brush. Users can learn the License Type of each data point through the tooltip. It is also possible to observe data points within a specific time range through selection. This can enrich the amount of information that the chart can provide, and can also improve the efficiency of user analysis of data.

<vegachart schema-url="{{ site.baseurl }}/assets/json/effective_time.json" style="width: 100%"></vegachart>

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/FlyingNightBird/FlyingNightBird.github.io/tree/main/assets/json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/FlyingNightBird/FlyingNightBird.github.io/blob/main/python_notebooks/license_visualization.ipynb" text="The Analysis" %}
</div>

