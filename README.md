# Integrated Health Assessment: Predicting Heart Disease and Diabetes with CDC Data

### Overview
This project aims to simultaneously predict heart disease and diabetes, bridging a gap in existing prediction models that typically focus on individual diseases. Leveraging the 2022 annual CDC survey data containing health-related information from over 400,000 adults, the analysis and modeling endeavors have unearthed valuable insights regarding the influence of physical status, regional health disparities, and correlations between health status and chronic diseases. Additionally, the project includes the development of a user-friendly website for predictions.

[Chronic Disease Prediction App](https://chronic-diseases.streamlit.app/)

<img src="https://github.com/sun712k/chronic-disease/assets/120434553/b5c88f48-9739-48a5-ac43-822ea0b7b546" alt="Image" width="60%">


### Data Understanding
Originally part of the Behavioral Risk Factor Surveillance System (BRFSS), the dataset underwent preprocessing by [KAMIL PYTLAK](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease/data), reducing nearly 300 variables to 40. The selected 40 variables cover physical status, personal habits, medical procedures, vaccinations, and other health indicators. The dataset exhibits class imbalance, which is mitigated through oversampling and/or class-weight modeling techniques. To enhance user-friendliness, the number of variables is reduced to less than 20.

<img width="400" alt="image" src="https://github.com/sun712k/chronic-disease/assets/120434553/b332e608-1aff-4374-af8a-25a6b4a8d3bc">
<img width="400" alt="image" src="https://github.com/sun712k/chronic-disease/assets/120434553/010282af-8217-49b9-bb5d-b75e389baaf0">

### Modeling and Evaluation 
Various models were experimented with, employing techniques such as resampling, class-weight adjustments, and parameter tuning. The final model demonstrated improved performance, achieving an 80% accuracy rate. Although the performance in disease-specific predictions was lower, with F1 macro scores ranging from 37% to 43%, the model effectively evaluates overall chronic disease risk, offering valuable insights for health assessments.

<img width="300" alt="image" src="https://github.com/sun712k/chronic-disease/assets/120434553/ad8b326b-33a8-43f1-aaee-f98cb54f50b0">

### Conclusion
The project has yielded valuable insights into the correlation between health status and chronic diseases. Although there are challenges with disease-specific predictions, the model's holistic view contributes to an 80% accuracy in health assessments. The website utilizing the prediction model can encourage users to adopt healthier lifestyles and undergo regular check-ups to reduce the prevalence of chronic diseases. Notably, regional health disparities exist, and interventions tailored to Southern states should be discussed. To increase prediction accuracy, additional features such as blood pressure and high cholesterol, recognized as high-risk factors for heart disease by the CDC, should be considered.

