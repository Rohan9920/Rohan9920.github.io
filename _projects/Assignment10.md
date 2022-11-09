---
name: IS 445 - Assignment 10
tools: [Python, altair, vega-lite]
image: assets/pngs/buildings.png
description: Analyze distribution of total no. of floors in buildings in different counties and agencies.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Visualization 1 - Count of buildings binned by floors per county

The below visualization depicts the count of buildings for each category of binner floors in each county. It gives an idea about the structure of buildings in a county. It also gives a hint if a county has more commercial buildings or if it is a more residential area.

In this visualization, I have used the vega-lite json coding style and used 'rect' for marks. My other encodings include County on the X axis and total floors on the Y axis that have been binned.

The default color scheme has been used. The different colors indicate the range of number of buildings from which goes up to 500.

The dataset has been used for the visualization as is. There were no requirements for any external transformations. Null and NA values had been checked and none were found.

The same vega-lite code was chosen from HW9. The specifications had to be added to 
```
alt.Chart.from_dict()
```
and comments had to be replaced from '//' to '#'.

<vegachart schema-url="{{ site.baseurl }}/assets/json/heat_map.json" style="width: 100%"></vegachart>

# Visualization 2 - Number of buildings per agency

The following visualization displays count of buildings per agency. There is atleast 1 record for each agency but due to the short bar height, some of them seem to be 0.

Similar to the above plot, vega-lite coding style has been used in this visualization. 'bar' has been used for marks and other encodings include agency name on the X axis and count of buildings on the Y axis. 

This visualization being a histogram does not have any column for color parameter. The default color scheme has been used.

Similar to the above visualization, no external data transformations were required for this plot. The distribution was straight forward and the dataset could be used as is.

The vega lite specification done for HW9 has been added in 

```
alt.Chart.from_dict()
```

and comments had to be replaced from '//' to '#'.

<vegachart schema-url="{{ site.baseurl }}/assets/json/hist.json" style="width: 100%"></vegachart>

# Visualization 3 - Interactivity

The below visualization consolidates the above 2 plots and demonstrates interactivity between them. The 'brush' parameter has been used as a window selector. The adjacent histogram then adjusts itself based on the window selected.

Using this interactive feature the user can have a look at the ditribution of count of buildings for the desired county or no. of floors. The non-interactive visualization was a bit cluttered and did not allow the user to pick required counties. 

Another addition to this visualization could be adding a dropdown which would allow the user to select a county directly from the list instead of having to find it on the X axis.

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard.json" style="width: 100%"></vegachart>


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Rohan9920/Rohan9920.github.io/blob/main/mudgalkar-rohan-assignment10.ipynb" text="The Analysis" %}
</div>

