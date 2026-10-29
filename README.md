# EcoSort-Waste-Management-
# EcoSort: Integrated Waste Management Assistant

## Project Overview

EcoSort is a waste management assistant that combines machine learning, image classification, text classification, and policy retrieval to help identify waste materials and provide relevant recycling guidance.

The project explores how AI can support waste sorting and encourage better recycling practices.

## Objectives

- Classify waste descriptions using natural language processing.
- Identify waste materials from images using a convolutional neural network (CNN) based on MobileNetV2.
- Retrieve relevant recycling policies based on the predicted waste category.
- Generate recycling instructions using a text-generation model.
- Integrate these components into a single waste management assistant.

## Waste Categories

The image dataset contains nine categories:

- Cardboard
- Food Organics
- Glass
- Metal
- Miscellaneous Trash
- Paper
- Plastic
- Textile Trash
- Vegetation

## Technologies Used

- Python
- TensorFlow and Keras
- MobileNetV2
- Scikit-learn
- TF-IDF vectorization
- Logistic Regression
- Transformers (FLAN-T5)
- NumPy and Pandas
- Jupyter Notebook

## Evaluation Results

The integrated assistant was evaluated using five text descriptions and 160 images.

| Component | Correct Predictions | Accuracy |
|---|---:|---:|
| Text classification | 4 out of 5 | 80.00% |
| Image classification | 20 out of 160 | 12.50% |

The text classifier performed better than the image classifier in these tests. The image classifier frequently predicted Miscellaneous Trash for images from other categories, indicating that further model and preprocessing improvements are needed.

The text evaluation used a small sample, so its results should not be interpreted as a reliable estimate of performance on all waste descriptions.

## Limitations and Future Improvements

- Investigate image preprocessing and model configuration.
- Improve image classification performance across all waste categories.
- Evaluate performance using larger and more representative test samples.
- Improve the relevance of retrieved recycling policies and generated instructions.
- Test the integrated assistant with real-world waste images and descriptions.

## How to Run

1. Clone or download this repository.
2. Set up the required Python environment and dependencies.
3. Open the project notebook in Jupyter Notebook.
4. Run the notebook cells in order, ensuring the required datasets and model dependencies are available.

## Project Status

This is an educational machine learning project. The integrated workflow demonstrates the connection between waste classification and recycling-policy retrieval, but the image classifier requires further improvement before practical use.
