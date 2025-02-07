# **Project Proposal**  
This is our final team project proposal for our Fall Class DECISION 546Q Modern Analytics taught by Professor Jiaming, Xu.
**Team #36**: Bohan Bai (bb422), Meiyi Guo (mg483), Ethan Jaglal (enj13), Atharv Verma (av300), Jingwen Yu (jy421)  

---

## **Problem Statement**  
Develop a deep learning model to predict a movie's revenue based on available features such as **genre, budget, cast, score, and release date**.  

---

## **Problem Background / Scenario**  
In the movie industry, predicting the potential revenue of a film **before its release** is crucial for:  
- Financial planning  
- Marketing strategies  
- Investment decisions  

Using a dataset of past movie performances and their associated attributes, a **predictive model** can provide valuable insights into how these factors contribute to a movie's success. This could assist:  
- 🎬 **Studios, directors, and production houses** in making data-driven decisions.  
- 💰 **Investors** in assessing potential profitability.  
- 📢 **Marketers** in optimizing advertising strategies.  

---

## **Data Source**  
📂 **Dataset:** [IMDb Movies Dataset](https://www.kaggle.com/datasets/ashpalsingh1525/imdb-movies-dataset/data)  

**Dataset includes the following columns:**  
- 🎥 **Movie Attributes**: `names`, `date_x`, `score`, `genre`, `overview`, `crew`, `orig_title`, `status`, `orig_lang`, `budget_x`, `revenue`, `country`.  
- 🔍 **Primary Features of Interest**: `genre`, `budget`, `crew`, `original language`, and `release date`.  
- 🎯 **Target Variable**: `Revenue`.  

---

## **Deep Learning Approach**  

### **Data Preprocessing**  
✔️ **Categorical Data Handling**: One-hot encoding for features like `genre`, `orig_lang`, and `country`.  
✔️ **Text Processing**: Use **word embeddings** (e.g., Word2Vec, GloVe, or Transformer models like BERT) for `overview` and `crew` to extract semantic information.  
✔️ **Date Feature Engineering**: Extract time-based information like **month, quarter, and year** from `date_x` to capture seasonality and trends.  
✔️ **Normalization**: Scale numerical features like `budget_x` for better model convergence.  

### **Model Architecture**  
🧠 **Neural Network Components**:  
- **Embedding Layers**: For handling categorical and text data.  
- **LSTM/GRU Layers**: If leveraging sequence data (e.g., release trends over time).  
- **Dense Layers**: Fully connected layers for combining all input features and making revenue predictions.  
- **Output Layer**: Single node for continuous revenue prediction using a **linear activation function**.  

### **Model Training**  
⚙️ **Optimization & Loss Function**:  
- **Loss Function**: Mean Squared Error (**MSE**) for regression.  
- **Optimizer**: **Adam optimizer** for adaptive learning rates.  
- **Evaluation Metrics**: Mean Absolute Error (**MAE**) or Root Mean Squared Error (**RMSE**).  
- **Natural Language Processing (NLP)**: Applied to text data types for better feature extraction.  

### **Hyperparameter Tuning**  
🔧 **Optimization Methods**:  
- **Manual Tuning**  
- **Bayesian Optimization**  
- **Grid Search**  
- **Random Search**  

---

## **Expected Result**  
A trained **deep learning model** that can predict movie revenue with **reasonable accuracy**.  
- 📊 **Performance Evaluation**: Metrics like **RMSE** or **MAE**.  
- ✅ **Validation**: K-fold cross-validation to ensure model generalizability.  

---

## **Potential Business Impact**  
💰 **Investment Decision-Making**:  
- Producers and investors can **allocate resources more effectively** to projects likely to yield high returns.  

📢 **Marketing Strategy**:  
- Insights from the model can **guide marketing campaigns**, targeting specific demographics and release timings to **maximize revenue**.  

⚠️ **Risk Management**:  
- Identifies potential **underperforming movies** early in the production pipeline, allowing for strategic pivots or cost management.  

🏆 **Competitor Analysis**:  
- By comparing **predicted revenue** with actual performance, businesses can **benchmark against competitors** and refine their strategies.  

🎥 **Future Movie Strategies**:  
- Plan future movies based on specific attributes to **predict success** before production begins.  

## 📜 **Final Write-up**
📄 **Read our full report here**:  
[IMDB Movies Analysis](https://docs.google.com/document/d/1_WH-OmBSVD6p75qBeeVgYIsLFAJPcRcl/edit?usp=sharing&ouid=105049261238731764444&rtpof=true&sd=true)  

