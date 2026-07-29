# 🧠 AI & Machine Learning Track 1: Master Plan

This repository tracks my journey through **Track 1 (AI & Machine Learning Foundations)** from the [Awesome AI Learning Guide by h9-tec](https://github.com/h9-tec/Awesome_ai_learning).

## 🎯 Learning Strategy: The Two-Step Execution Method
To avoid getting stuck on data formatting while learning new AI concepts, every stage follows a strict 2-step process:
* **Step 1 (Sandbox):** Complete the tutorial using the instructor's exact dataset (e.g., Titanic, MNIST digits) to master the algorithm cleanly.
* **Step 2 (Applied Real-World):** Immediately replicate the code in a new notebook, swapping the tutorial dataset for historical futures market data.

---

## 🟢 Stage 0: Foundations (Math, Python & Data Prep) (Weeks 1-3)
**Goal:** Master basic Python data manipulation, vectorization, linear algebra, and basic gradient intuition.

### 📚 Original Repository Resources
- [ ] **Course:** [Elements of AI (Univ. of Helsinki)](https://www.elementsofai.com/) - High-level conceptual foundation.
- [ ] **Interactive:** [Kaggle Learn](https://www.kaggle.com/learn) - Interactive tutorials on Python, Pandas, and data visualization.
- [ ] **Book:** *Mathematics for Machine Learning* (Deisenroth, Faisal, Ong) - Formal mathematical reference (Free PDF).

### 📺 Visual YouTube Alternatives (Step 1 Sandbox)
- [ ] **Math Visualized:** [3Blue1Brown - Essence of Linear Algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) (Vector spaces, matrix multiplication).
- [ ] **Data Visualized:** [Keith Galli - Pandas Complete Data Science Tutorial](https://www.youtube.com/watch?v=2uvysYbKdjM) (Data cleaning & transformation).
- [ ] **Stats Visualized:** [StatQuest - Statistics Fundamentals](https://www.youtube.com/playlist?list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9) (Mean, variance, probability distributions).

### ⚡ Step 2: Applied MNQ Project
* **Dataset:** Historical MNQ 1-minute futures data (2020 through July 2026).
* **Task:** Build a Python module using Pandas/NumPy to ingest raw 1-minute CSV data, filter strictly for the New York market session, align timestamps to the 09:30:00 AM EST/EDT open, and construct clean multi-timeframe feature sets (e.g., rolling ATR, volume spikes, session VWAP) without missing-value gaps.

---

## 🟡 Stage 1: Classical Machine Learning & Scikit-Learn (Weeks 4-8)
**Goal:** Understand supervised vs. unsupervised learning, train/test splits, decision trees, random forests, and gradient boosting.

### 📚 Original Repository Resources
- [ ] **Course:** [Andrew Ng Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction) (Coursera).
- [ ] **Practice:** Enter a beginner Kaggle competition (e.g., Titanic or House Prices) and submit a baseline model.

### 📺 Visual YouTube Alternatives (Step 1 Sandbox)
- [ ] **Lectures:** [Stanford CS229: Machine Learning (Andrew Ng)](https://www.youtube.com/playlist?list=PLoROMvodv4rMiGQp3WXShtMGgzqpfVfbU) - Full university lecture series.
- [ ] **Algorithms Visualized:** [StatQuest - Machine Learning Playlist](https://www.youtube.com/playlist?list=PLblh5JKOoLUICTaGLRoHQDuEAq44JND60) (Step-by-step decision trees, SVMs, Random Forests, XGBoost).
- [ ] **Coding Walkthrough:** [Daniel Bourke - Scikit-Learn in 6 Hours](https://www.youtube.com/watch?v=0B5eIE_1vpU) (End-to-end ML workflow).

### ⚡ Step 2: Applied MNQ Project
* **Objective:** Opening Range Breakout (ORB) Directional Classifier.
* **Task:** Using `scikit-learn` and `XGBoost`, train a binary classification model that takes the 09:30:00 AM EST reference price and opening candle metrics to predict breakout continuation probability.
* **Critical Constraint:** Implement `TimeSeriesSplit` for cross-validation to strictly eliminate look-ahead bias (ensuring future candles never leak into historical training splits).

---

## 🔴 Stage 2: Deep Learning & Frameworks (Weeks 9-12)
**Goal:** Build, train, and debug multi-layer neural networks, backpropagation, activation functions, and PyTorch tensors.

### 📚 Original Repository Resources *(Pick One Path)*
- [ ] **Path A (Top-Down):** [fast.ai Practical Deep Learning](https://course.fast.ai/) - Code first, deep theory second.
- [ ] **Path B (Bottom-Up):** Andrew Ng Deep Learning Specialization - Theory first, framework second.
- [ ] **Book:** *Neural Networks and Deep Learning* by Michael Nielsen.

### 📺 Visual YouTube Alternatives (Step 1 Sandbox)
- [ ] **Course Videos:** [Fast.ai 2022/2023 Full Course on YouTube](https://www.youtube.com/playlist?list=PLkVbIsAWN2ls1pYEEs0vEnP6Lh0d0Yd6v) (Practical PyTorch).
- [ ] **From Scratch:** [Andrej Karpathy - Building Micrograd](https://www.youtube.com/watch?v=VMj-3S1tku0) (Build backpropagation from pure Python).
- [ ] **PyTorch Deep Dive:** [Daniel Bourke - PyTorch for Deep Learning in 10 Hours](https://www.youtube.com/watch?v=V_xro1bcAuA) (Custom `nn.Module` and training loops).

### ⚡ Step 2: Applied MNQ Project
* **Objective:** Dynamic Stop-Loss & Re-entry Optimizer Network.
* **Task:** Build a custom PyTorch Multi-Layer Perceptron (MLP) or recurrent model (LSTM/GRU). Train the network on sequential price action candles to dynamically evaluate optimal stop-loss distances calculated specifically from newly formed setup candles during position re-entries.

---

## 🔥 Stage 3+: Transformers, LLMs & Advanced AI Systems (Post-Week 12)
**Goal:** Understand self-attention mechanisms, vector embeddings, vector databases, and Retrieval-Augmented Generation (RAG).

### 📚 Original Repository Resources
- [ ] **Course:** Andrej Karpathy's "Zero to Hero" Series.
- [ ] **Reference Book:** *Understanding Deep Learning* by Simon J.D. Prince.
- [ ] **Reading:** Anthropic's "Building Effective Agents" guide.

### 📺 Visual YouTube Alternatives (Step 1 Sandbox)
- [ ] **LLM Architecture:** [Andrej Karpathy - Let's build GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY) (Coding a Transformer step-by-step).
- [ ] **Attention Visualized:** [Umar Jamil - Attention Is All You Need Paper Walkthrough](https://www.youtube.com/watch?v=bCz4OMemCcA) (Visualizing matrix shapes and self-attention).
- [ ] **RAG Frameworks:** [James Briggs - LangChain & Vector Databases](https://www.youtube.com/playlist?list=PL8motc6AQTOcB1KGgG7z1E6NlV1_Q44Zl) (Connecting LLMs to local data).

### ⚡ Step 2: Applied MNQ Project
* **Objective:** Local Strategy & Journaling RAG Agent.
* **Task:** Build a local Python application using ChromaDB or Pinecone. Embed your C# strategy logic, NinjaTrader code snippets, trading parameters, and daily execution logs into a vector database to query your trading documentation in natural language.
