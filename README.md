# Clipboard Health Superweekend Challenge
This repository contains code and analysis for data visualization and machine learning modeling related to shift offer data. The goal of this project is to analyze key factors affecting shift claims, cancellations, and overall worker engagement, and to recommend strategic solutions to optimize shift fulfillment.

## Repository Overview
This repository consists of the following:
1. **Notebook**: The Jupyter Notebook can be found in `notebook` directory . It is implementing data analysis, visualization, and machine learning modeling
2. **Images**: All graphs and images generated from the code are stored in the `images` directory
3. **Python Source Code**: I have also stored 2 Python Code files in the `src` directory
4. **Results**: All the analysis, insights, recommendations & ML Model Analysis is stored in `results` directory
5. **Data**: The dataset i.e. the CSV File provided by Clipboard Health is in the `data` directory
6. **README**: Documentation to help understand the context, code, and findings

## Problem Objectives
This analysis focuses on understanding factors that influence shift outcomes, worker behavior, and workplace efficiency. The main objectives are:
1. **Understand Shift Claim Patterns**: Explore the data to understand how different factors impact the claim rates for shifts.
2. **Identify Opportunities for Improvement**: Highlight areas such as cancellation rates, worker engagement, and low-claimed shifts, and propose strategic improvements.
3. **Machine Learning Insights**: Utilize machine learning to predict which shifts are likely to be claimed and uncover the most important features driving this prediction.

## Data Visualization & Analysis
The data visualization section aims to provide a comprehensive overview of shift offers, worker behavior, and shift fulfillment trends. Key visualizations included in the notebook:
- **Distribution of Shift Outcomes**: Analyze the open, worked, and canceled shifts.
- **Revenue by Shift Slot**: Understand revenue generation based on different time slots (AM, PM, NOC).
- **Lead Time and Shift Outcome Analysis**: Explore the correlation between lead time and shift fulfillment.
- **Claim Rate by Rate Offered and Shift Slot**: Evaluate how pay rates impact the likelihood of a shift being claimed.

## Machine Learning Modeling
A Random Forest Classifier was used to predict shift claim likelihood. The modeling process included:
1. **Data Preparation**: Features like pay rate, duration, lead time, time slot, and day of the week were used as inputs. Categorical features were converted to dummy variables.
2. **Handling Imbalance**: SMOTE (Synthetic Minority Oversampling Technique) was used to handle class imbalance in the dataset.
3. **Model Training & Evaluation**: The model was trained using a train-test split and evaluated with cross-validation to ensure reliable performance.

Key metrics:
- **Cross-validation Accuracy**: ~96%
- **Feature Importance**: Duration, rate, and lead time were identified as the most important features.

## How to Use

To explore this repository:

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/aditibhide/Clipboard-Health-Superweekend-Challenge.git
   ```

2. **Dependencies**:
   Make sure you have the required libraries installed. You can install them using:
   ```sh
   pip install -r requirements.txt
   ```

3. **Run the Notebook**:
   Open the Jupyter Notebook file and execute the cells to see the analysis and visualizations.

## Results Summary
- **Shift Fulfillment Trends**: Higher pay rates are positively correlated with higher claim rates. NOC shifts tend to have a lower claim rate unless pay is significantly increased.
- **Cancellation Insights**: A small number of workers are responsible for a high cancellation rate, indicating the need for targeted cancellation reduction strategies.
- **Revenue Analysis**: AM and PM shifts generate more revenue compared to NOC shifts, and Saturday has the highest number of shifts posted.

## Contact
For questions or suggestions, feel free to open an issue or reach out to [aditibhide](https://github.com/aditibhide).

