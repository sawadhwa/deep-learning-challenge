# The report should contain the following:

# Overview of the analysis: Explain the purpose of this analysis.

# Results: Using bulleted lists and images to support your answers, address the following questions:

# Data Preprocessing

1. What variable(s) are the target(s) for your model?

    **Answer**: The target is the Is-Successful column
2. What variable(s) are the features for your model?

    **Answer**: The features list for this model are the following: name, application type, affliation, classification, use_case, organization, income, special consideration, status and ask amount
3. What variable(s) should be removed from the input data because they are neither targets nor features?

    **Answer**: EIN (Employee identification)

# Compiling, Training, and Evaluating the Model

4. How many neurons, layers, and activation functions did you select for your neural network model, and why?

    **Answer**: For this model, there were 3 hidden layers each with a lot of neurons because the compute seems to increase the accuracy above 75%. This is expensive and costly. The first activation is relu and the other layers are sigmoid as it might boost accuracy using the functions. Also readjusting the data so that names as a get dummies can factor into better scores.
5. Were you able to achieve the target model performance?

    **Answer**: Yes
6. What steps did you take in your attempts to increase model performance?

    **Answer**: One step that I took was to take NAME and convert it into data points which has the biggest impact on improving the efficiency. However, it is very costly and it requires using a third layer with a sigmoid activation function.

# Summary: Summarize the overall results of the deep learning model. 

  Overall, we reach an accuracy above 75%, 75% of the time. The applicant has an 80% chance to be successful if they follow these rules: name of applicants appears 5+ times, type of applications follow T3, T4, T5, T6, T7, T8, T9, T10 applications of following classification

# Include a recommendation for how a different model could solve this classification problem, 
# and then explain your recommendation.

  You can use a RandomForest model and compare the accuracies. You can see the code below 
