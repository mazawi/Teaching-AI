# Lecture 04 — Machine Learning Practical Examples

**Module:** OMC9000UK7, Principles and Applications of Artificial Intelligence and Machine Learning
**Programme:** MSc AI and Machine Learning, Gulf College
**Purpose:** 18 independently runnable simulated-data practicals, three each in six categories.

## Getting started
1. Install Python 3 and packages: `pip install -r requirements.txt`.
2. Open any example folder in Jupyter or VS Code.
3. Open `example.ipynb` and choose **Run All**.
4. Keep `dataset.csv` next to its notebook.
5. Study the metrics and the new-input prediction or policy at the end.

## Choosing valid evaluation measures
- **Classification:** accuracy, precision, recall, F1 and a confusion matrix (held-out data).
- **Regression:** MAE, RMSE, R² and residual plots. Classification metrics are inappropriate for a continuous target.
- **Clustering:** silhouette and (in simulation only) adjusted Rand index; cluster labels have arbitrary identifiers.
- **Anomaly detection:** accuracy, precision, recall, confusion matrix **only because simulated truth labels are provided for evaluation**.
- **Association rules:** support, confidence and lift; these are not classifier predictions.
- **Reinforcement learning:** episode reward, success and policy behaviour, not supervised accuracy.

## Exercises index

| # | Topic | Example | Dataset rows |
|---:|---|---|---:|
| 1 | Classification | [Car-type recommendation](01_Classification_Car_Type_Recommendation/example.ipynb) | 600 |
| 2 | Classification | [Student pass prediction](02_Classification_Student_Pass_Prediction/example.ipynb) | 750 |
| 3 | Classification | [Email spam classification](03_Classification_Email_Spam/example.ipynb) | 620 |
| 4 | Regression | [GPA estimator](04_Regression_GPA_Estimator/example.ipynb) | 680 |
| 5 | Regression | [Salary estimator](05_Regression_Salary_Estimator/example.ipynb) | 720 |
| 6 | Regression | [Apartment rent estimator](06_Regression_Apartment_Rent/example.ipynb) | 740 |
| 7 | Clustering (K-means) | [Customer segmentation with K-means](07_Clustering_Customer_Segmentation/example.ipynb) | 630 |
| 8 | Clustering (K-means) | [Student learning-pattern clustering](08_Clustering_Student_Study_Patterns/example.ipynb) | 570 |
| 9 | Clustering (K-means) | [Vehicle usage clustering](09_Clustering_Vehicle_Usage/example.ipynb) | 540 |
| 10 | Anomaly detection | [Suspicious transaction alerts](10_Anomaly_Suspicious_Transactions/example.ipynb) | 850 |
| 11 | Anomaly detection | [Equipment sensor anomalies](11_Anomaly_Machine_Sensor_Faults/example.ipynb) | 830 |
| 12 | Anomaly detection | [Unusual login activity](12_Anomaly_Unusual_Login_Activity/example.ipynb) | 780 |
| 13 | Association rule mining | [Supermarket basket associations](13_Association_Supermarket_Baskets/example.ipynb) | 650 |
| 14 | Association rule mining | [Course-selection patterns](14_Association_Course_Selection/example.ipynb) | 660 |
| 15 | Association rule mining | [Online-store accessory suggestions](15_Association_Online_Store/example.ipynb) | 620 |
| 16 | Reinforcement learning (tabular Q-learning) | [Robot navigation by Q-learning](16_Reinforcement_Grid_Robot/example.ipynb) | 80 |
| 17 | Reinforcement learning (tabular Q-learning) | [Battery charging and work decisions](17_Reinforcement_Battery_Management/example.ipynb) | 12 |
| 18 | Reinforcement learning (tabular Q-learning) | [Inventory ordering with Q-learning](18_Reinforcement_Inventory_Control/example.ipynb) | 132 |

## Academic and ethical caution
All data are artificially generated and should not be interpreted as factual patterns about real students, employees, medical outcomes, customers or people. Predictive results on simple simulations can be unrealistically good. Use real datasets only after permission, privacy controls and an appropriate research/teaching review.

## Lecture alignment
Lecture 04 explores supervised, unsupervised and reinforcement learning; classification, regression, clustering, anomaly detection, association rules; data representation, training/test separation, evaluation and generalisation. MLO1 and MLO3 are emphasised; discussions around choosing algorithms prepare students for MLO4.

**References:** Russell & Norvig (2021), Mitchell (1997), scikit-learn User Guide https://scikit-learn.org/stable/user_guide.html.