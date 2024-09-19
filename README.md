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
   - Handled missing values and normalization.
   - Performed feature selection to enhance model performance.
   - Applied SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance.
   
2. **Exploratory Data Analysis (EDA)**:
   - Analyzed feature distributions to understand their characteristics.
   - Used correlation matrices to identify relationships between features.
   
3. **Model Building**:
   - Trained a Random Forest Classifier to distinguish between signal and background events.
   - The model achieved perfect classification, highlighting its effectiveness in particle physics event classification.
   
4. **Model Evaluation**:
   - Evaluated using metrics like accuracy, precision, recall, and ROC AUC.
   - Achieved a perfect score across all evaluation metrics.
   
5. **Conclusion & Recommendations**:
   - Identified key features such as `Weight`, `DER_mass_MMC`, and `DER_mass_transverse_met_lep` that play a crucial role in event classification.
   - Recommended targeted experiments focusing on these influential features for further research.

## Key Insights
- **Feature Importance**: `Weight`, `DER_mass_MMC`, and `DER_mass_transverse_met_lep` are significant contributors to event classification.
- **Perfect Classification**: The Random Forest model achieved 100% accuracy, demonstrating its strong capability to classify particle physics events accurately.

## What's Next?
- **Real-Time Event Classification**: Applying this model in real-time particle physics experiments.
- **Further Research**: Exploring advanced feature engineering and other machine learning models to uncover more nuances in the data.

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
