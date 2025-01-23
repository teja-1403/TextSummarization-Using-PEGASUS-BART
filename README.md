# News Article Summarization Using PEGASUS and BART Model

This project explores and compares the capabilities of PEGASUS and BART models in summarizing news articles. While PEGASUS was fine-tuned for this specific task, BART was used without fine-tuning. The evaluation is based on ROUGE and Average Precision metrics to assess the quality and relevance of the generated summaries.

---

## **Introduction**

Text summarization is a critical task in natural language processing (NLP) that involves generating concise and coherent summaries from lengthy text. This project focuses on summarizing news articles using two state-of-the-art models:
- **PEGASUS**: Specifically designed for abstractive summarization tasks.
- **BART**: A versatile model capable of handling both generative and discriminative tasks.

The aim is to compare their performance and provide insights into their summarization abilities under different conditions.

---

## **Dataset Details**

### **Dataset Description**
The dataset comprises **112 rows** of news articles, each containing the following fields:
- **Sr. No**: Unique identifier for each record.
- **Newspaper Name**: Source of the news article.
- **Published Date**: The date the article was published.
- **URL**: Link to the original article.
- **Headline**: Title of the article.
- **Content**: Full content of the news article.
- **Human Summary**: Manually created summary of the article (used as a reference for evaluation).
- **Category**: Domain or topic of the article (e.g., Science and Technology, National News, Business, Environment, Health).

### **Dataset Link**
You can download the dataset [here](https://drive.google.com/file/d/1k3gjgRneahBi6umnVdErRWYv_-HMjIT7/view?usp=sharing) 

---

## **Methodology**

1. **Preprocessing**:  
   - Cleaned and tokenized the text data.  
   - Prepared the dataset for input to PEGASUS and BART models.  

2. **Model Training**:  
   - **PEGASUS**: Fine-tuned on the dataset to enhance summarization accuracy.  
   - **BART**: Used the pre-trained version without fine-tuning.  

3. **Evaluation Metrics**:  
   - **ROUGE (Recall-Oriented Understudy for Gisting Evaluation)**:  
     - ROUGE-1: Unigram overlap between generated and reference summaries.  
     - ROUGE-2: Bigram overlap between generated and reference summaries.  
     - ROUGE-L: Longest common subsequence overlap.  
   - **Average Precision**: Measures the relevance of generated summaries.

4. **Model Comparison**:  
   - Compared PEGASUS and BART based on the aforementioned metrics.

---

## **Results**

### **Evaluation Metrics**

**PEGASUS (Fine-Tuned):**  
- ROUGE-1: **0.4103**  
- ROUGE-2: **0.2144**  
- ROUGE-L: **0.3142**  
- Average Precision: **0.6169**

**BART (Pre-Trained):**  
- ROUGE-1: **0.4258**  
- ROUGE-2: **0.2063**  
- ROUGE-L: **0.3060**  
- Average Precision: **0.5170**

---

## **Conclusion**

- **BART**: Demonstrated robust summarization capabilities with slightly higher ROUGE-1 and ROUGE-L scores. Its ability to generate summaries without fine-tuning highlights the strength of its pre-trained architecture.  
- **PEGASUS**: Fine-tuning significantly improved its precision, as reflected in its higher ROUGE-2 and Average Precision scores, making it better at capturing relevant content. However, its overall performance was comparable to BART, emphasizing the importance of fine-tuning on larger, diverse datasets for further improvement.

---

## **Future Scope**

1. **Larger Dataset**: Extend the dataset with more diverse articles to enhance model generalization.  
2. **Additional Models**: Compare other state-of-the-art models like T5, GPT, and BERTSUM.  
3. **Hyperparameter Optimization**: Fine-tune the learning rate and batch size for further performance improvement.  
4. **Cross-Domain Summarization**: Apply these models to other domains, such as healthcare and research.  
5. **Real-Time Summarization**: Optimize models for faster inference to support real-time applications.  

---

## **Languages used** 

![python-logo-only](https://github.com/user-attachments/assets/a78aa447-fe92-4892-aaed-4dd6ea761795)

# 
📣 Feel free to have a look at all the files in this repository!🤗

❎ In case you find issues in any of my Repositories, you can Hit Me Up [here](https://github.com/issues)! 👈
