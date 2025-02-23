# Sentiment Analysis of Tweets  

## 📌 Overview  
This project focuses on **sentiment analysis of tweets**, classifying them into **positive, neutral, or negative** categories. The analysis is performed using **machine learning (Logistic Regression)** and **deep learning (CNN & LSTM)** models.  

The goal is to develop an **automated sentiment classifier** that can effectively handle **slang, abbreviations, and informal language** to extract meaningful insights from public opinion.  

## 📂 Dataset  
The dataset consists of **1.6 million tweets**, pre-labeled with sentiment scores:  
- **0** → Negative  
- **2** → Neutral  
- **4** → Positive  

🔗 The dataset source is provided in `dataset.txt`.  

## 🛠 Methodology  
### 1️⃣ **Data Preprocessing**  
- Removed **URLs, mentions, hashtags, and punctuation**.  
- Applied **TF-IDF vectorization** to convert text into numerical features.  

### 2️⃣ **Model Development**  
- **Logistic Regression:** Achieved ~50.2% accuracy, but struggled with capturing contextual sentiment.  
- **CNN (Convolutional Neural Network):** Achieved **80.7% accuracy**, effectively identifying local patterns in text.  
- **LSTM (Long Short-Term Memory Network):** Underperformed (~49.9% accuracy), likely due to hyperparameter tuning challenges.  

## 🔧 Requirements  
Install dependencies using:  
```sh  
pip install -r requirements.txt  
```  

## 🚀 Running the Project  
Run the Jupyter Notebook:  
```sh  
jupyter notebook  
```  
Open `notebook.ipynb` and execute all cells to train models and evaluate performance.  

## 📈 Results  
| Model                | Accuracy |  
|----------------------|---------|  
| Logistic Regression  | 50.2%   |  
| CNN                 | **80.7%**   |  
| LSTM                | 49.9%   |  

## 🔍 Future Improvements  
- Implement **Transformer models (BERT, RoBERTa)** for better contextual understanding.  
- Use **SHAP/LIME** to improve explainability of predictions.  
