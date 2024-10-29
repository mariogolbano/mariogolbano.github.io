---
layout: page
title: "Dielectric Lens Design for Collimation of RF Horn Antennas"
description: "Bachelor's Thesis in Telecommunications Engineering"
img: assets/img/cover_tfg.png  # Add a cover image in this path
importance: 1
category: work
related_publications: true
pdf_link: /assets/pdf/TFG_MARIO_GOLBANO.pdf  # Place the PDF in the assets/pdf folder
---

## Abstract

This Bachelor’s thesis focuses on the **design of dielectric lenses to enhance the directivity of horn antennas** used in anechoic chamber measurements. By designing a lens capable of collimating the beam from a horn antenna, the project aims to achieve higher directivity in primary radiation planes, improving the precision of antenna characterization.

The research utilizes Flann Standard Gain Horn antennas and explores various lens configurations, including rectangular and circular faces optimized to maximize radiated energy. The **CST STUDIO SUITE** electromagnetic simulation software was used extensively for design validation and simulation.

## Context in the Degree Program

This thesis is part of the **Telecommunications Engineering** curriculum and addresses the **high-precision characterization needs of the SWAT-UGR research group**, which focuses on 5G applications and high-frequency antenna technology. The solutions developed here enhance horn antenna directivity, providing valuable improvements in anechoic chamber measurements and high-performance telecommunications system characterization.

## Visualizations and Results

<div class="d-flex justify-content-center align-items-center">
    <div class="text-center mx-2">
        {% include figure.liquid loading="eager" path="assets/img/waveguide_design.png" title="WR22 Section Impedance" class="img-fluid rounded z-depth-1" style="width: 60%;" %}
        <div class="caption">Figure 1a: Waveguide WR22 with circular section adaptation design.</div>
    </div>
    <div class="text-center mx-2">
        {% include figure.liquid loading="eager" path="assets/img/circular_horn_lens.png" title="Circular Section Impedance" class="img-fluid rounded z-depth-1" style="width: 80%;" %}
        <div class="caption">Figure 1b: Final circular lens design achieving optimal directivity.</div>
    </div>
    <div class="text-center mx-2">
        {% include figure.liquid loading="eager" path="assets/img/Conical_antenna_lens_radiation.png" title="Conical Antenna with Lens and Radiation Pattern" class="img-fluid rounded z-depth-1" style="width: 60%;" %}
        <div class="caption">Figure 1c: Radiation pattern of the conical antenna with the designed lens.</div>
    </div>
</div>

<div class="text-center mt-3">
    {% include figure.liquid loading="eager" path="assets/img/Directivity_comparison.png" title="Directivity Comparison" class="img-fluid rounded z-depth-1" style="width: 60%;" %}
    <div class="caption">Figure 2: Comparison of directivity between optimized horns with and without the designed lens for different horn lengths.</div>
</div>


In this thesis, both the lens design and a waveguide adapter for the antenna were explored to potentially enhance the antenna's directivity while reducing the antenna length. This was aimed at achieving a collimated beam with a flat wavefront, which is essential for accurate antenna characterization. The impedance adaptation from the WR22 waveguide to the circular horn with the lens (Figure 1a) illustrates the progression towards this goal, while the improvements in directivity shown in Figure 1c validate the effectiveness of the design.
  
## Full Thesis Download

You can download the complete thesis document via the following link:

[Download Full Thesis PDF]({{ page.pdf_link }})
