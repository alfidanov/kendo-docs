---
title: Scatter Chart
meta_title: Guide for using HTML5 Scatter Charts 
meta_description: How to use Scatter and Scatter Line charts in Kendo UI DataViz.
slug: chart-scatter-type
publish: true
---

## XY Scatter Charts

The Scatter and Scatter Line series are suitable for plotting two-dimensional data.

Each data point is an array that contains two values - X and Y.

### Scatter Line Chart

    $("#chart").kendoChart({
        title: {
            text: "Charge current vs. charge time"
        },
        legend: {
            visible: true
        },
        seriesDefaults: {
            type: "scatterLine"
        },
        series: [{
            name: "0.8C",
            data: [[10, 10], [15, 20], [20, 25], [32, 40], [43, 50], [55, 60], [60, 70], [70, 80], [90, 100]]
        }, {
            name: "1.6C",
            data: [[10, 40], [17, 50], [18, 70], [35, 90], [47, 95], [60, 100]]
        }, {
            name: "3.1C",
            data: [[10, 70], [13, 90], [25, 100]]
        }],
        xAxis: {
            max: 90,
            labels: {
                format: "{0}m"
            },
            title: {
                text: "Time"
            }
        },
        yAxis: {
            max: 100,
            labels: {
                format: "{0}%"
            },
            title: {
                text: "Charge"
            }
        }
    });


Produces the following Scatter Line chart.

 ![Scatter Line Chart](chart-scatter-line.png)

#### Dash type

The default line type is solid. The following dash styles are available through the "dashType" option:

![Dash Type](chart-dash-types.png)

For example:

    series: [{
        name: "World",
        data: [15.7, 16.7, 20, 23.5, 26.6],
        dashType: "dot"
    }]


### Scatter Chart

Specifying "scatter" instead of "scatterLine" will remove the connecting lines

![Scatter Chart](chart-scatter.png)
