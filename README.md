# Arabic Name Generator

<p align="center">
  <img src="images/banner.png" width="900">
</p>

<p align="center">

Character-Level Arabic Name Generator built completely from scratch using an MLP Language Model inspired by Andrej Karpathy's **Neural Networks: Zero to Hero** series.

</p>

---

## Project Overview

This project trains a character-level neural network that learns the structure of Arabic names and generates entirely new names one character at a time.

Instead of predicting whole words, the model predicts the **next character** given the previous characters, allowing it to create realistic-looking Arabic names that never existed in the training dataset.

The goal of this repository is educational:

- Understand Language Models from first principles
- Implement everything manually
- Learn embeddings, MLPs, softmax, and autoregressive generation
- Avoid high-level deep learning libraries whenever possible

---

## Example

Input Context

```
عبد
```

Generated Names

```
عبدالرحيم
عبداللطيف
عبدالناصر
عبدالسلام
عبدالجليل
```

The model can also invent completely new names that resemble real Arabic names.

---

## Dataset

The dataset consists of Arabic first names.

Example:

```
محمد
أحمد
عبدالله
يوسف
خالد
سارة
فاطمة
ريم
ليان
```

---

## Model Architecture

```
Characters
      │
      ▼
Embedding Layer
      │
      ▼
Concatenate Context
      │
      ▼
Hidden Layer (MLP)
      │
      ▼
tanh
      │
      ▼
Linear Layer
      │
      ▼
Softmax
      │
      ▼
Next Character
```

---

## Learning Roadmap

- [x] Load dataset
- [x] Clean Arabic names
- [ ] Build vocabulary
- [ ] Encode characters
- [ ] Create training examples
- [ ] Build embedding table
- [ ] Implement MLP
- [ ] Train model
- [ ] Generate names
- [ ] Improve sampling

---

## Technologies

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Inspiration

This project is heavily inspired by

- Andrej Karpathy's **Neural Networks: Zero to Hero**
- makemore character-level language model

---

## Repository Status

🚧 Work in Progress

This repository is being built step by step while learning how language models work internally.

New commits will document every stage of development.

---

## Author

**Abdallah Aboudrari**

AI Engineering Student

GitHub:
https://github.com/aboudrari
