## CANCER GENE EXPRESSION CLASSIFICATION USING TRANSFER LEARNING AND EXPLAINABLE AI

## PROJECT SUMMARY
This project made use of Transfer Learning Approach in the classification of 33 Cancer Types and Explainable AI to understand the interpretability of the models.


## PROBLEM STATEMENT
Gene expression analysis is a complex process due to relatively few samples available with high dimensional data. That is why the transfer learning technique was employed in this paper to tackle this issue and RNA-Seq gene expression data from Pan-Cancer Atlas was used in the classification of 33 prevalent tumor types. The high dimensional RNA-Seq data was embedded into 2-D images and four pre-trained base models which include Xception, DensetNet169, ResNet50, and VGG19 were used. Some layers of the last convolutional block in the base model were trained to allow the models to learn some patterns/forms in the medical data since the models were trained on ImageNet data that does not have any class label belonging to medical data/gene expression data.
Furthermore, Explainable AI - IntegratedGradients was used to check the attribution of the image predicting a specific class label. This is to understand the part of the images leading to the prediction of the outcome.

## METHODOLOGY

![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/a5bdb9af-5923-47e2-9a00-cc299eea8212)







