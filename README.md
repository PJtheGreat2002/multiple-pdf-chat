# 📚 Multiple PDF Chat using LangChain, FAISS & OpenAI

This project allows you to **chat with multiple PDF documents** by leveraging the power of **LangChain**, **FAISS** for vector similarity search, and **OpenAI's GPT** model for answering queries from your PDFs.

> 🔄 Adapted from [ask-multiple-pdfs by alejandro-ao](https://github.com/alejandro-ao/ask-multiple-pdfs)

---

## 🌟 Features

- 📄 Upload **multiple PDFs**
- 🧠 Ask natural language **questions**
- 🧾 Extracts and processes PDF content using **PyMuPDF**
- 🔍 Uses **FAISS** for fast vector-based similarity search
- 🧠 Generates accurate answers using **OpenAI's GPT models**
- 🖥️ Simple and clean **Streamlit UI**

---

## 🚀 How It Works

1. PDFs are uploaded through the UI.
2. Text is extracted and split into manageable chunks.
3. Each chunk is embedded using OpenAI Embeddings.
4. FAISS builds an in-memory vector index from these embeddings.
5. When a user asks a question:
   - The app uses the vector index to retrieve relevant chunks.
   - LangChain’s `RetrievalQA` chain uses GPT to generate an answer.
6. The answer is shown in a styled chat interface.

---

## 📦 Tech Stack

| Tool | Purpose |
|------|---------|
| 🐍 Python | Core Programming Language |
| 🧾 PyMuPDF | PDF Text Extraction |
| 🧠 OpenAI API | Embeddings + GPT for QA |
| 🔗 LangChain | Retrieval + Prompt Chaining |
| 📦 FAISS | Vector Similarity Search |
| 🌐 Streamlit | Web Frontend |

---

## 🛠️ Installation

### 🔁 1. Clone the Repository

```bash
git clone https://github.com/PJtheGreat2002/multiple-pdf-chat.git
cd multiple-pdf-chat

```
### 🔁 2. Set up a Virtual Environment

```bash
python -m venv .pdfs
source .pdfs/bin/activate  # Windows: .pdfs\Scripts\activate

```
### 📥 3. Install Dependencies
```bash
pip install -r requirements.txt
```

## 🔐 Setup Environment Variables
```bash
OPENAI_API_KEY=your_openai_api_key_here
```
## ▶️ Run the App
```bash
streamlit run app.py
```

📄 License
This project is open-source and available under the MIT License.

🙌 Acknowledgements
LangChain
FAISS
OpenAI
Streamlit
Original repo by @alejandro-ao

👨‍💻 Author
PJ (Pratham Jain)
[GitHub Profile](https://github.com/PJtheGreat2002)
