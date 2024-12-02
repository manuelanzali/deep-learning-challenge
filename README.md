# deep-learning-challenge

Overview of the analysis: Explain the purpose of this analysis.

. The purpose of this analysis is to create the best binary classifier that would be able to reach the highest accuracy in selecting the applicants who will be successful if funded by Alphabet Soup. 


Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

1. What variable(s) are the target(s) for your model?

. The variables that are the targets for my model are NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.


2. What variable(s) are the features for your model?

. The variable that is the feature for my model is the IS_SUCCESSFUL variable. 


3. What variable(s) should be removed from the input data because they are neither targets nor features?

. The variable that should be removed from the input data is the EIN variable.



Compiling, Training, and Evaluating the Model

4. How many neurons, layers, and activation functions did you select for your neural network model, and why?

. I selected the number of neurons/input values based on each layer, First Hidden Layer: 85 neurons, Second Hidden Layer: 42 neurons, Third Hidden Layer: 21 neurons, and Output Layer: 1 neuron. I selected 5 layers; the input layer, first, second, and third innner layers, and the output layer. I selected one activation sigmoid function for each layer. I increased the number of neurons and layers as much as I could and chose only one type of activation function for each layer to use feature engineering to help increase the performance of the neural network model by speeding up the model, reducing loss, change how the model interprets inputs, and help the model consider a higher number of interactions between variables.


5. Were you able to achieve the target model performance?

. Yes, I was able to achieve the target model performance ( > 75% ). 


6. What steps did you take in your attempts to increase model performance?

. The steps that I took in my attempts to increase the model performance were focused on higher level hyper parameters. I worked on removing only the EIN variable rather than the EIN and the name to keep as much data as possible while maintaining high accuracy. I then created classes for the application_type variable to simplify the data in that column to help the model understand and train on the data easier. Next, I created cutoff values and replaced values in the classification, application_type, and name columns to keep as much data as possible here as well but simplify the information in these columns. I then used get_dummies to simplify the data in each of the other columns. Lastly, after scaling and fitting the model, I increased the neurons and layers in the hidden layers in the deep learning model. I used a high number of epochs in the training regimen as well to help the model achieve the desired performance.


Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

Results:

. The results of the deep learning model showed that the neural network model was very accurate in determining the applicants with the best chance of success in their ventures if funded by Alphabet Soup. The model had a passing accuracy, over 75%, at 76%. 


Recommendation:

. My recommendation of how a different model could solve this classification problem is using the Random Forest model. I would recommend this model because overall it is very efficient at achieving higher accuracy when classifying data. The random forest model works to use several decision trees trained on a random small piece of the initial data each, and all work together to create a strong classifier.
