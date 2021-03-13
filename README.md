# Skin-Diseases-Detection-Hackbash

Definition :- Dermatological Issues/disorders are most commonly spread worldwide. This can be caused by various fungal, bacterial, or skin allergies. Effective use of Emerging technologies like AI/ML can recognize such diseases. Computer Vision is one such platform that made the possibility of detecting the cause accurately through Images.The problem here is to develop an Application Programming Interface which can be easily integrated with Android app to detect the skin disease without any physical interaction with a Dermatologist.

Our Approach :- 

    ML model:
              1. We got these dataset: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T .We segregated the datasets of harvard. Combined all the datasets and trained the TFlite image classification model multiple times.
              2. We augmented dataset in two ways-
                    a. We used random flipping and rotation as two data augmentation techniques.
                    b. While in other method we added random noise in addition to the above techniques for data augmentation.
              3. We tested each of the augmented data in two ways-
                    a. Dropout rate 0.5, Epochs = 05, model_spec= efficientnet_lite0
                    b. Dropout rate 0.5, Epochs = 10, model_spec= efficientnet_lite0
              4. We got best result with 2nd dataset by using 2nd way(10 Epochs).
              5. We exported the trained model in tflite format to deploy in android app.

    Android app:
              1. 
    

1 What is the definition that you are working on 
2 How are you trying to solve the problem like what is your approach 
3 The Tech stack used like Django,React,etc
4 Video of the project and if it is ready completely you can deploy it that can help the judges to evaluate. It can also create a good impression
5 Resume, LinkedIn and GitHub profile url of all the team members 
