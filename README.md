


# Zomato Restaurant Clustering & Sentiment Analysis 🍽️

**Author:** Piyush Awal | AI & ML Enthusiast  
**Domain:** Unsupervised Machine Learning & Natural Language Processing (NLP)

## 📌 Project Overview
This project analyzes a comprehensive dataset of Zomato restaurants and customer reviews to extract actionable business insights. Using unsupervised machine learning (K-Means Clustering) and NLP (VADER Sentiment Analysis), the project groups similar restaurants and evaluates customer satisfaction to provide targeted recommendations for both customers and business stakeholders.

## 🎯 Objectives
* Perform Exploratory Data Analysis (EDA) on restaurant features (cost, ratings, cuisines).
* Clean and preprocess textual and numerical data.
* Engineer one-hot encoded features for complex categories (e.g., multi-cuisine offerings).
* Cluster restaurants into distinct market segments using K-Means.
* Analyze customer review sentiments using NLTK's VADER.
* Generate data-driven business insights for Zomato and platform users.

## 🛠️ Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (K-Means, StandardScaler)
* **Natural Language Processing:** NLTK (VADER)
* **Data Visualization:** Matplotlib, Seaborn

## 📊 Project Architecture
1. **Exploratory Data Analysis (EDA):** Analyzed the distributions of restaurant costs, customer ratings, and the popularity of specific cuisines. 
2. **Data Preprocessing:** Handled missing values (dropped empty reviews), standardized numerical features using `StandardScaler`, and one-hot encoded the `Cuisines` feature.
3. **Model Implementation (Clustering):** Used the **Elbow Method** to determine the optimal number of clusters ($K=7$). Applied the K-Means algorithm to group the restaurants based on their cost, rating, and cuisine similarities.
4. **Sentiment Analysis:** Processed nearly 10,000 raw text reviews using VADER, scoring them as Positive, Negative, or Neutral to gauge overall customer satisfaction.
5. **Business Insights:** Cross-referenced customer sentiments with restaurant clusters to identify the highest-performing market segments.

## 💡 Key Business Insights
* **Cost vs. Rating:** Discovered a moderate positive correlation (0.42) between the cost for one person and the average customer rating, indicating that premium pricing generally correlates with better customer experiences.
* **Market Segments:** Successfully identified 7 distinct market clusters. This clearly separates high-volume budget options (Clusters 1 & 4, average cost ₹500–₹616) from premium fine-dining experiences (Clusters 3 & 5, average cost ₹1300–₹2000).
* **Customer Sentiment:** Revealed an overwhelmingly positive baseline across the platform, with **74%** of customer feedback categorized as positive.
* **Recommendations:** North Indian and Chinese cuisines dominate the landscape, representing the safest entry point for new restaurants. Customers seeking guaranteed high satisfaction should be recommended to the premium clusters, which maintain the highest average ratings and positive sentiment ratios.

## 🚀 How to Run the Project
1. Clone this repository.
2. Ensure you have the required datasets: `Zomato Restaurant names and Metadata.csv` and `Zomato Restaurant reviews.csv` in your working directory.
3. Open the Jupyter/Colab Notebook (`zomato.ipynb`) and run the cells sequentially to reproduce the clustering and sentiment analysis outputs.
