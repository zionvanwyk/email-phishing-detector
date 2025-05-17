# COS 720: Email Phishing Detector

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![HuggingFace](https://img.shields.io/badge/%F0%9F%A4%97-HuggingFace-yellow)

A fine-tuned DistilBERT model for detecting phishing emails. This lightweight NLP model is optimised for real-time email filtering.

## Model Details

- **Model Name**: `zionia/email-phishing-detector`
- **Architecture**: DistilBERT-base-uncased (Sequence Classification)
- **Training Data**: [Phishing Email Dataset](https://huggingface.co/datasets/zionia/phishing-emails) 
- **Input**: Raw email text (English)
- **Output**: Binary classification (0 = Legitimate, 1 = Phishing)

## Performance

| Metric       | Value  |
|--------------|--------|
| Accuracy     | 99.5%  |
| Precision    | 99.5%  |
| Recall       | 99.4%  |
| F1-Score     | 99.5%  |

## Email Phishing Detector Interface

An interactive [HuggingFace space](https://huggingface.co/spaces/zionia/phishing-email-detector-project) has been created in which a user can paste in the text of some email and, after real-time analysis using the model, will return a label (Phishing or Legitimate) and confidence score. Other explainability features like highlighted suspicious email text are also available on this space.

## In This Repo:
- [**Data Uploading Script**](https://github.com/zionvanwyk/email-phishing-detector/blob/main/PhishingEmailDataHFUpload.ipynb): Uploads required Kaggle dataset csv file from Google Drive to HuggingFace.
- [**Model Fine-Tuning Script**](https://github.com/zionvanwyk/email-phishing-detector/blob/main/Phishing_Email_Model_Training%20(1).ipynb): Fine-tunes model on the uploaded dataset.
- [**Project Report**](https://github.com/zionvanwyk/email-phishing-detector/blob/main/COS_720_Project.pdf): Documentation for this project. 

