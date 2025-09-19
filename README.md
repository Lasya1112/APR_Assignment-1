Assignment-1: Wine Quality Prediction (SVM)

This project applies a Support Vector Machine (SVM) classifier on the UCI Wine Quality dataset to predict whether a wine is "good" or "not good" (binary classification).

📊 Dataset

Source: UCI Wine Quality Dataset

Data Used: White Wine dataset (winequality-white.csv) with 4898 samples and 11 chemical features

Target:

Converted into a binary label:

Good (1): quality ≥ 7

Not Good (0): quality < 7

⚙️ Installation & Requirements

Install dependencies using pip:

pip install -r requirements.txt


requirements.txt should contain:

pandas
numpy
matplotlib
seaborn
scikit-learn

▶️ Usage

Run the script from terminal:

python assignment1.py


This will:

Download and preprocess the dataset

Train an SVM classifier (RBF kernel)

Print evaluation metrics to the terminal

Save all plots and metrics into the outputs/ folder

📂 Outputs

After running, check the outputs/ directory. It will contain:

Metrics

svm_metrics_summary.csv → Contains accuracy, precision, recall, and F1-score

Plots

wine_quality_distribution.png → Distribution of wine quality scores

correlation_heatmap.png → Correlation heatmap of features with wine quality

svm_roc_curve.png → ROC curve for SVM classifier

svm_precision_recall_curve.png → Precision–Recall curve for SVM

📈 Results (Sample)

Example performance metrics on test data:

Metric	Value
Accuracy	~0.82
Precision	~0.70
Recall	~0.55
F1-score	~0.62

(Exact values may differ slightly due to randomness in train/test split.)

📑 Project Structure
Assignment-1/
│
├── assignment1.py              # Main script (SVM model training & evaluation)
├── requirements.txt            # Required dependencies
├── outputs/                    # Folder for all generated results
│   ├── wine_quality_distribution.png
│   ├── correlation_heatmap.png
│   ├── svm_roc_curve.png
│   ├── svm_precision_recall_curve.png
│   └── svm_metrics_summary.csv
└── README.md                   # This file

🚀 Conclusion

The SVM classifier achieves ~82% accuracy in distinguishing good vs not good wines.

Alcohol shows the strongest correlation with wine quality.

Model precision is higher than recall, meaning it is conservative when predicting “good” wines.

Future improvements could include handling class imbalance with SMOTE or trying ensemble models.