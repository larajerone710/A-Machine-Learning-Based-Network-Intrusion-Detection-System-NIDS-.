by 
Lara Jerone J

# Network Intrusion Detection using Machine Learning

This project implements a Network Intrusion Detection System (NIDS) using Python and the Scikit-learn library. The model is trained on the NSL-KDD dataset to classify network traffic as "Normal" or a specific type of "Attack."

## Project Overview

In computer communications and networking, security is a major challenge. This project builds an intelligent system to automate the detection of threats.

Instead of relying on static rules, this model uses a *Random Forest Classifier* (a machine learning algorithm) to learn the behavioral patterns of network connections. It analyzes 41 different features of a connection (like its protocol, service, and traffic statistics) to make a highly accurate prediction.

## Dataset

The model is trained and tested using the *NSL-KDD dataset*, a famous benchmark for NIDS research. This repository includes the two main files:

* NSL_KDD_Train.csv: The primary dataset used to *teach* the model.
* NSL_KDD_Test.csv: A separate dataset used to *evaluate* the model's performance on unseen data.

## 🚀 How to Run This Project

1.  *Download:* Download the ZIP of this repository and unzip it.
2.  *Open in VS Code:* Open the unzipped folder (NSL-KDD-Network-Intrusion-Detection-main) in Visual Studio Code.
3.  *Install Libraries:*
    * Open the NSL-KDD-Network-Intrusion-Detection.ipynb file.
    * Run the very first code cell, which contains:
        python
        !pip install numpy pandas scikit-learn matplotlib seaborn
        
4.  *Restart Kernel:* After the installation is complete, *you must restart the kernel. Click the **🔄 (Restart)* button in the top toolbar of the notebook.
5.  *Run All:* Click the *"Run All" (▶▶)* button at the top of the notebook. The notebook will run from top to bottom, load the data, train the model, and print the results.

## Methodology and Results

1.  *Data Loading:* The .csv files are loaded into pandas DataFrames.
2.  *Data Preprocessing:* The model can't understand text like "tcp" or "http". A LabelEncoder is used to convert all text-based columns into numbers that the model can understand.
3.  *Model Training:* A *Random Forest Classifier* is trained on the NSL_KDD_Train.csv data. It learns the complex patterns that distinguish 'normal' connections from 22 different types of attacks.
4.  *Evaluation:* The trained model is then tested against the NSL_KDD_Test.csv file.

*Final Result:* The model achieves an accuracy of *92.17%* in classifying unseen network traffic.

## 🛠 Technologies Used

* Python
* Jupyter Notebook
* *Pandas:* For loading and managing the data.
* *Scikit-learn (sklearn):* For the RandomForestClassifier, LabelEncoder, and calculating the accuracy_score.


Lara Jerone J
Author ✍
