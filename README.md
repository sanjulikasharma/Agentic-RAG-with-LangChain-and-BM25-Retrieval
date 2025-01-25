# Agentic-RAG with LangChain and BM25 Retrieval

This repository implements a **Retrieval-Augmented Generation (RAG)** system that answers user queries by retrieving relevant information from the Hugging Face Transformers documentation and generating accurate responses using a large language model (LLM).

## Key Features <a name="key-features"></a>

- **Retrieval-Augmented Generation (RAG):** Combines document retrieval with LLM-based generation for accurate and context-aware answers.
- **Transformers Documentation Knowledge Base:** Uses a curated dataset of Hugging Face Transformers documentation as the knowledge base.
- **BM25 Retrieval:** Implements BM25, a fast and efficient retrieval algorithm, to fetch relevant document chunks.
- **LLM-Powered Agent:** Utilizes `meta-llama/Llama-3.2-3B-Instruct` (via Hugging Face Inference API) for reasoning and response generation.
- **Modular and Extensible:** Designed to support alternative retrieval methods (e.g., semantic search) and LLMs.

## How It Works <a name="how-it-works"></a>

1. **Knowledge Base Preparation:**
   - Loads and processes the Hugging Face Transformers documentation dataset.
   - Splits documents into smaller chunks for efficient retrieval.

2. **Retrieval:** Uses BM25 to retrieve the most relevant document chunks based on the user's query.

3. **Generation:** Passes the retrieved information to the LLM to generate a coherent and accurate response.

4. **Agent Orchestration:** The `CodeAgent` manages the workflow, iteratively calling the retriever and LLM until a final answer is produced.

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Agentic-RAG-with-LangChain-and-BM25-Retrieval.git
   cd Agentic-RAG-with-LangChain-and-BM25-Retrieval

2. Set up your HuggingFace API Key:
   For this, you need to request access from "https://huggingface.co/meta-llama/Llama-3.2-3B-Instruct" and then need to create an API token with permissions set to "Read access to contents of all public gated repos you can access" and "Read access to contents of selected repos". Once you are done with it, you can just copy the token key and paste in the code. 

Your contributions are Welcome!
If you'd like to contribute, please follow these steps:
- Fork the repository.
- Create a new branch for your feature or bugfix.
- Commit your changes.
- Submit a pull request.
   
