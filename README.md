<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/51/IBM_logo.svg" alt="IBM Logo" width="200"/>
  
  <h1>🎓 AI-Powered Educational Admission Assistant</h1>
  <p>
    <strong>Retrieval-Augmented Generation (RAG) Based Intelligent Admission Support System</strong>
  </p>
  <p>
    <i>Developed as part of the IBM SkillsBuild Internship Project</i>
  </p>

  ![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)
  ![IBM watsonx](https://img.shields.io/badge/IBM-watsonx.ai-052FAD?logo=ibm)
  ![NVIDIA](https://img.shields.io/badge/NVIDIA-Embeddings-76B900?logo=nvidia)
  ![Langflow](https://img.shields.io/badge/Langflow-Workflow-FF4F00)
  ![ChromaDB](https://img.shields.io/badge/ChromaDB-Vector_DB-FF8000)
</div>

<hr />

## 🧑‍💻 Developer Profile

- **Name:** Gugulothu Bhavith
- **Institute:** JNTUH University College of Engineering Palair
- **Internship Duration:** 15 May 2026 – 15 June 2026
- **Domain:** Education
- **Email:** gugulothubhavith2005@gmail.com

---

## 📖 Overview

Educational institutions receive thousands of admission-related inquiries from prospective students, parents, and guardians. These queries typically involve eligibility criteria, fee structures, scholarship opportunities, and required documentation. Managing such requests manually results in delayed responses, inconsistent information delivery, and an immense administrative workload.

The **AI-Powered Educational Admission Assistant** solves this problem. It is a state-of-the-art **Retrieval-Augmented Generation (RAG)** system that understands natural language queries and retrieves accurate information directly from official admission documents, providing 24/7 intelligent, highly reliable support.

---

## 🏗️ Tech Stack & Technologies

- **Orchestration:** Langflow
- **LLM Engine:** IBM watsonx.ai (IBM Granite Foundation Models)
- **Embeddings:** NVIDIA Embeddings (BAAI BGE-M3)
- **Vector Database:** ChromaDB
- **Core Architecture:** Retrieval-Augmented Generation (RAG) & Agentic AI

---

## ⚙️ Architecture & Workflow

The system is built using an Agentic AI architecture designed to minimize hallucinations and ground responses entirely in official institutional knowledge.

### Workflow
1. **Ingestion**: Institutional documents (PDFs) are uploaded using the `Read File` component.
2. **Chunking**: Large documents are broken down into manageable chunks via `Split Text`.
3. **Embedding**: Chunks are converted into high-dimensional vector embeddings using `NVIDIA Embeddings`.
4. **Storage**: Vectorized data is stored in the `Chroma Vector Database` for fast semantic retrieval.
5. **Querying**: A student submits a question via `Chat Input`.
6. **Agentic Decision Making**: The `Tool Calling Agent` acts as an autonomous entity, deciding to query the vector database for relevant institutional knowledge.
7. **Generation**: The `IBM Granite Foundation Model` generates an accurate, context-aware response based *only* on the retrieved context.
8. **Output**: The response is presented to the user via `Chat Output`.

*Note: During development and testing, approximately **300,000 tokens** were successfully processed and utilized.*

---

## ✨ Novelty & Unique Features

- **Agentic AI Functionality:** The system employs a Tool Calling Agent that acts as an autonomous decision-making entity to select relevant retrieval tools dynamically.
- **Reduced Hallucinations:** Because answers are grounded strictly in the provided PDF knowledge base, the model avoids generating false or generic AI answers.
- **Enterprise-Grade AI:** Utilizes IBM's advanced Granite models for superior reasoning and natural language generation.
- **Education-Focused Design:** Specialized prompt templates and retrieval mechanisms tailor-made for institutional admission assistance.

---

## 📂 Repository Structure

```text
📁 IBM-Internship
│
├── 📄 app.json                 # Core Langflow configuration & workflow definition
├── 📄 IBM.pdf                  # Project documentation & problem statement
├── 📊 IBM-Internship.pptx      # Internship presentation and architectural blueprint
└── 📄 README.md                # Project documentation (You are here)
```

---

## 🚀 Getting Started

To run this Langflow pipeline locally:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/gugulothubhavith/AI-Educational-Admission-Assistant.git
   cd AI-Educational-Admission-Assistant
   ```
2. **Launch Langflow:**
   Ensure Langflow is installed (`pip install langflow`) and run `langflow run`.
3. **Import Workflow:**
   Navigate to the Langflow UI (usually `http://127.0.0.1:7860`), click **Import**, and upload the `app.json` file.
4. **Configure API Keys:**
   Insert your IBM watsonx.ai credentials and NVIDIA API keys into their respective nodes.
5. **Run & Chat:**
   Upload your institutional documents and interact with your new AI Admission Assistant!

---

## 🔮 Future Scope

The project has significant potential for future enhancements:
- **Voice-Based Assistant:** Adding speech-to-text and text-to-speech interaction capabilities.
- **Multilingual Support:** Expanding from English to include regional languages like Telugu and Hindi.
- **Omnichannel Integration:** Deploying the assistant on WhatsApp and as a dedicated Mobile App.
- **Career Guidance Module:** Implementing AI-based stream recommendations.
- **Online Admission Support:** End-to-end application form support and document verification.

---

<div align="center">
  <i>Developed with ❤️ during the IBM SkillsBuild Internship Program.</i>
</div>
