---
layout: page
title: Tensorial Diffraction Tomography
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

Here, we demonstrate volumetric reconstruction results of an isolated healthy muscle fiber using our inexpensive, LED-based, scanning-free system. High-contrast and high-resolution structural imaging of intrinsic signals in skeletal muscle fibers is crucial for the rapid detection of changes in myofibrillar organization that can lead to skeletal myopathies. Currently, imaging muscle tissue in 3D typically requires complex and expensive systems, such as second-harmonic generation (SHG) microscopy. Our system yields results comparable to those described for SHG imaging in the literature.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/tofu_2.png" title="Muscle fiber imaging" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Reconstructions of a muscle fiber. (a) The image of a muscle fiber with the center LED illumination. The imaging system is focused in the middle of the muscle fiber. (b) The reconstructed birefringence. The zoom-in region shows the structures of healthy muscle fibers. The image of the same muscle fiber at a different region, where a non-muscle fiber with a 90-deg bend is placed below the muscle fiber. The imaging system is focused between this and the muscle fiber. (d) The reconstructed orientation at different depths, with a zoom-in showing the fine sarcomere structure of muscle tissue. (e) Histogram of reconstructed orientation shown in (d).
</div>