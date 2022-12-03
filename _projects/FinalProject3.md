---
name: IS 445 - Final Project
tools: [Python, altair, vega-lite]
image: assets/pngs/buildings.png
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

Accidents caused due to spill of hazardous materials leads to severe side effects to human life and to the natural environment. The above visualization depicts how has the trend of spill accidents been over the past years in Illinois. To make the visualization easy to interpret, only the top 10 densely populated counties have been chosen.

The desired county can be chosen from the dropdown and the visualization adjusts itself to display the number of spill accidents caused over the past years. These incidents cover all the accidents caused due to leaks, spills, ruptures in containers, illegal dumps, abondoned bags, etc. 

Now, circling back to the title of this visualization. Yes, spill accidents are a matter of concern. The number of spill accidents is huge in the counties in Illinois. The count rose to over 1000 in COOK county in the years 1990 - 1994. These were the incidents that were reported. There could be many such accidents that never made it to the record books.

**Note: The X axis and Y axis limit may change if you change the county from the dropdown.** 

However, the central visualization does not convey a clear picture of casualties and financial damages caused in these accidents. The contextual visualizations convey this valuable information. The contextual visualization is not restricted to any county. It displays the consolidated records for Illinois state inclusive of all the counties.

## Context visualization 1:

<img src='/assets/pngs/injuries.png'>


The first contextual visualization depicts the number of injuries cuased due to hazardous materials spill accidents. These injuries rose to 400 in the year 2015. 

## Context visualization 2:

<img src='/assets/pngs/damages.png'>


The second contextual visualization displays the financial damages caused due to these accidents. Just a mere glance at the visualization shows that there have been high financial damages with 95M$ being the highest in the year 2015.


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/Rohan9920/Rohan9920.github.io/main/iema_hazardous_material_spills.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Rohan9920/Rohan9920.github.io/blob/main/mudgalkar-rohan-assignment10.ipynb" text="The Analysis" %}
</div>

