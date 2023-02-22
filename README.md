# cavity-detection
Keras implementation of mobilenet_v2 tuned model for cavity detection.
#Introduction 
Dental caries or cavities, more commonly known as tooth decay, are caused by a breakdown of the tooth enamel. This breakdown is the result of bacteria on teeth that breakdown foods and produce acid that destroys tooth enamel and results in tooth decay. Early cavity detection can mean less damage, less pain & less hassle down the road. While preventing decay is always the primary goal, we understand that not everyone has perfect oral health all the time, so early detection & treatment are essential tools for preserving your beautiful smile! X-rays can show tooth decay, fillings and gum disease.

The goal of our project was to develop a model that can process a panoramic x ray image and can separate the teeth with caries from the healthy teeth. With this model we speed up the process of cavity detection, and we also enable patients to have access to these information and be informed about their health

# Phases of project implementation:
Phase 1: Dataset collection
 In order to train a deep-learning model to classify whether a tooth is healty or with caries cavity, we needed an appropriate dataset with balanced distribution of images for the two classes:

We use data from Mendeley Data. The dataset consists of anonymized and deidentified panoramic dental X-rays of 116 patients, taken at Noor Medical Imaging Center, Qom, Iran. The subjects cover a wide range of dental conditions from healthy, to partial and complete edentulous cases. From each image we cut each tooth separately and classified it into one of the groups. In the end, we got a set of 401 pictures of healthy teeth, and 398 pictures of teeth with caries and 402 pictures with no caries, which we used further to train our model.

Phase 2:Dataset Preparation
   We have expanded the size of a training dataset by creating modified versions of images in the dataset. The dataset was divided on train 80% /test 20% folders with python code.
   
Phase 3: Training the model
    To solve this problem, we used pre-trained mobilenet_v2 model.Best overall train and test accuracy results were achieved using mobilenet_v2 model.
    
Phase 4:Detection of cavity in panoramic x-rays
   Finally we detected the xrays who are with cavity and nocavity.
  
# Conclusion:
  During the working process we faced some issues during collecting the data and quality of the images. Dental x-rays are considered personal data so we had a challenge to find public available images, because of that our dataset has limited resources. While training our model we received results with good accuracy. With access to more data we will be able to improve the accuracy of our model.
  
# Future work:
The purpose of this model is to save the time that dentists lose in reading the dental imaging. With this model, with the recording itself, they will receive a ready analysis and dentists will be able to immediately focus on the teeth that need to be repaired.

In Macedonia, especially in small places, X-rays are taken outside dental offices. Patients receive an X-ray, and then go to the dentist to read it. With this model, in addition to the x-ray image, they will receive an analysis, which will allow them to know if they have teeth that need to be repaired, how many and which teeth they are.















