# SQL Injection Detection Using Machine Learning

This repository contains the materials for a project developed at the Indian Institute of Information Technology, Surat, by students Ankit Gondha and Jitanshu Raut under the guidance of Dr. Pradeep Kumar Roy and Dr. Rajesh K. Ahir. The project focuses on detecting SQL injection attacks using a hybrid approach that combines machine learning, natural language processing, and regular expression analysis.

## Project Description

SQL injection (SQLi) is a prevalent security threat to web applications that manipulate SQL statements to execute malicious queries, allowing attackers unauthorized access to database resources. Our project addresses this critical security risk by developing a detection system capable of identifying SQL injection attempts with high accuracy.

### Problem Statement

Web applications are susceptible to various cyber-attacks, with SQL injection being one of the most effective due to vulnerabilities in the database query software. Traditional methods like input validation and parameterized queries are often bypassed by sophisticated hacking techniques. Therefore, an advanced approach that can evolve and adapt to new SQL injection strategies is required.

### Objectives

The main objective of our project is to:
- Develop a system that effectively detects SQL injection attacks.
- Combine regular expression analysis with advanced machine learning techniques to improve detection accuracy.
- Utilize the BERT model for processing SQL queries to enhance the understanding of complex queries.

## Methodology

Our approach involves three primary techniques:
1. **Regular Expression Analysis:** This technique uses regular expressions to detect patterns and keywords that are commonly associated with SQL injection attacks. It provides a first line of defense by filtering out obvious malicious queries.
2. **Machine Learning Techniques:** We employ several machine learning models to learn from both benign and malicious SQL queries. These models help identify less obvious patterns that might not be caught by regex analysis.
3. **Natural Language Processing (NLP):** Using the BERT model, our system gains a deeper understanding of the context within SQL queries, which helps in distinguishing between harmful and normal activities more accurately.

### Detailed Description of Components

1. **Regex Analysis:**
   - Regex patterns are used to match known malicious SQL query structures.
   - This method quickly flags potentially dangerous queries for further analysis.

2. **Machine Learning Models:**
   - **Random Forest:** A robust model that classifies queries based on features extracted from the data. It is known for its high accuracy and the ability to handle overfitting.
   - **Support Vector Machines (SVMs):** Used for their effectiveness in high-dimensional spaces, SVMs are critical for classifying complex query structures.
   - **BERT Model:** Implements a transformer-based architecture that excels in understanding the context and semantics of text, which is crucial for parsing and analyzing SQL queries.

3. **Data Preprocessing and Feature Extraction:**
   - We use techniques like TF-IDF, bag of words, and word embeddings to convert SQL queries into a format that can be processed by machine learning models.

## Experimental Setup

### Datasets

Our models are trained and tested on a variety of datasets that include benign and malicious SQL queries. These datasets are sourced from public platforms such as GitHub and Kaggle, providing a diverse range of scenarios for robust testing.

### Performance Metrics

We evaluate our models based on several metrics:
- **Accuracy:** Overall correctness of the model.
- **Precision and Recall:** Effectiveness in identifying positive instances.
- **F1 Score:** Harmonic mean of precision and recall, providing a balance between the two.

## Results

Our system demonstrated promising results in detecting SQL injection attacks:
- **Random Forest** showed an accuracy of 81.33%, with a precision of 99.00% and an F1-score of 84.13%.
- **SVMs** achieved a precision of 93.60%, though they had lower recall, indicating room for improvement.
- **BERT Model** excelled with an accuracy of 98.11%, a near-perfect precision, and an F1-score of 98.07%, indicating very high efficacy in detecting SQL injections.

## Contributer

<a href="https://github.com/jitanshuraut">
  <img src="[https://contrib.rocks/image?repo=OWNER/REPO](https://avatars.githubusercontent.com/u/96559286?v=)" />
</a>
