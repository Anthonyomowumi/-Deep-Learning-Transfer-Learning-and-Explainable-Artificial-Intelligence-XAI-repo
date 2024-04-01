## CANCER GENE EXPRESSION CLASSIFICATION USING TRANSFER LEARNING AND EXPLAINABLE AI


## PROJECT SUMMARY
This project made use of Transfer Learning Approach in the classification of 33 Cancer Types and Explainable AI to understand the interpretability of the models.

## PROBLEM STATEMENT
Gene expression analysis is a complex process due to relatively few samples available with high dimensional data. That is why the transfer learning technique was employed in this paper to tackle this issue and RNA-Seq gene expression data from Pan-Cancer Atlas was used in the classification of 33 prevalent tumor types. The high dimensional RNA-Seq data was embedded into 2-D images and four pre-trained base models which include Xception, DensetNet169, ResNet50, and VGG19 were used. Some layers of the last convolutional block in the base model were trained to allow the models to learn some patterns/forms in the medical data since the models were trained on ImageNet data that does not have any class label belonging to medical data/gene expression data. Furthermore, Explainable AI - IntegratedGradients was used to check the attribution of the image predicting a specific class label. This is to understand the part of the images leading to the prediction of the outcome. 


## I. DATASET ACQUISTION
Publicly available RNA-Seq Expression data (Secondary data) are used in this work [10]. The Cancer Genome Atlas (TCGA) has sequenced and handled a sizable quantity of tumor tissues. From these samples, TCGA further evaluated over 11,000 tumors from the 33 most common types of cancer, which enabled the creation of the Pan-Cancer Atlas. The National Cancer Institute (NCI) and the National Human Genome Research Institute jointly founded the TCGA project in 2006 with the goal of customizing and identifying the genetic mutations responsible for various cancer types using genome sequencing and bioinformatics 

![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/4f80db6f-6a1e-4c65-8d33-3c3204b57e0b)


## II. DATA PREPROCESSING AND TRANSFORMATION
A. 



## V. CONCLUSION
In this study, based on the Pan-Cancer Atlas provided 33 most prevalent tumor types, a transfer learning methodology to classify genomic data (Gene Expression data) was employed. The experimental result in this study shows that the pre-trained model- VGG19, Xception, DenseNet169, and ResNet50 with a fine-tuning procedure like retraining of some part of the convolutional layer/block to effectively learn some patterns/forms in the gene expression/medical data and the common fully connected layer retraining method of the models is good in classifying gene expression data. ResNet50 performed better in this study achieving an accuracy of 92% on the 10% test set with a precision of 90%, recall of 88%, and F1 score of 89%. This performance on the unseen data (test data) shows that there is a good generalization performance of the model. The proposed methodology in this paper, transfer learning and base models’ architectures fine-tuning can work well to identify tumor types based on their gene expression and will work well with other tumor types not included in this study as well as other genomics data analysis. It is faster and less computationally expensive. Also, the use of IntegratedGradients on the images gives a clearer view of which part of the image is attributing the cause of the prediction of the various classes. It is shown in this work that a good generalization performance is achieved. The accuracy of the methodology used in this paper shows good performance of the pre-trained models on tumor type classification as well as the interpretability of the results given using Explainable AI.


