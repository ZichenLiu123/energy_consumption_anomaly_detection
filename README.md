# Energy Consumption Prediction Model

## Project Overview
This project aims to predict whether the monthly energy consumption of university buildings will exceed the established baseline. The work, conducted in collaboration with the Sustainability Office at the University of Toronto, focuses on using weather data and energy consumption records to assist in the efficient management of energy usage, supporting both economic and environmental sustainability.

## Key Features
- **Data Collection**: Weather data and building energy consumption data were collected and merged for analysis. Historical data from 2018 to 2021 were used.
- **Baseline Calculation**: The baseline energy consumption for each building was established as the mean monthly consumption over the entire period.
- **Feature Engineering**: Created several features related to weather patterns, such as temperature, humidity, precipitation, and more, which were used to predict energy consumption.
- **Class Imbalance Handling**: Applied SMOTE (Synthetic Minority Over-sampling Technique) to address the class imbalance in months where consumption exceeded the baseline.

## Machine Learning Models
- **Logistic Regression**: Established baseline performance, with a focus on binary classification (exceeding baseline or not).
- **Random Forest**: Trained and optimized using Grid Search to improve prediction accuracy.
- **Gradient Boosting**: Incorporated for its robustness in handling non-linear relationships.
- **Ensemble Model**: Combined Logistic Regression, Random Forest, and Gradient Boosting models into a Voting Classifier to leverage their collective strengths.

## Results
- **Accuracy**: Achieved a balanced accuracy of 67% with both precision and recall scores around 0.67.
- **Feature Importance**: The key features influencing predictions were temperature (max/min), humidity (max/min), precipitation, rain, snow, and the month of the year.

## Future Work
- **Advanced Feature Engineering**: Introduce more complex features, including interaction terms and lagged variables.
- **Model Optimization**: Explore additional ensemble techniques such as stacking and boosting.
- **Real-Time Implementation**: Develop a real-time prediction system for continuous monitoring and insights.
- **Cross-Validation**: Implement cross-validation to enhance the model's robustness and generalizability.

## Tech Stack
- **Language**: Python
- **Libraries**: Pandas, Scikit-learn, GridSearchCV, SMOTE
- **Models**: Logistic Regression, Random Forest, Gradient Boosting, Voting Classifier

## Business Impact
The project provides a predictive framework that can guide the University of Toronto's facility managers in efficiently managing energy consumption. By leveraging weather data and advanced machine learning techniques, this model offers insights into key factors driving energy usage, enabling more proactive energy management strategies.

## Acknowledgments
Special thanks to the Sustainability Office at the University of Toronto for providing the data and support for this project.
