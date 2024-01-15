# Chronic Disease Project: Predicting Heart Disease and Diabetes

## Overview
This project aims to simultaneously predict heart disease and diabetes, addressing a gap in existing Kaggle projects that focus on individual diseases. Utilizing the 2022 annual CDC survey data with 400k+ adults' health-related information, the analysis and modeling efforts have yielded valuable insights into the impact of physical status, regional health disparities, and correlations between health status and chronic diseases. The models, with resampling, class-weight, and parameter tuning, exhibit improved performance, contributing to an 80% accuracy. While disease-specific prediction performance is lower (f1 macro score: around 37-43%), the model effectively assesses overall chronic disease risk, providing valuable information for health assessments. The project lays a foundation for understanding and predicting chronic diseases, with potential for future enhancements.

[Chronic Disease Prediction App](https://chronic-diseases.streamlit.app/)
---

### Data Source
Utilized 2022 CDC survey data (preprocessed by KAMIL PYTLAK), covering 400k+ adults and health-related information. [Preprocessing details](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease/data).

### Project Purpose
Leveraging the latest CDC dataset, the aim is to empower individuals with predictions for both prevalent chronic diseases: heart disease and diabetes, aiding in health assessment and preventive measures. The project also involves developing a website for user-friendly predictions. 

### Project Focus
- **Challenges:**
  - **Class Imbalance:** Addressed through oversampling and class weights for optimal accuracy.
  - **Complex Dataset:** Reduced 39 variables to less than 20 for enhanced user interaction.

- **Decision Paths:**
  - **Path A:** Oversample all minority instances, followed by feature selection.
  - **Path B:** Oversample with a specific ratio, conduct feature selection, and implement a class-weighted model.
  - **Path C:** Direct feature selection followed by a class-weighted model.

### Conclusion
The project achieved valuable insights into the correlation between health status and chronic diseases. While disease-specific predictions have challenges, the model's holistic view contributes to an 80% accuracy in health assessments.

### Recommendations
- **Targeted Interventions:** Tailor interventions for Southern states facing regional health disparities.
- **Health Promotion:** Encourage healthier lifestyles and regular check-ups to reduce chronic disease prevalence.

### Challenges
- **Cross-Validation Issues:** Addressed by creating a separate validation set due to challenges with cross_val_score and gridsearch.
- **Model Generalization:** Features selected may not generalize well to other models, highlighting the need for careful feature selection.
