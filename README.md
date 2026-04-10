# Quantum Superposition Embeddings for Multi-Meaning Word Representation

## 📌 Overview

This project presents a **hybrid classical–quantum Natural Language Processing (NLP) model** designed to address the challenge of **polysemy** (words having multiple meanings depending on context).

Traditional word embedding models such as Word2Vec assign a **single static vector** to each word, which limits their ability to capture multiple meanings. This project introduces a novel approach using **quantum superposition** to encode multiple semantic meanings into a single representation.

---

## 🚀 Key Idea

We leverage concepts from **quantum computing**, particularly:

* Superposition
* Entanglement
* Variational Quantum Circuits (VQC)

This allows a word to exist in a **probabilistic combination of meanings**, rather than a fixed vector.

---

## 🧠 Architecture

The model follows a **multi-stage hybrid pipeline**:

### 1. Classical Embedding Layer

* Maps words to **128-dimensional dense vectors**
* Implemented using a sparse embedding layer

### 2. Compression Network

* A feed-forward neural network
* Reduces 128D embeddings → **6D vector** (for 6 qubits)
* Uses activation functions (GELU + tanh)

### 3. Quantum Layer (Core Component)

* 6-qubit **Variational Quantum Circuit (VQC)**
* Input features encoded as **rotation angles**
* Includes:

  * Pauli-Y rotations
  * Strongly entangling layers

### 4. Quantum Measurement

* Produces a **64-dimensional probability distribution (2⁶ states)**
* Represents the word’s semantic meaning in quantum space

### 5. Similarity & Prediction

* Uses cosine similarity between word representations
* Outputs probability of contextual relationship

---

## ⚙️ Training Methodology

* Model trained using:

  * **Skip-Gram with Negative Sampling (SGNS)**
  * Binary classification objective

* Key techniques:

  * Mikolov subsampling
  * Negative sampling (1:10 ratio)
  * AdamW optimizer
  * SparseAdam for embeddings
  * Gradient clipping
  * Cosine annealing scheduler

---

## 📊 Results

* Dataset: **AG News Dataset**
* Validation Accuracy: **90.66%**
* Demonstrated:

  * Strong semantic clustering
  * Effective handling of polysemy
  * Meaningful word relationships

---

## 💡 Why This Matters

* Overcomes limitations of classical embeddings
* Provides **multi-meaning representations** in a single vector
* Highly **parameter-efficient** compared to large transformer models
* Bridges **Quantum Machine Learning (QML)** and NLP

---

## 📈 Key Features

* Hybrid classical + quantum architecture
* End-to-end trainable model
* Efficient semantic encoding
* Scalable framework for future quantum hardware

---

## ⚠️ Limitations

* Uses quantum simulation (not real hardware)
* Limited to 6 qubits due to computational constraints
* Scaling requires actual quantum processors

---

## 🔮 Future Work

* Deployment on real quantum hardware
* Integration with transformer-based models
* Context-aware dynamic quantum embeddings
* Evaluation on more NLP tasks (NER, sentiment analysis, etc.)

---

## 👨‍💻 Team

* M. Sai Nishanth
* E. Sai Praneeth
* Desu Deepesh
* Shubhadeep Datta
* P. Preetham Reddy
* K. Sri Harshavardhan

---

## 🎓 Institution

School of Computer Science
VIT-AP University

---

## 🙏 Acknowledgement

We sincerely thank **Deepti Godavarthi ma’am** for her valuable guidance and continuous support throughout this project.

---

## 🏷️ Keywords

Quantum Computing, NLP, Word Embeddings, Quantum Machine Learning, Variational Quantum Circuits, Deep Learning

---

## 📬 Contact

For queries or collaboration, feel free to connect with the team.
