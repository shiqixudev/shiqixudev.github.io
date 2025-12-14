---
layout: page
title: Parallelized Diffuse Correlation Imaging
description: Imaging hemo-dynamics at single photon sensitivity
img: assets/img/proj/crepe.png
importance: 1
category: work
related_publications: false
---

Noninvasive optical imaging through dynamic scattering media has numerous important biomedical applications but still remains a challenging task. While standard diffuse imaging methods measure optical absorption or fluorescent emission, few works to date, however, have aimed to experimentally measure and process such temporal correlation data to demonstrate deep-tissue video reconstruction of decorrelation dynamics. In this work, a single-photon avalanche diode array camera is utilized to simultaneously monitor the temporal dynamics of speckle fluctuations at the single-photon level from 12 different phantom tissue surface locations delivered via a customized fiber bundle array. Then a deep neural network is applied to convert the acquired single-photon measurements into video of scattering dynamics beneath rapidly decorrelating volume.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/pdci1.jpg" title="Workflow" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Flow diagram of proposed method for imaging temporal decorrelation dynamics. (A) Illustration of parallelized diffuse correlation imaging (PaDI) measurement strategy. Scattered coherent light from source to multiple detector fibers travels through decorrelating scattering media along unique banana-shaped paths. Fully developed speckle on the tissue surface rapidly fluctuates as a function of deep-tissue movement. Green dashed box marks deep-tissue dynamics areas of interest for imaging. (B) Computed autocorrelation curves from time-resolved measurements of surface speckle at different tissue surface locations. (C) Autocorrelation variations caused by deep-tissue dynamics are computationally mapped into spatially resolved images of transient dynamics.
</div>

To assess the performance of our PaDI system, we first turn to an easily reconfigurable nonbiological liquid phantom setup that offers the ability to flexibly generate unique image targets with known spatial and temporal properties. To mimic decorrelation rates and scattering properties of human tissue, we utilized a turbid, rapidly decorrelating liquid phantom filled with colloidal polystyrene microspheres solution enclosed in a custom-designed thin-walled cuvette. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/pdci2.jpg" title="Benchtop demonstration" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   (A) Schematic of PaDI system for imaging decorrelation. Back-scattered coherent light from single input port is collected by 12 multimode fibers (MMF) at tissue phantom surface and guided to SPAD array camera. (B) Profile view of the tissue phantom imaging experiment. Digital micro-mirror device (DMD) and vessel phantom serve as source of temporal dynamics and is hidden beneath phantom by placing it immediately adjacent (separated by coverglass). All sources and detectors are placed on the same side of phantom. Colormap provides qualitative photon distribution map, where quantitative plot of sub-surface photon distribution is in Figure S1B, Supporting Information. (C) A set of DMD patterns that can be used to generate spatiotemporal varying dynamics. (D) Simulation of photon-sensitive region of our 12-fiber system. (E) A picture of the tissue phantom we use in experiments.
</div>

Finally, we extended our method to healthy human subjects in controlled experiments to monitor forearm muscular blood flow during restriction and prefrontal cortex cerebral blood flow during cognitive tasks.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj/pdci3.png" title="Human psychology monitoring experiments" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Study design (a) and principle of dual-detection with PDCS (blood flow suppression in forearm via pressure cuff) (b) at the forearm and (c) the forehead (cognitive blood flow activation in prefrontal cortex).
</div>

#### Further reading

Xu, Shiqi, et al. ["Imaging Dynamics Beneath Turbid Media via Parallelized Single‐Photon Detection."](https://doi.org/10.1002/advs.202201885) Advanced Science 9.24 (2022): 2201885.

Xu, Shiqi, et al. ["Transient motion classification through turbid volumes via parallelized single-photon detection and deep contrastive embedding."](https://www.frontiersin.org/articles/10.3389/fnins.2022.908770/full) Frontiers in neuroscience 16 (2022): 908770.

Kreiss, Lucas, et al. ["Beneath the surface: revealing deep-tissue blood flow in human subjects with massively parallelized diffuse correlation spectroscopy."](https://doi.org/10.1117/1.NPh.12.2.025007) Neurophotonics 12.2 (2025): 025007-025007.

