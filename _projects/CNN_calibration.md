---
layout: page
title: Calibration of Convolutional Neural Networks (CNNs) using Temperature Scaling
description: Exploring the calibration of CNNs through temperature scaling to improve model reliability in binary classification tasks.
img: assets/img/header_CNN_calibration.png  # Update this with your header image path
importance: 1
category: ML/IA
related_publications: false
pdf_link: /assets/pdf/CNN_calibration.pdf  # Place the project report in assets/pdf
---

## Abstract
This project investigates the calibration of Convolutional Neural Networks (CNNs) using temperature scaling to enhance their reliability in binary classification tasks. The project primarily focuses on understanding how well a CNN's predicted probabilities align with actual outcomes through calibration metrics like **Expected Calibration Error (ECE)** and **reliability diagrams**.

Two models were used to achieve these objectives:

1. **LeNet-5**: A simple CNN architecture trained from scratch.
2. **DenseNet-121**: A more complex pre-trained model, fine-tuned for binary classification.

Both models were trained on the **CIFAR-10 dataset**, filtered to include only images of **birds** and **cats**. The calibration process was evaluated through **reliability diagrams** and **ECE calculations**, showing significant improvements after applying **temperature scaling**.

---

## Model Descriptions

### Model 1: LeNet-5
The **LeNet-5** model was adapted for binary classification to distinguish between cats and birds in the CIFAR-10 dataset. The architecture was modified to include **dropout layers** and **batch normalization** for better performance.

#### Key Layers:
- Two convolutional layers with ReLU activation.
- Two max-pooling layers.
- Three fully connected layers with a **sigmoid activation** for binary classification.

| Layer Type          | Output Shape | Activation Function |
|---------------------|--------------|---------------------|
| Conv Layer 1        | (6, 28, 28)  | ReLU                |
| Max Pooling Layer 1 | (6, 14, 14)  | -                   |
| Conv Layer 2        | (16, 10, 10) | ReLU                |
| Max Pooling Layer 2 | (16, 5, 5)   | -                   |
| Fully Connected 1   | 120          | ReLU                |
| Fully Connected 2   | 84           | ReLU                |
| Output Layer        | 1            | Sigmoid             |

The model's performance was evaluated using:

- **Accuracy**
- **Reliability Diagrams**
- **Expected Calibration Error (ECE)**

---

### Model 2: DenseNet-121
In addition to LeNet-5, the project also explores **DenseNet-121**, a **pre-trained model** from the torchvision library, fine-tuned for binary classification.

Key modifications:

- Replaced the last classification layer to adapt the model for binary classification.
- Applied **temperature scaling** to calibrate the model’s predictions.

| Model Name  | Layers    | Parameters |
|-------------|-----------|------------|
| DenseNet-121 | 121       | ~7 million |

---

## Calibration Techniques
The project focuses on improving model calibration using **temperature scaling**, a post-processing method that adjusts the predicted probabilities by a temperature parameter `T`. Lowering or increasing this parameter helps to **smooth the probabilities** and **reduce calibration errors**.

#### Steps to Apply Temperature Scaling:
1. Train the model and obtain logits.
2. Adjust the logits with a temperature parameter.
3. Recalculate the probabilities and evaluate the **Expected Calibration Error (ECE)**.

---

## Results
The project shows a clear improvement in model calibration after applying temperature scaling.

### Reliability Diagram Comparison
Below are the **reliability diagrams** comparing the initial model predictions and the calibrated predictions using the optimal temperature factor for both models.

<div class="row justify-content-sm-center">
    <div class="col-md-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/reliability_diagram_LENET.png" title="LeNet-5: Reliability Diagram Before and After Temperature Scaling" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-md-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/reliability_diagram_DENSE.png" title="DenseNet-121: Reliability Diagram Before and After Temperature Scaling" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The reliability diagram highlights the difference between the predicted probabilities and actual outcomes. The red line shows the calibrated model, which significantly reduces the calibration error compared to the initial predictions highlighted in blue.

---

## Dataset
The project uses a filtered version of the **CIFAR-10 dataset**, containing images of **birds** and **cats**. The dataset is preprocessed to include only these two categories, and the images are normalized for training.

| Class | Label |
|-------|-------|
| Bird  | 0     |
| Cat   | 1     |

The dataset can be downloaded from the following link:

- [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)


---
This project was carried out in collaboration with [Elena Almagro](https://www.linkedin.com/in/elena-almagro-azor-a06942217/) and [Juan Muñoz](https://www.linkedin.com/in/juan-munoz-villalon/).

---
## Full Report
You can download the complete report document via the following link:

[Download Full Report PDF]({{ page.pdf_link }})

---
## GitHub Repository
You can find the Python notebook for this project, with its results and the whole process on [GitHub](https://github.com/mariogolbano/Research-projects-analysis-NLP/tree/main)


