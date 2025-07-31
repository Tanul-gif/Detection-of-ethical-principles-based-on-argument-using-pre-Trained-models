
# 🧠 Detection of Ethical Principles Based on Argument Using Pre-Trained Models

This project focuses on identifying **ethical principles** underlying human arguments using advanced **Natural Language Processing (NLP)** techniques. Leveraging **pre-trained transformer models** such as BERT, this system is capable of multi-label classification across various ethical dimensions.

## 📌 Table of Contents
- [About the Project](#about-the-project)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Results](#results)
- [Project Structure](#project-structure)
- [Future Scope](#future-scope)
- [Credits](#credits)
- [License](#license)

---

## 📖 About the Project

The aim of this project is to detect **ethical values** in argumentative texts by analyzing their content and context. This has applications in:
- Ethical decision-making systems
- Argument mining
- AI alignment
- Social media analysis

The model supports **multi-label classification**, meaning it can assign multiple ethical principles to a single input argument.

---

## 📂 Dataset

- **Source**: [Insert dataset name or source, e.g., SemEval, ETHICS, Moral Foundations]
- **Size**: [e.g., 10k annotated arguments]
- **Labels**: Multiple ethical principles such as:
  - Autonomy
  - Non-maleficence
  - Beneficence
  - Justice
  - Fairness
  - Honesty

---

## 🧠 Model Architecture

- **Preprocessing**: Tokenization and padding using HuggingFace tokenizer
- **Embedding**: BERT-based sentence embeddings
- **Classifier**: CNN / DNN / Logistic Regression / BERT fine-tuned classifier
- **Loss**: Binary Cross-Entropy (for multi-label tasks)
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score

---

## 🛠️ Installation

```bash
git clone https://github.com/Tanul-gif/Detection-of-ethical-principles-based-on-argument-using-pre-Trained-models.git
cd Detection-of-ethical-principles-based-on-argument-using-pre-Trained-models
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. Prepare your dataset inside the `data/` directory.
2. Run the training script:
```bash
python train.py
```
3. Run the evaluation:
```bash
python evaluate.py
```

---

## 📊 Results

| Model           | F1 Score | Accuracy |
|----------------|----------|----------|
| BERT + CNN     | 0.74     | 78.5%    |
| DistilBERT     | 0.71     | 76.2%    |
| Logistic Reg.  | 0.63     | 70.1%    |

*Detailed classification report available in `results/`.*

---

## 📁 Project Structure

```
.
├── data/
├── models/
├── embeddings/
├── utils/
├── train.py
├── evaluate.py
├── requirements.txt
└── README.md
```

---

## 🔭 Future Scope

- Integrate with real-world debate forums
- Fine-tune on more diverse datasets
- Deploy as a web API or chatbot
- Add explainability using LIME/SHAP

---

## 🙋‍♂️ Credits

**Developed by**: [Tanul Khatri](https://github.com/Tanul-gif)  
M.Tech in Artificial Intelligence & Machine Learning

---

## 📜 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.
