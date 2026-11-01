# Sentiment Analysis of Amazon Reviews

Compares two ways of reading the mood of a customer review: **VADER**, a rule-based word-list approach, and **RoBERTa**, a pre-trained transformer model. Both are run on 5,000 Amazon food reviews and checked against the star rating each customer gave.

Built with Python, NLTK, Hugging Face Transformers, pandas and seaborn in a Jupyter notebook.

## The data

The Amazon Fine Food Reviews dataset (`Reviews.csv`). The notebook uses the first **5,000 reviews**, each with its review text and a 1 to 5 star score.

## What the notebook does

1. **Quick look at the data.** Counts how many reviews there are for each star rating.
2. **NLTK basics.** Splits an example review into words, tags the parts of speech and picks out named entities (for example, it spots "Quaker Oats" as an organisation).
3. **VADER.** Scores every review as negative, neutral and positive, plus one overall "compound" score. Charts compare these scores with the star ratings.
4. **RoBERTa.** Runs the same reviews through `cardiffnlp/twitter-roberta-base-sentiment`, a model already trained for sentiment, and gets its negative, neutral and positive scores.
5. **Compare the two.** A pair plot puts both models' scores side by side, coloured by star rating.
6. **Look at where they disagree with the stars.** For example, the review each model finds most positive among 1-star reviews, and most negative among 5-star reviews.
7. **Hugging Face pipeline.** A short demo of the one-line `pipeline("sentiment-analysis")` approach.

A small number of reviews raised an error in the RoBERTa step and were skipped.

## Charts

VADER scores by star rating:

![VADER sentiment by star rating](https://github.com/user-attachments/assets/68edf0b6-5ba6-4c71-844e-80b2c89ad3dd)

RoBERTa scores by star rating:

![RoBERTa sentiment by star rating](https://github.com/user-attachments/assets/d22cb53b-981c-42ea-9ad6-f22959776b98)

VADER and RoBERTa compared:

![Model comparison](https://github.com/user-attachments/assets/5c5c7ec8-3fba-429d-b9cb-10c4a140e1fe)

## Run it

```bash
git clone https://github.com/shashank274/Sentiment_Analysis.git
cd Sentiment_Analysis
pip install -r requirements.txt
```

Download `Reviews.csv` (the Kaggle "Amazon Fine Food Reviews" dataset), put it in this folder, then open `main.ipynb` in Jupyter. The RoBERTa model (about 500 MB) downloads automatically the first time.

---

More of my work: [portfolio-pied-gamma-88.vercel.app](https://portfolio-pied-gamma-88.vercel.app)
