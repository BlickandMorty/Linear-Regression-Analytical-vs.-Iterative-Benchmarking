# The Matrix Solver: Analytical Math vs. Gradient Descent

### 🧪 Project Overview
This project benchmarks the **Moore-Penrose Pseudo-inverse** (Direct Linear Algebra) against **Gradient Descent** (Iterative AI) for solving Linear Regression.

### 📊 Benchmark Results
| Method | Time (s) | Error (MSE) |
| :--- | :--- | :--- |
| **Pseudo-inverse (Exact)** | **0.46s** | **0.24775** |
| **Gradient Descent (AI)** | 5.13s | 0.24779 |

### 🧠 Core Insights

#### 📉 THE "N-CUBED" LIMIT (Scalability)
While the **Analytical Method** won this round, it has a "Wall."
* **Complexity:** $O(n^3)$
* **The Reality:** Inverting a matrix requires memory that grows cubically. If this dataset had **50,000+ features**, the Pseudo-inverse would crash the system. 
* **CRITICAL TAKEAWAY:** Gradient Descent ($O(n)$) is the necessary winner for "Big Data" because it scales linearly.

#### 📏 THE LINEARITY RULE (Complexity)
* **Direct Solution:** The Moore-Penrose Inverse "jumps" to the answer in one step. This only works for **Linear Problems**.
* **AI Necessity:** Deep Learning (like Computer Vision) creates non-linear landscapes. There is no "inverse button" for a Neural Network; you MUST use Gradient Descent to find the solution.

### 🛠️ Tech Stack
* **Python**
* **NumPy** (Linear Algebra)
* **Matplotlib** (Visualization)
