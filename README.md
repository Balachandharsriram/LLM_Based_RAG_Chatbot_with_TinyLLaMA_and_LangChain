# 🤖 LLM-Based RAG Chatbot with TinyLLaMA and LangChain

This project demonstrates building a **Retrieval-Augmented Generation (RAG) chatbot** using a lightweight LLM (**TinyLLaMA**) along with **LangChain** for orchestrating retrieval and prompt injection. The chatbot can dynamically pull data from a document store or vector DB to provide context-aware, grounded responses.

---

## 🚀 Features

✅ Use TinyLLaMA for fast, resource-friendly language generation  
✅ Integrate with LangChain for RAG pipeline orchestration  
✅ Perform vector-based retrieval to fetch relevant chunks  
✅ Interactive Q&A demo via Jupyter Notebook

---

## 🛠️ Tech Stack

- Python 🐍
- Jupyter Notebook 📓
- Hugging Face Transformers 🤗
- TinyLLaMA (tiny language model)
- LangChain 🦜🔗
- FAISS / ChromaDB for embeddings store
- PyTorch

---

## 📂 Project Structure

```

📁 LLM\_RAG\_Chatbot
├── LLM\_Based\_RAG\_Chatbot\_with\_TinyLLaMA\_and\_LangChain.ipynb
└── README.md

````

---

## ✨ How It Works

1. **Embed documents:**  
   Use Sentence Transformers or similar to convert documents into dense vectors and store them in a vector database.

2. **User query:**  
   Accept a question from the user.

3. **Retrieve relevant chunks:**  
   Compute embedding of the query and find top-k similar documents.

4. **Generate answer:**  
   Use TinyLLaMA with LangChain’s `RetrievalQA` chain to combine retrieved context with the question, prompting the LLM to generate a grounded answer.

---

## 🚀 Getting Started

### Installation

```bash
git clone https://github.com/your-username/rag-chatbot.git
cd rag-chatbot

# Install required packages
pip install transformers langchain faiss-cpu sentence-transformers
````

(If you are using ChromaDB instead of FAISS: `pip install chromadb`)

---

### Running the Notebook

```bash
jupyter notebook LLM_Based_RAG_Chatbot_with_TinyLLaMA_and_LangChain.ipynb
```

---

## 🚀 Future Improvements

* Swap TinyLLaMA for larger models if resources allow
* Add Streamlit / Gradio interface for live chat
* Include summarization of long documents before indexing

---

## 💡 Acknowledgements

* [TinyLLaMA](https://huggingface.co/TinyLLaMA)
* [LangChain](https://github.com/langchain-ai/langchain)
* [FAISS](https://github.com/facebookresearch/faiss)
* [Hugging Face Transformers](https://huggingface.co/transformers/)
