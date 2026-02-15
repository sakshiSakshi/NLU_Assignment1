# NLU_Assignment1: Problem4 

Sports vs Politics Text Classifier

So, here’s what’s going on: this project sorts news articles into either sports or politics using machine learning. I tried out three different algorithms—Logistic Regression, Naive Bayes, and Support Vector Machine—to see which one does the best job.

Dataset

- Sports articles: Sourced from the 20 Newsgroups
- Politics articles: Sourced from the 20 Newsgroups
- Categories picked: 20 categories down to just five sub-groups: two for Sports (rec.sport.baseball, rec.sport.hockey) and three for Politics (talk.politics.guns, talk.politics.mideast, talk.politics.misc)
- Total samples:  2,821 training documents and 1,878 testing documents.

Features

- TF-IDF vectorisation, using both single words and pairs (unigrams + bigrams)
- Cleaned up the text (lowercase, got rid of punctuation)
- Split everything into 80% for training, 20% for testing
- Used cross-validation to double-check results

Models

1. Logistic Regression – It’s straightforward and easy to explain.
2. Multinomial Naive Bayes – Takes a probabilistic angle.
3. Linear SVM – Focuses on drawing the sharpest line between categories.

Results

| Model                | Accuracy | Precision | Recall | F1-Score |  
|----------------------|----------|-----------|--------|----------|
| Logistic Regression  |0.7817    |0.7883     |0.7817  |0.7826    |  
| Naive Bayes          |0.7925    |0.7980     |0.7925  |0.7876    |
| SVM                  |0.7676    |0.7685     |0.7676  |0.7660    |

You can see the side-by-side results in the charts—model comparison and confusion matrices.

How to Run

# Clone the repository
git clone https://github.com/yourusername/sports-politics-classifier

And run in your terminal, alternatively, you can download the Colab notebook, the ipynb file, and run in Google Colab.

That’s it. The setup’s pretty simple—just follow those steps, and you’re good to go.

 
