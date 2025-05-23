# **Smart ECG Analysis: Arrhythmia Prediction with Machine Learning**

## **Contributors**  
- Shruti Maru  
- Medha Tripathi  

## **Overview**  
This project focuses on detecting and predicting different types of cardiac arrhythmias using machine learning models based on Electrocardiogram (ECG) signals. By training models on labeled datasets, we aim to automate arrhythmia classification, improving diagnostic accuracy and reducing human error.  

## **Background & Motivation**  
Arrhythmia refers to irregular heart rhythms, which can range from harmless to life-threatening. Electrocardiogram (ECG) is a widely used, cost-effective, and non-invasive tool for capturing heart activity. However, manually interpreting large ECG datasets is time-consuming and prone to human error, leading to misclassification.  

To enhance efficiency, we leverage machine learning for automated arrhythmia detection. The UCI Machine Learning Repository provides an ECG dataset transformed into QRS complexes (column 10) based on the R-peak (column 19) of 17 different heartbeat types. Given the class imbalance, we employ weighted class models with proportionate sampling. Our approach includes:  
- Extracting QRS complexes using annotated files with R-peak as the center.  
- Designing and training machine learning models, including deep neural networks.  
- Hyperparameter tuning for optimal performance.  
- Splitting the dataset into 70% training and 30% testing data.  
- Implementing **1D Convolutional Neural Networks (1D-CNN), Multi-Layer Perceptron (MLP), Support Vector Machine (SVM),** and **K-Nearest Neighbors (KNN)** with k-fold cross-validation.  

## **Model Selection & Justification**  

### **Support Vector Machine (SVM)**  
- Reliable for stratified datasets and effective for classification and regression.  
- Achieved the highest accuracy of **73.53% using a linear kernel and a weighted loss function**.  

### **K-Nearest Neighbors (KNN)**  
- Requires no prior training, allowing seamless integration of new data without impacting accuracy.  
- Performs well in pattern recognition for ECG signals.  

### **Multi-Layer Perceptron (MLP)**  
- MLPs are universal approximators that capture non-linear relationships in data.  
- Suitable for classification tasks involving categorical labels.  

### **1D Convolutional Neural Network (1D-CNN)**  
- Primarily used for image classification but applicable to waveform analysis.  
- Automatically extracts relevant features, improving classification accuracy.  

## **Results & Conclusion**  
Our models successfully classified arrhythmia types, addressing class imbalance through proportionate sampling. Accuracy values ranged between **60% and 70%**, with a peak accuracy of **73.53% using SVM with a linear kernel and a weighted loss function**.  

This project demonstrates the potential of machine learning in automating arrhythmia detection, reducing human intervention, and enhancing diagnostic precision.
