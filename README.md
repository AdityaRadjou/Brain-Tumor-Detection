# Machine Learning techniques for MRI-based Brain Tumor Detection
Aditya Radjou

## Abstract
Brain tumors used to be detected by radiologists on MRI Scans. This task is important - as it involves human lives - but very time consuming for medical professionals. Recognizing the potential for automation to streamline this process, research has been done to enhance clinical outcomes by deploying high-performing and rapid models

This project aims at predicting the nature of a tumor (glioma, meningioma, or pituitary) if it exists on any MRI scan. I have experimented two known models for this task: Support Vector Machines (SVM) and 2D-Convolutional Neural Networks (2D-CNN). To train these models, I used a 160 MB dataset on Kaggle (https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset).

## Table of results:

### 

| Model        | Training time (hours) | Accuracy
|--------------|:---------------------:|:---------:|
| SVM w/o PCA  | 3                     | 0.94
| SVM w/ PCA   | 0.3                   | 0.92
| 2D-CNN       | 0.3                   | 0.93

## Conclusion

In this context, the 2D-CNN wins the performance-speed tradeoff. Despite a marginal decrease in accuracy (1%), the 2D-CNN produces results 10 times faster than the basic SVM. Additionaly, the time saved by feature extraction does not make the SVM model faster than the CNN model. 
This project showed the value of CNN models, able to swiftly undergo training across extensive dimensions and yield reliable results
