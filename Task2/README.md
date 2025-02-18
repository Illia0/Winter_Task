# Named Entity Recognition + Image Classification Pipeline

## Overview

This project implements a machine learning pipeline that consists of two models responsible for different tasks:

1. **Named Entity Recognition (NER):** Extracts animal names from a given text.
2. **Image Classification:** Identifies the animal present in an image.

The main goal is to verify whether a given textual description matches the contents of an image.

## Workflow

1. The user provides a text input, e.g., *"There is a cow in the picture."*
2. The user uploads an image containing an animal.
3. The pipeline processes the text using the NER model to extract the animal entity.
4. The image classification model predicts the animal category in the image.
5. The system compares the extracted entity with the classified image result and returns a boolean value indicating whether they match.

## Components

- **Dataset:**
  - The image dataset contains at least 10 animal classes.
  - The NER model was trained using a dataset containing sentences with animal references.
- **NER Model:** Transformer-based model (e.g., RoBERTa) trained to recognize animal names in text.
- **Image Classification Model:** CNN-based model trained to classify animals.
- **Pipeline Script:** A script that integrates both models and provides the final validation output.

## Installation & Setup

### Prerequisites

- Python 3.8+
- Required libraries (install using `pip`):
  ```sh
  pip install torch torchvision transformers tensorflow datasets numpy pillow
  ```

### Running the Pipeline

The trained models are large and cannot be uploaded to GitHub. To use the pipeline, you need to train the NER model first before running the inference.

1. Train the NER model:
   ```sh
   python NER.py
   ```

2. Ensure the trained models are available:
   - NER model: `ner_model/`
   - Image classification model: `my_model.keras`



## Results

- The NER model achieves **high accuracy** in extracting animal names.
- The image classifier correctly classifies **10 animal categories**.
- The integrated pipeline successfully determines whether the text description matches the image content.

## Future Improvements

- Extend the dataset with more animal categories.
- Improve NER model to handle misspellings and synonyms.
- Optimize image classifier with a larger dataset and advanced architectures.




