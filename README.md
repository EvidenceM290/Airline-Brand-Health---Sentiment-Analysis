
---

# **Airline Brand Health - Sentiment Analysis**

## **Overview**
This project evaluates the **brand health** of two major airlines—**Southwest** and **American Airlines**—through sentiment analysis. The analysis utilizes **machine learning and natural language processing (NLP)** techniques to quantify brand perception based on publicly available articles, news headlines, and reviews converted to pdfs.

The sentiment analysis was conducted using:
- **KNIME Workflow** for text preprocessing and model execution.
- **R Programming** for association rules and supporting analysis.

## **Data Sources**
1. **Text Data**: Pdf converted essays of **publicly available articles, news headlines, and reviews.** on both brands
2. **Sentiment Scoring**: Sentiment scores were extracted and analyzed.
3. **Association Rules**: Conducted in **R** to identify patterns in word associations.

---

## **Key Findings**

### **1. Sentiment Analysis Statistics**
- **American Airlines**: Mean sentiment score **0.085**.
- **Southwest Airlines**: Mean sentiment score **0.096**.
- **Conclusion**: Southwest had a slightly higher sentiment score, suggesting a marginally more favorable perception.

| Airline        | Mean Sentiment Score | Standard Deviation | Skewness | Kurtosis |
|---------------|---------------------|--------------------|----------|----------|
| American      | **0.085**            | 0.327              | 1.647    | 4.947    |
| Southwest     | **0.096**            | 0.374              | 1.051    | 3.191    |

### **2. Word Cloud Analysis**
- **American Airlines**:
  - Frequent words: *American, travel, premium, global, program, innovation, commitment*.
  - Sentiment suggests a **corporate, global presence** with a focus on **premium services**.
  
- **Southwest Airlines**:
  - Frequent words: *Southwest, low-cost, friendly, customer, flexible, budget*.
  - Sentiment reflects **affordable pricing, customer service, and flexibility**.

### **3. Model Performance**
- Both **KNIME** and **R Programming** were used for **preprocessing, sentiment tagging, and association rules**.
- The **KNIME workflow** performed **sentiment tagging and text processing**.
- **Association Rules in R** identified co-occurrences of key terms in sentiment-heavy contexts.

---

## **Sentiment Analysis Workflow**
- **Preprocessing**: Text cleaning, stemming, tokenization.
- **Sentiment Tagging**: Dictionary-based tagging for **positive/negative words**.
- **Feature Engineering**: Term Frequency (TF), Inverse Document Frequency (IDF).
- **Sentiment Scoring**: Sentiment values extracted for evaluation.
- **Association Rules**: R's **`arules`** package used to identify meaningful patterns.

---

## **Visualizations**

### **American Airlines Analysis**
![American Statistics](https://github.com/EvidenceM290/Pricing-Sensitivity-Selection-Bias-Analysis-Starbucks-Rewards-Program-/blob/main/images/American%20Statistics.png)

![American Visual](https://github.com/EvidenceM290/Pricing-Sensitivity-Selection-Bias-Analysis-Starbucks-Rewards-Program-/blob/main/images/American%20Visual.png)

![American Model Workflow](https://github.com/EvidenceM290/Pricing-Sensitivity-Selection-Bias-Analysis-Starbucks-Rewards-Program-/blob/main/images/AmericanModelFlow.png)

---

### **Southwest Airlines Analysis**
![Southwest Statistics](https://github.com/EvidenceM290/Pricing-Sensitivity-Selection-Bias-Analysis-Starbucks-Rewards-Program-/blob/main/images/SouthWest%20Statistics.png)

![Southwest Visual](https://github.com/EvidenceM290/Pricing-Sensitivity-Selection-Bias-Analysis-Starbucks-Rewards-Program-/blob/main/images/SouthWest%20Visual.png)

![Southwest Model Workflow](https://github.com/EvidenceM290/Pricing-Sensitivity-Selection-Bias-Analysis-Starbucks-Rewards-Program-/blob/main/images/SouthWestModelFlow.png)

---

## **Implementation Details**
### **KNIME Workflow**
1. **PDF Parsing**: Extract text from generated documents.
2. **Text Preprocessing**: Stopword removal, stemming, case conversion.
3. **Sentiment Tagging**: Dictionary-based **positive/negative word classification**.
4. **Frequency Analysis**: TF-IDF and term frequency weighting.
5. **Visualization**: Word clouds and sentiment statistics.


---

## **Conclusion & Business Insights**
1. **Southwest slightly outperforms American in sentiment scores**.
2. **Frequent terms in American Airlines indicate a premium corporate image**, while **Southwest focuses on affordability and customer service**.
3. **Actionable Insights**:
   - American Airlines: **Leverage corporate branding and expand premium offerings**.
   - Southwest Airlines: **Continue customer-focused initiatives and budget-friendly strategies**.

---

## **Future Enhancements**
- Improve **sentiment lexicon** with **contextual embeddings**.
- Use **deep learning (BERT, LSTMs) for better sentiment classification**.


---

### **Repository Structure**
```
/Airline-Sentiment-Analysis/
│── data/  (PDF essays for both airlines)
│── models/  (KNIME workflows, R scripts)
│── results/  (Sentiment scores, association rules)
│── images/  (Visualizations)
│── README.md  (This document)
│── Airline_Brand_Health.Rmd  (Main RMarkdown Report)
```

