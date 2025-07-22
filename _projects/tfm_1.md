---
layout: page
title: "A Data-Driven Framework for Wireless Communications"
description: "Master’s Thesis in Telecommunications Engineering"
img: assets/img/tfm_portada.png  # Add a cover image in this path
importance: 1
category: RF
related_publications: false
pdf_link: /assets/pdf/Master_thesis_Mario_Golbano.pdf  # Place the PDF in the assets/pdf folder
---

## Abstract

This Master's thesis presents a comprehensive framework for the **generation, simulation of interferences, visualization, and recovery of wireless signals** using deep learning foundation models. The approach involves training a foundation model on synthetic I/Q signals to enhance the robustness and accuracy of wireless signal recovery in the presence of various interferences.

The research encompasses:

- **Signal Generation**: Development of a MATLAB GUI for creating synthetic OFDM signals with configurable modulations and impairments.
- **Interference Simulation**: Implementation of a Python-based environment to simulate Bluetooth and other OFDM signal interferences.
- **Data Visualization**: Tools in Python for visualizing and analyzing the generated and recovered signals.
- **Signal Recovery Model**: Design and training of a U-Net neural network for recovering signals affected by interferences.

The proposed model demonstrates significant improvements in signal recovery accuracy compared to traditional methods, particularly in scenarios with high interference.

Further information about the project along with all the developed framework can be accessed at:
[Thesis GitHub Repository](https://github.com/mariogolbano/TFM-foundation-model-wireless-signals)


## Some Images from Framework

<div class="row align-items-center">
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/waveguide_design.png" title="WR22 Section Impedance" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 1a: Waveguide WR22 with circular section adaptation design.</div>
    </div>
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/circular_horn_lens.png" title="Circular Section Impedance" class="img-fluid rounded z-depth-1" style="width: 110%;" %}
        <div class="caption">Figure 1b: Final circular lens design achieving optimal directivity.</div>
    </div>
</div>

<div class="row justify-content-center">
    <div class="col-12 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/MATLAB_GUI_gen_1.png" title="MATLAB GUI for signal generation" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 2: MATLAB GUI for selecting modulations or technologies.</div>
    </div>
</div>

<div class="row align-items-center">
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/MATLAB_GUI_gen_2.png" title="Configurable Parameters for WiFi VHT" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 3: Configurable Parameters for WiFi VHT.</div>
    </div>
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/MATLAB_GUI_gen_3.png" title="Configurable Parameters for OFDM" class="img-fluid rounded z-depth-1" style="width: 110%;" %}
        <div class="caption">Figure 4: Configurable Parameters for OFDM.</div>
    </div>
</div>

<div class="row justify-content-center">
    <div class="col-12 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/interf_sim.png" title="Interferences Simulation" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 5: Python Notebook for simulating interferences from dataset.</div>
    </div>
</div>

<div class="row align-items-center">
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/interf_sim_wave.png" title="Interference Waveform Simulation" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 6: Interference Waveform Simulation.</div>
    </div>
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/interf_sim_spec.png" title="Interference Spectrum Simulation" class="img-fluid rounded z-depth-1" style="width: 110%;" %}
        <div class="caption">Figure 7: Interference Spectrum Simulation.</div>
    </div>
</div>

<div class="row justify-content-center">
    <div class="col-12 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/MATLAB_GUI_eval.png" title="MATLAB GUI for evaluation of recovered signals" class="img-fluid rounded z-depth-1" style="width: 150%;" %}
        <div class="caption">Figure 8: MATLAB GUI for evaluation of recovered signals.</div>
    </div>
</div>


## Conclusions

The results demonstrate that the **data-driven framework** developed in this thesis significantly improves wireless signal recovery in environments with various interferences. The framework integrates signal generation, interference simulation, and signal recovery, providing a comprehensive tool for evaluating the performance of machine learning models in realistic communication environments.

By leveraging a custom-built dataset, the framework offers a more accurate representation of real-world scenarios compared to traditional signal processing methods. The **UNet neural network**, used for interference mitigation, showed promising results, particularly in scenarios with high interference, demonstrating its potential for future applications in wireless communications.

This work lays the foundation for future research in machine learning-based wireless signal processing, offering a versatile and scalable approach for addressing interference challenges in 5G, IoT, and other advanced communication systems.

## Full Thesis

You can download the complete thesis document via the following link:

[Download Full Thesis PDF]({{ page.pdf_link }})
