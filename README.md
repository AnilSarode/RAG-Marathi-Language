## INTRODUCTION

This repository has been created to understand the basics of the RAG pipeline in LLM engineering using ***Marathi***, one of the INDIAN languages. 
Thanks to Ed Donner-https://github.com/ed-donner, LinkedIn profile-https://www.linkedin.com/in/eddonner/ for the great course LLM Engineering: Master AI, Large Language Models & Agents.
The code is taken from the fifth week of the same course and modified as per the requirement. 

## Installation
1. Please install all the prerequisite packages using the `requirements.txt` file.
2. Please install the following package to create the embeddings out of the text.
   
   `https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`

   OR

3. ```
   pip install sentence-transformers langchain

   ```
## Results:
From the `rag_test_0.ipynb`, you will learn about context-based learning as shown below.

<img width="1374" height="468" alt="image" src="https://github.com/user-attachments/assets/dce8e3ed-774b-4155-890a-a0c8d6eb8c5f" />

When the code does not find the context, it shows below result 
<img width="1408" height="206" alt="image" src="https://github.com/user-attachments/assets/b35ad123-4541-4e63-bb33-a0de9b61b7b8" />

And when the model `gpt-4o-mini` is involved, it gives the correct answer when the context is correct. 

<img width="1640" height="895" alt="Screenshot from 2025-07-13 20-36-46" src="https://github.com/user-attachments/assets/a529326c-1a4c-458f-9c04-41fcbdab1374" />

However, if the context is given differently, then interestingly, `gpt-4o-mini` will give the wrong answer or hallucinate, as shown below. 

<img width="1640" height="895" alt="Screenshot from 2025-07-13 20-38-11" src="https://github.com/user-attachments/assets/0318bbfc-ad91-4d5f-9cf9-1296a8cb4bef" />


The code from `rag_test_1.ipynb` to `rag_test_4.ipynb` explains the whole RAG pipeline developed with the help of LangChain. You can see that the advantage of the Vector Database is that the model 
works and gives the correct answer even after the context is varied. 

<img width="1408" height="227" alt="image" src="https://github.com/user-attachments/assets/9b9c1289-8550-4474-8ca3-5170179d80c2" />

### Vector Representation of Tokens. 
<img width="939" height="691" alt="image" src="https://github.com/user-attachments/assets/8c916368-5f58-49cc-8c69-ac07e8c94415" />

#### **NOTE: I am using the paid OpenAI API's to invoke the model `gpt-4o-mini`.** 

### More Results:
<img width="1626" height="881" alt="image" src="https://github.com/user-attachments/assets/05f363fc-31ed-4cc6-bd83-84c075263bd8" />

