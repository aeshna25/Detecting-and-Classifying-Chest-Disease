# Detecting-and-Classifying-Chest-Disease
Develop a model that can detect and classify 4 different chest disease from X-Ray images. 

## Understanding Dataset
For this problem, we have 2 datasets with 4 different type of XRay images. The training dataset has 133 images for each type of Chest Disease.
The Chest Dignosis we are dealing with in the projects are
1. Covid19
2. Bacterial Pneumonia X-ray
3. Viral Pneumonia X-ray
4. Normal Xray

For the prediction aspect, I applied **CNN**, where the first layers are used to extract high level general features and the last few layers are used to perform Classification. To overcome the vanishing gradient problem, ResNET(ImageNET training) was applied which,through its feature **Skip connection** overcomes this limitation. 

Finally to improve the model's performance, I used **Transfer Training**, in which a network that has been trained to perform a specific task is being reused as a starting point for another similar task.

The model was trained using 
- activation functions like : relu and softmax
- Generalization steps: Dropout layers
- Checking overfiiting: Early stopping after 20 epochs

Some results of the model can been seen below.

![Predicting Chest Disease](https://github.com/aeshna25/Detecting-and-Classifying-Chest-Disease/blob/main/Data/healthcare.png)
