---
name: IS 445 - Final Project
tools: [Python, altair, vega-lite]
image: assets/pngs/spill_accidents.png
description: Analyze distribution of total no. of floors in buildings in different counties and agencies.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Do you need to worry about spill accidents? 

<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/interactive_viz.json" style="width: 100%"></vegachart>

## Explanation of the visualization:

Accidents caused due to spill of hazardous materials lead to severe side effects to human life and to the natural environment. The above visualization depicts how has the trend of spill accidents been over the past years in Illinois. To make the visualization easy to interpret, only the top 10 densely populated counties have been chosen.

The desired county can be chosen from the dropdown and the visualization adjusts itself to display the number of spill accidents caused over the past years. The visualization is an interactive bar graph with the default color scheme. These incidents cover all the accidents caused due to leaks, spills, ruptures in containers, illegal dumps, abondoned bags, etc. 

Now, circling back to the title of this visualization. Yes, spill accidents are a matter of concern. The number of spill accidents is high in the counties in Illinois. Some of the counties recorded more than 1000 accidents. Moreover, these were only the incidents that were reported. There could be many such accidents that never made it to the record books.

*Note: The X axis and Y axis limit may change if you change the county from the dropdown.* 

The central visualization is limited to the accidents reported in the state of Illinois. The contextual visualizations further broaden this study and give a detailed information about the accidents reported in all the states of the USA. Both of the below visualizations have been taken from the official website of the US Department of Transportation.

## Context visualization 1:

<img src='/assets/pngs/cv1.png'>

The above visualization displays the heatmap of hazardous liquid accidents in the US. Texas and Oklahoma seem to be the hot spots for these accidents. Western states reported very low number of accidents. 

## Context visualization 2:

<img src='/assets/pngs/cv2.png'>

This visualization shows the complex network of pipelines throughout the United States. This would help understand which states would be more prone to accidents and preventive measures can be applied accordingly. There seems to be a heavy network of hazardous liquid in the state of Illinois.

The contextual visualizations analyze the liquid accidents in the United States supplementing the interactive visualization that focuses on all types of hazardous accidents and spills in Illinois. 

*Note: The python analysis notebook was going beyond the 100 MB github upload limit. The dataset was occupying 37 MB of space. However, the resulting ipynb notebook ended up consuming 110 MB of space. I had to switch to git lfs to accomodate my analysis file. However, it is not being rendered properly on github. Users would need to download the file to access the code to the interactive visualization.*


### References:

1. Data Visualization Overview. PHMSA. (n.d.). Retrieved December 3, 2022, from <https://www.phmsa.dot.gov/data-and-statistics/pipeline/data-visualization-overview>  

2. So, K., Christianson, A., Villagomez, A., Rowland-Shea, J., Jackson, C., Sozan, M., Murphy, N., &amp; Jarsulic, M. (2022, October 4). 10 years after Deepwater Horizon, oil spills and accidents are on the rise. Center for American Progress. Retrieved December 3, 2022, from <https://www.americanprogress.org/article/10-years-deepwater-horizon-oil-spills-accidents-rise/> 


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/Rohan9920/Rohan9920.github.io/main/iema_hazardous_material_spills.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Rohan9920/Rohan9920.github.io/blob/main/mudgalkar-rohan-FinalProject-3.ipynb" text="The Analysis" %}
</div>

