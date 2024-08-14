# HR Chatbot using ChatGPT, LangChain, Pinecone and Streamlit on Python Language

### Instructions
---
Backend file --> `hr_agent_backend_local.py`if not want to use Azure.  
Have not used any Azure components - the API is from platform.openai.com, and the CSV file is stored local computer

#### How to use this repo

1. Install python 3.10. 
2. Clone the repo to a local directory.
3. Navigate to the local directory and run this command in your terminal to install all prerequisite modules - `pip install -r requirements.txt`
4. Input your API keys in the `hr_agent_backend_local.py` file (or `hr_agent_backend_azure.py` if you want to use the azure version; you can uncomment it in the frontend.py file)
5. Run command `streamlit run hr_agent_frontent.py` in your terminal

#### Storing Embeddings in Pinecone

1. Create a Pinecone account in [pinecone.io](pinecone.io)
2. Run the Jupyter Notebook file --> 'store_embeddings_in_pinecone.ipynb', and replace the Pinecone and OpenAI API keys (for  the embedding model) with your own.


---
### Tech Stack
---

[Azure OpenAI Service](https://azure.microsoft.com/en-us/products/cognitive-services/openai-service) - the OpenAI service offering for Azure customers.  
[LangChain](https://python.langchain.com/docs/get_started/introduction.html) - development frame work for building apps around LLMs.    
[Pinecone](https://www.pinecone.io/) - the vector database for storing the embeddings.  
[Streamlit](https://streamlit.io/) - used for the front end. Lightweight framework for deploying python web apps.  
[Azure Data Lake](https://azure.microsoft.com/en-us/solutions/data-lake) - for landing the employee data csv files. Any other cloud storage should work just as well (blob, S3 etc).    
[Azure Data Factory](https://azure.microsoft.com/en-ca/products/data-factory/) - used to create the data pipeline.  
[SAP HCM](https://www.sap.com/sea/products/hcm/what-is-sap-hr.html) - the source system for employee data.   
