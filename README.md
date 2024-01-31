ML A3

Overview
This project focuses on sentiment analysis using machine learning classifiers SVM and MLP to investigate potential gender biases in the provided dataset.

Dataset
The dataset comprises training, validation, and test sets available in three formats: raw, embeddings, and TF-IDF.

Implementation Details:

Libraries Used:
pandas
matplotlib
sklearn

Data Loading:
The datasets for training, validation, and test are loaded using pandas.

Data Cleaning:
An 'Unnamed' column is dropped from each dataset, if present.

Data Visualization:
Distribution of ratings in the training dataset.
Gender-based distribution of ratings.


Baseline Model (ZeroR):
ZeroR classifier is initialized and trained on the training data.
Its accuracy is then evaluated on the validation data, and further broken down by gender.

Multilayer Perceptron (MLP):
An MLP is trained using the TF-IDF and embeddings representation of the training data.
Its performance is evaluated on the validation dataset using accuracy, confusion matrix, and a classification report.
The MLP's performance is also assessed separately on male and female reviews using the embeddings representation.

Support Vector Machine (SVM):
An SVM is trained using the TF-IDF and embeddings representation of the training data.
Its performance is evaluated on the validation dataset using accuracy, confusion matrix, and a classification report.
The SVM's performance is also assessed separately on male and female reviews using the embeddings representation.

Support Vector Machine (SVM) for submission:
An SVM with an RBF kernel is trained on the embeddings representation of the training data.
Predictions are made on the test dataset using this SVM.
Submission: Predictions from the SVM are saved into a submission DataFrame.

Running the Code:
Ensure all the required libraries are installed and the datasets (TRAIN.csv, VALIDATION.csv, TEST_NO_LABELS.csv, and their embeddings and TF-IDF versions) are available in the working directory.

Execute the Python cells to run the entire sentiment analysis in jupyter notebook.