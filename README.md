# Ethical Price Prediction Web Application

This project is a machine learning-powered ethical price prediction system developed as part of a team internship project. The goal is to help consumers and businesses assess whether a product's price is fair, overpriced, or underpriced based on real-world ethical factors.

## Overview

The web app uses a Random Forest regression model to predict product prices based on category, item, and city. It then compares the predicted price with a fair pricing range calculated using production cost, sustainability score, local demand, fair wage multiplier, and profit margins.

Users can:
- Predict ethical prices for items
- Compare prices between two cities
- View visual analysis (price distribution, trend, and marketplace comparison)
- Check prediction history

## Tech Stack

- **Backend:** Python, Flask
- **Frontend:** HTML, CSS (Jinja2 templates)
- **ML Model:** Random Forest Regressor (Scikit-learn)
- **Data Handling:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn

## Folder Structure

```
project-root/
│
├── app.py                          # Flask web app
├── model_updated.py                # Model logic + price fairness calculations + graphs
├── ethical_pricing_mock_dataset_extended.csv  # Dataset
│
├── templates/
│   ├── index.html                  # Main UI
│   ├── about.html                  # About page
│   └── history.html                # History table
│
└── static/
    ├── plot_distribution.png
    ├── plot_trend.png
    └── plot_marketplace.png
```

## Features

- Predicts ethical price for selected item, category, and city
- Labels output as: Ethical, Underpriced, or Overpriced
- City-wise price comparison with summary table
- Live graph generation:
  - Price distribution
  - Monthly price trend
  - Marketplace pricing comparison
- Stores all prediction history in session
- Dynamic dropdowns based on selected categories

## How to Run

1. Clone the repo:

```
git clone https://github.com/himanshuujangirr/ethical-pricing-prediction
cd your-repo-name
```

2. Install dependencies:

```
pip install flask pandas numpy matplotlib seaborn scikit-learn
```

3. Run the app:

```
python app.py
```

4. Open your browser and go to:

```
http://127.0.0.1:5000
```

## Contribution

This was a group project built by a team of 6 members as part of an internship. My contributions included:
- Integrating the Random Forest ML model
- Building Flask backend and API routes
- Designing the UI (tabbed navigation, history, compare, about pages)
- Creating automated graph visualizations

## Contact

Himanshu Jangir  
Email: honnyjangir@gmail.com  
LinkedIn: https://www.linkedin.com/in/himanshuujangirr/
