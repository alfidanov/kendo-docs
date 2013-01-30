---
title: ChartValueAxisItemLabels
slug: php-ChartValueAxisItemLabels
tags: api, php
publish: true
---

# \Kendo\Dataviz\UI\ChartValueAxisItemLabels

A PHP class representing the labels setting of ChartValueAxisItem.


## Methods

### background
The background color of the labels. Any valid CSS color string will work here, including
hex and rgb
#### Parameters

##### $value `string`



#### Example 
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->background('value');

### border

#### Parameters

##### $value `\Kendo\Dataviz\UI\ChartValueAxisItemLabelsBorder|array`

The border of the labels.


#### Example - using \Kendo\Dataviz\UI\ChartValueAxisItemLabelsBorder

    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $border = new \Kendo\Dataviz\UI\ChartValueAxisItemLabelsBorder();
    $color = 'value';
    $border->color($color);
    $labels->border($border);

#### Example - using array

    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $color = 'value';
    $labels->border(array('color' => $color));

### color
The text color of the labels. Any valid CSS color string will work here, including hex and rgb.
#### Parameters

##### $value `string`



#### Example 
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->color('value');

### font
The font style of the labels.
#### Parameters

##### $value `string`



#### Example 
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->font('value');

### format
The format of the labels.
#### Parameters

##### $value `string`



#### Example 
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->format('value');

### margin
The margin of the labels.
#### Parameters

##### $value `float|`



#### Example  - using float
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->margin(1);

### mirror
Mirrors the axis labels and ticks.
If the labels are normally on the left side of the axis,
mirroring the axis will render them to the right.
#### Parameters

##### $value `boolean`



#### Example 
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->mirror(true);

### padding
The padding of the labels.
#### Parameters

##### $value `float|`



#### Example  - using float
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->padding(1);

### rotation
The rotation angle of the labels.
#### Parameters

##### $value `float`



#### Example 
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->rotation(1);

### skip
Number of labels to skip.
Skips rendering the first n labels.
#### Parameters

##### $value `float`



#### Example 
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->skip(1);

### step
Label rendering step.
Every n-th label is rendered where n is the step
#### Parameters

##### $value `float`



#### Example 
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->step(1);

### template
The label template.
Template variables:
#### Parameters

##### $value `string|\Kendo\JavaScriptFunction`



#### Example  - using string
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->template('value');

#### Example  - using \Kendo\JavaScriptFunction
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->template(new \Kendo\JavaScriptFunction('function() { }'));

### visible
The visibility of the labels.
#### Parameters

##### $value `boolean`



#### Example 
    $labels = new \Kendo\Dataviz\UI\ChartValueAxisItemLabels();
    $labels->visible(true);
