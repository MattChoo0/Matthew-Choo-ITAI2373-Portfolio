# NewsBot Intelligence System
### ITAI 2373 – NLP Midterm Project
**Team MAEL**

## Project Overview

For our midterm project, we developed a NewsBot Intelligence System that uses Natural Language Processing (NLP) and machine learning to analyze news articles.

Our goal was to combine the NLP techniques we learned in class into one working system. NewsBot can automatically classify news articles, analyze sentiment, identify named entities, and examine grammatical patterns.

This system could be useful for news organizations and businesses that need to process large amounts of news content.

## Dataset

We used the BBC News Classification dataset from Kaggle, which was approved by our instructor.

Our dataset includes **1,490 news articles** across five categories:

- Business
- Entertainment
- Politics
- Sport
- Technology

We divided the data into 80% training and 20% testing.

**Dataset source:** [BBC News Classification – Kaggle](https://www.kaggle.com/competitions/learn-ai-bbc/data)

## NLP Techniques Used

Our project includes all eight modules covered in class.

1. **Business Application:** Explained how NewsBot could help with news categorization and media monitoring.
2. **Text Preprocessing:** Cleaned articles using tokenization, stopword removal, and lemmatization.
3. **TF-IDF:** Converted text into numerical features and identified important words.
4. **POS Tagging:** Identified nouns, verbs, adjectives, and other grammatical patterns.
5. **Syntax Parsing:** Analyzed grammatical relationships between words.
6. **Sentiment Analysis:** Used VADER to identify positive, negative, and neutral sentiment.
7. **Text Classification:** Compared Logistic Regression, Multinomial Naive Bayes, and Random Forest.
8. **Named Entity Recognition:** Identified people, organizations, locations, dates, and money amounts. We also analyzed how often entities appeared together.

## Machine Learning Results

We trained and compared three classification algorithms.

| Model | Test Accuracy |
|---|---|
| Logistic Regression | 96.31% |
| Multinomial Naive Bayes | 97.65% |
| Random Forest | 93.96% |

Multinomial Naive Bayes achieved the highest accuracy in our initial comparison.

We also optimized Logistic Regression using GridSearchCV. The best C value was 10.0, with a cross-validation accuracy of 96.39%.

We used the tuned Logistic Regression pipeline in our final NewsBot demonstration.

## NewsBot Testing

We tested our final system with three news articles that were not included in our training data.

| Article | Predicted Category | Sentiment |
|---|---|---|
| Business | Business | Positive |
| Politics | Politics | Negative |
| Sports | Sport | Positive |

NewsBot correctly predicted the categories of all three articles. It also extracted named entities, performed POS tagging, and identified grammatical relationships.

We noticed some limitations. For example, the sentiment analysis sometimes did not match the overall meaning of an article, and some named entities were labeled incorrectly.

## How to Run the Project

1. Open the Jupyter notebook in Google Colab.
2. Run the setup cells to install the required libraries.
3. Upload the BBC News dataset ZIP file when prompted.
4. Run the notebook cells in order.
5. Review the NLP analyses, charts, and classification results.
6. In the final NewsBot demonstration, upload three news articles to test the system.
7. Review the predicted categories, sentiment scores, named entities, POS tagging, and syntax results.

The final demonstration supports PDF, TXT, DOCX, JPG, and PNG files. Image files require OCR to extract text.

The project was developed using Google Colab and Python. We used libraries including pandas, scikit-learn, spaCy, NLTK, matplotlib, and document-processing libraries.

## Team Contributions

All four team members worked together on preprocessing, troubleshooting, running the notebook, and testing the final NewsBot system. We also divided responsibilities among the group members.

- **Matt Choo:** Worked on dataset selection, data preparation, and TF-IDF analysis to identify important terms in news articles.
- **Armani:** Worked on sentiment analysis and text classification, helping NewsBot identify article categories and emotional tone.
- **Elham:** Helped organize and review the final notebook, check the project requirements, test the system, and prepare the GitHub repositories for submission.
- **Laura:** Prepared the group reflective journal, organized our experiences and challenges, and documented each member's contributions to the project.

We worked together to combine the different NLP techniques into one system and make sure the final project ran correctly.

## Future Improvements

In the future, we could improve NewsBot by using a larger and more diverse dataset, adding more news categories, and improving sentiment and entity recognition.

We could also create a simple user interface where people could paste articles and receive results without running Python code.

## Conclusion

This project helped us understand how different NLP techniques can work together in a complete application. We gained experience with text preprocessing, machine learning, model evaluation, and testing.

We also learned the importance of teamwork, troubleshooting, and checking model results. NewsBot gave us practical experience applying NLP to a real-world problem.
