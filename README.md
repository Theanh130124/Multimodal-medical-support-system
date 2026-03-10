# Multimodal-medical-support-system
AI-powered multimodal medical support chatbot that combines RAG and computer vision for common disease assistance and X-ray image analysis.

**Developed by: TRAN THE ANH**


# Training ViT_MAE_xrays link
https://colab.research.google.com/gist/Theanh130124/586c5199b8fc677133fbfe0aa54830a3/vit_mae_xrays.ipynb

## 1. PROJECT INTRODUCTION
### 1.1 Overview and Context
This study presents the development of an intelligent medical support chatbot designed to assist users with common illnesses. The system integrates Retrieval-Augmented Generation (RAG) to enhance response generation by combining large language models with an external medical knowledge base, enabling accurate and context-aware medical guidance. In addition, the system incorporates computer vision for X-ray image analysis using the Vision Transformer (ViT) with a Masked Autoencoder (MAE) framework for improved feature extraction and classification performance. To improve efficiency, a prompt-caching technique is applied to reduce response time and computational costs. Experimental results show that the proposed system achieves an accuracy of up to 90%.


### 1.2 Requirements and Goals

Given this reality, the project demands a technological solution to help people access accurate and safe medical information.

The specific requirement is to develop an Artificial Intelligence (AI) application capable of:

1.  Image recognition of the X-RAYS
2.  Symptom analysis described by the user.
3.  Providing reliable preliminary advice.



## 2. TECHNOLOGY STACK

The chatbot system leverages several advanced technologies:

| Technology                               | Role in the System                                                                                                                                                                                    |
| :--------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Flask**                                | Serves as the web framework for deploying the application and handling communication between users and the AI modules.                                                                                |
| **RAG (Retrieval-Augmented Generation)** | Integrated with LangChain to enhance Natural Language Processing (NLP) by retrieving relevant medical knowledge and generating accurate, context-aware responses.                                     |
| **ViT + MAE**                            | Used for chest X-ray image analysis. The MAE model performs self-supervised pretraining to learn robust image representations, while Vision Transformer (ViT) performs the final classification task. |
| **Redis**                                | Implements prompt caching to store previously processed prompts, reducing response time and computational costs during repeated queries.                                                              |
| **MySQL**                                | Stores user information and chat history, supporting system management and personalized interactions.                                                                                                 |
| **Qdrant**                               | Serves as the vector database for storing embeddings and enabling efficient semantic retrieval within the RAG pipeline.                                                                               |
| **Selenium**                             | Used to automatically collect medical knowledge data from reputable healthcare websites to build the knowledge base.                                                                                  |




