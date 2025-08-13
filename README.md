Project: E-Commerce Chatbot

Tools & Technologies: Generative AI, Retrieval-Augmented Generation (RAG) using LLaMA 3.3 and GROQ, Python, Web Scraping, SQL

This project is a Proof of Concept (POC) for an intelligent, AI-powered chatbot designed specifically for an e-commerce platform. Its primary goal is to enable seamless, human-like interactions with customers by accurately identifying the intent behind their queries and providing real-time, context-aware responses.

By integrating Generative AI with RAG architecture, the chatbot combines natural language understanding with up-to-date data retrieval from the platform’s database. This ensures responses are not only accurate but also relevant to current inventory, prices, and policies.

Core Capabilities:
* Intent Recognition: Classifies user queries into specific intents for accurate handling.
* Real-Time Database Access: Fetches live product data, stock availability, and pricing.

Current Supported Intents:
* FAQ – Triggered for policy-related or general questions (e.g., Is online payment available?).
* SQL – Activated for product search and filtering requests (e.g., Show me all Nike shoes below Rs. 3000).


Folder Structure:
resources/ – Contains all chatbot application code, including intent classification, RAG pipeline, and response generation.

web-scraping/ – Scripts for scraping product and policy data from the e-commerce website to keep the chatbot knowledge base updated.

This POC demonstrates the potential for scalable, automated customer service that reduces response times, improves customer engagement, and supports advanced features like personalized recommendations and contextual search.


product screenshot : 

<img width="1221" height="881" alt="product-ss" src="https://github.com/user-attachments/assets/fe79241b-77fb-47bd-9675-e7f16d6d0326" />




Architecture :
<img width="2320" height="856" alt="architecture-diagram" src="https://github.com/user-attachments/assets/ce1f7909-054f-44ab-be60-b6baaf6b18eb" />



### Set-up & Execution

1. Run the following command to install all dependencies. 

    ```bash
    pip install -r app/requirements.txt
    ```

1. Inside app folder, create a .env file with your GROQ credentials as follows:
    ```text
    GROQ_MODEL=<Add the model name, e.g. llama-3.3-70b-versatile>
    GROQ_API_KEY=<Add your groq api key here>
    ```

1. Run the streamlit app by running the following command.

    ```bash
    streamlit run app/main.py
    ```

