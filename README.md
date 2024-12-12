# CultureConnect Machine Learning

Focusing on the machine learning aspects of our project **CultureConnect**, an app designed to help users understand their emotions and discover suitable cafe recommendations based on their mood.



## 📊 Tasks

### **1. Data Collection:**
- Collect mood-related text data from various sources.
- Gather cafe information tailored to different emotional states.
- Compile a comprehensive dataset of emotional expressions and cafe environments.

### **2. Data Labeling:**
- Label the dataset with the following mood categories:
  - Sadness
  - Joy
  - Love
  - Anger
  - Fear
  - Surprise


### **3. Modeling:**
Build three distinct models:
- **Mood Detection Model:** Utilize the Bidirectional LSTM with Embedding Neural Network architecture for emotion classification.
- **Cafe Recommendation Model:** Implement content-based filtering using TensorFlow and cosine similarity.
- **Text Summarization:** Fine-tune the architecture to generate mood-based insights.


## 🔧 Model Architecture
- **Text Preprocessing:**
  - Text data is tokenized and padded for uniform input sequences.
  - Employed one-hot encoding for mood labels.

- **Mood Detection Model:**
  - Built using a sequential neural network architecture:
    - **Embedding Layer:** Maps words to dense vector representations.
    - **Bidirectional LSTM:** Captures both past and future dependencies in text.
    - **Global Max Pooling Layer:** Aggregates sequence information.
    - **Dense Layers:** Fully connected layers for classification.
  - Optimized using cross-entropy loss and Adam optimizer.

    ![Model Evaluation](assets/model-architecture.png) 

- **Cafe Recommendation System:**
  - Employs cosine similarity to match user moods with cafe data embeddings.
  - Determines recommendations based on user reviews and lighting levels of cafes.

    ![Model Evaluation](assets/Architecture.png) 

## 📃 Dataset
- **Mood Detection Training Data:** Labeled and weighted text data.
- **Cafe Recommendation Database:** Information on cafes, including names, locations, ratings, and emotional suitability.



## 🎨 Model Demo
Explore our model demonstrations:
- [Mood Detection Model and Cafe Recommendation System](https://mood-prediction-train.streamlit.app/)


---

## 🔢 Model Evaluation
Comprehensive analysis of model performance, including:
- Accuracy metrics.
![Model Evaluation](assets/training-validation.png)
- Confusion matrix.
![Model Evaluation](assets/confusion.png)
- Emotional classification confidence scores.
![Model Evaluation](assets/confidence.png)

---

## 📖 References
1. Vaswani, A., et al. (2017). *Attention Is All You Need.* NeurIPS Conference.
2. Devlin, J., et al. (2018). *BERT: Pre-training of Deep Bidirectional Transformers.* ACL Conference.
3. Raffel, C., et al. (2019). *Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer.* JMLR.
4. Radford, A., et al. (2018). *Improving Language Understanding by Generative Pre-Training.*
5. Liu, Y., et al. (2019). *RoBERTa: A Robustly Optimized BERT Pretraining Approach.*
6. Sanh, V., et al. (2020). *DistilBERT, a distilled version of BERT: smaller, faster, cheaper, and lighter.*
7. Houlsby, N., et al. (2019). *Parameter-Efficient Transfer Learning for NLP.*


[def]: assets/architecture.png