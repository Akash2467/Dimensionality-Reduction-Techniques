# Dimensionality-Reduction-Techniques
Dimensionality Reduction Techniques for BMI Classification
This project applies and compares three popular dimensionality reduction techniques—PCA, SVD, and t-SNE—on the ANSUR II Male Dataset. The objective is to reduce high-dimensional numeric data and improve the classification of individuals into BMI categories using machine learning models.

Dataset
Dataset Name: ANSUR II Male Dataset
Description: Contains anthropometric measurements of male U.S. Army personnel
Target Variable: BMI_class

Objective
Reduce the number of input features while retaining most of the variance
Visualize and compare different dimensionality reduction methods
Evaluate classification performance using Random Forest and SVC models on reduced feature sets

Dimensionality Reduction Techniques
Principal Component Analysis (PCA)
Cumulative variance was used to determine the optimal number of components
Selected 3 components based on the scree plot and elbow method

Results:

95% accuracy using Random Forest

Good accuracy using SVC as well

Truncated Singular Value Decomposition (SVD)
Reduced dimensionality to 35 components to retain 95% variance

Results:

92% accuracy using Random Forest

98% accuracy using SVC

t-SNE (t-distributed Stochastic Neighbor Embedding)
Used for 2D visualization and comparative performance evaluation

Optimal perplexity identified as 50 using KL divergence analysis

Results:

93% accuracy using Random Forest

92% accuracy using SVC

Models Used
Random Forest Classifier

Support Vector Classifier (SVC)

Each model was trained and tested on the transformed data generated by PCA, SVD, and t-SNE.

Visualizations
Scree plots for PCA and SVD

2D scatter plots for t-SNE projections

KL Divergence vs Perplexity plot for tuning t-SNE

Classification reports and accuracy scores

Results Summary
Technique	Components Used	Random Forest Accuracy	SVC Accuracy
PCA	        3	                    95%	                   ~95%
SVD	        35	                  92%	                    98%
t-SNE	      2	                    93%	                    92%

Technologies and Libraries
pandas, numpy

matplotlib, seaborn

scikit-learn for preprocessing, decomposition, modeling

PCA, TruncatedSVD, TSNE from sklearn
