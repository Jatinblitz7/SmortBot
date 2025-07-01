# 🧠 SmortBot – AI-Powered News Question Answering

SmortBot is an intelligent news analytics tool that allows users to paste up to **3 article URLs** and ask natural language questions about the content. Powered by **LangChain**, **HuggingFace Transformers**, and **FAISS**, SmortBot processes news data into vector embeddings and answers questions using a lightweight LLM — all within an interactive **Gradio** UI.

---

## 🚀 Features

- 🔗 **Multi-URL Ingestion**: Process up to 3 article links at once with automatic content cleaning and chunking.
- 🧠 **Context-Aware QA**: Get answers strictly grounded in the given articles using retrieval-augmented generation (RAG).
- ⚡ **Efficient Embedding**: Texts are embedded using `all-MiniLM-L6-v2` and stored in FAISS for fast retrieval.
- 💬 **Interactive UI**: Clean, styled Gradio interface with status indicators and tabbed layout.
- 💾 **Local Caching**: Stores vector DB on disk for quick reloading without reprocessing.

---

## 🧪 Tech Stack

| Component        | Tool/Library                          |
|------------------|---------------------------------------|
| LLM              | LaMini-Flan-T5-783M (HuggingFace)     |
| Embedding Model  | all-MiniLM-L6-v2                      |
| Vector Store     | FAISS                                 |
| Text Splitter    | RecursiveCharacterTextSplitter        |
| UI Framework     | Gradio                                |
| Orchestration    | LangChain                             |

---

## 📸 UI Preview
The interface has two tabs:

- "Step 1: Load Article URLs" – Paste your news article links here and click Process Articles.

- "Step 2: Ask a Question" – Ask anything related to the articles and get an LLM-generated answer with sources.
