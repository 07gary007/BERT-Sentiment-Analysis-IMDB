# BERT Sentiment Analysis: Traditional vs. Deep Learning

## 🚀 Project Overview
This project performs an end-to-end sentiment analysis on the **IMDB 50K Movie Reviews dataset**. [cite_start]It focuses on comparing traditional machine learning baselines with state-of-the-art transformer models to find the optimal balance between performance and computational efficiency[cite: 281, 286].

## 📊 Key Results
| Model | Configuration | Accuracy | F1-Score |
| :--- | :--- | :--- | :--- |
| **BERT** | **Fine-tuned (5e-5 LR)** | **89.98%** | **0.9005** |
| SVM | RBF Kernel, C=10 | 88.92% | 0.8900 |
| Naive Bayes | Alpha=5.0 | 85.10% | 0.8511 |

[cite_start]*BERT achieved the highest accuracy, while SVM proved to be a highly efficient alternative for production environments[cite: 546, 608].*

## 🛠️ Tech Stack
- [cite_start]**Languages**: Python [cite: 411]
- [cite_start]**Libraries**: PyTorch, Hugging Face Transformers, Scikit-learn, Pandas [cite: 411, 412]
- **Deployment Idea**: Containerized using **Docker** for consistent environment reproduction.

## 🧠 Key Insights
- [cite_start]**Transfer Learning**: Fine-tuning BERT provided superior semantic understanding compared to training LSTMs from scratch[cite: 584, 586].
- [cite_start]**Efficiency**: SVM training took seconds compared to hours for BERT, offering a strategic trade-off for resource-constrained applications[cite: 592, 593].
