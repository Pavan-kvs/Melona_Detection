# Melanoma-CNN-Prediction
>Problem statement: To build a CNN-based model which can accurately detect melanoma. Melanoma is a type of cancer that canbe deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin 
Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and 
all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are 
slightly dominant.

 The data set contains the following diseases:

1.Actinic keratosis <br>
2.Basal cell carcinoma <br>
3.Dermatofibroma <br>
4.Melanoma <br>
5.Nevus <br>
6.Pigmented benign keratosis <br>
7.Seborrheic keratosis <br>
8.Squamous cell carcinoma <br>
9.Vascular lesion

# Project Pipeline

Data Reading/Data Understanding → Defining the path for train and test images  <br>

Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180. <br>
Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset <br>
Model Building & training : 
Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1). <br>
Choose an appropriate optimiser and loss function for model training <br>
Train the model for ~20 epochs  <br>
Write your findings after the model fit. You must check if there is any evidence of model overfit or underfit. <br>
Choose an appropriate data augmentation strategy to resolve underfitting/overfitting  <br>
Model Building & training on the augmented data : 
Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1). <br>
Choose an appropriate optimiser and loss function for model training <br>
Train the model for ~20 epochs <br>
Write your findings after the model fit, see if the earlier issue is resolved or not? <br>
Class distribution: Examine the current class distribution in the training dataset 
- Which class has the least number of samples? <br>
- Which classes dominate the data in terms of the proportionate number of samples?
Handling class imbalances: Rectify class imbalances present in the training dataset with Augmentor library. <br>
Model Building & training on the rectified class imbalance data : <br>
Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1). <br>
Choose an appropriate optimiser and loss function for model training <br>
Train the model for ~30 epochs <br>

# Conclusions
1. overfitting is reduced by using an augmentation layer and then due to class imbalance, model performance is not good.
2. we solved the class imbalance by using the augmentor library. The resulting model gave moderate performance and accuracy
3. Still, we need to carry out operations in a model for better accuracy in the validation 
