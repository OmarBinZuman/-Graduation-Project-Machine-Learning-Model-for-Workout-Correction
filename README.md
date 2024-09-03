Workout Correction Model 

The Workout Correction Model is designed to help individuals correct their exercise form without needing a coach. We are currently focusing on a prototype for push-ups.

THE PROTOTYPE:

Dataset: We used a dataset from [Kaggle](https://www.kaggle.com/datasets/mohamadashrafsalama/pushup) with videos of correct and incorrect push-ups.

Data Processing:
Video to Images: We created a Python function to split the videos into training and testing sets, convert them to images, and reorder them.
Augmentation: To improve the model’s accuracy, we applied data augmentation techniques using ImageDataGenerator to vary the images.


Model: We used a pre-trained ResNet model, froze all layers except for the last 10, and added custom layers. After training on the push-up dataset, we achieved an accuracy of 95%.


NOTE: This is only the prototype stage of the project, and our goal is to use AI to provide real-time feedback on multiple exercises
