# Data450-Project1

This project scrapes multiple BBC News RSS feeds using a lightweight AI-powered webscraper.

## Structure: 
The system pulls data from four BBC News RSS feeds: 
1. Health
2. Business
3. Technology
4. Science & Environment

Each feed provides structured XML entries containing publish date, headline, link, and descriptions. 

## Methodology:
1. The program uses RSS parsing to extract news items from each category. Each article is stored with the source, feed category, title, publishing date, link, and description.
2. A locally installed LLM (via Ollama) is used to analyze headlines in batches. For each headline, the model generates topic classification, sentiment analysis, and key terms.
