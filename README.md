# SMS Spam Detector

## Background
This project involves refactoring code from an existing SMS text classification solution to create a linear Support Vector Classification (SVC) model. The model is trained to distinguish between spam and non-spam ("ham") text messages. Upon successful creation and training, a Gradio app is developed to host the application, allowing users to test text messages. The application provides instant feedback, indicating whether a text is classified as spam based on the model's performance.

## Files
To get started, download the following files necessary for this assignment:

- Module 21 Challenge files

## Before You Begin
Complete the following preparatory steps:

1. Create a new repository on GitHub or GitLab named `sms_spam_detector`. This project should not be added to an existing repository.
2. Clone the newly created repository to your local machine.
3. Add the starter files you downloaded to your local repository.
4. Push the changes to your remote repository on GitHub or GitLab.

## Challenge Instructions

### Create the SMS Classification Function
1. Open the `gradio_sms_text_classification.ipynb` notebook.
2. Using code from `sms_text_classification_solution.ipynb`, create a function named `sms_classification` by performing the following steps:
   - Set the `features` variable to the text message column of the DataFrame.
   - Set the `target` variable to the "label" column of the DataFrame.
   - Split the data into training and testing sets, with the `test_size` set to 33%.
   - Build a pipeline using `TfidfVectorizer` and `LinearSVC` to transform the test set to compare it to the training set.
   - Fit the model to the transformed training data and return the model.
   - Load `SMSSpamCollection.csv` into a DataFrame and call the `sms_classification` function with the DataFrame. Set the result to the "text_clf" variable.

### Create the SMS Prediction Function
1. In the same notebook, use the `sms_prediction` function to predict the classification of new text messages by:
   - Creating a variable to hold the prediction of a new text.
   - Using a conditional statement to determine if the text message is "ham" or "spam".
   - Returning an appropriate message indicating whether the text is spam or not.

### Create the Gradio Interface Application
1. Create a Gradio Interface application that takes a textbox for inputs and has a textbox for outputs, with appropriate labels for each.
2. Launch the application and provide a URL to share the application.

### Requirements
Ensure your project meets the following criteria:

- **SMS Classification Function** (50 points): Follow the detailed instructions for setting variables, splitting data, building a pipeline, fitting the model, reading the CSV, and setting the "text_clf" variable.
- **SMS Prediction Function** (30 points): Implement the prediction logic, including the conditional statement and returning appropriate messages for "ham" and "spam".
- **Gradio Interface Application** (20 points): Successfully create and share the Gradio Interface application, ensuring it operates as expected without errors after a user submits a text message.

## Testing
Use the following messages to test your application:
1. "You are a lucky winner of $5000!"
2. "You won 2 free tickets to the Super Bowl."
3. "You won 2 free tickets to the Super Bowl. Text us to claim your prize."
4. "Thanks for registering. Text 4343 to receive free updates on medicare."

## Conclusion
Upon completion, this project will demonstrate your ability to refactor code, utilize machine learning models for classification, and deploy a simple machine learning application using Gradio.
