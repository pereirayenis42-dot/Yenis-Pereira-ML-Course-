## ITAI 1371: Introduction to Machine Learning - Final Project 🚀## 📊 Data Storytelling: Sentiment Analysis Investigation
📅 Due Date: Refer to Course Schedule
⏳ Time Allotment: Approx. 5-7 hours of work
📥 Submission: Submit a single ZIP file containing your notebook/code, data, and final report.
------------------------------
## 🎯 Project Goal
Your mission is to develop a sentiment analysis model using advanced machine learning techniques. As a data storyteller 🗣️, you will transform raw text (reviews, tweets, etc.) into actionable insights. This project tests your ability to handle unstructured data, perform complex preprocessing, and evaluate model performance using NLP-specific metrics.
## ⚖️ Academic Integrity & Use of AI Tools

* 👤 This is an individual project. Your analysis and report must be your own work.
* ✅ You are permitted to use AI code assistants (like GitHub Copilot) to help you write cleaning functions, vectorize text, and debug your models.
* ❌ You are NOT permitted to use AI to generate your final report or your interpretations of the model's errors.
* 🔍 To ensure academic integrity, your report must address specific examples of misclassified text from your unique dataset.

------------------------------
## 📈 Grading Rubric (100 Points Total)

| Section | Task | Points |
|---|---|---|
| Part 1: Data Selection 📂 | Choose and load a relevant text dataset (e.g., Sentiment140). | 10 |
| Part 2: NLP Preprocessing 🧼 | Implement text cleaning (stop words, punctuation) and tokenization. | 20 |
| Part 3: Vectorization 🔢 | Successfully transform text into numerical data (e.g., TF-IDF). | 10 |
| Part 4: Modeling 🤖 | Train at least two different models (e.g., Random Forest vs. Neural Network). | 20 |
| Part 5: Evaluation 📏 | Compare models using Accuracy, Precision, Recall, and F1-score. | 20 |
| Part 6: Final Report 📝 | Summarize methodology and provide a deep dive into your conclusions. | 15 |
| Overall ✨ | Code follows best practices, is well-documented, and runs error-free. | 5 |

------------------------------
## 💡 Tips for Success

* The Power of Preprocessing: In NLP, your model is only as good as your data cleaning. Show how removing "noise" 🧹 improved your results.
* Metric Matters: Explain why you might care more about Precision or Recall in your specific context (e.g., does a false positive "angry" tweet 😡 matter more than a missed one?).
* Visual Storytelling: Include word clouds ☁️ or frequency charts in your EDA to show the most common sentiment-driven words.

------------------------------
## ✅ Self-Check Before Submission

* Dataset is included or linked in the documentation.
* Code is well-commented and includes a logical flow.
* Final report clearly justifies the choice of the "best" model.
* The submission is packaged in a single, organized ZIP file 📦.

---

## 📖 Data Dictionary: IMDb Dataset
The dataset contains a total of 50,000 movie reviews labeled for sentiment analysis.

| Column Name 🏷️ | Description 📝 | Data Type 🔢 | Example Value 💡 |
|---|---|---|---|
| review | The full text of the movie review. | string | "One of the best movies I've seen..." |
| sentiment | The target label (Positive or Negative). | string | "positive" |

------------------------------
## 📂 Dataset Details

* Source: [IMDb Dataset of 50K Movie Reviews (Kaggle)](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews) 🔗
* Total Rows: 50,000 observations 📊
* Target Distribution: Balanced (25,000 positive, 25,000 negative) ⚖️

## 🛠️ Quick Setup Tip
Since this dataset uses strings for the sentiment (e.g., "positive", "negative"), you will need to encode them into numbers before training your models:

# Quick encoding for your 'Part 3: Vectorization'
df['label'] = df['sentiment'].apply(lambda x: 1 if x == 'positive' else 0)
