# DFU Image Classification
Diabetes Foot Ulcer Image Classification using Deep Learning Methods
![dfu-1573641113](https://github.com/stellacherotich/DFU-Image-Classification/assets/114439636/47d31fbf-40d3-49b6-8bac-2147c879349f)
## Introduction
Diabetes is a chronic medical condition affecting blood sugar control.<br>There are two main types of diabetes:
  1. Type 1 Diabetes - linked to autoimmune factors
  2. Type 2 Diabetes - often associated with one's lifestyle. It is the most prevalent type out of the two.

Both of these types can result in complications such as heart disease, nerve impairment, and delayed wound healing.

**Diabetic Foot Ulcers**(DFUs) are a specific complication that can arise in people with diabetes. They are open sores or wounds that develop on the feet, most commonly on the bottom of the feet. DFUs are a result of multiple factors associated with diabetes, including poor circulation, nerve damage (neuropathy), and reduced immune function.

DFUs can become serious if left *untreated*. They have the potential to lead to infections that can spread to the bone or bloodstream, potentially resulting in the need for amputation.
## Objectives
The main objective of this project is:

- To build a machine learning model that will accurately identify whether a given image of a foot ulcer indicates a diabetic foot ulcer or not.

#### **Success Metrics**
The primary gauge of success was as follows:
- Accuracy: This metric represents the proportion of accurate classifications when identifying diabetic foot ulcers.
<br>The achievement target for accuracy was set at over 85%.

## The Data
The data was retrieved from [Kaggle](https://www.kaggle.com/datasets/laithjj/diabetic-foot-ulcer-dfu). This dataset contains a collection of images showcasing various stages of diabetic foot ulcers.
There are two main folders that were generated in order to carry out the classification, these include:

- Training - This was taken from the Patches Folder ; The images were separated into their respective classes. 

- Test - This was generated through converting the original Test Set folder, so that all the images were in a uniform format.

### Distribution of the training dataset
![Distribution of Training Dataset](https://github.com/stellacherotich/DFU-Image-Classification/assets/114439636/1c8bb40a-0eb9-458f-b18f-53952b9c9d62)

### Distribution of the Test dataset
![Test Data Distribution](https://github.com/stellacherotich/DFU-Image-Classification/assets/114439636/a6d65ba8-ae52-4ea6-a2c4-9e6b732c7ccb)

By leveraging this dataset and applying deep learning techniques, the project aims to contribute to the early and accurate detection of diabetic foot ulcers, ultimately assisting in timely medical interventions and reducing the risk of severe complications.

## **Modeling**
The chosen models for this project encompass a range of techniques to explore and optimize the performance:

1. **Deeply Connected Neural Network (Baseline Model)**: This served as the initial model, forming the foundation for comparison against more advanced approaches.

2. **Convolutional Neural Network (CNN)**: Introducing convolutional layers, this model is well-suited for image data, as it can identify spatial patterns and features within the images.

3. **Tuned CNNs**: These models likely involve variations of the CNN architecture that have been fine-tuned to achieve better accuracy and generalization on the specific task.

   
## **Model Evaluation**

![image](https://github.com/stellacherotich/DFU-Image-Classification/assets/114439636/c50d11a6-e151-4d6d-bac3-b7842d021a67)


This table highlights how all three models performed against each other. The baseline model did not perform as well as the CNN and Tuned CNN model. <br>
Therefore, based on the accuracy and loss score, the best performing model was the **Tuned CNN** model.

## **Conclusion**
Analyzing the performance of the Test data, the following conclusions can be drawn:

The evaluation results indicate that the model achieved a test accuracy of approximately 91.41%, showcasing its ability to accurately identify diabetic foot ulcers within the test images. The corresponding test loss, measuring around 0.928, reflects the alignment between the model's predictions and the actual outcomes. These findings emphasize the model's potential as a valuable tool for proficiently detecting diabetic foot ulcers, thereby offering significant relevance in medical contexts and patient management.

## **Recommendations**
1. **Enhancing Data Access** : It's important to consider the possibility of data bias towards specific communities. To further elevate model performance, a strategic approach involves collecting a more diverse dataset. This expansion not only fine-tunes the model's accuracy but also ensures its effectiveness across various demographic groups.

2. **Transfer Learning** : This approach involves harnessing the knowledge embedded within pre-trained neural network architectures, which have been honed on expansive datasets such as ImageNet. By tweaking these insights to suit the needs of the DFU classification, the model's abilities are elevated to accurately categorize Diabetic Foot Ulcers.

3. **Elevating Awareness of Early DFU Signs**: Giving priority to educating individuals about the initial signs of Diabetic Foot Ulcers (DFU) can have a profound impact on the overall outcomes. When people are informed about the early symptoms of DFU, they are better equipped to take action promptly. This timely response can play a pivotal role in preventing situations where the only option left might be amputation. By spreading awareness about these early indicators, they can be more empowered to seek medical attention, receive appropriate care, and potentially avoid more severe complications associated with DFUs.

4. **Holistic Support for DFU Patients**: Offering counseling and therapy to individuals grappling with DFUs marks a substantial step. This support system not only aids them in their health journey but also contributes to their emotional well-being. Extending this assistance to their families empowers them to provide effective care, fostering a comprehensive approach to diabetic patient well-being.

## **Next Steps**

To further amplify the impact of this project, the next step involves developing a user-friendly web application. This app will serve as an accessible platform to provide valuable insights and assistance related to Diabetic Foot Ulcers (DFUs). This would be of benefit to healthcare professionals seeking comprehensive resources, and anyone seeking to enhance their understanding of DFUs and their management.

---

### **References**
1. Alzubaidi, L., Fadhel, M. A., Oleiwi, S. R., Al-Shamma, O., & Zhang, J. (2020). DFU_QUTNet: Diabetic foot ulcer classification using novel deep convolutional neural network. Multimedia Tools and Applications, 79(21), 15655-15677.

2. Alzubaidi, L., Fadhel, M. A., Al-Shamma, O., Zhang, J., Santamaría, J., & Duan, Y. (2021). Robust application of new deep learning tools: An experimental study in medical imaging. Multimedia Tools and Applications, 1-29.

3. Alzubaidi, L., Fadhel, M. A., Al-Shamma, O., Zhang, J., Santamaría, J., Oleiwi, S. R., & Duan, Y. (2020). Towards a better understanding of transfer learning for medical imaging: A case study. Applied Sciences, 10(13), 4523.
