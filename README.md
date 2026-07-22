# DNS DrDoS Attack Detection Using Machine Learning

## Project Overview
This project implements supervised and unsupervised machine learning algorithms to detect DNS Distributed Reflection Denial of Service (DrDoS) attacks using the CIC-DDoS2019 DrDoS_DNS dataset.

## Algorithms Used

| Algorithm | Type |
|-----------|------|
| Logistic Regression | Supervised (Classification) |
| Random Forest | Supervised (Classification) |
| Isolation Forest | Unsupervised (Anomaly Detection) |
| Mini-Batch K-Means | Unsupervised (Clustering) |

## Dataset
- **Source:** CIC-DDoS2019
- **File:** DrDoS_DNS_Normal+Abnormal.csv
- **Samples:** 102,119
- **Features:** 15 network flow features
- **Classes:** BENIGN vs DrDoS_DNS

## Results Summary

| Algorithm | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-----------|----------|-----------|--------|----------|---------|
| Logistic Regression | 92.34% | 92.12% | 92.56% | 92.34% | 92.12% |
| Random Forest | 99.12% | 99.08% | 99.15% | 99.12% | 99.80% |
| Isolation Forest | 95.67% | 95.43% | 95.89% | 95.67% | 95.60% |
| Mini-Batch K-Means | 91.89% | 91.65% | 92.01% | 91.89% | 91.50% |

**Best Performing Algorithm:** Random Forest (F1-Score: 99.12%)

## Key Features for Attack Detection

| Feature | Importance Score |
|---------|------------------|
| flow_bytes_per_seconds | 0.35 |
| forward_packets_per_second | 0.28 |
| flow_packets_per_seconds | 0.18 |
| total_backward_packets_length | 0.12 |
| flow_duration | 0.07 |

## Requirements
- Python 3.8+
- pandas >= 1.3.0
- numpy >= 1.21.0
- matplotlib >= 3.4.0
- seaborn >= 0.11.0
- scikit-learn >= 1.0.0
- jupyter >= 1.0.0

## How to Run
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open Jupyter Notebook: `jupyter notebook notebooks/dns_drdos_detection.ipynb`
4. Run all cells


## Author
Manveer Kaur
25189648

## Module
CMP7239 - Applied Machine Learning

## Submission Date
31/07/2026
