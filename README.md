# Chronic Disease Project: Predicting Heart Disease and Diabetes

## Project Purpose
Leveraging the latest CDC dataset, the aim is to empower individuals with predictions for both prevalent chronic diseases:heart disease and diabetes, aiding in health assessment and preventive measures. The project also involves developing a website for user-friendly predictions. [Chronic diseases prediction app](https://chronic-diseases.streamlit.app/)

## Project Focus
- **Challenges:**
  - **Class Imbalance:** Addressed through oversampling, class weights, and feature selection for optimal accuracy.
  - **Complex Dataset:** Reduced 39 variables to less than 20 for enhanced user interaction.

- **Decision Paths:**
  - **Path A:** Oversample all minority instances, followed by feature selection.
  - **Path B:** Oversample with a specific ratio, conduct feature selection, and implement a class-weighted model.
  - **Path C:** Direct feature selection followed by a class-weighted model.

## Data Source
Utilized 2022 CDC survey data (preprocessed by KAMIL PYTLAK), covering 400k+ adults and health-related information. [Preprocessing details](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease/data).

## Conclusion
The project achieved valuable insights into the correlation between health status and chronic diseases. While disease-specific predictions have challenges, the model's holistic view contributes to an 80% accuracy in health assessments.

## Recommendations
- **Targeted Interventions:** Tailor interventions for Southern states facing regional health disparities.
- **Health Promotion:** Encourage healthier lifestyles and regular check-ups to reduce chronic disease prevalence.

## Challenges
- **Cross-Validation Issues:** Addressed by creating a separate validation set due to challenges with cross_val_score and gridsearch.
- **Model Generalization:** Features selected may not generalize well to other models, highlighting the need for careful feature selection.
