# Champion–Challenger Sentiment Analysis with Hugging Face and MLflow

The project compares two pretrained sentiment-classification models using Hugging Face Transformers and MLflow:

- Champion candidate: `distilbert-base-uncased-finetuned-sst-2-english`
- Challenger: `siebert/sentiment-roberta-large-english`

It evaluates accuracy, macro-F1, precision, recall and inference latency; applies a predefined model-selection rule; registers the models in MLflow; assigns champion/challenger aliases; and predicts on new input data.

## Project files

The project source and supporting files will be preserved from the original repository. Refer to the original README for the complete methodology, execution instructions, evaluation results and limitations.

## Run

Install dependencies:

```bash
pip install -r requirements.txt
```

Start the MLflow tracking server in one terminal:

```bash
python -m mlflow server --host 127.0.0.1 --port 5000 --backend-store-uri sqlite:///mlflow.db
```

In another terminal, run the project scripts from the project directory in the order documented in the original README.

## Note

Existing metrics, predictions and plots are results from the original author's run; they should not be interpreted as independently reproduced results from this repository.
