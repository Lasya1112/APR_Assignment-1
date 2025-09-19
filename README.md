# 🍷 Wine Quality Prediction using SVM  
---

##  Project Overview
This project applies a **Support Vector Machine (SVM)** classifier on the **UCI Wine Quality Dataset** to classify wines into:  
- **Good Quality (1):** quality ≥ 7  
- **Not Good (0):** quality < 7  

The dataset contains **4898 white wine samples** with **11 physicochemical features** (e.g., acidity, residual sugar, alcohol).  
The goal is to predict whether a wine is "good" or "not good" based on these features.  

---

##  Install Dependencies
pip install -r requirements.txt

## Run the Script
python assignment1.py

# 📊 Results & Evaluation
## Performance Metrics
Metric	      Value
Accuracy   	  ~0.83
Precision	  ~0.77
Recall	      ~0.35
F1-score	  ~0.48

* High accuracy and precision
* Lower recall due to dataset imbalance (fewer "good" wines)

## Visualizations
1. Wine Quality Distribution

Shows imbalance between good and not good wines.


2. Feature Correlation Heatmap

Correlation between physicochemical properties and quality (alcohol is most correlated).


3. ROC Curve

Evaluates classifier performance across thresholds.


4. Precision–Recall Curve

Shows tradeoff between precision and recall.

## Conclusion

* The SVM model achieves ~83% accuracy in classifying wines.

* Strengths: Reliable when predicting "good" wines (high precision).

* Weaknesses: Misses some good wines (low recall due to imbalance).
