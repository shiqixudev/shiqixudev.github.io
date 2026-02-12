---
layout: page
title: Flow-based Volumetric Computed Tomography
description: Generative model-regularized CT reconstruction
img: assets/img/proj/dps_thumbnail.png
importance: 2
category: work
related_publications: false
category: hidden
---

Recent works in generative prior regularized image reconstruction show state-of-the-art results in reducing noise and structural artifacts. In this work, we explore the feasibility of using generative priors, such as flow matching models, to regularize volumetric cone beam computed tomography (CBCT) reconstruction. We show such methods noticeably reduce noise and cone beam and streak artifacts from short-scan and rotational laminography, therefore have great potential to be used in high throughput CBCT applications.

<div class="row justify-content-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/dps_workflow.png" title="Workflow" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Proposed regularized reconstruction workflow
</div>


Short-scan, also known as 180+ fan scan, is a widely used circular scanning trajectory for asymmetric samples. In industry CT settings, this is useful for anisotropic samples that either need to be placed close to the source for higher geometric magnification (GeoMag), or to avoid high attenuation along certain directions. However, for CBCT, especially in the high cone angle regions, short scan can result in streak artifacts. Figure below shows reconstruction of a foam-structure sample using various method. From both filted backprojection (FBP) and unregularized iterative reconstruction, we see We see expected streaking artifacts at boundary, and elongated cone beam artifacts, as well as noise. The noise2noise-based DeepReconIC method removes both noise and most steaking artifacts, but was not able to recover smeared and distorted features. Both score-based and flow-based reconstruction are able to surpress noise, while flow-based method shows superior results in artifact removal and feature recovery. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/dps_shortscan.png" title="Stereoscopic configuration" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Results from short-scan.
</div>

Another popular geometry typically used for large, flat samples is rotational laminography. To scan a plate-like sample, such as a wafer or a printed circuit board, it is often advantageous to use a rotational laminography trajectory for improved throughput and reduced beam-hardening. However, reconstruction from such a trajectory suffers from smearing cone-beam artifacts, as well as vignetting or a truncated field of view (FOV). From the results in the figure below, we see these artifacts in the FBP reconstruction. DeepReconIC is able to remove noise but is unable to mitigate cone-beam artifacts. Both score-based and flow-based reconstruction reduce both noise and artifacts while recovering the structures, while the flow-based method clearly outperforms the others.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/dps_cl.png" title="Stereoscopic configuration" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Results from rotational laminogrpahy.
</div>

