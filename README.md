# Cancer Cell Classification Using Deep Learning 

This project aims to classify cancerous and non-cancerous cell images using deep learning models. The primary objective was to train and evaluate multiple CNN architectures to determine the most effective model for accurate classification.

## Project Overview

This repository contains:
- **Exploratory Data Analysis (EDA)** to understand dataset distribution and augmentation effects.
- **Baseline CNN Model** as a reference classifier.
- **Transfer Learning Models** (EfficientNet, MobileNet, and ResNet) to improve classification performance.
- **Evaluation Metrics & Comparisons** including confusion matrices, precision-recall reports, and ROC curves.

## Steps for Execution

### Step 1: Exploratory Data Analysis (EDA)
EDA provides insights into dataset distribution and augmentation effects. To replicate EDA, refer to:
- **EDA Report**: [`EDA.md`](EDA.md)
- **Jupyter Notebook**: [`src/CancerCellClassification_EDA.ipynb`](notebooks/CancerCellClassification_EDA.ipynb)
- **HTML Report**: [`src/CancerCellClassification_EDA.html`](notebooks/CancerCellClassification_EDA.html)

### Step 2: Train & Evaluate Models
Model training and evaluation are documented in:
- **Training & Validation Notebook**: [`src/Train_Test_Validate_Phase1.ipynb`](notebooks/Train_Test_Validate_Phase1.ipynb)
- **HTML Report**: [`Tsrc/rain_Test_Validate_Phase1.html`](notebooks/Train_Test_Validate_Phase1.html)

To replicate results, run the Jupyter notebooks in the order provided.

## Dataset Sample Visualizations

### **Training Data Samples**

<img src="results/Train_test/sample_train.png" width="600"/>

### **Validation Data Samples**

<img src="results/Train_test/sample_validation.png" width="600"/>

### **Test Data Samples**

<img src="results/Train_test/sample_test.png" width="600"/>

## Model Training & Evaluation
-----
### **Baseline Model**
The baseline CNN was trained as a reference.

- **Training Progress**
  
  <img src="results/Train_test/basemodel_epoch.png" width="600"/>

- **Classification Report**
  
  <img src="results/Train_test/basemodel_precision_recall.png" width="600"/>

- **Confusion Matrix**
  
  <img src="results/Train_test/basemodel_confusion_matrix.png" width="600"/>

- **Sample Predictions**
  
  <img src="results/Train_test/basemodel_true_vs_predicted.png" width="600"/>

### **Transfer Learning Models**

I fine-tuned **EfficientNetB0, MobileNetV2, and ResNet50** for performance improvement.
-----
#### **EfficientNet**
- **Training Progress**
  
  <img src="results/Train_test/EfficientNet_epoch.png" width="600"/>

- **Classification Report**
  
  <img src="results/Train_test/efficientNet_precision_recall.png" width="600"/>

- **Confusion Matrix**
  
  <img src="results/Train_test/EfficientNet_confusion_matrix.png" width="600"/>

- **Sample Predictions**
  
  <img src="results/Train_test/EfficientNet_true_vs_predicted.png" width="600"/>

-----
#### **MobileNet**
- **Training Progress**
  
  <img src="results/Train_test/MobileNet_epoch.png" width="600"/>

- **Classification Report**
  
  <img src="results/Train_test/MobileNet_precision_recall.png" width="600"/>

- **Confusion Matrix**
  
  <img src="results/Train_test/MobileNet_confusion_matrix.png" width="600"/>

- **Sample Predictions**
  
  <img src="results/Train_test/MobileNet_true_vs_predicted.png" width="600"/>

-----
#### **ResNet**
- **Training Progress**
  
  <img src="results/Train_test/ResNet_epoch.png" width="600"/>

- **Classification Report**
  
  <img src="results/Train_test/ResNet_precision_recall.png" width="600"/>

- **Confusion Matrix**
  
  <img src="results/Train_test/ResNet_confusion_matrix.png" width="600"/>

- **Sample Predictions**
  
  <img src="results/Train_test/ResNet_true_vs_predicted.png" width="600"/>

-----
### **Model Comparison**
To compare the models, I analyzed ROC curves and classification metrics.

- **ROC Curve**
  
  <img src="results/Train_test/ROC_ModelComparision.png" width="600"/>

## Conclusion

- **EfficientNetB0** provided the best balance betIen accuracy, recall, and computational efficiency.
- **MobileNetV2** delivered competitive performance with loIr resource requirements.
- **ResNet50** shoId high precision but loIr recall, indicating a tendency to misclassify malignant cases.

This project demonstrates how deep learning can be effectively utilized in **medical image classification**. The structured pipeline ensures reproducibility and can be extended to other classification tasks.
