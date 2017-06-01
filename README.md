# Intrusion Detection System: A Robust Machine Learning Approach 
#### We aim to find a robust approach of IDS using ML algorithms that can work different datasets, so we collect three datasets, e.g., KDDCup99, NSL-KDD and GureKDD. While NSL-KDD is processed version of existing KDDCup99 dataset, hence those are same dataset, which does not suit with our goal to use different datasets for testing and training. Descriptions of these datasets are given below

## A.	KDDCup99
The KDD dataset was used in the UCI KDD1999 competition. The objective of the competition is to develop intrusion detection system models to detect attack categories i.e. DOS, PROBE, R2L and U2R. The KDD Cup99 dataset available in three different files such as KDD full dataset, which contains 489,8431, instances, KDD Cup 10% dataset, which contains 494,021 instances, KDD Corrected dataset which contains 311,029 instances. We use the full dataset for our study

## B.	GureKDD
GureKDDcup [6] dataset contains connections of kddcup99 (database of UCI repository) but it adds its payload (content of network packets) to each of the connections. It will permit to extract information directly from the payload of each connection to be used in machine learning processes. 

## METHODOLOGY

After collecting the datasets, we take KDDcup99 as training and GureKDD as testing. Then we select the algorithms for our study. Before feeding the data in the ML algorithms we preprocess the datasets. We also perform manual investigation and modification to make the datasets compatible to run the algorithms

### Data preprocessing 
Data preprocessing is the most time consuming and complex task of preparing for subsequent analysis as per requirement for IDS model. If the dataset contains duplicate records then the clustering or classification algorithms take more time and also provides inefficient results. To achieve more accurate and efficient model your dataset should be free from noise and redundancy samples. To do data preprocessing, we perform following steps

a)	Remove duplicate records</br>
b)	Removing outliers</br>
c)	Perform numeric transformation (e.g., log scale)</br>
d)	 Normalize the dataset.</br>

### Feature Selection</br>
Feature selection is an important data processing step. Selecting the appropriate features can increase the efficiency of ML algorithms; at the same time it reduces the curse of data dimensionality. There are many techniques for features selection among which information gain (IG) and principal component analysis are the two most popular approaches in the literature. 

### Analysis
There are several criteria by which the ML/DM methods for cyber could be compared:
•	Accuracy </br>
•	Time for training a model</br>
•	Understandability of the final solution (classification)</br>
•	Time for classifying an unknown instance with a trained model</br>

### Conclusion
In this study we have used different ML algorithms on different datasets to build a robust approach for IDS. We have found Random Forest (RF) has performed the best among the selected algorithms along with the preprocessing steps. We would recommend usage of decision tree base (e.g., RF) for a robust anomaly base IDS.
