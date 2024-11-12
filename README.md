# CSCI1470_FinalProject

Authors: Geordie Young, Justin Hickey, Amelia Zug, and Brendan Leahey

Introduction
    Bone fractures are commonplace, affecting people of all ages and conditions. Computer vision based classifiers serve as a promising tool for radiologists to accurately and quickly assess bone fractures and carry out treatment. The goal of our project is to better identify bone fractures and provide doctors another opinion when diagnosing injuries. We were inspired by the paper Detection of bone fracture based on machine learning techniques in which Ahmed and Hawezi employ classical machine learning techniques including support vector machines to attain task-leading accuracy. Here, we apply transfer learning with several deep convolutional neural networks in hopes of improving upon these classical methods.

Methodology
    Data
        The data we used was sourced from publicly available Kaggle and FracAtlas datasets containing bone fracture images from a spectrum of bones. Our train dataset contains about 684 fractured and 704 non-fractured images from various bones. Our test dataset contains around 30 fractured and 30 non-fractured images randomly sampled without repetition of patients. 
    Model Architecture
        Our inputted x-ray images are preprocessed and augmented for robust and precise learning. A pre-trained classifier extracts low-level image features from the scans, and output tensors flow through a fine-tuned binary classification head for prediction of bone fractures.

Results
    We achieved a final test accuracy of around 88% for all models, surmounting our benchmark goal of 80% and hitting our target range of 80-90% to be consistent with the original paper. Our models also attained a high AUROC metric surpassing our goal of 80-90% indicating that the model has better discrimination ability. 

    Final Test Accuracy per Model:
    VGG-16: 88%
    ResNet-50: 87%
    Inceptionv3: 88%

Reflection
    Overall this project was successful. We finetuned three pretrained models to more accurately identify bone fractures in x-ray images and surmounted our base goal accuracy of 80%. Moreover we succeeded in reaching our stretch goal of attaining an AUROC score of 80-90% for all models. Beyond metrics we were able to successfully identify and preprocess high quality fracture image data and build upon our inspiration paper using two new datasets. We successfully troubleshot difficulties with preprocessing by identifying issues with our original dataset, filtering out unwanted images, and bolstering our data with more high-quality images from a different source. If given more time we would have hoped to further fine tune the pretrained models to maximize accuracy and precision while minimizing loss. Overall our team enjoyed the process and found this project incredibly valuable.

