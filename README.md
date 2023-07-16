# Chatbot-Langchain
Developed a Chatbot using the Langchain from which users can upload the document and make a conversation using OpenAI's GPT model.

Langchain is a framework mainly for creating web applications powered by Large Language Models. Through which we can connect it with external data sources or API's. The Large Language model used here is OpenAI's GPT 3.5 turbo. It has better language understanding capabilities than its predecessor. This enhancement enables the model to more effectively comprehend and generate responses that are relevant to the given context or query.

In this application, the chatbot can make conversations out of documents. Here we can upload documents, make conversations about the document, view chat history, and also have the option to delete it. The documents are split into chunks and stored in a Vector Database as embeddings. The embeddings are generated through the OpenAI embeddings module. Here DocArrayInMemorySearch is used. It is a document index provided by Docarray that stores documents in memory.

The LLM without memory cannot respond using knowledge of previous interactions. The memory allows a Large Language Model (LLM) to remember previous interactions with the user. In this, memory is handled outside of the model i.e., stored externally. So along with the query, the chat history is also sent as a context. The result is shown in the dashboard.
