# 🚗 Vehicle Classification with Explainable AI (XAI) 🚲

## 📌 Project Overview
This project utilizes **Transfer Learning (MobileNetV2)** to classify **Cars vs. Bikes** with high efficiency and minimal computational overhead. 

Beyond simple classification, it integrates **Explainable AI (Grad-CAM)**. This allows the model to "explain" its decision-making by generating visual heatmaps, revealing which specific features—like wheels, headlights, or handlebars—the model focused on to reach a prediction.

---

## 🌟 Key Features
* **High-Accuracy Classification:** Efficient binary classification between cars and bikes.
* **Transfer Learning:** Optimized feature extraction using a pretrained **MobileNetV2** backbone.
* **Explainable AI (Grad-CAM):** Provides visual justification for every prediction to eliminate "black-box" uncertainty.
* **Multi-View Interpretability:** Supports grayscale attention maps, colored heatmaps, and original image overlays.
* **Confidence Scoring:** Real-time probability percentages for every output.

---

## 🏗 Model Architecture


* **Base Model:** MobileNetV2 (Pretrained on ImageNet).
* **Global Average Pooling:** Used to reduce spatial dimensions while retaining critical features.
* **Classifier Head:** Custom Dense layer designed for binary classification.
* **Framework:** TensorFlow & Keras.

---

## 🔍 Explainable AI (Grad-CAM)
Grad-CAM (Gradient-weighted Class Activation Mapping) is implemented to:
1.  **Highlight Critical Regions:** Identify parts of the vehicle (e.g., the grille of a car or frame of a bike) that drive the classification.
2.  **Debug Model Logic:** Verify that the model is focusing on the object rather than irrelevant background noise.
3.  **Build Trust:** Provide a visual "reasoning" layer for users and developers.



---

## 📂 Project Structure
To keep the repository clean, the dataset is not uploaded directly. Please refer to `project_structure.txt` for the full directory map.

### Local Setup:
1.  Create a folder named `dataset`.
2.  Inside, create `train` and `test` folders.
3.  Inside both, create subfolders named `car` and `bike`.
4.  Populate these with your images (Recommended size: **224x224**).

---

## 📊 Dataset Information
* **Source:** [Car vs Bike Classification Dataset (Kaggle)](https://www.kaggle.com/datasets/utkarshsaxenadn/car-vs-bike-classification-dataset)
* **Format:** RGB Images
* **Input Size:** 224 x 224 pixels

---

## 🚀 How to Run
1.  **Clone the Repo:**
    ```bash
    git clone [https://github.com/Patel-Sujal-18/Image-Classification-Project/blob/main/Image_Classification.ipynb]
    ```
2.  **Prepare Dataset:** Follow the folder structure mentioned in the Project Structure section.
3.  **Load Model:** Ensure `vehicle_classifier_model.keras` is in the root directory.
4.  **Execute:** Run the prediction script/notebook to see the:
    * Classification Label
    * Confidence Score
    * Grad-CAM Heatmap Visualization

---

## 🛠 Future Improvements
* Expansion to multi-class classification (Trucks, Vans, etc.).
* Web-based deployment using **Streamlit**.
* Real-time video stream classification.
