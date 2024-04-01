## Cancer Gene Expression Classification Using Transfer Learning and Explainable AI Project

## Abstract

Existing traditional methods mostly use feature selection combined with simple classifiers for gene expression analysis showing average classification performance.
In recent years, deep learning algorithms have been applied in different applications and achieved better performance compared to these traditional methods, 
but deep learning algorithms require a huge amount of data for training purposes.

However, Gene expression analysis is a complex process due to relatively few samples available with high dimensional data. 
That is why the transfer learning technique was employed in this paper to tackle this issue and RNA-Seq gene expression data from 
Pan-Cancer Atlas was used in the classification of 33 prevalent tumor types. The high dimensional RNA-Seq data was embedded into 2-D images and four pre-trained base models 
which include Xception, DensetNet169, ResNet50, and VGG19 were used. Some layers of the last convolutional block in the base model 
were trained to allow the models to learn some patterns/forms in the medical data since the models were trained on ImageNet data that does not have any class label
belonging to medical data/gene expression data.

ResNet50 performed better with an accuracy of 92% on the 10% test set with a precision of 90%, recall of 88%, and F1 score of 89%. 
This performance on the unseen data (test data) shows that there is a good generalization performance of the model. 
Furthermore, Explainable AI - IntegratedGradients was used to check the attribution of the image predicting a specific class label. 
This is to understand the part of the images leading to the prediction of the outcome. 
Overall, the study was good in achieving its aim and could be applied to other genomics data.


## Project Summary
Gene expression analysis is a complex process due to relatively few samples available with high dimensional data. That is why the transfer learning technique was employed in this paper to tackle this issue and RNA-Seq gene expression data from Pan-Cancer Atlas was used in the classification of 33 prevalent tumor types. The high dimensional RNA-Seq data was embedded into 2-D images and four pre-trained base models which include Xception, DensetNet169, ResNet50, and VGG19 were used. Some layers of the last convolutional block in the base model were trained to allow the models to learn some patterns/forms in the medical data since the models were trained on ImageNet data that does not have any class label belonging to medical data/gene expression data. Furthermore, Explainable AI - IntegratedGradients was used to check the attribution of the image predicting a specific class label. This is to understand the part of the images leading to the prediction of the outcome. 
