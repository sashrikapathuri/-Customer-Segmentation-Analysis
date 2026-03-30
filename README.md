# Customer-Segmentation-Analysis
📊 Customer Segmentation Analysis
A complete pipeline for customer segmentation using RFM analysis (Recency, Frequency, Monetary), clustering with KMeans, visualizations, and NLP-based sentiment analysis. This project provides insights into customer behavior and uses machine learning techniques for segmentation and predictive modeling.

🚀 Features
RFM Analysis to classify customers based on their purchase behavior. KMeans Clustering to group customers into segments. Data Visualizations using Seaborn, Matplotlib, and Plotly. Sentiment Analysis with VADER and TextBlob to analyze customer reviews. WordCloud Generation for visualizing text data. Logistic Regression for predicting repurchases. Dash Integration for building interactive dashboards (optional).

🗂️ Dataset
The dataset is sourced from Kaggle's Ecommerce Data and contains transactional records from a UK-based online retailer.

📋 Requirements
Make sure you have the following packages installed: bash

pip install pandas scikit-learn matplotlib seaborn plotly dash nltk textblob wordcloud kagglehub
🔧 Installation and Usage Clone the repository: bash

git clone https://github.com/your-username/customer-segmentation.git
cd customer-segmentation
Run the notebook locally: Open Google Colab or Jupyter Notebook. Load the Customer Segmentation Analysis.ipynb notebook. Dataset Download: Download the dataset using the KaggleHub API:

import kagglehub
path = kagglehub.dataset_download("carrie1/ecommerce-data")
🧠 Project Overview
Data Cleaning and Preprocessing Drop rows with missing customer IDs. Filter out invalid transactions (quantities or prices ≤ 0). Create a TotalPrice column (Quantity × UnitPrice).

RFM Analysis RFM analysis groups customers based on: Recency: Days since the last purchase. Frequency: Number of purchases. Monetary: Total spending.

KMeans Clustering Standardize RFM values using StandardScaler. Apply KMeans clustering to segment customers into 3 or 4 clusters.

Data Visualizations Seaborn Scatterplots to show RFM clusters. Monthly Revenue Trend and Top Purchased Products. Heatmaps for correlation between features.

Sentiment Analysis with NLP Use VADER and TextBlob for sentiment scores. Generate WordClouds for customer feedback.

Machine Learning for Predictive Analytics Apply Logistic Regression to predict repurchases. Evaluate model performance using a Confusion Matrix and Classification Report.

📊 Key Visualizations
-3D Cluster Plot of Customer Segments.
-Top 10 Countries by Revenue.
-Monthly Revenue Trend.
-WordCloud of customer reviews.

📝 Usage of Sentimernt Analysis
Screenshot 2024-10-17 at 3 11 03 PM
📈 Example Visualizations
Monthly Revenue Trend: Screenshot 2024-10-17 at 3 11 44 PM

Top 10 Most Purchased Products: Screenshot 2024-10-17 at 3 11 59 PM

3D view of Customer Segment

 Screen.Recording.2024-10-17.at.5.21.10.PM.online-video-cutter.com.mp4 
Customer Segmentation with K-Means image

Sales Forecast using ARIMA image

🎯 Future Improvements
Add Dash App for interactive dashboards. Explore other clustering methods like DBSCAN or Hierarchical Clustering. Enhance predictive analytics with Random Forest or XGBoost models. Deploy the analysis on a cloud platform for live monitoring.

🤝 Contributing
Feel free to fork this repository and submit pull requests to enhance the project!

🧑‍💻 Author
Vidit Sheth

💬 Feedback
If you have any questions or feedback, feel free to reach out via GitHub Issues.

🔗 Links
Kaggle Dataset: https://www.kaggle.com/datasets/carrie1/ecommerce-data?select=data.csv
Project Notebook on Colab: https://colab.research.google.com/drive/1oYqfi7Q9h-XClifhAD-yGAAD_wurIg0w?usp=sharing
