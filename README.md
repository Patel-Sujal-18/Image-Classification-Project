# Image-Classification-Project
A Deep Learning-based vehicle classifier using MobileNetV2 and Transfer Learning. Features Explainable AI (Grad-CAM) to generate visual heatmaps, highlighting exactly which features the model uses to distinguish between cars and bikes.
# Project Overview
This project uses Transfer Learning (MobileNetV2) to classify Cars vs. Bikes with high efficiency. It features Explainable AI (Grad-CAM) to generate visual heatmaps, revealing exactly which image features—like wheels or handlebars—drive the model's decision-making.
# Key Features
Car vs Bike Classification: High-accuracy binary classification.

Transfer Learning: Efficient feature extraction using MobileNetV2.

Explainable AI (Grad-CAM): Visual justification for every prediction.

Multi-View Interpretability: Outputs include grayscale attention maps, colored heatmaps, and original image overlays.

Confidence Scoring: Provides a probability percentage for every classification.
Model Architecture
Base Model: MobileNetV2 (Pretrained on ImageNet).

Global Average Pooling: Reduces spatial dimensions while retaining important features.

Classifier Head: Custom Dense layer for binary output.

Framework: TensorFlow & Keras.
Explainable AI (Grad-CAM)
Grad-CAM (Gradient-weighted Class Activation Mapping) is used to:

Highlight Critical Regions: Identify specific parts of the vehicle (e.g., the frame of a bike or the grille of a car) that drive the classification.

Debug Model Logic: Ensure the model is looking at the vehicle and not the background.

Build Trust: Provide a visual "reasoning" for the classification.

Visual Outputs:

Original Image: The raw input.

Heatmap: High-intensity regions indicating model focus.

Overlay: Combined view for direct comparison.
