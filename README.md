# Histopathologic Cancer Detection
This repo contains files for the week 3 peer-graded assignmennt in CU Boulder's MSDS 5511 Deep Learning course. The assignment is to compete in the Kaggle Competition [Histopathologic Cancer Detection](https://www.kaggle.com/competitions/histopathologic-cancer-detection/overview).

### Purpose
From the competition web page, the purpose is "to identify metastatic cancer in small image patches taken from larger digital pathology scans. The data for this competition is a slightly modified version of the PatchCamelyon (PCam) benchmark dataset (the original PCam dataset contains duplicate images due to its probabilistic sampling, however, the version presented on Kaggle does not contain duplicates)." 

### Dataset
The [datset](https://www.kaggle.com/competitions/histopathologic-cancer-detection/overview) is provided by Bas Veeling, Babak Ehteshami Bejnordi, Geert Litjens, and Jeroen van der Laak. The dataset is described in detail in their papers [*Rotation Equivariant CNNs for Digital Pathology*](https://arxiv.org/abs/1806.03962) and [*Diagnostic Assessment of Deep Learning Algorithms for Detection of Lymph Node Metastases in Women With Breast Cancer*](https://jamanetwork.com/journals/jama/fullarticle/2665774).

### Modelling approach
Three convolutional neural networks are trained below. Model 2 had the best prediction accuracy and Kaggle score. Model 2 is a convolutional neural network (CNN) with 3 convolutional layers, 3 max pooling layers, and 1 fully connected layer. The model was trained for 20 epochs on 198022 images with the Adam optimizer, the .001 default learning rate, and a batch size of 32 images. The model was validated on 22003 images. 

### Final Model
Model 2 is saved as HCD_model2.h5
