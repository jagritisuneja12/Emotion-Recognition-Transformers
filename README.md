# Emotion-Recognition-Transformers

# Emotion Recognition in Social Media Using Transformer-Based Architectures

## Project Overview
This project explores emotion classification from social media text using transformer-based models, specifically **RoBERTa** and **XLNet**. Social media platforms present unique challenges, such as context-dependent expressions and unstructured data. The key contributions of this project include:
- Fine-tuning RoBERTa and XLNet for emotion classification.
- Introducing **back-translation** as a data augmentation technique to improve generalization.
- Implementing an ensemble model to combine predictions and enhance accuracy.

The ensemble model achieved a test accuracy of **92.80%**, outperforming individual models.

---

## Methodology

### 1. Dataset
The project utilizes the **Hugging Face Emotion Dataset**, which includes six emotion labels:
- Sadness
- Joy
- Love
- Anger
- Fear
- Surprise

### 2. Models
- **RoBERTa**: A robustly optimized version of BERT, ideal for capturing context in long sequences.
- **XLNet**: A transformer model employing permutation-based training for bidirectional context learning.

### 3. Data Augmentation
- Back-translation was applied using MarianMT models to introduce paraphrased variations.

### 4. Ensemble Approach
An ensemble model was created by combining RoBERTa and XLNet predictions using a weighted average of their logits.

---

## Results
The ensemble model achieved the following performance metrics:
- **Accuracy**: 92.80%
- **Precision**: High across most emotions, with slight improvements in underrepresented classes.
- **F1-Score**: Competitive across all emotions.

For detailed performance, see the `Report.pdf` file in this repository.

---

## Limitations and Future Work
1. **Data Augmentation**: Exploring advanced techniques to enhance robustness.
2. **Ensemble Optimization**: Dynamic tuning of ensemble weights.
3. **Multilingual Texts**: Extending the approach to multilingual datasets.

---

## File Structure
- `code/`: Contains Python scripts for data preprocessing, model training, and evaluation.
- `report/`: Includes the detailed project report (`Report.pdf`).
- `README.md`: This file.

---




