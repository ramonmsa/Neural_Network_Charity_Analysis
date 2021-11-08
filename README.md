# Neural_Network_Charity_Analysis
## Purpose
To create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results
    
-  ### Data Preprocessing
    -   __What variable(s) are considered the target(s) for your model?__
        - *IS_SUCCESSFUL*
    -   __What variable(s) are considered to be the features for your model?__
        - *APPLICATION_TYPE*
        - *AFFILIATION*
        - *CLASSIFICATION*
        - *USE_CASE*
        - *ORGANIZATION*
        - *INCOME_AMT*
        - *SPECIAL_CONSIDERATIONS*
        - *ASK_AMT*
        - *STATUS*
        - *NAME*
    -   __What variable(s) are neither targets nor features, and should be removed from the input data?__
        - *EIN*

- ### Compiling, Training, and Evaluating the Model
  - __How many neurons, layers, and activation functions did you select for your neural network model, and why?__
    - In order to achieve  *accuracy higher then 75%*, the number of neurons, layers and activation functions used was chosen as following:
      - __Number of Layers__:
        - Total of __*4*__ layers being:
          - __*three*__ hidden layers and 
          -  __*one*__ output layer.
        - __Number of Neurons__:
          - Total of __*177*__ layers being:
            - __*100*__ neurons in the first layer,
            - __*60*__ neurons in the second layer,
            - __*16*__ neurons in the third layer and
            - __*one*__ neurons in the output layer.
        - __Number of Activation Functions__:
          - Total of __*two*__ types of activation functions being:
            - __*ReLu*__ for the *first* and *second* layers and
            - __*Sigmoid*__ for the *third* and *output* layer.
  - __Were you able to achieve the target model performance?__
    - By choosing the set up above the model was able to perform around __77%__ of accuracy as it can be seeing on the screen shot below.<br>
      ![image](https://user-images.githubusercontent.com/69650068/140667996-e058bd06-28c2-4111-ac44-0ccd702ed7eb.png)
  - __What steps did you take to try and increase model performance?__
    - In order to increase model performance compering with the previous code the following steps were implemented:
      - In the *Data Processing* stage: 
        - Dropped only __*EIN*__ column
        - Binned additional columns such as __*INCOME_AMT*__ and __*NAME*__ and aggregating values less than *3000* and and values less then 10 for each variable respectively.
      - In the *Model* portion of the code:
        - Increased the __quantity of layers in one__ using *Sigmoid* as activation function and *giving 16 neurons* to this additional layer.  
        - Increased the number of *neurons* to __100 in the first layer__ and __60 in the second layer__. 

## Summary

By having a model that performs 77% accurate, the understanding is that a satisfactory result is will be delivery when classifying which applicants will successful.
However, since the dataset is relatively small and the outcome is a binary classification, I would recommend clustering the features a build a unsupervised model instead. This could reduce costs to process the model and perhaps enable us to find equal or better model accuracy.
