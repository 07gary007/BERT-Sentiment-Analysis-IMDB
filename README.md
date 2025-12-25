# BERT Sentiment Analysis: Traditional vs. Deep Learning

## 🚀 Project Overview
This project performs an end-to-end sentiment analysis on the **IMDB 50K Movie Reviews dataset**. It focuses on comparing traditional machine learning baselines with state-of-the-art transformer models to find the optimal balance between performance and computational efficiency.

## 📊 Key Results
| Model | Configuration | Accuracy | F1-Score |
| :--- | :--- | :--- | :--- |
| **BERT** | **Fine-tuned (5e-5 LR)** | **89.98%** | **0.9005** |
| SVM | RBF Kernel, C=10 | 88.92% | 0.8900 |
| Naive Bayes | Alpha=5.0 | 85.10% | 0.8511 |

*BERT achieved the highest accuracy, while SVM proved to be a highly efficient alternative for production environments.*

## 🛠️ Tech Stack
- **Languages**: Python 
- **Libraries**: PyTorch, Hugging Face Transformers, Scikit-learn, Pandas
- **Deployment Idea**: Containerized using **Docker** for consistent environment reproduction.

## 🧠 Key Insights
- **Transfer Learning**: Fine-tuning BERT provided superior semantic understanding compared to training LSTMs from scratch.
- **Efficiency**: SVM training took seconds compared to hours for BERT, offering a strategic trade-off for resource-constrained applications.
