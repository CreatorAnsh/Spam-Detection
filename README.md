Spam-Sleuth AI: Spam Detection LLM
This is a lightweight, end-to-end spam detection system that utilizes a fine-tuned Large Language Model (LLM). The project provides a complete machine learning pipeline, from data preprocessing and model fine-tuning to real-time inference. It is designed to classify incoming text as "spam" or "not spam" with high accuracy, serving as a practical example of applying modern Natural Language Processing (NLP) techniques to a real-world problem.

Features
Custom Fine-Tuning: The project demonstrates how to adapt a powerful, pre-trained LLM on a custom-labeled dataset to specialize in spam detection, achieving high performance for this specific task.

Text Preprocessing: A robust pipeline handles tokenization and normalization, which are crucial steps in preparing raw text data for a model to consume effectively.

Inference API: A simple and scalable REST API is included, allowing for real-time spam detection. This API can be integrated into other applications, such as a mail client or a messaging service.

Performance Metrics: The repository provides scripts to evaluate the model's effectiveness using key metrics like accuracy, precision, and recall, ensuring you can measure and track its performance.

Technologies
Python: The core programming language.

PyTorch / TensorFlow: Leading deep learning frameworks for model development.

Hugging Face Transformers: A key library for accessing and fine-tuning state-of-the-art pre-trained LLMs.

Flask / FastAPI: Used to build the lightweight and efficient REST API for model inference.

tiktoken: A fast tokenizer that is compatible with models like GPT, used for text tokenization.

Getting Started
Clone the repository to your local machine:

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

Install the required Python packages:

pip install -r requirements.txt

The model is trained on a custom dataset located in the data/ directory.

To run the API, execute python api.py and send a request to the /predict endpoint to get a prediction.
