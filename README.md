## How Sweet: Sweetness Sentiment Analysis in Amazon Food Reviews

### Project Overview
This project focuses on analyzing how people express their emotional responses to sweetness in Amazon food and drink reviews. 
Moving beyond general sentiment, it aims to uncover nuanced taste perceptions, preference expressions, and the specific vocabulary used to describe their feeling about sweentness. 
Ultimately, providing insights into subjective taste and the social language of sweetness.
---

### Key Features & Methodology

- **Targeted Data Extraction**: Focused on reviews mentioning "sweet" and their surrounding context from the Amazon Fine Food Reviews dataset
- **Comprehensive Preprocessing**: Utilized SpaCy for tokenization, lemmatization, and custom stopword removal (preserving negations)
- **Manual Labeling**: A subset of 100 reviews was meticulously labeled into 'Positive', 'Negative', and 'Neutral' sweetness sentiments
- **Feature Engineering**: Combined TF-IDF vectorization with engineered features VADER sentiment scores, negation/intensifier flags, and original review ratings
- **Model Training**: Trained Logistic Regression, Support Vector Machine, and Random Forest classifiers
- **Linguistic Insights**: Visualized the most influential words and phrases for positive and negative sweetness sentiment contexts
- **Interactive Demo**: A Gradio-based web interface for real-time, interactive sentiment analysis of new text inputs
---

### Project Structure

── amazon-fine-food-reviews/
   ├── Reviews.csv                 
   ├── sweet_reviews_subset.csv    
   ├── sweet_reviews_cleaned.csv   
   ├── manual_labeling_sample.csv  
   ├── manual_labeling_sample_done.csv
   └── models/                     
       ├── best_logistic_regression_model.pkl
       ├── best_svc_model.pkl
       └── best_random_forest_model.pkl
── README.md                       
── How_Sweet_Cleaned.ipynb



---

### Key Outcomes

- A functional sentiment analysis pipeline for nuanced sweetness expressions
- Trained and evaluated multiple machine learning models, demonstrating their ability to classify subjective taste preferences
- Created an interactive Gradio application for real-time model testing and qualitative assessment


---

### Future Work

- Expand Labeled Dataset: Increase the size of the manually labeled data, potentially leveraging active learning

- Explore Advanced Models: Investigate more sophisticated architectures for enhanced performance

- Refine Feature Engineering: Further optimize numerical features and explore more complex feature interactions

- In-depth Error Analysis: Conduct detailed analysis of misclassifications to identify specific model weaknesses

- Enhance Gradio Interface: Add features like prediction confidence scores



