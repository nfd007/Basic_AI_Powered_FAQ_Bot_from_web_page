<img width="500" height="700" alt="chatbot" src="https://github.com/user-attachments/assets/a66d6276-06f9-45e6-9eeb-9954744c76c1" />

Basic AI-Powered FAQ Bot
Table of Contents

- Overview
- Features
- Installation
- Usage
- How it Works
- Customization
- Sample Output
- Architecture Diagram
- Workflow
- License

Overview
The Basic AI-Powered FAQ Bot is a simple chatbot that leverages AI to answer common questions automatically. Designed for educational and prototyping purposes, it matches user queries to FAQ entries using smart text matching.

General workflow of FAQ bots: user asks → AI finds answer → bot responds

Features

- Natural language question answering
- Fast, accurate FAQ retrieval
- Simple to update FAQ dataset
- Easy to extend with new features


Installation
Prerequisites
Python 3.7+, Jupyter Notebook, Packages: scikit-learn, numpy, pandas
Setup Steps
pip install scikit-learn numpy pandas
Install Jupyter (if needed)
pip install notebook
Installing Python and packages

Usage

1. Clone or download this repo
2. Open the notebook:
    jupyter notebook Basic_AI_Powered_FAQ_Bot.ipynb
3. Run cells step by step, following notebook prompts.
4. Ask questions in the interface provided and see answers.

Notebook Q&A session

How it Works
1. Load FAQ Data
The bot stores FAQs in a list (or you can load from a CSV).

faq_list = [
    {"question": "What is your name?", "answer": "I'm an AI FAQ bot."},
    {"question": "How do I use this bot?", "answer": "Type your question."},
]


FAQ database (concept)

2. Text Vectorization
The bot converts questions to numerical vectors using TF-IDF.
TF-IDF concept: Words mapped to numbers

3. Similarity Matching
When a user asks a question, the bot uses cosine similarity to match it to the closest FAQ.
Cosine similarity measures question similarity

4. Return the Answer
The bot returns the answer from the best-matching FAQ entry.
Bot responds with answer

Customization
To add or edit FAQs, just update faq_list:
faq_list.append({"question": "New Q?", "answer": "New A!"})
Customizing your FAQ data

Sample Output

User: How can I use this bot?
Bot: Type your question and I'll try to answer it.

Example chat between user and bot

Architecture Diagram
<img width="896" height="1452" alt="arch" src="https://github.com/user-attachments/assets/7279d6d7-bf5b-4827-8689-d9d8f052f690" />


