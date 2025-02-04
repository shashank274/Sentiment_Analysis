# Sentiment Analysis of Amazon Reviews

![Project Banner](https://raw.githubusercontent.com/your-username/your-repo/main/path-to-your-image.png)

## 📌 Project Overview
This project analyzes sentiment in Amazon customer reviews using **VADER** and **RoBERTa** models. The goal is to compare the sentiment classification accuracy of both models and visualize the distribution of sentiments.

## 📊 Methodology
1. **Data Collection** - Extracted Amazon product reviews dataset.
2. **Preprocessing** - Cleaned text, removed stopwords, and normalized data.
3. **Sentiment Analysis**:
   - **VADER (Valence Aware Dictionary and sEntiment Reasoner)** for rule-based sentiment analysis.
   - **RoBERTa (Robustly Optimized BERT Approach)** for deep-learning-based sentiment classification.
4. **Visualization & Insights** - Compared the sentiment classification results using different metrics.

## 📌 Models Used
### 1️⃣ VADER
- Lexicon-based sentiment scoring.
- Best for short, informal texts like social media comments.
- Outputs **positive, neutral, or negative** sentiment.

### 2️⃣ RoBERTa
- Transformer-based deep learning model.
- Fine-tuned for sentiment classification.
- More accurate than lexicon-based methods for complex texts.

## 🔍 Sentiment Distribution Visualizations
### 1️⃣ VADER Sentiment Distribution
![image](https://github.com/user-attachments/assets/68edf0b6-5ba6-4c71-844e-80b2c89ad3dd)


### 2️⃣ RoBERTa Sentiment Distribution
![image](https://github.com/user-attachments/assets/d22cb53b-981c-42ea-9ad6-f22959776b98)


### 3️⃣ Model Comparison
![image](https://github.com/user-attachments/assets/5c5c7ec8-3fba-429d-b9cb-10c4a140e1fe)


## 🚀 Insights
- **Comparison of VADER and RoBERTa** in classifying sentiments.
- Observations on where **rule-based vs. deep learning** approaches perform better.
- Potential applications for **customer feedback analysis** in e-commerce.

## 🛠 Technologies Used
- **Python**
- **NLTK** (VADER)
- **Hugging Face Transformers** (RoBERTa)
- **Matplotlib & Seaborn** (Visualizations)

## 📌 How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run sentiment analysis:
   ```bash
   python sentiment_analysis.py
   ```

## 📜 License
This project is licensed under the MIT License.

## 🤝 Contributing
Feel free to submit a pull request or open an issue if you find any improvements!

## 📞 Contact
- **Email:** your-email@example.com
- **GitHub:** [your-username](https://github.com/your-username)
