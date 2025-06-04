# RAG FAQ Chatbot (n8n + Pinecone + OpenAI)

## 📸 Workflow preview

![Workflow Preview](workflow-preview.png)

This project is a fully automated **Retrieval-Augmented Generation (RAG) Chatbot** built with **n8n**, **Pinecone**, and **OpenAI**.

The chatbot can analyze FAQ documents stored in **Google Drive**, automatically index them into a **vector database** (Pinecone), and answer user questions based on the most relevant document content.

---

## 🚀 Features

- Automatic document processing from Google Drive
- Recursive text splitting and embeddings generation
- Pinecone vector database for fast semantic search
- Real-time RAG pipeline: retrieve relevant context + generate response
- Integration with OpenAI LLM (GPT-4, GPT-3.5, Claude, Gemini, etc.)
- Example use case: FAQ Chatbot

---

## 🛠️ Tech Stack

- [n8n](https://n8n.io/)
- [Pinecone](https://www.pinecone.io/) (vector database)
- [OpenAI API](https://platform.openai.com/) (LLM + embeddings)
- Google Drive API (document source)
- (Optional) LangChain Agents (if used)

---

## ⚙️ How it works

1️⃣ New FAQ document added to Google Drive  
2️⃣ Workflow downloads document and splits text into chunks  
3️⃣ Generates embeddings and stores in Pinecone  
4️⃣ User asks a question (via chat or API)  
5️⃣ The pipeline retrieves relevant chunks from Pinecone  
6️⃣ OpenAI LLM generates an answer based on retrieved context  
7️⃣ Answer is returned to the user

---

## 💡 Use Cases

- Company FAQ chatbot
- HR policy chatbot
- Customer support chatbot
- Documentation assistant
- Internal knowledge base

---

## 🚀 How to run

1️⃣ Import `rag-faq-chatbot.json` into your n8n instance  
2️⃣ Configure credentials:
   - Google Drive API
   - Pinecone API
   - OpenAI API  
3️⃣ Set your Google Drive folder ID in the workflow  
4️⃣ Start the workflow → ready to use!


---

## 🙋 Author

**Alexandru Muscalu**  
[LinkedIn](https://www.linkedin.com/in/alexandru-muscalu-510635219/)  
