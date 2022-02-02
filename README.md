# Neural Network Alphabet Soup 
ML Charity Analysis
## Purpose
To present a study of a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results

- In order to achieve  *accuracy higher then 75%* a total of 4 layers was necessary being __*three*__ hidden layers and __*one*__ output layer. The __neurons__ were desitribuited in such a way that __*100*__ neurons were placed in the first layer, __*60*__ neurons in the second layer, __*16*__ neurons in the third layer and __*one*__ neurons in the output layer giving the total of __*177*__ __Neurons__. __*Two*__ types of activation functions were chosen to compose the model being __*ReLu*__ for the *first* and *second* layers and __*Sigmoid*__ for the *third* and *output* layer.
  ![image](https://user-images.githubusercontent.com/69650068/140667996-e058bd06-28c2-4111-ac44-0ccd702ed7eb.png)
  
## Challenges

- In order to reach a model accuracy performing as high as __77%__ it was necessary:
    - Reduced density of few features such as __*INCOME_AMT*__, __*APPLICATION_TYPE*__, __*CLASSIFICATION*__ and __*NAME*__ by binning them.<br> <img width="341" alt="image" src="https://user-images.githubusercontent.com/69650068/152148176-376950aa-b918-489a-9358-2df0f8a30009.png"> <br>
    *Example of binning done to the feature INCOME_AMT*<br>
    - Setting up *Sigmoid* as activation function to the third layer and giving it *16 neurons* was found to be relevant.<br> <img width="545" alt="image" src="https://user-images.githubusercontent.com/69650068/152146767-2e4bee2e-e2cb-4f0d-bbf5-da198b59ed12.png">


## Summary

By having a model that performs 77% accurate, the understanding is that a satisfactory result will be delivered when predicting the successful applicants.
However, since the dataset is relatively small, even though and the outcome is a binary classification, I would recommend clustering the features and build an unsupervised model instead. This could reduce costs to process the model and perhaps enable us to find equal or better model accuracy.
