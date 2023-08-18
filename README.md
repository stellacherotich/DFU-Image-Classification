# DFU-Image-Classification
Diabetes Foot Ulcer Image Classification using Deep Learning Methods
![dfu-1573641113](https://github.com/stellacherotich/DFU-Image-Classification/assets/114439636/47d31fbf-40d3-49b6-8bac-2147c879349f)
## Introduction
Diabetes is a chronic medical condition affecting blood sugar control.<br>There are two main types of diabetes:
  1. Type 1 Diabetes - linked to autoimmune factors
  2. Type 2 Diabetes - often associated with one's lifestyle. It is the most prevalent type out of the two.

Both of these types can result in complications such as heart disease, nerve impairment, and delayed wound healing.

**Diabetic Foot Ulcers**(DFUs) are a specific complication that can arise in people with diabetes. They are open sores or wounds that develop on the feet, most commonly on the bottom of the feet. DFUs are a result of multiple factors associated with diabetes, including poor circulation, nerve damage (neuropathy), and reduced immune function.

DFUs can become serious if left *untreated*. They have the potential to lead to infections that can spread to the bone or bloodstream, potentially resulting in the need for <i>**amputation**</i>.

## Objectives
The main objectives of this project are:


1. To build a machine learning model that will accurately identify whether a given image of a foot ulcer indicates a diabetic foot ulcer or not.

2. To Develop a comprehensive classification system that can differentiate between various stages of diabetic foot ulcers, helping medical professionals to assess the severity and choose appropriate treatment strategies.

#### **Success Metrics**
The primary gauge of success was as follows:
- Accuracy: This metric represents the proportion of accurate classifications when identifying diabetic foot ulcers.
<br>The achievement target for accuracy was set at over 85%.

## The Data
The data was retrieved from [Kaggle](https://www.kaggle.com/datasets/laithjj/diabetic-foot-ulcer-dfu). This dataset contains a collection of images showcasing various stages of diabetic foot ulcers.
There are three main folders that were generated in order to carry out the classification, these include:

- Training - This was taken from the Patches folder

- Test - This was generated through converting the original Test Set folder, so that all the images were in a uniform format.

### Distribution of the training dataset
![Distribution of Training Dataset](https://github.com/stellacherotich/DFU-Image-Classification/assets/114439636/1c8bb40a-0eb9-458f-b18f-53952b9c9d62)

### Distribution of the Test dataset
![Test Data Distribution](https://github.com/stellacherotich/DFU-Image-Classification/assets/114439636/a6d65ba8-ae52-4ea6-a2c4-9e6b732c7ccb)

By leveraging this dataset and applying deep learning techniques, the project aims to contribute to the early and accurate detection of diabetic foot ulcers, ultimately assisting in timely medical interventions and reducing the risk of severe complications.

## Modeling
The models that were used include:
1. Deeply Connected Neural Network - This was the baseline model.
2. CNN
3. Tuned CNNs
4. Dropout L2 Regularization
   
## Model Evaluation

![image](https://github.com/stellacherotich/DFU-Image-Classification/assets/114439636/c50d11a6-e151-4d6d-bac3-b7842d021a67)


This table highlights how all three models performed against each other. The baseline model did not perform as well as the CNN and Tuned CNN model. <br>
Therefore, based on the accuracy and loss score, the best performing model was the **Tuned CNN** model.

## Conclusion
Analyzing the performance of the Test data, the following conclusions can be drawn:

The evaluation results indicate that the model achieved a test accuracy of approximately 91.41%, showcasing its ability to accurately identify diabetic foot ulcers within the test images. The corresponding test loss, measuring around 0.928, reflects the alignment between the model's predictions and the actual outcomes. These findings emphasize the model's potential as a valuable tool for proficiently detecting diabetic foot ulcers, thereby offering significant relevance in medical contexts and patient management.

## Recommendations
1. Getting more access to data -- The data might be biased towards a certain community therefore in order to improve model performance more data should be collected to optimise the model's performance even more.

2. Increase awareness on the early signs of DFU, that way early treatment can be provided therefore avoiding a situation where an individual has to get their limb(s) amputated.

3. Providing counseling/therapy to individuals who already have DFU's ; this should help support them in their health journey, in addition, their family should also receive the same support so that they can effectively cater to the needs of the diabetic patient.
