---
layout: page
title: "A Data-Driven Framework for Wireless Communications"
description: "Master’s Thesis in Telecommunications Engineering"
img: assets/img/cover_tfm.png  # Add a cover image in this path
importance: 1
category: RF
related_publications: true
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


## Some Images from Framework

<div class="row align-items-center">
    <figure class="col-6 text-center mb-3">
        <img src="assets/img/MATLAB_GUI_gen (1).png" alt="MATLAB GUI for signal generation" class="img-fluid rounded z-depth-1 img-70">
        <figcaption>Figure 1: MATLAB GUI for selecting modulations or technologies.</figcaption>
    </figure>
    <figure class="col-6 text-center mb-3">
        <img src="assets/img/MATLAB_GUI_gen (2).png" alt="Configurable Parameters for WiFi VHT" class="img-fluid rounded z-depth-1 img-110">
        <figcaption>Figure 2: Configurable Parameters for WiFi VHT.</figcaption>
    </figure>
</div>

<div class="row justify-content-center">
    <figure class="col-12 text-center mb-3">
        <img src="assets/img/MATLAB_GUI_gen (3).png" alt="Configurable Parameters for OFDM" class="img-fluid rounded z-depth-1 img-110">
        <figcaption>Figure 3: Configurable Parameters for OFDM.</figcaption>
    </figure>
</div>

<div class="row align-items-center">
    <figure class="col-6 text-center mb-3">
        <img src="assets/img/interf_sim.png" alt="Interferences Simulation" class="img-fluid rounded z-depth-1 img-70">
        <figcaption>Figure 4: Python Notebook for simulating interferences from dataset.</figcaption>
    </figure>
    <figure class="col-6 text-center mb-3">
        <img src="assets/img/interf_sim_wave.png" alt="Interference Waveform Simulation" class="img-fluid rounded z-depth-1 img-110">
        <figcaption>Figure 5: Interference Waveform Simulation.</figcaption>
    </figure>
</div>

<div class="row justify-content-center">
    <figure class="col-12 text-center mb-3">
        <img src="assets/img/interf_sim_spec.png" alt="Interference Spectrum Simulation" class="img-fluid rounded z-depth-1 img-110">
        <figcaption>Figure 6: Interference Spectrum Simulation.</figcaption>
    </figure>
</div>

<div class="row justify-content-center">
    <figure class="col-12 text-center mb-3">
        <img src="assets/img/MATLAB_GUI_eval.png" alt="MATLAB GUI for evaluation of recovered signals" class="img-fluid rounded z-depth-1 img-150">
        <figcaption>Figure 7: MATLAB GUI for evaluation of recovered signals.</figcaption>
    </figure>
</div>


## Conclusions

The results demonstrate that the **data-driven framework** developed in this thesis significantly improves wireless signal recovery in environments with various interferences. The framework integrates signal generation, interference simulation, and signal recovery, providing a comprehensive tool for evaluating the performance of machine learning models in realistic communication environments.

By leveraging a custom-built dataset, the framework offers a more accurate representation of real-world scenarios compared to traditional signal processing methods. The **UNet neural network**, used for interference mitigation, showed promising results, particularly in scenarios with high interference, demonstrating its potential for future applications in wireless communications.

This work lays the foundation for future research in machine learning-based wireless signal processing, offering a versatile and scalable approach for addressing interference challenges in 5G, IoT, and other advanced communication systems.

## Full Thesis

You can download the complete thesis document via the following link:

[Download Full Thesis PDF]({{ page.pdf_link }})
