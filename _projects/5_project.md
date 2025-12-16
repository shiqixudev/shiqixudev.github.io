---
layout: page
title: Micro-camera array microscope
description: Gigapixel video at micrometer resolution
img: assets/img/proj/mcam2.png
importance: 2
category: work
related_publications: false
---

The information content that any optical imaging system can acquire is limited by the spatial bandwidth product. As a result, classical optical imaging systems are typically limited to either high resolution or a large field of view. In this project, we explore using a densely packed array of “micro-cameras” to jointly image a large field of view (FOV) simultaneously at high resolution. Each micro-camera within the array images a unique area of the sample; data acquired by the 54 micro-cameras are then digitally combined into composite frames. The total pixel count of these frames significantly exceeds that of standard microscope systems.

<div class="row">
    <div class="col-sm mt-3 mt-md-0" style="max-width: 600px; margin: 0 auto;">
        {% include figure.liquid loading="eager" path="assets/img/proj/umpa_p2.png" title="Imaging system" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Each camera images a sub-FOV at high resolution, and during post-processing, the images are composited into a large FOV, gigapixel image.
</div>

Moreover, we can configure the camera array in a stereoscopic setting where multiple cameras image the same FOV. Using triangulation, we can create a high-resolution, high-precision RGB-D image.

<div class="row">
    <div class="col-sm mt-3 mt-md-0" style="max-width: 600px; margin: 0 auto;">
        {% include figure.liquid loading="eager" path="assets/img/proj/umpa_p2.png" title="Stereoscopic configuration" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Each FOV is imaged by multiple cameras, generating an RGB-D image with a high-resolution, high-precision height map.
</div>

Finally, we can also configure the camera in at high resolution mode, such that all the cameras are imaging non-overlapping FOV. This will require scanning (for a few steps) for getting sub-micron resolution images. This allows to image multiple pathological slices within minutes, enabling new clinical applications such as rapid on-site evulation. 


In addition, with a mirror trick, we can also config all the cameras to image a volumetric sample from different angles all at once, to create a tomographic reconstruction. (to be finished)
