# Internet-Censorship-A-Data-Driven-Investigation

### **Overview**

Internet censorship restricts access to information and suppresses freedom of expression through methods like DNS blocking, TCP/IP filtering, and HTTP throttling. Analyzing censored network data over time can uncover targeted content types, censorship frequencies, and evolving practices. This project examines a dataset from Russia (October 2022) to identify patterns, enforcement techniques, and changes in censorship dynamics, aiding efforts to promote digital freedom and develop anti-censorship tools.

### **Data**

OONI is an open-source initiative that detects and documents internet censorship, traffic manipulation, and network performance issues globally, using a dataset from October 2022 of Russia with over 1,000,000 measurements.


### **Repository Structure**

This repository contains the following key files and code snippets:
1. DM_Project_Final_Code: This is the main code that integrates all steps in the project, including data preprocessing, classification, and clustering analysis. It is a Colab notebook.
2. Clustering Code: This code is for reference and includes clustering techniques, specifically K-Means clustering, for analyzing censorship data.
3. Decision Tree Code: This code is for reference and demonstrates the decision tree classification approach to identify censorship patterns.

### **Requirements**

1. pandas: For data manipulation and analysis.
2. csv: For reading and writing CSV files.
3. math: For mathematical operations.
4. numpy: For numerical operations and handling arrays.
5. matplotlib.pyplot: For plotting graphs and visualizations.
6. collections.Counter: For counting elements in a collection.
7. collections.defaultdict: For working with dictionaries with default values.
8. sklearn.model_selection.KFold: For cross-validation and splitting the dataset.
9. gensim: For Word2Vec embedding and natural language processing.
10. sklearn.preprocessing.normalize: For normalizing data.
11. sklearn.metrics.rand_score, adjusted_rand_score: For evaluating clustering performance using Rand Index.
12. google.colab.files: For uploading files in Colab.

### **Project Code**

1. Dataset Import and Preprocessing: This snippet imports the dataset and performs initial preprocessing, such as handling missing values, encoding categorical variables, and normalizing data to prepare it for further analysis.
2. Data Preprocessing for Decision Tree and Clustering: This snippet separately preprocesses the data for classification (decision tree) and clustering tasks. It ensures that the data is appropriately formatted and ready for both methods, with necessary feature extraction and encoding.
3. Decision Tree Classification and Cross-Validation: This snippet performs classification using a decision tree. It applies cross-validation to evaluate the performance of the classifier, ensuring the model generalizes well on unseen data. The output includes accuracy and the Gini index for each split.
4. Confusion Matrix Representation: This snippet visualizes the results of the decision tree classification using a confusion matrix. It helps to evaluate the model’s performance in terms of true positives, false positives, true negatives, and false negatives, providing a clearer picture of its predictive ability.
5. Word2Vec Encoding for Clustering: These snippets perform data encoding using Word2Vec, a neural network model that generates vector representations of words (or data points) to capture their relationships and semantic meaning. This encoding technique is useful for clustering tasks, particularly in understanding the similarity of censorship patterns across different data points.
6. Clustering with K-Means: This snippet performs clustering using the K-Means algorithm, which groups the data into clusters based on similarity. It helps to identify patterns of censorship by grouping similar types of censorship events together, revealing insights about how censorship enforcement occurs over time.
7. Calculating Rand Index for Clustering Validation: This snippet calculates the Rand index to validate the output of the clustering. The Rand index measures the similarity between the predicted clusters and the true labels, providing a quantitative way to assess the quality of the clustering results

### **Usage**

1. DM_Project_Final_Code.ipynb notebook notebook will guide you through the entire analysis pipeline, from data preprocessing to classification and clustering.
2. The code snippets are organized within the Colab notebook. You can run each snippet step by step or modify them according to your specific needs.
3. Once the code has been executed, you can review the output, including the confusion matrix, classification accuracy, and clustering results. Use the generated plots and metrics to gain insights into censorship patterns and validate the findings.

