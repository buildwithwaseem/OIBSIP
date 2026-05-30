**See Task 4 :** https://nbviewer.org/github/buildwithwaseem/OIBSIP/blob/main/EmailSpamD.ipynb

# ✉️ Task 4: Email/SMS Spam Detection

This project focuses on Natural Language Processing (NLP) to build a machine learning model that automatically classifies SMS or emails into **Spam** or **Ham** (legitimate messages).

## 🛠️ The Workflow & Technical Approach

### 1. Text Preprocessing & Cleaning
Raw text data cannot be directly fed into a machine learning algorithm. To fix this, I used:
* **Tokenization:** Breaking down sentences into individual words.
* **Vectorization (TF-IDF / CountVectorizer):** Converted text strings into a matrix of token counts and numerical vectors so that the model can understand word importance.

### 2. Model Selection
I implemented the **Multinomial Naive Bayes** classifier. 
* *Why Naive Bayes?* It works on text probability features and is the industry standard for baseline text classification and spam filtering due to its speed and high efficiency with discrete features.

### 3. Key Evaluation Metrics
Instead of just relying on raw accuracy, the model was evaluated using:
* **Confusion Matrix:** To track True Positives (correctly identified spam) and False Positives (legitimate emails wrongly flagged as spam).
* **Precision & Recall:** Crucial for spam detection because we don't want important/useful emails to accidentally end up in the spam folder.

## 📈 Key Insights & Learning
* Words like *'free'*, *'winner'*, *'prize'*, and *'urgent'* had the highest text weightage in the spam classification category.
* Text cleaning and choosing the right vectorizer has a much bigger impact on NLP model performance than just tuning the algorithm hyperparameters.

## 💻 Tech Stack Used
- **Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, CountVectorizer / TF-IDF
- **Environment:** Google Colab
