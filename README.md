<h1> Credit-Risk-Analysis---ML-Clustering-and-Classification (In progress...) </h1>

<h3>Source Dataset: https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29 </h3>

## Overview

<p> Project ini terbagi menjadi tiga bagian, EDA, Clustering dan Classification. Dan pada bagian clustering, di project ini menggunakan <b>K-Means Clustering, Agglomerative Hierarchical Clustering, dan DBSCAN.</b> Sedangkan pada bagian classification, project ini menggunakan <b>Random Forest Classifier dan XGBoost Classifier.</b>
  
## Results

### Clustering

#### K-Means
![GitHub Logo](/images/1.png)
![GitHub Logo](/images/2.png)

#### Agglomerative Clustering
![GitHub Logo](/images/3.png)
![GitHub Logo](/images/4.png)

#### DBSCAN Clustering
![GitHub Logo](/images/5.png)


### Evaluation Metrics for Classification model
 
Metrik Evaluasi pada project ini yang digunakan adalah : <b>F1 Score, recall, precision, ROC-AUC Score, dan Matthews correlation coefficient.</b> Dikarenakan dataset ini tidak termasuk kategori dataset yang <i>highly-imbalanced</i>, maka model terbaik dapat dipilih dari ROC-AUC Score tertinggi. Dan ini hasilnya:
  
| Classifier | F1 Score | recall | precision | ROC-AUC Score | Matthews correlation coefficient| 
|   :---:      |     :---:      |    :---:      |   :---:      |     :---:      |          :---: |
| XGBoost Classifier   | 0.820359    |  	0.978571   | 0.706186   | 0.514286    | 0.076753   |
| Random Forest Classifier     | 0.827381       |  	0.992857     | 	0.709184  | 0.521429        | 0.140283      |
 
 Dari hasil di atas, dapat dilihat bahwa Random Forest memiliki ROC-AUC Score lebih tinggi daripada XGBoost. Dimana dapat disimpulkan bahwa Random Forest, classifier yang lebih baik dalam pembandingan antara kedua model. Namun sayangnya keduanya punya nilai Matthews correlation coefficient yang mendekati 0. Tapi kabar baiknya, mereka memiliki recall yang sama-sama tinggi, yang artinya keduanya dapat menebak dengan baik orang-orang yang beresiko untuk diberi pinjaman.
 
 ### Learning Curve
 
Learning Curve yang akan ditunjukkan hanya untuk Random Forest Classifier, sedangkan untuk XGBoost Classifier terdapat di notebook pada bagian <i>classification</i>

![GitHub Logo](/images/rfc.png)
 
 
 
 [GitHub](https://github.com/Stev-create)

