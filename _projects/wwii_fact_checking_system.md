---
layout: page
title: WWII Fact-Checking RAG System
description: Development of a Retrieval-Augmented Generation (RAG) system to verify the veracity of World War II-related statements using a specific corpus and large language models.
img: assets/img/wwii_fact_check_cover.png  # Path for header image
importance: 1
category: ML/AI
related_publications: false
---

## Abstract

This project focuses on developing a Retrieval-Augmented Generation (RAG) system designed to automatically verify the veracity of statements related to World War II. By integrating semantic search techniques with large language models (LLMs), the system retrieves relevant information from a curated corpus and employs the LLM to assess the truthfulness of the input statements. The project was undertaken as part of a master's program in collaboration with my colleagues, aiming to contribute to the field of automated fact-checking.

Further information about the project, along with the actual project can be found at this [GitHub Repository](https://github.com/Robertoguisasola/Fact-cheking_system_NLP).

## Key Components

1. **RAG System Architecture**:
   - Combines semantic search using FAISS with LLMs to retrieve and generate responses.
   - Utilizes Meta's Llama 3 Instruct model for generating factual responses.
   - Incorporates BERTScore for evaluating the quality and relevance of generated content.

2. **Data Corpus**:
   - A curated collection of World War II-related texts serving as the knowledge base.
   - Enables the system to retrieve contextually relevant information for fact-checking.

3. **Evaluation Metrics**:
   - BERTScore is employed to assess the semantic similarity between generated responses and ground truth data.
   - Provides a quantitative measure of the system's performance in generating accurate and contextually appropriate content.

4. **User Interface**:
   - A graphical user interface (GUI) developed to facilitate user interaction with the system.
   - Allows users to input statements and receive fact-checked responses in an accessible manner.

5. **Configuration and Dependencies**:
   - Configuration files (`config.json`, `requirements.txt`, `environment.yml`) to manage system settings and dependencies.
   - Ensures reproducibility and ease of setup for future use and development.

## Installation

To set up the environment and install the necessary dependencies, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/Robertoguisasola/Fact-cheking_system_NLP.git
   cd Fact-cheking_system_NLP
   ```

2. Create and activate a Conda environment:

   ```bash
   conda env create -f environment.yml
   conda activate fact_checking_env
   ```

3. Alternatively, if you prefer using `pip`, install the dependencies listed in `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```

4. Download the required models and datasets as specified in `data_download.py` and `config.json`.

## Usage

To run the system, execute the following command:

```bash
python gui.py
```

This will launch the GUI, allowing you to input statements and receive fact-checked responses.

## Evaluation

The system's performance is evaluated using BERTScore, which measures the semantic similarity between the generated responses and the ground truth. The evaluation script is integrated into the pipeline and can be accessed through the GUI.

## Contributions

This project was developed as part of a master's program in collaboration with my colleagues:
- Juan Muñoz Villalón
- Elena Almagro Azor
- Roberto Martínez-Guisasola Guerrero
