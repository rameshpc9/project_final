MSc Data Science Project – Final Report
Module: 7PAM2002
Department: Physics, Astronomy and Mathematics
Student: Ramesh Dasari (SRN: 23038360)
Supervisor: Carolyn Devereux
Submission Date: 29-04-2025
Project Title: Breast Cancer Detection Using Machine Learning Models: A Comparative Study of Random Forest, XGBoost, and Artificial Neural Networks
GitHub Repository: github.com/rameshpc9/project_final

Declaration
This report is submitted as part of the requirements for the MSc Data Science degree at the University of Hertfordshire. I confirm that the work is entirely my own and complies with the university’s academic integrity and ethics standards. No human participants were involved in this project, and all data used was anonymised and publicly available.

Abstract
Breast cancer continues to be a significant cause of mortality among women worldwide. The goal of this project is to develop and compare machine learning models to classify tumors as benign or malignant using the Wisconsin Breast Cancer Diagnostic Dataset. After preprocessing the data through encoding and normalization, three classifiers—Random Forest, XGBoost, and Artificial Neural Network (ANN)—were trained and evaluated using accuracy, precision, recall, F1-score, and ROC-AUC. The ANN achieved the highest accuracy at 98.2%, closely followed by Random Forest and XGBoost. The results underscore the potential of AI-powered early detection tools in clinical decision-making.

Project Overview
The research investigates the ability of advanced machine learning models to accurately identify breast cancer using clinical features extracted from digitized FNA (fine needle aspirate) images. The models tested include ensemble methods (Random Forest, XGBoost) and a neural network classifier (ANN). Performance was validated on stratified train-test splits with techniques like class balancing and hyperparameter tuning.

Dataset Description and Preprocessing
The dataset used was sourced from the UCI Machine Learning Repository and contains 569 instances with 30 numerical features representing cell characteristics. The target variable (diagnosis) was encoded (Malignant = 1, Benign = 0). Data was scaled using StandardScaler and class imbalance was addressed using upsampling techniques. No missing values were present in the dataset, making it suitable for direct model application.

Methodology
Each model underwent training using a balanced and normalized dataset. For XGBoost, class weighting was adjusted to handle imbalance. Random Forest was trained using balanced class weights. The ANN was implemented using MLPClassifier with one hidden layer. Evaluation metrics were computed using test predictions, and ROC curves were plotted to visualize performance.

Results Summary
All models performed well with precision scores of 1.00 on malignant predictions, meaning no false positives were detected. The ANN and XGBoost models had a recall of 0.90, whereas Random Forest had the highest recall at 0.93, making it the most balanced and reliable model. ROC-AUC scores were extremely high across all models, with Random Forest leading at 0.9965.

Analysis and Insights
Random Forest emerged as the best-performing model in terms of both classification metrics and clinical relevance. Its ability to maintain high recall and precision makes it suitable for deployment in real-world cancer detection settings. ANN and XGBoost also performed admirably and provide viable alternatives depending on resource and interpretability constraints.
