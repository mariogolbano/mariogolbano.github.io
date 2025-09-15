---
layout: page
title: "Visual Object Tracking Using Particle Filter"
description: "Optimizing a particle filter for visual object tracking using advanced color, texture, and shape descriptors to improve accuracy in complex scenarios."
img: assets/img/object_tracking_cover.png  # Add a cover image in this path
importance: 2
category: ML/AI
related_publications: false
pdf_link: /assets/pdf/computer_challenge.pdf  # Link to the PDF file
---

## Abstract

This report presents an optimization of the **particle filter** used for **visual object tracking**. The goal of the project was to enhance the robustness and accuracy of the baseline particle filter by integrating additional features such as **adaptive update**, **texture description (LBP)**, and **HOG (Histogram of Oriented Gradients)** descriptors.

The research includes:

- **Particle Filter Algorithm**: The implementation was based on [Bagdanov et al., 2007], with optimizations including an adaptive update mechanism and spatial division for better tracking.
- **Texture and Shape Features**: Local Binary Patterns (LBP) and HOG descriptors were incorporated to improve object recognition in complex environments.
- **Performance Evaluation**: The Jaccard Index (JI) was used to evaluate the performance of different versions of the filter, highlighting improvements in accuracy.

## Example

In the following images we can see how the bounding box keeps track of the object (skater in this case) after several frames of the video. The Ground Truth bounding box is represented in green while the predicted one is represented in blue, for comparison. 

<div class="row align-items-center">
    <figure class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/particle_filter1.png" title="Particle Filter Initialization" class="img-fluid rounded z-depth-1 img-70" %}
        <figcaption>Figure 1: Ground Truth Box (green) vs Predicted Object Box (Blue) at start.</figcaption>
    </figure>
    <figure class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/particle_filter2.png" title="Tracking Results" class="img-fluid rounded z-depth-1 img-110" %}
        <figcaption>Figure 2: Ground Truth Box (green) vs Predicted Object Box (Blue) tracking.</figcaption>
    </figure>
</div>

## Key Findings

The particle filter optimization demonstrated a significant improvement in the **Jaccard Index (JI)**, particularly in scenarios where the object exhibited rapid movements and complex background noise. The modifications tested during the project included:

- **Adaptive Update & Spatial Division**: These modifications led to more accurate tracking in dynamic environments.
- **LBP and HOG Descriptors**: Both descriptors enhanced the object tracking capabilities, particularly in cluttered scenes with varying textures.
- **Acceleration Model**: This approach did not yield improvements, suggesting that the existing model was sufficient for the tracking task.

## Conclusion

This project successfully demonstrates how the integration of advanced feature descriptors and adaptive techniques can improve the robustness of **particle filter-based visual tracking systems**. The results provide a solid foundation for further research into **real-time object tracking** in complex environments.

As shown in the report below, by appliying our changes, we achieved to increase the mean Jaccard Index from 0.33 to 0.51.

All necessary files are at the [GitHub Repository](https://github.com/mariogolbano/ObjectTracking_ParticleFilter/tree/main) in case someone wants to try it out. 

## Full Report

You can download the complete report document via the following link:

[Download Full Report PDF]({{ page.pdf_link }})
