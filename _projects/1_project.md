---
layout: page
title: Tensorial diffraction tomography
description: Imaging transparent cells with optical diffraction
img: assets/img/publication_preview/tofu.png
importance: 1
category: work
related_publications: true
---

Due to their high water content, cells and tissues are mostly transparent under visible light microscopy. While exogenous dyes, such as histopathology stains or fluorescence, can introduce significant microscopy contrast and specificity, these enhancements typically perturb cell physiology or require painstaking sample preparation. In this work, we introduce a non-scanning, label-free tomographic microscopy method for quantitative simultaneous imaging of refractive index and polarization information from specimens in 3D.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/tofu_1.png" title="Instrumentation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   The imaging setup consists of a standard microscope equipped with an LED matrix, a polarization generator, and a polarization-sensitive camera. Permittivity tensors of anisotropic samples are computationally recovered from polarized intensity measurements across three dimensions. 
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
