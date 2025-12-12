# research-RAG-chatbot
A Retrieval-Augmented Generation (RAG) based chatbot that reads, understands, and answers questions from research papers. This project extracts text from PDF research papers, embeds the content using Sentence Transformers, stores it in a FAISS vector database, and uses an LLM to generate accurate, context-aware answers.

# Project Overview  

This chatbot allows users to:  
	->Upload research papers (PDF format)  
	->Automatically extract and chunk the text  
	->Convert text chunks into embeddings  
	->Store embeddings in a FAISS vector index for fast retrieval  
	->Retrieve context relevant to user queries  
	->Generate answers using an LLM (Falcon-7B-Instruct or any HuggingFace model)  

The result is an AI assistant that can summarize papers, explain methods, highlight contributions, and answer technical questions.

# Tech Stack  

-Python  
-HuggingFace Transformers  
-Sentence Transformers (all-mpnet-base-v2)  
-LangChain  
-FAISS Vector Database  
-PyMuPDF (PDF text extraction)  
-Google Colab / Jupyter Notebook  

# Features  

-PDF research paper ingestion  
-Intelligent text chunking  
-Embedding generation using powerful transformer models  
-Vector similarity search using FAISS  
-Question-answering with an instruction-tuned LLM  
-End-to-end RAG pipeline that mirrors industry-grade GenAI applications

# Project Structure
research-rag-chatbot/  
│  
├── data/          	     # Research paper PDFs  
├── notebooks/      	      # Colab / Jupyter notebooks  
├── src/              	    # Python source code (optional)  
└── README.md           	  # Project documentation  

# How It Works  
1)Upload research paper PDFs  
2)Extract text using PyMuPDF  
3)Split text into manageable chunks  
4)Convert text into dense embeddings  
5)Store embeddings in a FAISS index  
6)On a user query:  
         -Retrieve top-k similar chunks  
         -Provide them to a large language model  
         -Generate an accurate, context-based response  

# Example Queries  
“Summarize the methodology in simple words.”  
“What problem does this paper solve?”  
“Explain the main contributions.”  
“What models are compared in this study?”  

# Use Cases  
-Students reading complex research papers  
-Researchers summarizing literature  
-AI enthusiasts learning how RAG works  
-Anyone working with long-form PDF content  

# Future Improvements  
-Build a web UI using Streamlit or Gradio  
-Add more LLM options  
-Support for multiple papers and multi-document search  
-Add metadata filtering and ranking  
