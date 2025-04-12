<h1>Play Store Sentiment Analysis on App Data</h1>

**Project Goal:**

• We created a model that checks if the text written about an app is positive, neutral, or negative. This helps us understand what people feel about different apps.


**Dataset Used:**

• File Name: apps.csv

• The file has columns like App name, Category, Rating, Reviews, Size, Installs, Type, Price, etc.

• We used the App column for this project and added custom sentiment labels (-1, 0, 1) to test the model.


**Steps We Followed in Google Colab:**

1. Imported Libraries:
We added the tools we needed like pandas, nltk, sklearn, etc.


2. Loaded the Data:
Opened the apps.csv file and checked the data.


3. Prepared the Data:
Kept only the App column and manually added sentiment values:

   -1 for negative

    0 for neutral

    1 for positive



4. Cleaned the Text:
Removed extra spaces, punctuation, stopwords (like “the”, “and”), and changed everything to lowercase.


5. Converted Text to Numbers (Vectorization):
Used TF-IDF to change text into numbers so the model can understand.


6. Trained the Model:
Used the Naive Bayes algorithm to train the sentiment model.


7. Checked the Model:

Accuracy: 74%

The model worked well with positive data, but was a bit weak for neutral and negative because we had less of those in the dataset.



8. Created Visuals:

Made a bar chart showing the number of positive, neutral, and negative texts.

Showed the confusion matrix to check prediction results.



**Tools Used:**

• Python

• Google Colab

• Pandas

• NLTK

• Scikit-learn

• Seaborn and Matplotlib for graphs



**Conclusion:**

• This project taught us how to clean text, build a machine learning model, and check if the model is working correctly. It’s a basic sentiment analysis example, which can be helpful in real life for analyzing app reviews or public feedback.
