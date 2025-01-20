# Encoder-Decoder

## Project Overview 🎯📄✨
This project focuses on fine-tuning the **T5 model** to summarize news articles from the CNN/Daily Mail dataset. The goal is to generate concise summaries of articles. 🌟📰🤖

## Team Members 👩‍💻👩‍💻👩‍💻
- **Laiba Idrees** (SP22-BAI-022)
- **Aliza Yousaf** (SP22-BAI-006)
- **Hafsa Atiq** (SP22-BAI-016)
- **Fatima Zafar** (SP22-BAI-014)
- **Shugufta Zahra** (SP22-BAI-046)

## Technologies Used 💻🛠️📊
- Python
- TensorFlow (CPU)
- PyTorch
- Hugging Face Transformers
- Datasets Library
- Google Colab 🌐🖥️⚡

## Setup Instructions 🚀📥🔧

### Installation 🔄📦🖱️
Install required libraries:
```bash
!pip install tensorflow-cpu
!pip install transformers datasets torch
```

### Dataset 🗂️📈📥
The **CNN/Daily Mail** dataset (v3.0.0) is used and downloaded via the `datasets` library. 📚🌐✅

### Preprocessing 📝⚙️📊
Articles are tokenized with T5 tokenizer. Inputs are truncated to 256 tokens, and outputs (summaries) to 64 tokens. ✂️🔠🔍

### Model Training 🏋️‍♀️🤖🎓
- Base model: **T5-small**.
- Encoder layers frozen to reduce computation.
- Training: **1 epoch**, `2e-5` learning rate, batch size `4`. 🕒📉🔬
- Mixed precision (`fp16`) enabled for faster training. 🚀⚡

### Results 🏆📊✅
The fine-tuned model is saved as `t5_fine_tuned_model.zip`. 🎉📂🔗

### Inference 🤔🔍📜
Example articles are summarized by the model, demonstrating its capability to generalize. ✨📄🤖

## Running the Code 🖥️⚡✅
1. Install libraries.
2. Execute code in Python (e.g., Google Colab). 🚀👨‍💻
3. Test with the example or your own articles. 🗂️📝✅

### Example Output 🌟📰📋
#### Input Article:
```
ISLAMABAD, RAWALPINDI: At least 11 people were killed after a bus met an accident and overturned on the M-14 Motorway near Fateh Jang on Monday.
...
```

#### Generated Summary:
```
At least 11 killed and 22 injured in a bus accident on M-14 Motorway due to driver's negligence.
```

## Files in the Repository 📁📜💻
- `Assignment5.py`: Full code.
- `t5_fine_tuned_model.zip`: Fine-tuned model.
- `README.md`: This file. 🗂️📖✨

## Acknowledgments 🙏🌟📚
Thanks to **Ma'am Zobia Rehman** for her guidance. 🌟🤝✨



