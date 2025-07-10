# 🎥 YouTube Video QnA System

This is a locally hosted AI application that lets users input a **YouTube video URL**, automatically fetches the **transcript**, and then allows the user to ask **questions based on that transcript**. Using semantic search and a local LLaMA 3.1–8B model, it generates precise and context-aware answers — entirely offline after fetching the transcript.

---

## 🔍 Features

- 🔗 Input any public YouTube video URL
- 🧠 Fetches and processes transcript using YouTube API
- 💬 Ask questions in natural language based on the video's content
- 🧠 Powered by **LLaMA 3.1 – 8B**, running locally via Ollama
- 🔍 Retrieves relevant context using **FAISS vector store**
- 🛡️ All AI processing is local — only transcript fetch uses internet

---

## 🧰 Tech Stack

| Component            | Tool / Library                                 |
|---------------------|------------------------------------------------|
| LLM Backend          | `llama3:8b` via Ollama                         |
| Transcript Fetching  | `youtube_transcript_api`                      |
| Text Chunking        | `RecursiveCharacterTextSplitter`              |
| Embedding Model      | `all-MiniLM-L6-v2` (HuggingFace)              |
| Vector Store         | FAISS                                          |
| Retrieval Logic      | LangChain’s `RetrievalQA`                     |
| Chat Interface       | Streamlit                                     |

## 📷 Screenshot
![YT Video QnA System]()
