<h1> Credit-Risk-Analysis---ML-Clustering-and-Classification (In progress...) </h1>

<h3>Source Dataset: https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29 </h3>

## Overview

<p> Pada bagian clustering, di project ini menggunakan K-Means Clustering, Agglomerative Hierarchical Clustering, dan DBSCAN. Sedangkan pada bagian classification, project ini menggunakan Random Forest Classifier dan XGBoost Classifier.
  
## Results
 
Metrik Evaluasi pada project ini yang digunakan adalah : <b>F1 Score, recall, precision, ROC-AUC Score, dan Matthews correlation coefficient.</b> Dikarenakan dataset ini tidak termasuk kategori dataset yang <i>highly-imbalanced</i>, maka model terbaik dapat dipilih dari ROC-AUC Score tertinggi. Dan ini hasilnya:
  
| Classifier | F1 Score | recall | precision | ROC-AUC Score | Matthews correlation coefficient| 
|   :---:      |     :---:      |    :---:      |   :---:      |     :---:      |          :---: |
| XGBoost Classifier   | 0.820359    |  	0.978571   | 0.706186   | 0.514286    | 0.076753   |
| Random Forest Classifier     | 0.827381       |  	0.992857     | 	0.709184  | 0.521429        | 0.140283      |
 
 Dari hasil di atas, dapat dilihat bahwa Random Forest memiliki ROC-AUC Score lebih tinggi daripada XGBoost. Dimana dapat disimpulkan bahwa Random Forest, classifier yang lebih baik dalam pembandingan antara kedua model. Namun sayangnya keduanya punya nilai Matthews correlation coefficient yang mendekati 0. Tapi kabar baiknya, mereka memiliki recall yang sama-sama tinggi, yang artinya keduanya dapat menebak dengan baik orang-orang yang beresiko untuk diberi pinjaman. 

