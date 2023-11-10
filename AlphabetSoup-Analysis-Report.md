1. Overview of the analysis: Explain the purpose of this analysis.
- The purpose of this analysis is to use the previous applicant data from the CSV file to build a model to help predict if new applicants will receive funding from the AlphabetSoup organization.

2. Results: Using bulleted lists and images to support your answers, address the following questions:
    Data Preprocessing
    - What variable(s) are the target(s) for your model?
        The target for the model is the 'IS_SUCCESSFUL' column.

    - What variable(s) are the features for your model?
        The features are all the other columns in the data frame besides the 'IS_SUCCESSFUL' column.

    - What variable(s) should be removed from the input data because they are neither targets nor features?
        The EIN and NAME columns should be removed as they contain a lot of data and they are not necessary in determining the prediction of whether or not the applicant will receive funding or not.

    Compiling, Training, and Evaluating the Model
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?
        For my neural network model I selected to have 2 hidden layers. The first containing 8 neurons and the second containing 5 neurons. For each of the hidden layers I used the ReLU activation function. My input layer was determined by the number of features in the data. The output layer had 1 neuron and used the Sigmoid activation function.

    - Were you able to achieve the target model performance?
        No, I was unable to get my model above 73.4% in the original model and 73.57% in my optimized model.

    - What steps did you take in your attempts to increase model performance?
        I changed the cutoff values for the bins and I increased the amount of neuron each hidden layer had. After doing this, I could still not figure out how to reach an accuracy above 75%.


3. Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
- The overall results of this deep learning model is an accuracy of about just over 73%. This is not ideal as optimizations should take the model to a 75% accuracy rate. I was unable to figure out how to change my model enough to gain the 2% to reach target model performance. The only recommendation I could think of is maybe performing a Random Forest model on this data as it is a bit simpler and might allow for easier interpretation.