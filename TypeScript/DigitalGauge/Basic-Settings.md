---
layout: post
title: Basic-Settings
description: basic settings
platform: typescript
control: Digital Gauge
documentation: ug
---

# Basic Settings

## Height and Width Customization

The basic customization for any control is to set the dimension. Here dimension refers to two major attributes such as **height** and `width`. The **height** and **width** assigned in the control will render the canvas element in the given size. The code example to set **height** and **width** is as follow.

{% highlight html %}

<div id="DigitalGauge1"></div>

{% endhighlight %}

{% highlight javascript %}

/// <reference path="../tsfiles/jquery.d.ts"></reference>
/// <reference path="../tsfiles/ej.web.all.d.ts"></reference>

module DigitalGaugeComponent {

 $(function () {
        // For Digital Gauge rendering
       var digitalGaugeSample = new ej.datavisualization.DigitalGauge($("#DigitalGauge1"),{
            // For setting height of the canvas element.
          height:200,
            // For setting width of the canvas element.
          width:500,
            // For setting text
          value: "Syncfusion"
        })
    });
}


{% endhighlight %}



Execute the above code examples to render the **Digital****Gauge** as follows. 

![](Basic-Settings_images/Basic-Settings_img1.png)



## Responsive Layout

* For any display devices, the control will be rendered based on the space available in that device. For this purpose, **resizing** property is given to the **Digital Gauge** control. The **Digital Gauge** renders with a given value. 

* When the browser resize the canvas element checks the dimension with its parent element. If there are any changes in parent dimension, **Gauge** control will changes the dimension based on its parent element change. This feature is enabled by using the property `isResponsive`


{% highlight html %}

<div id="DigitalGauge1"></div>

{% endhighlight %}

{% highlight javascript %}

$(function () {
        // For Digital Gauge rendering
       var digitalGaugeSample = new ej.datavisualization.DigitalGauge($("#DigitalGauge1"),{
            // For setting width of the canvas element.
            width:800,
            // For enabling resize.
           isResponsive: true,
})
    });


{% endhighlight %}



Execute the above code examples to render the **Digital****Gauge** as follows. 

![](Basic-Settings_images/Basic-Settings_img2.png)



## Themes

`Themes` give the good appearance to the control. There are two types of **Themes** available for **Digital****Gauge** as follows

* flat light

* flat dark

{% highlight html %}

<div id="DigitalGauge1"></div>

{% endhighlight %}


{% highlight javascript %}


 $(function () {
        // For Digital Gauge rendering
        var digitalGaugeSample = new ej.datavisualization.DigitalGauge($("#DigitalGauge1"),{
            // For setting width of the canvas element.
            width:800,
            // For enabling resize.
          isResponsive: true,
            // For setting theme for digital gauge.
          themes: "flatdark",
            // For setting text
          value: "LOS ANGELS 40 KM"
        })
    });


{% endhighlight %}



Execute the above code examples to render the **Digital****Gauge** as follows. 

![](Basic-Settings_images/Basic-Settings_img3.png)



