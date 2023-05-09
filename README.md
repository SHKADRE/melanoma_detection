# Skin Cancer CNN - by Shailesh Kadre Oct 2022, AI ML C46 Batch
### Problem statement
- To build a CNN based model which can accurately detect melanoma.
- Melanoma is a type of cancer that can be deadly if not detected early
- It accounts for 75% of skin cancer deaths.

## General Information
- This assignment uses a dataset of about 2357 images of skin cancer types. 
- The dataset contains 9 sub-directories in each train and test subdirectories. 
- The 9 sub-directories contains the images of 9 skin cancer types respectively.
#### There are following 3 stages of model building
## Model 1- CNN model with raw data
- Use keras.preprocessing
- Create a dataset
- Define some parameters for the loader:
- Data Visualization- View all the nine cancer classes
## Conclusions of model 1
- With the  model1, I got an training accuracy of approximately 94% and validation accuracy of 85% (at 30th epoch) , The model is  overfitting and needs improvements
- We can see that validation accuracy is not incresing above 51 to 55% approximately
- Validation loss is increasing after 5 epochs
- It's a clear case of overfitting
-
## Model 2- CNN model with data Augmentation and 20% dropout 
## Conclusions of model 2
- The accuracy of model has improved and overfitting reduced
- Accuracy can be further improved
- Class imbalance is observed amongst 9 different claases which needs attenstion for further accuracy improvements

## Model 3- CNN model with class imbalance treatent and dropout
## Conclusions of model 3
- data_augmentation helped to some extent but the model was still overfitting and accuracy was not satisfacory
- data_augmentation plus class imbalance treatment plus dropout layers definitely helped
- With the final model, I got an training accuracy of approximately 80% and validation accuracy of 80% (at 29th epoch) which is satisfactory, The model is not overfitting with the above improvements 
- The model accuracy can be improved further with still better hyperpameter tuning
