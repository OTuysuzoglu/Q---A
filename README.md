Built Answering System with BERT Model	and Fine-Tuned the Model on My Data Set

Objective:

This project was established to build a Question Answering (QA) system using Hugging Face Transformers library with a BERT (Bidirectional Encoder Representation from Transformers) model. The BERT model was deployed on CoQA (Conversational Question Answering dataset released by Stanford) dataset. The model was then fine-tuned on the dataset to provide accurate and efficient answers to user questions.

Roles and Responsibilities:

•	Reviewing relevant literature and documentation for BERT model.

•	Supporting other collaborators on project.

•	Data set loading and data cleaning.

•	Building of question-answering functions, including:

    •	Tokenized contexts (text) and questions using Tokenizer provided by Hugging Face Transformers.
  
    •	Transformed text and questions into BERT’s required input format, including input IDs, attention masks, and token type IDs.
  
    •	Calculated the start and end points to reconstruct the answer.
  
•	Fine-tuned the BERT model with the following steps:

    •	Created a function to truncate and map the start and end tokens to the context.
  
    •	Set up optimizer function, learning rate schedule, and some training hyperparameters. 
  
    •	Converted the dataset to the tf.data.Dataset format.
  
    •	Configured the model with compile. 
    •	Created callback to push my model to Hub with PushToHubCallback.
  
    •	Fine-tuned the model with training dataset, validation dataset, proper number of epochs, and custom callback.
  
•	Evaluated the model and fine-tuned model performance.

Tools and Technologies: Python, Pandas, Transformers, Keras, TensorFlow, json, NumPy
