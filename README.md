# 🧠 AI & Machine Learning Foundations: Track 1

This repository tracks my progress through Track 1 of the Awesome AI Learning roadmap. The curriculum is optimized for visual learning, pairing core concepts with highly-rated video tutorials and practical Python execution.

---

## 🗺️ Learning Roadmap

### 1️⃣ Python & Data Engineering Foundations
Before building AI models, it is essential to comfortably manipulate datasets and write modular code.

* **Key Topics:** Object-Oriented Programming (OOP), vectorization with NumPy, data cleaning/transformation with Pandas, and data visualization.
* **Practical Milestone:** Clean a raw, messy dataset (e.g., a massive CSV of historical MNQ futures data spanning 2020 through July 2026), perform exploratory data analysis (EDA), and export a clean feature set using Pandas.

#### Video Resources & Task List
- [ ] **Corey Schafer:** [Python OOP Tutorials](https://www.youtube.com/playlist?list=PL-osiE80TeTsqhIuOqKhwlXsIBIdSeYtc) (Understand classes, methods, and clean modular code)
- [ ] **Keith Galli:** [Pandas Complete Tutorial](https://www.youtube.com/watch?v=vmEHCJofslg) (Real-world walkthrough of data analysis)
- [ ] **freeCodeCamp:** [NumPy Tutorial for Beginners](https://www.youtube.com/watch?v=QUT1VHiLmmI) (Visual breakdown of multi-dimensional array operations)

---

### 2️⃣ Mathematical Foundations for AI
Understanding the geometric intuition behind vectors, matrices, calculus gradients, and core statistics.

* **Key Topics:** Vectors, dot products, matrix multiplication, partial derivatives, gradient descent, mean/variance, probability distributions.
* **Practical Milestone:** Hand-calculate a 2D matrix multiplication and visualize cost reduction using gradient descent on a simple curve.

#### Video Resources & Task List
- [ ] **3Blue1Brown:** [Essence of Linear Algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) (Visual animations explaining matrix transformations)
- [ ] **3Blue1Brown:** [Essence of Calculus](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr) (Visual explanation of derivatives and gradients)
- [ ] **StatQuest:** [Statistics Fundamentals](https://www.youtube.com/playlist?list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9) (High-energy, visually intuitive explanations)

---

### 3️⃣ Classical Machine Learning & Scikit-Learn
Mastering standard machine learning algorithms before moving into neural networks. 

* **Key Topics:** Supervised vs. Unsupervised learning, Linear/Logistic Regression, Decision Trees, Random Forests, Gradient Boosting (XGBoost), Cross-Validation.
* **Practical Milestone:** Build an end-to-end classification model in `scikit-learn` using hyperparameter tuning (e.g., classifying directional bias relative to a specific reference line price at exactly 09:30:00 AM EST/EDT).

#### Video Resources & Task List
- [ ] **StatQuest:** [Machine Learning Playlist](https://www.youtube.com/playlist?list=PLblh5JKOoLUICTaGLRoHQDuEAq44JND60) (Step-by-step breakdown of algorithms with zero hand-waving)
- [ ] **Daniel Bourke:** [Scikit-Learn in 6 Hours](https://www.youtube.com/watch?v=0B5eIE_1vpU) (Hands-on, practical coding tutorial built around real datasets)

---

### 4️⃣ Deep Learning & Neural Network Fundamentals
Transitioning from classical ML into deep learning by building neural networks from scratch and utilizing PyTorch.

* **Key Topics:** Perceptrons, activation functions (ReLU, Sigmoid), forward passes, backpropagation, loss functions, PyTorch Tensors, `nn.Module`.
* **Practical Milestone:** Build, train, and evaluate a robust classification network utilizing custom training loops in PyTorch to ensure logical stop-loss or risk calculations trigger accurately on newly formed data.

#### Video Resources & Task List
- [ ] **Andrej Karpathy:** [Neural Networks: Zero to Hero (Micrograd)](https://www.youtube.com/watch?v=VMj-3S1tku0) (Building a backpropagation engine from absolute scratch in Python)
- [ ] **3Blue1Brown:** [But what is a Neural Network?](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) (Visual insight into how weights and biases operate)
- [ ] **Daniel Bourke:** [PyTorch for Deep Learning](https://www.youtube.com/watch?v=V_xro1bcAuA) (Full step-by-step visual and hands-on PyTorch coding course)

---

### 5️⃣ Transformers, LLMs & Practical AI Applications
Learning the architecture powering modern Generative AI and Large Language Models.

* **Key Topics:** Self-Attention Mechanism, Transformer Architecture, Tokenization, Vector Embeddings, Vector Databases, Retrieval-Augmented Generation (RAG).
* **Practical Milestone:** Build a local RAG application that queries external PDF documents using Python and a vector database.

#### Video Resources & Task List
- [ ] **Umar Jamil:** [Attention Is All You Need Explained](https://www.youtube.com/watch?v=bCz4OMemCcA) (Visual paper walkthrough mapping tensor shapes)
- [ ] **Andrej Karpathy:** [Let's build GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY) (Step-by-step coding tutorial to build a generative Transformer)
- [ ] **James Briggs:** [LangChain & Vector Databases](https://www.youtube.com/playlist?list=PL8motc6AQTOcB1KGgG7z1E6NlV1_Q44Zl) (Practical guides on building modern LLM pipelines)

---

## 🛠️ Repository Structure

To keep your code organized, maintain the following folder structure in this repository:

| Directory | Purpose |
| :--- | :--- |
| `/01_data_engineering` | Python scripts, Jupyter notebooks, and Pandas EDA files. |
| `/02_math_foundations` | NumPy array testing and manual gradient descent scripts. |
| `/03_classical_ml` | Scikit-Learn models, XGBoost scripts, and hyperparameter grids. |
| `/04_deep_learning` | PyTorch architectures and custom training loop files. |
| `/05_transformers` | RAG pipelines, API connection scripts, and LangChain tests. |

> **Note:** Add a `.gitignore` file to ensure you do not upload large raw datasets or virtual environment folders (`.venv`) to GitHub.
