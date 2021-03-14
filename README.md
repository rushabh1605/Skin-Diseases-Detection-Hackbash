# Skin-Diseases-Detection-Hackbash

We are team technophiles and participated in 24hrs hackathon organized by DSC. Our Problem Definition : An Application Programming Interface which can be easily integrated with Android to detect the skin disease without any physical interaction with a Dermatologist. 

Our college name: Pandit Deendayal Energy University(PDEU)

Team Members: Rushabh Thakkar, Divy Patel, Denish Kalariya, and Yug Thakkar.


> **Problem Definition :**

Dermatological Issues/disorders are most commonly spread worldwide. This can be caused by various fungal, bacterial, or skin allergies. Effective use of Emerging technologies like AI/ML can recognize such diseases. Computer Vision is one such platform that made the possibility of detecting the cause accurately through Images.The problem here is to develop an Application Programming Interface which can be easily integrated with Android app to detect the skin disease without any physical interaction with a Dermatologist.


> **Our Approach :**

    ML model:
              1. We got these dataset: shorturl.at/bAMZ5.
              2. We segregated the datasets of harvard. Combined all the datasets and trained the TFlite image classification model multiple times.
              3. We augmented dataset in two ways-
                    a. We used random flipping and rotation as two data augmentation techniques.
                    b. While in other method we added random noise in addition to the above techniques for data augmentation.
              3. We tested each of the augmented data in two ways-
                    a. Dropout rate 0.5, Epochs = 05, model_spec= efficientnet_lite0
                    b. Dropout rate 0.5, Epochs = 10, model_spec= efficientnet_lite0
              4. We got best result with 2nd dataset by using 2nd way(10 Epochs).
              5. We exported the trained model in tflite format to deploy in android app.

     Android app:
              1. We used example provided by Google of TFLite image_classifier model.
              2. We replaced the orignal model files with our own model files.
              3. We added a button to redirect user to map showing nearest available dermatologist.
              4. We changed some UI features, added app icon and changed the name of the app to make our final app.
  
  
> **Codes:**   
    
- image_segrigation.py - used to segrigate images into various categories from HAM-10000 dataset
- data_aug_rem.py - scans the folders and do random data removal or data-augmentation(as per arguments in code) to get requiered number of samples per class, avoiding any class bias.
- image_classification.py - calls TFlite image_classifier model and trains it with given dataset according to the arrguments. It also gives output of trained model as TFlite and labels files, which are used to deploy the model on the android app.


> **Tech Stack Used :-**

    TensorFlow Lite

    Android Studio (java)

    Google maps(URL based) API


> **Video:** 
[<img height="30" src = "https://img.shields.io/badge/Youtube-%23E4405F.svg?&style=for-the-badge&logo=Youtube&logoColor=white">][Youtube]
[youtube]: https://youtu.be/bV5bhKFsdYY

> **APK file:** [Link to APK File](https://drive.google.com/file/d/10DnwVU_na934VCRcrFEpBOYV6pfqOaVp/view?usp=sharing)


> **Profiles of team member:** 
[<img height="30" src = "https://img.shields.io/badge/gmail-c14438?&style=for-the-badge&logo=gmail&logoColor=white">][gmail] 
[<img height="30" src="https://img.shields.io/badge/linkedin-blue.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />][LinkedIn]
[<img height="30" src="https://img.shields.io/badge/github-black.svg?&style=for-the-badge&logo=github&logoColor=white" />][Github]


- Rushabh Thakkar

[linkedin](https://www.linkedin.com/in/rushabhthakkar/)
[github](https://github.com/rushabh1605)
[resume](https://drive.google.com/file/d/1MrEST2m7OiMRPsB-F7QaoezXCIzPOo8W/view?usp=sharing)

- Divy Patel

[linkedin](www.linkedin.com/in/divy-patel-7b369118b)
[github](https://github.com/Divy2000)
[resume](https://drive.google.com/file/d/15co1lwJ51Ld9ydJyfPFAF2lXNLlU-3ZA/view?usp=sharing)

- Denish Kalariya

[linkedin](https://www.linkedin.com/in/denish-kalariya-b22a641ba/)
[github](https://github.com/Dk-21)
[resume](https://drive.google.com/file/d/1gPyanEH-bpqPr0HxINCMX1v-Ufz2Jbm2/view?usp=sharing)

- Yug Thakkar

[linkedin](https://www.linkedin.com/in/yug-thakkar-6a0021179/)
[github](https://github.com/yugthakkar16)

