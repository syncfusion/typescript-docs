---
layout: post
title: Text-Configuration
description: text configuration
platform: typescript
control: Tile
documentation: ug
---

# Text Configuration

The **"data-ej-showText”** attribute is used to show or hide the **Tile** caption. By default, the **“data-ej-showText”** attribute is to **true** on initialization**.** The **“data-ej-text”** attribute is used to set the caption of a **Tile** as a **Text** on initialization. The **"data-ej-textAlignment”** attribute is used to align the Tile text as **normal** on initialization. The possible position values for “**data-ej-textAlignment”** are as follows: 

1. normal
2. left
3. right
4. center

Refer to the following code examples.

{% highlight html %}


    <div id="tile"></div>
    
{% endhighlight %}

Add the following code inside the **script** tag.

{% highlight javascript %}

  /// <reference path="tsfiles/jquery.d.ts" />
 /// <reference path="tsfiles/ej.web.all.d.ts" />

module TileViewComponent {
    $(function () {
          var tile1 = new ej.Tile($("#tile1"), {
         tileSize: "medium",
         imagePosition: "center",
         textAlignment: "center", 
         imageUrl: "http://js.syncfusion.com/UG/web/Content/tile/camera.png",
          text: "Camera"
   });
 });
}

{% endhighlight %}



![](Text-Configuration_images/Text-Configuration_img1.png)

