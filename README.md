# Emotion-detection-ML
This project aims to detect emotions from short text messages (e.g., tweets, captions, comments) using a BERT-based transformer model, with a focus on handling emojis and informal text.
emotion_detection_project/
│
├── data/ # Raw dataset (input)
│ └── Book1.xlsx
│
├── cleaned/ # Cleaned dataset (output of script)
│ └── cleaned_emotion_dataset.xlsx
│
├── scripts/ # Python scripts for cleaning and training
│ ├── 1_clean_data.py
│ └── 2_train_emojibert.py
│
├── models/ # Trained model directory
│ └── emoji_bert_model/
│
├── logs/ # Training logs
│ └── training_logs.txt
│
├── requirements.txt # Python dependencies
└── README.md # Project overview

## 💡 Project Goals

- Clean raw emotion-tagged textual data with emojis.
- Use BERT-like models to classify text into emotion categories.
- Support continual learning (future update).
- Save trained models for reuse and deployment.

## 📦 Requirements

Install required packages using:

```bash
pip install -r requirements.txt
if not there install
pip install pandas openpyxl transformers torch ftfy emoji scikit-learn
python scripts/1_clean_data.py
python scripts/2_train_emojibert.py

