This repository serves as a centralized collection of professional-grade NLP and Computer Vision pipelines, focusing on fine-tuning transformer models and deploying them using the Hugging Face ecosystem.

# Hugging Face Models Collection

A comprehensive set of Jupyter notebooks demonstrating end-to-end machine learning workflows, from data preprocessing and parameter-efficient fine-tuning (PEFT) to model explainability and deployment.

## 🚀 Key Projects & Notebooks

### 1. Fast DistilBERT Sentiment Analysis
* **Task**: Binary sentiment classification on a subset of the IMDb dataset.
* **Model**: `distilbert-base-uncased`.
* **Features**: Includes a gradient-based saliency pipeline to visualize word importance (explainability) and direct deployment to Hugging Face Spaces.

### 2. MobileNetV2 Image Classifier
* **Task**: Multi-class image classification using transfer learning.
* **Model**: `MobileNetV2` with a custom classifier head and data augmentation.
* **Deployment**: Features an automated script to create a Gradio-based Hugging Face Space, including `app.py` and `requirements.txt` generation.

### 3. PersonaChat Bot (LoRA)
* **Task**: Conversational AI fine-tuned on the PersonaChat augmented dataset.
* **Model**: `microsoft/DialoGPT-small`.
* **Optimization**: Utilizes Low-Rank Adaptation (LoRA) via the PEFT library for efficient training.

### 4. Abstractive Text Summarization
* **Task**: Sequence-to-sequence summarization of news articles.
* **Model**: `t5-small` fine-tuned on the CNN/DailyMail dataset.
* **Metrics**: Implements ROUGE score evaluation for research-grade performance tracking.

## 🛠️ Tech Stack
* **Frameworks**: PyTorch, TensorFlow, Keras.
* **Libraries**: `transformers`, `datasets`, `evaluate`, `peft`, `accelerate`, `captum`.
* **Deployment**: Hugging Face Hub, Spaces, and Gradio.

## 📖 How to Use
1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/Karna14314/Hugginface_models.git
    ```
2.  **Setup Credentials**: Ensure you have a Hugging Face "Write" token. Several notebooks allow you to use Colab Secrets (`HF_TOKEN`) or manual login.
3.  **Run in Colab**: Each notebook includes an "Open in Colab" badge for immediate execution.

## 📂 Repository Structure
* `Fine_tune_Sentiment_Model.ipynb`: NLP classification + Explainability.
* `MobileNetV2.ipynb`: Computer Vision + Gradio deployment.
* `PersonaChat.ipynb`: Dialogue modeling + PEFT/LoRA.
* `Text_Summarization_with_T5.ipynb`: Seq2Seq summarization.
