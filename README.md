# Fashion-Recommender-System-using-H-M-Dataset
Project in Recommender Systems Course

🎯 Project Objective
To design and develop a scalable, data-driven Fashion Recommendation System for H&M, with the goal of enhancing user engagement, boosting conversion rates, and delivering a tailored shopping experience across mobile and web platforms.

This solution intelligently suggests clothing products to customers based on purchase behavior, demographics, and seasonal trends, thereby mimicking real-world personalization strategies seen in successful platforms like Amazon and Stitch Fix.

💼 Business Value
Increased Sales & Retention: Personalized suggestions that adapt to each customer's preferences drive higher click-through and purchase rates.

Cold-Start Mitigation: A robust strategy using popularity, affordability, seasonality, and demographic targeting ensures relevant suggestions even for new users.

Customer Segmentation: Insight-driven marketing strategies tailored for new, frequent, and premium shoppers.

Trend Adaptability: Time-aware architecture that captures seasonality, sale events, and evolving user behavior.

Scalability Path: Framework ready to evolve into a hybrid model using advanced methods like Neural Networks and LLMs when compute resources allow.

📊 Dataset Summary
Sourced from Kaggle's H&M competition:

31M+ transactions

1.3M customers

105K+ fashion articles

Product images available for UI/UX enhancements

🛠️ Key Features
Feature	Description
🔍 User Profiling	Leverages purchase history, age, membership status
🧠 Content-Based Filtering	Uses product type, color, and Word2Vec from descriptions
🔗 Collaborative Filtering (SVD)	Captures latent preferences from sparse user-item matrix
❄️ Cold Start Strategy	Combines top-selling, seasonal, and age-based trends
📈 Segmentation & Clustering	K-means applied on user activity and demographics
🔄 Rolling Window Validation	Time-based splitting for realistic evaluation

📈 Evaluation Metrics
Metric	Purpose
Precision@10	Measures relevance of top recommendations
Recall@10	Captures completeness of relevant suggestions
F1-Score / MAP@10	Balanced performance measure and rank sensitivity

Despite using only ~2.5% of the full dataset on limited hardware, the system achieved comparable performance to industry benchmarks like Amazon’s baseline model.

🔁 Ensemble Results
Final deployment combines:

Collaborative Filtering

Neural Network

BERT-based KNN model
Optimized using LGBMRanker, achieving:

🎯 Precision: 0.2540

🎯 Recall: 0.8079

🔮 Future Extensions
Extension	Stakeholder Benefit
🔁 Hybrid Modeling	Combines CF + content models for diversity and accuracy
📆 Sequential Recommendations	Predicts purchases based on time-sensitive behavior
🌐 Context-Aware Suggestions	Adapts to device, time of day, season, or geo-location
🧑‍🤝‍🧑 Social Graph Recommendations	Suggests based on peer purchases and trends
🧠 LLM-Powered Summarization	Auto-generates user-specific fashion insights from reviews

🧩 Tech Stack
Python, Pandas, Scikit-learn, NLTK, Gensim (Word2Vec)

SVD, Cosine Similarity, K-Means Clustering

Evaluation: Precision, Recall, F1, MAP

Visualization: Matplotlib, Seaborn

Deployment Ready for: Integration into React / Mobile UI mockups

🙋 Why It Matters
This project bridges the gap between data science and customer-centric fashion retail. It highlights how basic yet interpretable models, enhanced by real user behavior, can deliver measurable business impact—even before introducing deep learning.

The architecture, methodology, and insights serve as a blueprint for building commercially deployable recommender systems, tailored for e-commerce growth.
