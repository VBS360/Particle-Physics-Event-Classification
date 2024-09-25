# Particle Physics Event Classification

![Header Image](https://github.com/user-attachments/assets/f733ae23-b9d8-4518-be65-822317663ee2)

## Overview
Welcome to the **Particle Physics Event Classification** project! This project leverages machine learning to classify particle physics events into either signal (s) or background (b). Accurate classification is crucial in the field of particle physics to identify events of interest and filter out noise, aiding researchers in their exploration of fundamental particles and their interactions.

## Problem Statement
In particle physics, experiments generate a vast amount of data where only a fraction is of actual interest. This project aims to build a robust machine learning model to classify events into either signal (s) or background (b), facilitating the identification of significant events.

## Dataset
The dataset contains 250,001 rows and 33 columns. Each row represents an event, with features derived from particle physics experiments. The features include kinematic properties and other attributes that help distinguish signal events from background noise.

## Approach
1. **Data Preprocessing**:
   - Handled missing values (e.g., placeholder values like 999) and normalized the features.
   - Performed feature selection to improve model performance.
   - Applied SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance by oversampling the minority class (signal events).

2. **Exploratory Data Analysis (EDA)**:
   - Analyzed feature distributions to understand the data’s spread and identify potential outliers or anomalies.
   - Used correlation matrices to uncover relationships between key features.
   - Visualized class imbalances between signal and background events.

3. **Model Building**:
   - **Logistic Regression**: Trained a Logistic Regression model as a baseline to classify signal vs. background events. Despite good accuracy (98.59%) and ROC AUC (0.937), it slightly underperformed on non-linear interactions in the data.
   - **Random Forest Classifier**: Developed a more complex Random Forest model that handled non-linearities effectively, achieving perfect classification (100% accuracy).

4. **Model Evaluation**:
   - Evaluated both models using accuracy, precision, recall, F1-Score, and ROC AUC.
   - **Logistic Regression**: Achieved an accuracy of 98.59% with slight underperformance in recall for background events.
   - **Random Forest**: Achieved perfect scores across all evaluation metrics, proving its strong capability in particle physics event classification.

5. **Conclusion & Recommendations**:
   - Both models identified key features like `Weight`, `DER_mass_MMC`, and `DER_mass_transverse_met_lep` as crucial for accurate classification.
   - Recommended focusing on these influential features in future particle physics experiments to enhance the interpretability and accuracy of models.
   - Suggested further exploration of non-linear models like Random Forest for real-time classification tasks.

## Key Insights
- **Model Comparison**:
   - **Logistic Regression**: Strong performance (98.59% accuracy, 0.937 ROC AUC), ideal for simpler, linear relationships and interpretability.
   - **Random Forest**: Achieved perfect classification, proving more suitable for handling complex patterns in particle physics data.
- **Feature Importance**: Key features such as `Weight`, `DER_mass_MMC`, and `DER_mass_transverse_met_lep` played significant roles in event classification across both models.

## What's Next?
- **Real-Time Event Classification**: Deploy the Random Forest model in real-time particle physics experiments to promptly classify signal vs. background events.
- **Further Research**:
   - Investigate **advanced feature engineering** to uncover hidden patterns in the data.
   - Experiment with other machine learning models like Gradient Boosting or Neural Networks to potentially improve on the baseline Logistic Regression model.
   - Continue to explore **Logistic Regression** for scenarios requiring model simplicity and transparency.

## How to Use
1. Clone the repository: 
   ```bash
   git clone https://github.com/VBS360/Particle-Physics-Event-Classification.git
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebook to explore the project:
   ```bash
   jupyter notebook Particle_Physics_Event_Classification.ipynb
   ```

## Repository Structure
- `Particle_Physics_Event_Classification.ipynb`: Jupyter notebook containing the complete analysis and model building process.
- `data/`: Folder containing the dataset (if available).
- `images/`: Folder containing images and visualizations used in the project.
- `Header Image.png`: Header image for this README file.

## Contact
If you have any questions or feedback, feel free to reach out to Vatsal Shah at vatsal793@gmail.com.
