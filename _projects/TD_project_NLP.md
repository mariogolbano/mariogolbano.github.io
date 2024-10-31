---
layout: page
title: Analysis of Research Projects
description: Developing a robust pipeline for data preprocessing and text vectorization for classification tasks.
img: assets/img/header_NLP_project.png 
importance: 1
category: ML/IA
related_publications: false
---

This project focuses on analyzing and classifying research project descriptions through various Natural Language Processing (NLP) techniques. The main goal is to process and classify text data to extract meaningful insights from a large dataset of research projects.

## Project Overview

Our approach involves several key steps:

1. **Data Preprocessing Pipeline**:
   We built a preprocessing pipeline to clean and standardize the text data, removing irrelevant information such as HTML tags and URLs, expanding contractions, and lemmatizing terms. This step is essential to prepare the data for accurate vector representation. The pipeline is versatile and can be extended to other text classification tasks.

2. **Text Vectorization Techniques**:
   We implemented three vectorization methods to convert text into numerical representations:
   - **TFIDF (Term Frequency-Inverse Document Frequency)**: Captures the importance of terms across documents.
   - **Word2Vec**: Provides dense vector embeddings with context-based similarities.
   - **BERT (Bidirectional Encoder Representations from Transformers)**: Uses transformer-based embeddings for deeper contextual understanding.

3. **Classification Models**:
   Using the preprocessed and vectorized data, we trained classification models, including Random Forest (via Scikit-learn) for traditional vectorizations and fine-tuned BERT for deep learning-based classification. These models were evaluated to determine the most effective approach for categorizing research projects.

## Insights

- **Comparative Analysis**: TFIDF, Word2Vec, and BERT were compared for performance. Word2Vec showed improved context-based classification over TFIDF, while BERT provided the highest accuracy due to its robust handling of semantic relationships.
- **Use Cases**: The pipeline allows researchers to identify projects related to specific themes or keywords efficiently.

## Visuals

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/tabla_NLP.png" title="Classification Results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Comparison of classification results across different vectorization methods.
</div>



This project exemplifies the integration of data preprocessing, vectorization, and classification to achieve efficient categorization of large-scale textual data.

This project was carried out in collaboration with [Elena Almagro](https://www.linkedin.com/in/elena-almagro-azor-a06942217/) and [Juan Muñoz](https://www.linkedin.com/in/juan-munoz-villalon/).
