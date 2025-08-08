# Spam-Sleuth AI: Spam Detection with LLMs

Spam-Sleuth AI is a lightweight spam detection system built using a fine-tuned Large Language Model (LLM). It includes everything from data preprocessing and training to a REST API for real-time inference. The model classifies incoming text as either **spam** or **not spam**, and serves as a practical example of how to apply modern NLP techniques to a real-world problem.

---

## Features

- **Custom Fine-Tuning**  
  Fine-tune a pre-trained LLM on your own labeled dataset for accurate, task-specific spam detection.

- **Text Preprocessing Pipeline**  
  Includes tokenization and normalization to clean and prep text data before feeding it to the model.

- **Inference API**  
  A simple REST API (Flask or FastAPI) for real-time spam predictions. Easily pluggable into chat apps, mail clients, etc.

- **Evaluation Scripts**  
  Measure model performance using accuracy, precision, recall, and more. Good for tracking and comparisons.

---

## Tech Stack

- Python  
- PyTorch / TensorFlow  
- Hugging Face Transformers  
- tiktoken  
- Flask or FastAPI (your choice)

---

## Project Structure
```
spam-sleuth-ai/
├── app/
│   ├── __init__.py
│   ├── api.py                 # REST API (Flask or FastAPI)
│   └── inference.py           # Prediction logic using the trained model
│
├── data/
│   ├── raw/                   # Raw input data (e.g. before cleaning)
│   ├── processed/             # Cleaned/normalized data
│   └── spam_dataset.csv       # Final labeled dataset
│
├── models/
│   ├── checkpoints/           # Intermediate checkpoints (optional)
│   └── fine_tuned_model.pt    # Final trained model
│
├── scripts/
│   ├── train.py               # Fine-tune the LLM on your dataset
│   ├── evaluate.py            # Evaluate model performance
│   └── preprocess.py          # Data cleaning and tokenization
│
├── tests/
│   └── test_inference.py      # Basic unit tests for the API/model
│
├── notebooks/
│   └── exploration.ipynb      # Data exploration, EDA, or prototyping
│
├── requirements.txt           # Python dependencies
├── README.md                  # Project documentation
├── .gitignore                 # Ignore data/model/cache files
└── config.yaml                # Configuration for training/inference

```

### Clone the repo

```bash
git clone https://github.com/your-username/spam-sleuth-ai.git
cd spam-sleuth-ai
```
## Install dependencies
```
pip install -r requirements.txt
```
## Example API Usage
Send a POST request to /predict:
```
{
  "text": "You've won a free iPhone! Click here to claim."
}
```
## Response:
```
{
  "prediction": "spam"
}
```
### Contributing
If you find issues or have ideas to improve the project, feel free to open an issue or submit a PR.
```

---

Let me know if you'd like a `Dockerfile`, a sample `predict()` function in the API, or help wiring up the `/predict` endpoint with FastAPI or Flask.
```
