# Web-Scraping RAG Pipeline (Astra DB, Groq & Hugging Face)

A Jupyter Notebook demonstrating a fully free-to-run Retrieval-Augmented Generation (RAG) pipeline. This project scrapes live web content, stores it in a cloud-native vector database, and queries it using high-speed LLM inference—all without running expensive models locally or paying for API credits.

## Features

* **100% Free Cloud Architecture:** Offloads embedding generation to the free **Hugging Face Inference API** and LLM responses to **Groq's** free tier.
* **Automated Web Ingestion:** Uses LangChain's `WebBaseLoader` and `BeautifulSoup` to scrape, parse, and clean articles directly from URLs.
* **Cloud Vector Database:** Integrates **DataStax Astra DB** (Cassandra) via `cassio` for highly scalable, remote vector storage.
* **Lightning-Fast Inference:** Powered by ChatGroq (`mixtral-8x7b-32768`) for incredibly fast and accurate conversational responses based on the scraped context.

## Tech Stack

* **Environment:** Jupyter Notebook
* **Framework:** LangChain
* **LLM:** Llama-3.1-8b-instant (via Groq API)
* **Embeddings:** Hugging Face Inference API (`all-MiniLM-L6-v2`)
* **Vector Database:** DataStax Astra DB (Cassandra)

## Prerequisites

Before running this notebook, ensure you have the following free accounts set up:

* Python 3.8 or higher
* A free [Groq API Key](https://console.groq.com/)
* A free [Hugging Face Access Token](https://huggingface.co/settings/tokens) (Read access is sufficient)
* A free [DataStax Astra DB Account](https://astra.datastax.com/) (You will need your Database ID and an Application Token)

## Installation & Setup

**1. Clone the repository**
```bash
git clone [https://github.com/rishabh148/RAGs-to-Riches.git](https://github.com/rishabh148/RAGs-to-Riches.git)
cd RAGs-to-Riches.git
