# Bank Marketing Campaign Analysis

## Overview
This project analyzes a Portuguese banking institution's marketing campaigns to predict whether a client will subscribe to a term deposit. The analysis compares the performance of various machine learning classifiers (K-Nearest Neighbors, Logistic Regression, Decision Trees, and Support Vector Machines) to identify the most effective model for predicting customer subscription behavior.

## Data Source
The dataset comes from the [UCI Machine Learning repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing) and contains information about:
- Client demographics (age, job, marital status, education)
- Campaign information (contact type, month, day, duration)
- Previous campaign outcomes
- Economic indicators

## Key Findings

### Model Performance
- Decision Tree emerged as the best performer with ROC-AUC score of 0.759
- KNN showed high accuracy (89.5%) but lower ROC-AUC
- Logistic Regression demonstrated stable but lower overall performance

### Important Features
The most influential features for predicting term deposit subscription were:
1. Previous campaign outcome
2. Age and age groups
3. Marital status
4. Contact type
5. Month of contact

### Campaign Insights
- Success rates vary significantly by month
- Previous contact outcomes strongly influence success probability
- Age and marital status are key demographic factors

## Recommendations

### Campaign Optimization
1. Timing:
   - Focus campaigns during months with historically higher success rates
   - Optimize contact timing based on day-of-week patterns

2. Customer Targeting:
   - Prioritize customers with positive previous interactions
   - Focus on age groups showing higher conversion rates
   - Tailor approach based on marital status and job type

3. Process Improvements:
   - Implement real-time prediction system using Decision Tree model
   - Monitor and update model periodically
   - Consider collecting additional relevant features

## Repository Structure
- `bank_campaigns.ipynb`: Main Jupyter notebook containing analysis
- `banking.py`: Python script with model implementation
- `images/`: Directory containing visualization plots
  - Feature importance plot
  - Decision tree visualization
  - ROC curves comparison
  - Distribution plots

## Requirements
- Python 3.x
- Required packages:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn

## Usage
1. Clone the repository
2. Install required packages: `pip install -r requirements.txt`
3. Run the Jupyter notebook: `jupyter notebook bank_campaigns.ipynb`

## Future Enhancements
1. Technical Implementation:
   - Deploy model as API for real-time predictions
   - Create dashboard for campaign performance monitoring
   - Set up automated model retraining pipeline

2. Business Integration:
   - Train marketing team on model insights
   - Develop targeted scripts based on key features
   - Set up A/B testing framework

## Author
Tyler Scharf https://www.linkedin.com/in/tylerscharf

## License
This project is licensed under the MIT License - see the LICENSE file for details.
