# 🚢 Shipping Delay Prediction using Machine Learning

## Overview
Machine learning model predicting shipping delays at ports by analyzing weather conditions, vessel characteristics, port congestion, and operational factors.

## Business Problem
Port delays cost the maritime industry billions annually. Accurate predictions enable:
- Proactive resource allocation
- Improved customer communication
- Optimized berth scheduling
- Reduced operational costs

## Technical Approach

### Dataset
- 5,000 synthetic shipping records
- Features: vessel type, cargo type, weather, congestion, vessel age, maintenance scores
- Target: Binary classification (delayed/on-time)

### Models Implemented
1. **Random Forest Classifier**
   - 100 estimators, max depth 10
   - Cross-validation ROC-AUC: 0.88

2. **Gradient Boosting Classifier**
   - 100 estimators, max depth 5
   - Cross-validation ROC-AUC: 0.90

### Results
- **Accuracy:** 85-90%
- **ROC-AUC Score:** 0.88-0.90
- **Top Predictive Features:** Weather conditions, port congestion, vessel age

## Key Insights
- Storm weather increases delay probability by 40%
- Port congestion above level 7 is critical factor
- Vessels older than 20 years show higher delay rates

## Technologies Used
```python
- Python 3.8+
- Scikit-learn
- Pandas, NumPy
- Matplotlib, Seaborn


## Installation & Usage
# Clone repository
git clone https://github.com/YOUR-USERNAME/data-science-portfolio.git

# Navigate to project
cd 01-shipping-delay-predictor

# Install dependencies
pip install -r requirements.txt

# Run model
python shipping_delay_predictor.py

## Future Enhancements

##Deploy as REST API##
##Real-time predictions integration##
##Extended features (route complexity, crew experience)##
##Multi-class classification (delay duration categories)##
