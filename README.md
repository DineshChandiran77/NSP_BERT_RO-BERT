Next Sentence Prediction using BERT and RoBERTa (Ensemble Approach)

This project demonstrates a Next Sentence Prediction (NSP) system using both BERT and RoBERTa models. It combines the predictions from both models to create a more robust, context-aware ensemble capable of determining whether a sentence logically follows another.

Key Features:

Fine-tuned BERT model on custom NSP data using WikiText-103

Integrated RoBERTa model (pretrained) for comparison and ensemble prediction

Ensemble logic (majority vote) to overcome limitations of individual models

Hard negative sampling to test deep contextual understanding (not just grammar fluency)

Interactive Gradio interface with prediction visualizations

Detailed metrics: Accuracy, Classification Report, Confusion Matrix


Technologies Used:

Python, PyTorch, Transformers (HuggingFace)

scikit-learn, seaborn, matplotlib

Gradio for interactive UI

WikiText-103 dataset


How It Works:

1. Generates sentence pairs (positive + hard negative) from WikiText.


2. Trains BERT for NSP with early stopping.


3. Uses both BERT and RoBERTa for prediction and compares their probability outputs.


4. Outputs a final YES/NO answer with bar chart visualizing each model’s confidence.



Use Cases:

Evaluating sentence continuity in dialogue systems

Improving coherence in summarization

Training contextual understanding in AI reading comprehension models
