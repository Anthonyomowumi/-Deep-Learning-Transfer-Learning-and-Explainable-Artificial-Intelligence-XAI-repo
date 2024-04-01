## CANCER GENE EXPRESSION CLASSIFICATION USING TRANSFER LEARNING AND EXPLAINABLE AI

## PROJECT SUMMARY
This project made use of Transfer Learning Approach in the classification of 33 Cancer Types and Explainable AI to understand the interpretability of the models.

## PROBLEM STATEMENT
![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/e30c5f70-d84c-4a20-8e00-28d9ba523cf1)
tcome. 


## I. METHODOLOGY
![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/4f80db6f-6a1e-4c65-8d33-3c3204b57e0b)

### A. DATASET ACQUISTION
Publicly available RNA-Seq Expression data (Secondary data) are used in this work [10]. The Cancer Genome Atlas (TCGA) has sequenced and handled a sizable quantity of tumor tissues. From these samples, TCGA further evaluated over 11,000 tumors from the 33 most common types of cancer, which enabled the creation of the Pan-Cancer Atlas. The National Cancer Institute (NCI) and the National Human Genome Research Institute jointly founded the TCGA project in 2006 with the goal of customizing and identifying the genetic mutations responsible for various cancer types using genome sequencing and bioinformatics 

### B. DATA DESCRIPTION
33 tumor types of RNA-Seq gene expression data, normalized to level 3 were used in this study (Available at Pan Cancer Atlas) [12]. The information includes a cancer-type classification column, 20531 genes were reduced to 10363 by filtering out the genes using a threshold variance of 1.19 to filter out genes whose samples remain almost unchanged across the expression levels, and 10446 tumor samples (Rows). The details of the 33 tumor types, cohort names, and the number of samples.
![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/64cd9478-5a57-4d03-867a-0e3ed3576598)

### C. FEATURE SELECTION

### D. LOG TRANSFORMATION AND IMAGE SYSNTHESIS

### E. 



## V. CONCLUSION
In this study, based on the Pan-Cancer Atlas provided 33 most prevalent tumor types, a transfer learning methodology to classify genomic data (Gene Expression data) was employed. The experimental result in this study shows that the pre-trained model- VGG19, Xception, DenseNet169, and ResNet50 with a fine-tuning procedure like retraining of some part of the convolutional layer/block to effectively learn some patterns/forms in the gene expression/medical data and the common fully connected layer retraining method of the models is good in classifying gene expression data. ResNet50 performed better in this study achieving an accuracy of 92% on the 10% test set with a precision of 90%, recall of 88%, and F1 score of 89%. This performance on the unseen data (test data) shows that there is a good generalization performance of the model. The proposed methodology in this paper, transfer learning and base models’ architectures fine-tuning can work well to identify tumor types based on their gene expression and will work well with other tumor types not included in this study as well as other genomics data analysis. It is faster and less computationally expensive. Also, the use of IntegratedGradients on the images gives a clearer view of which part of the image is attributing the cause of the prediction of the various classes. It is shown in this work that a good generalization performance is achieved. The accuracy of the methodology used in this paper shows good performance of the pre-trained models on tumor type classification as well as the interpretability of the results given using Explainable AI.


