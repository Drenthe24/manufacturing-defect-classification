# Manufacturing Defect Classification

Machine learning project for predicting defective parts in a manufacturing environment using production process data.

---

## Overview

This project focuses on building a supervised machine learning model to classify conforming and defective parts in a production line.

The goal is not only predictive accuracy, but also to support **operational decision-making** in industrial contexts.

---

## Business Context

In manufacturing environments, defects are often caused by complex interactions between process variables rather than single factors.

This project simulates a real-world scenario where:

- data is collected from production processes  
- defects must be detected early  
- decisions must balance quality and operational cost  

---

## Approach

The project includes:

- Exploratory Data Analysis (EDA)  
- Data preprocessing and feature engineering  
- Time-based train/test split  
- Training and comparison of multiple models:
  - Logistic Regression  
  - Decision Tree  
  - Random Forest  
- Model evaluation with focus on real-world impact  

---

## Key Insights

- Defects are not separable using single variables  
- Process instability (vibration, cycle time, temperature) plays a key role  
- Random Forest outperforms linear models but still shows limited recall  

This highlights the importance of **data quality and feature richness** over model complexity.

---

## Results

- Best model: **Random Forest**  
- High precision (~0.87)  
- Low recall for defective parts (~10%)  

The model is reliable when predicting defects, but misses a significant portion of them.

---

## Business Value

The model can be used as a **decision support system** to:

- identify high-risk parts  
- prioritize quality inspections  
- monitor critical process parameters  

---

## Repository Structure

```
manufacturing-defect-classification/
├── data/
│   └── parts_production_data.csv
├── notebook/
│   └── AutomaParts_Git.ipynb
└── README.md
```

---

## How to Run

1. Clone the repository  
2. Open the notebook  
3. Run all cells  

---

## Final Considerations

This project demonstrates how machine learning can support industrial processes even when predictive performance is not perfect.

The main value lies in:

- understanding process behavior  
- identifying critical variables  
- supporting better operational decisions

---

## Example Use Case

If the model predicts a defect probability > 0.8:
- route part to additional inspection
- log process parameters
- trigger alert on production line

---

## Disclaimer

This project is based on a simulated industrial use case.  
All data and identifiers are anonymized.
