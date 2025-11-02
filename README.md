# Anomaly Detection in Financial Transactions

## Overview

This project identifies unusual or suspicious financial transactions using machine learning. By combining data exploration, statistical thresholds, and Isolation Forest, it flags transactions that deviate from normal behavior and simulates real-world risk detection used in banking and fintech fraud systems.

## Objectives
* Analyze transaction patterns across amount, frequency, and timing
* Visualize behavioral trends and detect outliers
* Train and evaluate an Isolation Forest anomaly detection model
* Build an interactive input system to classify user-provided transactions in real time

## Methods
* Dataset: 1000 simulated financial transactions
* Tech stack: Pandas, Scikit-learn, Plotly, Matplotlib, Seaborn
* Approach:
	* EDA to explore user, timing, and transaction patterns
	* Statistical anomaly checks (2 standard deviation rule)
	* Isolation Forest with SMOTE to handle rare anomaly cases
	* Classification report and confusion matrix for evaluation
	* Interactive user input for anomaly prediction

## Key Findings
* Isolation Forest achieved ~99% accuracy with strong recall for anomalies
* True anomalies represent roughly 2% of transactions
* High-value transactions and unusually high frequency often signal risk
* SMOTE improved minority anomaly detection during model training

## Outcome

A reproducible anomaly detection pipeline that combines statistical logic, machine learning, and interactive prediction. Useful as a foundation for fraud detection systems, transaction monitoring dashboards, or risk-scoring engines in fintech environments.

## Future Work
* Add temporal features (rolling transaction windows)
* Incorporate additional behavior-based signals (geo-location, device ID)
* Deploy as a web or API-based fraud screening tool
* Test deep-learning approaches like Autoencoders