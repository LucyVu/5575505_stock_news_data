# About this project

The goal of this project is to build a retrieval augmented generation (RAG) system, based on a large language model (LLM). The RAG system is built for financial domain, particularly related to Tesla and Elon Mush news. The system will combine both the generative/informational power of large language models, along with an ability to retrieve specialised information that would not be in the training data of the LLM (i.e. it will be able to generate content based on knowledge that was not publicly available at the point of training).

Broadly speaking, the approach will be incorporated the following steps:

1. Identify a relevant domain in which to work. This can range from a more general area, such as academic research in a specific topic, through to something more company specific, e.g. using company-specific data/information.

2. Source a dataset/knowledge-base to use in your RAG system. This should be a set of documents, and you can use a publicly available dataset (e.g. from Kaggle).

3. Determine a set of tests (e.g. queries) that the RAG system should be able to achieve if it is to perform as a working system (and out perform the LLM alone).

4. You will need to chunk and embed the knowledge-base (using a pretrained embedding model of your choice) and store it in a vector database.

5. Develop an appropriate prompt template to query the LLM.

6. Create a query pipeline that will process (embed) a query; retrieve relevant information from the vector database; present the query and additional information to the LLM as a prompt template; and return the generated content.

7. Test the system thoroughly and document any future improvements you would make.


# Results
This project successfully developed and evaluated a Retrieval-Augmented Generation (RAG) system tailored to financial news related to Tesla and Elon Musk. Through the integration of advanced embedding models, chunking techniques, and query refinement, the system consistently produced relevant and accurate responses, outperforming traditional models in handling complex financial queries. The combination of the sentence-transformers/all-mpnet-base-v2 model, sentence window chunking, and refine response mode emerged as the most accuracy and effective configuration. However, for shorter training time and sufficient performance, the combination of BAAI/beg-small-en-v1.5, semantic_chunking and refine response mode could be the optimal choice. 

Besides, the study also highlighted certain limitations, such as the system’s focus on a narrow dataset and the high computational costs involved. Future research should focus on expanding the dataset to include broader financial topics and improving computational efficiency to make the system more adaptable for real-time financial applications. By doing so, the system can be further refined and optimized for a wider array of financial news queries, offering significant potential for analysts, researchers, and investors seeking timely and accurate information.


# Achievment:
•	Earned the highest grade in the course (80/100) 

![image](https://github.com/user-attachments/assets/348018aa-104a-4e70-9926-128798a3fdd0)

• **Professor Feedback:** The project deals with a Financial News utilizing the dataset "2022 tesla & elon musk financial news" from Kaggle. The analysis displays depth and clarity and is comprehensive and insightful. The document is very appropriately structured. The code examples provided are very useful, well-chosen and exhaustive, covering all relevant aspects. Evaluation metrics are appropriately utilized, and the process is clearly explained.
