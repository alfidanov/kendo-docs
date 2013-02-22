---
title: SparklineSeriesItemTarget
slug: php-dataviz-ui-sparklineseriesitemtarget
tags: api, php
publish: true
---

# \Kendo\Dataviz\UI\SparklineSeriesItemTarget

A PHP class representing the target setting of SparklineSeriesItem.


## Methods

### border

The border of the target.

#### Returns
`\Kendo\Dataviz\UI\SparklineSeriesItemTarget`

#### Parameters

##### $value `\Kendo\Dataviz\UI\SparklineSeriesItemTargetBorder|array`


#### Example - using [\Kendo\Dataviz\UI\SparklineSeriesItemTargetBorder](/api/wrappers/php/Kendo/Dataviz/UI/SparklineSeriesItemTargetBorder)
    <?php
    $target = new \Kendo\Dataviz\UI\SparklineSeriesItemTarget();
    $border = new \Kendo\Dataviz\UI\SparklineSeriesItemTargetBorder();
    $color = 'value';
    $border->color($color);
    $target->border($border);
    ?>

#### Example - using array

    <?php
    $target = new \Kendo\Dataviz\UI\SparklineSeriesItemTarget();
    $color = 'value';
    $target->border(array('color' => $color));
    ?>

### line

The target line.

#### Returns
`\Kendo\Dataviz\UI\SparklineSeriesItemTarget`

#### Parameters

##### $value `\Kendo\Dataviz\UI\SparklineSeriesItemTargetLine|array`


#### Example - using [\Kendo\Dataviz\UI\SparklineSeriesItemTargetLine](/api/wrappers/php/Kendo/Dataviz/UI/SparklineSeriesItemTargetLine)
    <?php
    $target = new \Kendo\Dataviz\UI\SparklineSeriesItemTarget();
    $line = new \Kendo\Dataviz\UI\SparklineSeriesItemTargetLine();
    $width = new ();
    $line->width($width);
    $target->line($line);
    ?>

#### Example - using array

    <?php
    $target = new \Kendo\Dataviz\UI\SparklineSeriesItemTarget();
    $width = new ();
    $target->line(array('width' => $width));
    ?>
