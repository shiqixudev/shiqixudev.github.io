---
layout: page
title: High-throughput rotational laminography
description: 3D icnline advanced packaging inspection
img: assets/img/proj/nlx_snip.png
importance: 1
category: work
related_publications: false
---

Three-dimensional integrated circuit (3D IC) packaging offers superior performance and energy efficiency over 2D IC packaging but requires reliable, high-throughput in-line inspection to detect defects like misaligned interconnects and voids. X-ray computed laminography (CL) is an effective technique for high-throughput volumetric imaging of large, planar samples, which is well-suited for wafer-level 3D IC packaging inspection.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/nlx_1.png" title="Rotational laminography" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Due to the significantly shorter photon path, rotational laminography can drastically reduce scan time compared to standard circular trajectory cone beam CT.
</div>

However, due to stringent time requirements demanded by inline semiconductor manufacturing inspection applications, which typically require completing inspection per region-of-interest (ROI) within minutes, the shot-noise limited scans tend to resulting in reconstructions that are too noisy for robust downstream metrology and defect analysis. To meet this challenge, we developed a self-supervised workflow to create a generalist deep learning model for high-resolution (~2.3 gigavoxels per scan) volumetric CT image denoising by pre-training the model on a large number of semiconductor packaging datasets. We showcase that the generalist model has superior zero-shot denoising capability on a varity of semiconductor packaging samples. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/nlx_2.jpeg" title="Generalist model for volumetric image denoising" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Denoised reconstruction on samples containing A. memory stack, B. TSV arrays with programmed void from IMEC, and C. a semiconductor package with C4 bump cracks. Extracted from doi.org/10.1093/mam/ozaf048.984
</div>

In addition, because computed laminography geometry violates Tuy's data sufficiency condition, reconstructions typically exhibit butterfly-like cone-beam artifacts. To address this, we present a self-supervised deep image restoration workflow that produces noise-free, artifact-free volumetric reconstructions. The core of our proposed pipeline is an unbiased progressive artifact removal algorithm designed to suppress laminographic artifacts. These artifact-corrected volumes are then used to train a deep image restoration network, improving image quality without increasing inference time. We demonstrate the efficacy of this method on a variety of samples scanned with an in-house prototype system.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/nlx_3.png" title="Self-supervised cone-beam artifact removal" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Volumetric reconstruction of a dynamic random-access memory (DRAM) sample. Noise reduction and artifact removal are applied simultaneously to improve image quality without increasing inference time. Extracted from doi.org/10.1117/12.3028278
</div>

