# BERT vs. Traditional Models: A Comparative Study on Sentiment Analysis

## 🚀 Project Overview
This project evaluates the effectiveness of various machine learning architectures—ranging from traditional statistical models to state-of-the-art Transformers—on the **IMDB 50K Movie Reviews dataset**. 

The goal was to identify the optimal balance between **predictive accuracy** and **computational overhead**, providing a framework for selecting models in real-world production environments.

## 📊 Experimental Results
Through five rigorous trials, the models were evaluated using Accuracy, Precision, Recall, and F1-Score.

| Model | Configuration | Test Accuracy | F1-Score | Training Time |
| :--- | :--- | :--- | :--- | :--- |
| **BERT** | **Fine-tuned (Hugging Face)** | **89.98%** | **0.9005** | ~2 Hours (GPU) |
| SVM | RBF Kernel (C=10, Gamma=0.1) | 88.92% | 0.8900 | < 5 Minutes |
| LSTM | 256 Hidden Units + Dropout | 85.20% | 0.8509 | ~30 Minutes |
| Naive Bayes | TF-IDF (NGrams 1-2) | 85.10% | 0.8511 | < 1 Minute |



### 📈 Key Performance Insights
* **Transformer Superiority**: BERT achieved the highest accuracy (**89.98%**) due to its bidirectional context awareness, though it requires significant GPU resources.
* **The SVM "Sweet Spot"**: SVM achieved an impressive **88.92% accuracy**, only 1% lower than BERT, while being orders of magnitude faster to train and deploy.
* **Overfitting Control**: Implemented Early Stopping and Dropout (0.5) to stabilize the LSTM and BERT training processes.

## 🛠️ Tech Stack
* **Deep Learning**: PyTorch, Transformers (Hugging Face)
* **Machine Learning**: Scikit-learn (SVM, NB, KNN)
* **Data Processing**: Pandas, NumPy, NLTK
* **Infrastructure**: Google Colab (NVIDIA T4 GPU)

## 🧠 Strategic Decision Making
This research demonstrates that while **BERT** is ideal for high-precision needs, **SVM with TF-IDF** remains a highly competitive and cost-effective choice for low-latency, resource-constrained applications.
