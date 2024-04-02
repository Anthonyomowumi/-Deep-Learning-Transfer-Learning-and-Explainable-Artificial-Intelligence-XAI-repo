## CANCER GENE EXPRESSION CLASSIFICATION USING TRANSFER LEARNING AND EXPLAINABLE AI

## PROJECT SUMMARY
This project made use of Transfer Learning Approach in the classification of 33 Cancer Types and Explainable AI to understand the interpretability of the models.


## PROBLEM STATEMENT
Gene expression analysis is a complex process due to relatively few samples available with high dimensional data. That is why the transfer learning technique was employed in this paper to tackle this issue and RNA-Seq gene expression data from Pan-Cancer Atlas was used in the classification of 33 prevalent tumor types. The high dimensional RNA-Seq data was embedded into 2-D images and four pre-trained base models which include Xception, DensetNet169, ResNet50, and VGG19 were used. Some layers of the last convolutional block in the base model were trained to allow the models to learn some patterns/forms in the medical data since the models were trained on ImageNet data that does not have any class label belonging to medical data/gene expression data.
Furthermore, Explainable AI - IntegratedGradients was used to check the attribution of the image predicting a specific class label. This is to understand the part of the images leading to the prediction of the outcome.

## METHODOLOGY
Publicly available RNA-Seq Expression data (Secondary data) are used in this work. The Cancer Genome Atlas (TCGA) has sequenced and handled a sizable quantity of tumor tissues. From these samples, TCGA further evaluated over 11,000 tumors from the 33 most common types of cancer, which enabled the creation of the Pan-Cancer Atlas. The National Cancer Institute (NCI) and the National Human Genome Research Institute jointly founded the TCGA project in 2006 with the goal of customizing and identifying the genetic mutations responsible for various cancer types using genome sequencing and bioinformatics 
![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/c652088b-8bdf-46b5-a769-db27c58ad781)

The figure belw shows the images after Feature Selection, Log transformation and Image synthesis of the 33 classes

![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/3747b167-465a-49eb-8d93-59adb5068a9a)


## EXPERIMENTAL SETUP AND ANALYSIS
Four models—VGG19, ResNet50, DenseNet169, and Xception—were chosen after experimenting with a variety of base CNN pre-trained model architectures, including EfficientNetB0, MobileNet, and others. VGG19 is a deep architecture CNN network of 19 layers, including 1 SoftMax layer, 5 max-pooling layers, 3 fully connected layers, and 16 convolutional layers.
33 image class data were randomly split using the split-folder package in Python in the ratio of 80:10:10 (8342: 1030: 1074) for the pre-trained model training, validation, and testing of the model's performance. Also, the images were modified into 3-channel images through a channel duplication mechanism allowing the pre-trained model to process the images as RGB channel images. The grayscale intensity is essentially used as the value for all three color channels in the model, which handles all three channels equally by the models

## EXPERIMENTAL RESULTS
![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/f6526793-52e6-4dce-b0de-c79d37e55903)

![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/bc612add-c6e4-4ee0-944c-286a8b2825e6)

Inspecting the performance metrics, accuracy was less considered in this study because the data contains an imbalance class distribution. Therefore, taking the performance metrics of the ResNet50 architecture, the precision of 90% explains that when the model predicts a tumor presence, there is a 90% chance that the model is accurate while Recall/Sensitivity of 88% indicates that the model correctly predicted 88% of the actual tumor instances. In other words, the model has an 88% chance of discovering and predicting a tumor when one is present. The Figures below shows the ResNet50 model accuracy and model loss for the train (8342 samples in total) and validation test (1030 samples in total) for 25 epochs.

![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/5143c5a0-851f-4de0-aac8-a2ce84a47e48)


![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/ae7a7d0d-a4fb-48d5-a11e-83f93fdeccda)



An image from class 1 (BLCA) was used to inspect this. The image was preprocessed and transformed using the ResNet50 preprocess input library in the TensorFlow keras library. “Figure 6” shows the explainability of the model prediction and why it is predicting the class label “BLCA/class1” in the code. By overlaying the attribution values for each pixel over the original image on the heatmap with the black image baseline, the attributions are shown. The pixel's attribution value is obtained by adding the three-color channels' individual attribution values. Green pixels represent positive attributions, whereas red pixels represent negative attributions. The attributions are scaled in a range and show which genes or portions of the image are responsible for the observed results.


![image](https://github.com/Anthonyomowumi/-Deep-Learning-Transfer-Learning-and-Explainable-Artificial-Intelligence-XAI-repo/assets/93340041/0df635a2-c45f-4996-a9ab-5a93d8f68e6d)



## CONCLUSION
In this study, based on the Pan-Cancer Atlas provided 33 most prevalent tumor types, a transfer learning methodology to classify genomic data (Gene Expression data) was employed. The experimental result in this study shows that the pre-trained model- VGG19, Xception, DenseNet169, and ResNet50 with a fine-tuning procedure like retraining of some part of the convolutional layer/block to effectively learn some patterns/forms in the gene expression/medical data and the common fully connected layer retraining method of the models is good in classifying gene expression data. ResNet50 performed better in this study achieving an accuracy of 92% on the 10% test set with a precision of 90%, recall of 88%, and F1 score of 89%. This performance on the unseen data (test data) shows that there is a good generalization performance of the model. The proposed methodology in this paper, transfer learning and base models’ architectures fine-tuning can work well to identify tumor types based on their gene expression and will work well with other tumor types not included in this study as well as other genomics data analysis. It is faster and less computationally expensive. Also, the use of IntegratedGradients on the images gives a clearer view of which part of the image is attributing the cause of the prediction of the various classes. It is shown in this work that a good generalization performance is achieved. The accuracy of the methodology used in this paper shows good performance of the pre-trained models on tumor type classification as well as the interpretability of the results given using Explainable AI.



