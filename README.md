# Neural_Network_Charity_Analysis

## Overview of the Analysis 
The objective of this analysis was to use deep learning methodology to train a Neural Network model and then evaluate its performance based on features desigated during preprocessing . 

## Results

* Data Preprocessing 
- The target variable for this model is the "IS_SUCCESSFUL" column 

- The following variables are considered features of the model : 
> APPLICATION_TYPE
> AFFILIATION
> CLASSIFICATION
> USE_CASE
> ORGANIZATION
> STATUS
> INCOME_AMT
> SPECIAL_CONDSIDERATIONS
> ASK_AMT

- The following variables are neither target nor features and were removed:
> EIN
> NAME

* Compiling , Training and Evaluating the Model
- Based on the fact that the number of input features was large (43), I decidec to start with a conservative number(1)     of neurons to evaluate the initial performance and used the "Relu" activation function due to its simplifying output when used in neural network models
![screenshot]()
![screenshot]()

- After multiple attempts and changes to the feature set the target performance was not achieved. 
![screenshot]()

- Stepts taken in attempt to increase accuracy were as follows:
* Removed binned columns 
![screenshot]()

* Increased the number of hidden layers and neurons
![screenshot]()

* Changed the activation parameters while increasing hidden features
![screenshot]()
![screenshot]()


## Summary
Overall the neural network was only able to achieve a maximum accuracy of ~ 72% . Other attempts that were made to increase accuracy included using supervised learning models to apply a more linear approach seeing that the expected outcome is a classification based problem with a clearly deifined target i.e Was the money used effectively. 
These methods when applied to the preprocessed data using the same metrics did not increase the accuracy and in some cases performed noticeable worse. 
![screenshot]()
A third linear model test took an exceedingly long time to produce results and therefore cannot be reliably recommended. 
![screenshot]()
Bearing in mind the computing power required to execute a neural network and based on the results observed, I would position using the RandomForestClssifier on a dataset seuch as this.
