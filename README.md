# Simple-RAG-Project

RAG: Retrieval-Augmented Generation

Welcome to the RAG (Retrieval-Augmented Generation) repository! This project explores and implements techniques for combining information retrieval with generative models to produce more accurate, context-aware, and up-to-date outputs.

METHODOLOGY:
In RAG projects , we want to use a system of retrieving to find the nearest answer to our question and then use a llm to present the answer in shapeof sentences. 

I used 2 kinds of RAG methods : closed-book method and open-book method .
The closed-book method refers to a setting where a language model answers questions using only the information stored within its pre-trained parameters-essentially, its "memory" from training data. In this approach, the model cannot access or retrieve any external documents or databases during inference.
The open-book method allows the model to access and retrieve relevant information from external sources, such as documents or databases, at inference time. In the context of RAG (Retrieval-Augmented Generation), this means the model first retrieves pertinent documents based on the user’s query and then generates an answer using both the retrieved context and its internal knowledge. This approach mimics real-world scenarios where referencing materials is permitted and is particularly useful for questions requiring up-to-date or domain-specific information that may not be present in the model’s original training data.

At first i tested thes 2 methods with a simple given document and then tested with a dataset of multiple text files . inside these text files there are texts extracted from wikipedia about astronomy of solar system planets. 

There is also a llm that is not supplied with the augmented data .

then couple of questions are asked from all these 3 models , their answers and also the real answers from the text are shown and then the answers are checked to see whether they're correct or not.

the without-RAG model is "google/flan-t5-large".
the closed-method llm  is  "deepset/roberta-base-squad2".
the open-method llm is "google/flan-t5-large" with its specific tokenizer and its embedder is 'all-MiniLM-L6-v2'.

you can use what other ones you like:)

HOW TO RUN THE CODE :
1.give file path of astronomy dataset to file path needed under create_file_content_dict function.
2.install every library that is needed but you dont have them locally.
3.run the code and see the outputs.

CONTACT :
For questions or suggestions, please open an issue or contact shimabeiranvand5@gmail.com.
Feel free to modify this template to better fit your project’s specifics!
