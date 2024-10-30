# PROJECT DESCRIPTION

This project focuses on developing a sentiment analysis model to evaluate customer feedback from five fast-food restaurants: Village Burger, Lucky's Burger & Brew, AZN Sandwich Bar, Cheeseburger Bobby's, and Farm Burger. By analyzing online reviews, the project aims to uncover underlying themes in customer feedback to assess key business performance indicators such as overall customer satisfaction, potential for customer retention, and business viability.

# TECHNOLOGIES USED

- **Machine Learning Models**: CNN, RNN, SVM, Random Forest, Naive Bayes
- **NLP Techniques**: CountVectorizer, TF-IDF, LDA, NMF
- **SMOTE**: For handling class imbalance and improving model performance
- **Hyperparameter Tuning**: To enhance model accuracy rates

# METHODOLOGY

### **Step 1: Data Loading**

- **Code:** We used `pd.read_csv()` from the `pandas` library to load the online reviews dataset into a DataFrame.
- **Explanation:** Loading data is the initial step in any data project. It allows us to bring the raw data into our environment for examination and preparation for analysis.

### **Step 2: Data Exploration**

- **Code:** We employed `.head()`, `.info()`, and `.describe()` functions from `pandas` to inspect the dataset's structure and contents.
- **Explanation:** Data exploration helps in understanding the dataset's organization, identifying data types, and summarizing basic statistics like mean, count, and unique values. This step is crucial for gaining insights into the dataset and identifying any data quality issues.

### **Step 3: Data Cleaning**

- **Code:** We checked for missing values using `isnull().sum()` and addressed any discrepancies by filling or removing them as necessary.
- **Explanation:** Data cleaning ensures that the dataset is accurate and complete. Handling missing or erroneous data is essential to avoid biasing the results of the sentiment analysis.

### **Step 4: Text Preprocessing**

- **Code:** We applied techniques such as tokenization, stemming, and removing stop words using libraries like `nltk` or `spaCy`.
- **Explanation:** Text preprocessing prepares the data for analysis by converting raw text into a structured format. This step helps in reducing noise and improving the quality of the input data for subsequent modeling.

### **Step 5: Feature Extraction**

- **Code:** We utilized the `TfidfVectorizer` from `sklearn.feature_extraction.text` to transform the cleaned text data into numerical features.
- **Explanation:** Feature extraction is critical in NLP, as it converts text into a format suitable for machine learning algorithms. Using TF-IDF helps emphasize important words in the context of the reviews.

### **Step 6: Topic Modeling**

- **Code:** We implemented Latent Dirichlet Allocation (LDA) using `sklearn.decomposition` to identify underlying topics within the reviews.
- **Explanation:** Topic modeling helps uncover hidden themes in the dataset by grouping words that frequently occur together. This step provides insights into common customer sentiments regarding food quality, service, and setting.

### **Step 7: Model Selection and Training**

- **Code:** We implemented several machine learning models, including SVM and Random Forest, from `sklearn`, and trained them on the extracted features.
- **Explanation:** Choosing the right model is crucial for effective sentiment analysis. We trained FIVE  models to compare their performance and select the best one based on accuracy and other metrics.

### **Step 8: Model Evaluation**

- **Code:** We evaluated the trained models using metrics such as accuracy, precision, recall, and F1-score, utilizing `sklearn.metrics`.
- **Explanation:** Model evaluation helps in assessing the effectiveness of the trained models. By analyzing performance metrics, we can determine how well the models classify sentiment in the reviews.

 # KEY INSIGHTS

Our analysis yielded insightful results regarding customer sentiment across the five restaurants. Village Burger emerged as the standout performer with the highest number of positive reviews at 535 and the lowest number of negative reviews, totaling only 60. In contrast, Cheeseburger Bobby’s faced significant challenges, receiving the most negative reviews at 182. Farm Burger Dunwoody exhibited a balanced sentiment distribution with 84 negative reviews, indicating areas for improvement. Lucky’s Burger & Brew Marietta garnered more than 400 positive reviews alongside 61 negative ones. Lastly, AZN Sandwich Bar recorded a total of 346 positive reviews but also had a relatively high number of negative reviews at 161, highlighting areas that need attention.
The qualitative analysis identified key topics from the reviews using methods like Latent Dirichlet Allocation and Non-Negative Matrix Factorization. The main topics included:

- **Dining Experience**
- **Customer Service**
- **Service Efficiency**
- **Food Quality**
- **Service and Food**

These topics significantly influence customer satisfaction and retention.

### **Dining Experience**

Lucky's Burger & Brew Marietta and Farm Burger Dunwoody excelled in providing a positive dining experience. Conversely, Cheeseburger Bobby's, despite many positive reviews, needs to address concerns raised in negative feedback. Village Burger has a favorable reputation, even with fewer comments.

### **Customer Service**

Customer service is a critical area for all restaurants. Farm Burger Dunwoody and Cheeseburger Bobby's received numerous negative reviews, indicating a need for improvement. AZN Sandwich Bar has more positive feedback but also significant room for enhancement.

### **Service Efficiency**

Village Burger demonstrated strong service efficiency, outperforming others. AZN Sandwich Bar and Cheeseburger Bobby's showed mixed results, indicating inconsistencies that require attention. Farm Burger Dunwoody and Lucky's Burger & Brew Marietta also appeared effective in this regard.

### **Food Quality**

Village Burger leads in both the volume and positivity of food quality reviews. Farm Burger Dunwoody and Cheeseburger Bobby's also received favorable comments, highlighting food quality as a strength. AZN Sandwich Bar, with fewer reviews, is positively perceived in this category.

### **Service and Food**

The synergy of service and food quality drives customer satisfaction. Restaurants excelling in both, such as Village Burger, garnered the most positive feedback. Cheeseburger Bobby's and AZN Sandwich Bar also showed strong overall performance, while Farm Burger Dunwoody received favorable remarks despite fewer reviews.

This sentiment analysis project provides a comprehensive understanding of customer perceptions across the different restaurants, emphasizing the critical aspects of food quality, service efficiency, and dining experiences. These insights can guide targeted improvements to enhance customer satisfaction and loyalty, ultimately contributing to the long-term success of each establishment.
