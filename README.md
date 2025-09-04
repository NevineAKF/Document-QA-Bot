📄 Document QA Bot (RAG Architecture)
🚀 Overview

This project is a document-based question-answering chatbot developed as part of the IBM AI Engineering Capstone.
It leverages LangChain and Gradio to implement a Retrieval-Augmented Generation (RAG) pipeline, enabling users to upload PDF files and receive source-grounded answers.

The system is designed to:

Minimize hallucinations by grounding answers in retrieved text.

Handle long documents through chunking and embedding.

Dynamically update with new documents.

⚙️ Tech Stack

Programming: Python

Frameworks & Libraries: LangChain, Gradio

Machine Learning: LLMs, Embeddings

Data Handling: ChromaDB for vector storage

Other Tools: PyTorch / TensorFlow (for ML support), HuggingFace models

🧩 Architecture (RAG Pipeline)

Document Loading – PDFs are uploaded and parsed.

Text Splitting – Documents are split into chunks for efficient retrieval.

Embedding Generation – Each chunk is embedded into a vector space.

Vector Store – Vector Store – Chunks are stored and indexed in ChromaDB.

Retriever + LLM – Relevant chunks are retrieved and passed to the LLM.

Answer Generation – The LLM generates a grounded answer with context.

User Interface – Gradio provides a simple and interactive web app.

📷 Demo 

<img width="1325" height="608" alt="QA_bot" src="https://github.com/user-attachments/assets/9206c1cd-6b1a-40d7-b374-eb9dff89f17f" />

🔧 Installation & Usage
# Clone the repository
git clone https://github.com/NevineAKF/Document-QA-Bot.git
cd Document-QA-Bot

# Create environment & install dependencies
pip install -r requirements.txt

# Run the app
python app.py


Then open the Gradio link in your browser to interact with the chatbot.

💡 Example Use Cases

Research assistants (summarizing and answering from papers).

Policy and legal document Q&A.

Knowledge management systems in enterprises.

Education and training content assistants.

📜 License

This project is open-sourced under the MIT License.
