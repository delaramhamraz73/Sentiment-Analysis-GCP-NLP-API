
# Sentiment Analysis with Google's Natural Language API

You will find out how to connect to the gcp natural language API through your local computer, 
Do the sentiment analysis via Google's api and save the results in an excel file. you will be able 
to make new excel files and new sheets through the program.



## Appendix

**Google Natural Language API:**

The Google Natural Language API is an easy to use interface to a set of powerful NLP models which have been pre-trained by Google to perform various tasks. As these models have been trained on enormously large document corpuses, their performance is usually quite good as long as they are used on datasets that do not make use of a very idiosyncratic language. 
The biggest advantage of using these pre-trained models via the API is, that no training dataset is needed. The API allows the user to immediately start making predictions, which can be very valuable in situations where little labeled data is available. 
The Natural Language API comprises five different services:
-	Syntax Analysis 
-	Sentiment Analysis 
-	Entity Analysis 
-	Entity Sentiment Analysis 
-	Text Classification
Syntax Analysis:

For a given text, Google’s syntax analysis will return a breakdown of all words with a rich set of linguistic information for each token. The information can be divided into two parts:
-	Part of speech: This part contains information about the morphology of each token. For each word, a fine-grained analysis is returned containing its type (noun, verb, etc.), gender, grammatical case, tense, grammatical mood, grammatical voice, and much more.
-	Dependency trees: The second part of the return is called a dependency tree, which describes the syntactic structure of each sentence.

Sentiment Analysis:

Google’s sentiment analysis will provide the prevailing emotional opinion within a provided text. The API returns two values: The “score” describes the emotional leaning of the text from -1 (negative) to +1 (positive), with 0 being neutral.
The “magnitude” measures the strength of the emotion.

![Table](https://github.com/delaramhamraz73/Sentiment-Analysis-GCP-NLP-API/blob/main/Table.png)

**Google’s sentiment analysis model** is trained on a very large dataset. Unfortunately, there is no information about its detailed structure available.

Entity Analysis:

Entity Analysis is the process of detecting known entities like public figures or landmarks from a given text. Entity detection is very helpful for all kinds of classification and topic modeling tasks.
The Google Natural Language API provides some basic information about each detected entity and even provides a link to the respective Wikipedia article if it exists. Also, a salience score is calculated. This score for an entity provides information about the importance or centrality of that entity to the entire document text. Scores closer to 0 are less salient, while scores closer to 1.0 are highly salient.
Entity Sentiment Analysis
While the Sentiment Analysis API finds all displays of emotion in the document and aggregates them, the Entity Sentiment Analysis tries to find the dependencies between different parts of the document and the identified entities and then attributes the emotions in these text segments to the respective entities.

Text Classification:

The Google Natural language API comes with a plug-and-play text classification model.
The model is trained to classify the input documents into a large set of categories. The categories are structured hierarchical, e.g. the Category “Hobbies & Leisure” has several sub-categories, one of which would be “Hobbies & Leisure/Outdoors” which itself has sub-categories like “Hobbies & Leisure/Outdoors/Fishing.”

Google Natural Language API **Disadvantages**:

The Google Natural Language API is a very convenient option for quick, out-of-the-box solutions. Very little technical knowledge and no understanding of the underlying machine learning models is required.
The main disadvantage is its inflexibility and the lack of access to the models. The models cannot be tuned to a specific task or dataset.
In a real-world environment, most tasks will probably require a more tailored solution than the standardized Natural Language API functions can provide.
For this scenario, Google AutoML Natural Language is more suitable.


