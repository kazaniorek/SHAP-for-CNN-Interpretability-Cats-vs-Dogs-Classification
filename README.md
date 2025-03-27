
# SHAP for CNN Interpretability – Cats vs Dogs Classification

This project explores how SHAP (SHapley Additive exPlanations) can be used to visualise and interpret the predictions of Convolutional Neural Networks (CNNs) trained on the Cats vs Dogs dataset. It compares different CNN architectures and their attention to image regions, helping us understand what the model "sees."

## Goals

- Train and evaluate different CNN architectures on image data.
- Apply SHAP to visualise feature importance per pixel.
- Understand if high-performing models actually focus on relevant features.

## CNN Architectures Compared

1. **Basic CNN** – standard convolutional structure.
2. **Optimised CNN** – added layers, batch normalisation, and better dropout.
3. **Augmented CNN** – trained with data augmentation for improved generalisation.

## Key Techniques

- SHAP Image Explainer with smoothed visualisations
- Visualkeras for model structure visualisation
- Comparative heatmap analysis of different CNNs
- Accuracy vs explainability insight

## Findings

- **Basic CNN** often focused on irrelevant features like background and shadows.
- **Optimised CNN** improved focus on relevant areas (e.g. face, eyes, fur).
- **Augmented CNN** achieved the best generalisation but sometimes over-relied on texture.
- SHAP helped reveal cases where high accuracy masked unreliable focus.

## Technologies Used

- Python
- TensorFlow / Keras
- SHAP
- Visualkeras
- Matplotlib, NumPy
- Cats vs Dogs dataset (TensorFlow Datasets)

## How to Run

1. Install required packages:
   ```bash
   pip install tensorflow shap visualkeras matplotlib numpy
   ```

2. Open the notebook:
   - `30030295_Poster_Shap.ipynb`

3. Run all cells to reproduce training, predictions and SHAP heatmaps.

## Author

Mariusz Sołtycz

---

This project was submitted as part of the MSc AI module "Machine Learning and Autonomous Systems" as a research poster presentation on explainable AI.
