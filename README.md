# Amazon Product Review Sentiment Classifier using DistilBERT

Fine-tuned DistilBERT on 500,000 Amazon product reviews using Hugging Face Transformers and PyTorch for binary sentiment classification.

## Dataset

Amazon Polarity Dataset

- Training Samples: 500,000
- Test Samples: 20,000

## Model

- DistilBERT
- Binary Sequence Classification

## Training Configuration

- Epochs: 2
- Batch Size: 64
- Mixed Precision Training (FP16)
- GPU: NVIDIA A100-40GB

## Results

| Metric | Score |
|----------|-------|
| Accuracy | 94.955% |
| F1 Score | 94.967% |
| Validation Loss | 0.151 |

## Tech Stack

- Python
- PyTorch
- Hugging Face Transformers
- Scikit-learn

## Hardware Used

NVIDIA A100-40GB GPU

## Repository Structure

```text
amazon-product-review-sentiment-classifier/
│
├── notebook.ipynb
├── README.md
├── requirements.txt
├── images/
└── amazon_sentiment_model/
```

## Sample Predictions

| Review | Prediction |
|----------|----------|
| This product is absolutely amazing! | Positive 😊 |
| Worst purchase I have ever made. | Negative 😞 |
| Quality exceeded my expectations. | Positive 😊 |
| Completely useless and broke after one day. | Negative 😞 |

## Future Improvements

- Deploy using Streamlit
- Publish model to Hugging Face Hub
- Experiment with RoBERTa and DeBERTa
- Train on 1M+ reviews
