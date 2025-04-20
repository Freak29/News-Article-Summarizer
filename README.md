<div align="center">
  <h1><strong>News Article Summarizer
    (Mahakumbh Festival)</strong></h1>
</div>
This project automatically generates summaries of Indian news articles about the Mahakumbh by following three main steps:

## Task 1. Dataset Collection
- **Scraping:** Uses Selenium and BeautifulSoup to scrape articles from Indian Express.
- **Extraction & Storage:** Extracts titles, dates, and summaries, saving them as `mahakumbh_articles.csv`.

## Task 2. Dataset Annotation
- **Cleaning & Preparation:** Cleans the text and combines the title and summary.
- **Ground Truth:** Uses the original summary as the annotated summary.

## Task 3. Model Development & Summarization
- **Model:** Utilizes the pre-trained `T5-base` for abstractive summarization.
- **Processing & Training:** Tokenizes and splits the dataset; trains with Hugging Face’s `Seq2SeqTrainer`, logging loss and ROUGE scores.
- **Evaluation:** Tracks validation loss and ROUGE metrics to assess performance.
- **Generation:** Produces high-quality summaries and saves them in `outputT5_fixed.csv`.

### **Contributors & Work Distribution (IITP)**  

1. **Aditya Vilasrao Bhagat (2411AI27)** – Led dataset collection, including web scraping, storage, and initial processing. Also handled text cleaning and preparation.  
2. **Divyanshu Singh (2411AI41)** – Took charge of model development, implementing tokenization, dataset splitting, and training setup.  
3. **Vaibhav Shikhar Singh (2411AI48)** – Focused on model training, evaluation, and final performance assessment.  
