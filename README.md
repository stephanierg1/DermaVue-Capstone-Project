# DermaVue-Capstone-Project: AI-Driven Personalized Skincare

Machine Learning Approach to Skincare Product Recommendations

By: Stephanie Ros

# Overview

DermaVue is an AI-driven skincare recommendation system. It analyzes user's skin conditions using a multi-label classification model, and recommends skincare products based on their individual needs and preferences. 

# Structure

**Streamlit.ipynb** - Streamlit web application for users to interact with the recommendation system, including features to input personal information, preferences and face image. Finally, users' skin condition is evaluated by the model and they are given a set of product recommendations based on their skin's needs and preferences. 

**Recommender System Evaluation.ipynb** - Recommendation System's performance evaluation, computes metrics to assess how good recommendations are. 

**mobilenetv2_finetuned_augmentation.keras** - Final trained model used for skin condition predictions.

**Model Training Using Original Dataset (10 classes).ipynb** - Data Exploratory Analysis, Models' Pre-tranining Comparison, and MobileNetV2 fine-tuning using 2 different strategies. The dataset used for these model versions' training contained 10 different classes.  

**Model Training Using Smaller Dataset (8 classes).ipynb** - Models' Pre-tranining Comparison, and MobileNetV2 fine-tuning using 2 additional strategies, once the most unbalanced classes where dropped from the dataset. The resulting dataset used for these versions contained 8 classes. 

**README.md** — Current file.

# Model Development 
First, 3 models where pre-trained and compared: MobileNetV2, ResNet50, EfficientNetB3. Then, the best performing one, MobileNetV2, was fine-tuned and used for the final product. 

**Datasets:** 

  **Skin Conditions for Model Training:** Skin Problems Multi-label Dataset from Roboflow

  **Skincare Products for Recommendation System:** Skincare Products Clean Dataset from Kaggle 

**Metrics:** 

  **Model Testing:** Macro F1, Micro F1, AUC, Precision, Recall 

  **Recommendation System Testing:** Precision, Recall, Coverage

# Run Instructions 

1. Open on Google Colab and upload all files.
2. Install dependencies: !pip install streamlit pyngrok
3. Add Libraries: tensorflow, keras, numpy, pandas, scikit-learn, streamlit, pyngrok, PIL, seaborn, matplotlib, kagglehub, ImageDataGenerator (Keras)
4. Run App: Streamlit.py

# References 

Shakya, D. (2023). Oily, Dry, and Normal Skin Types Dataset. Retrieved from https://www.kaggle.com

Kittipongdaja, P. (2023). Skin-Problem-MultiLabel Dataset [Open source dataset]. Roboflow Universe. Retrieved February 16, 2025, from https://universe.roboflow.com/parin-kittipongdaja-vwmn3/skin-problem-multilabel

