---
layout: page
title: "HT-DEMUCS for Interference Mitigation"
description: "Master’s Thesis in Machine Learning: On the Generalization of Deep Neural Network-Based Interference Rejection to Unseen Signal Constellations"
img: assets/img/htdemucs-cover.png  # Add a cover image in this path
importance: 1
category: ML/AI
related_publications: false
pdf_link: /assets/pdf/ML_MarioGolbanoCorzo_Thesis.pdf  # Place the PDF in the assets/pdf folder
---

## Abstract

This Master's thesis presents the **HT-DEMUCS model**, a deep learning-based framework designed for **interference mitigation** in radio frequency (RF) communication systems. The project focuses on the development and evaluation of a neural network architecture capable of separating multi-source RF interference from clean signals using the **HT-DEMUCS** framework, inspired by high-resolution time-frequency analysis. 

Beyond RF signals, this thesis also investigates the **generalization of the model** to a wide range of signal constellations, including unseen constellations that were not part of the training data. The **HT-DEMUCS model** has been designed to be versatile and robust, enabling its application in scenarios where the signal types are not known a priori, making it applicable for broader communication environments like 5G, IoT, and beyond.

The research includes the following core aspects:

- **Signal Dataset**: Generation and preprocessing of a large RF signal dataset that includes various interference scenarios like co-channel and adjacent channel interference, ensuring a diverse training set.
- **Model Architecture**: Design and implementation of the **HT-DEMUCS** model, which employs deep convolutional layers to separate multi-source interference from the original signal, leveraging high-resolution time-frequency analysis.
- **Training Pipeline**: Development of an efficient and scalable training pipeline designed to optimize the model for both performance and computational efficiency, including strategies for **generalizing across unseen signal constellations**.
- **Generalization to Unseen Signal Constellations**: Evaluation of the model’s ability to generalize to **unseen constellations**, testing its robustness and adaptability across different signal types not encountered during training.
- **Performance Evaluation**: Comprehensive analysis of the model’s interference mitigation accuracy compared to traditional signal separation techniques and its ability to handle real-world communication environments.

The proposed **HT-DEMUCS model** demonstrates a significant improvement in interference rejection, particularly in complex and overlapping interference environments, and shows promising results for generalization to various communication systems.

Further details and resources can be accessed via the project’s GitHub repository:
[HT-DEMUCS GitHub Repository](https://github.com/mariogolbano/HTDEMUCS-for-interference-mitigation)

<div class="row align-items-center">
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/ht-demucs-arch.png" title="HT-DEMUCS Model Architecture" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 1: HT-DEMUCS Model Architecture for interference mitigation.</div>
    </div>
</div>

<div class="row align-items-center">
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/sig-metrics-htdemucs.png" title="Signal-metrics performance of HT-DEMUCS" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 2: Signal-metrics performance of HT-DEMUCS.</div>
    </div>
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/ber-htdemucs.png" title="Bit-metrics performance of HT-DEMUCS" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 3: Bit-metrics performance of HT-DEMUCS.</div>
    </div>
</div>

<div class="row align-items-center">
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/64qam_hy.png" title="Signal Recovery Results on Seen Constellations" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 4: Signal recovery results after applying HT-DEMUCS interference mitigation on seen constellations.</div>
    </div>
    <div class="col-6 text-center mb-3">
        {% include figure.liquid loading="eager" path="assets/img/256qam_hy.png" title="Signal Recovery Results on Unseen Constellations" class="img-fluid rounded z-depth-1" style="width: 70%;" %}
        <div class="caption">Figure 5: Signal recovery results after applying HT-DEMUCS interference mitigation on unseen constellations.</div>
    </div>
</div>

## Conclusions

The **HT-DEMUCS model** has proven effective in mitigating interference in RF signals, demonstrating superior performance over traditional methods. The model achieves high-quality separation of clean signals from various sources of interference, providing a valuable tool for wireless communication systems facing harsh interference environments.

By employing deep learning techniques, this work highlights the potential of machine learning models in improving signal processing for real-world communication systems. Moreover, the model's ability to generalize across **different interference scenarios** and signal constellations, including **unseen constellations**, makes it a scalable solution for applications in diverse and evolving wireless communication standards such as 5G, IoT, and beyond.

The framework developed in this thesis offers a robust solution for interference rejection, laying the groundwork for future research on neural network-based signal processing models that can handle unknown and dynamic signal environments.

## Full Thesis

You can download the complete thesis (paper format) document via the following link:

[Download Full Thesis PDF]({{ page.pdf_link }})
