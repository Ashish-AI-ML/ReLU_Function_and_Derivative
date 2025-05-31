# ReLU Function and Derivative 🔍

This repository explains the **ReLU (Rectified Linear Unit)** activation function used in deep learning, including its mathematical formulation, implementation in Python, and its significance during training and backpropagation.

---

## 📌 What is ReLU?

**ReLU** stands for **Rectified Linear Unit**. It is an activation function that introduces non-linearity into neural networks while being computationally efficient.

### ➕ Mathematical Definition

\[
\text{ReLU}(x) = \max(0, x)
\]

### 🧠 Intuition:
- If `x > 0`: returns `x`
- If `x <= 0`: returns `0`

---

## ⚙️ Derivative of ReLU

The derivative is essential during **backpropagation** to update weights.

\[
\frac{d}{dx} \text{ReLU}(x) = 
\begin{cases}
1 & \text{if } x > 0 \\
0 & \text{if } x \leq 0
\end{cases}
\]

### 🔥 Use in Training:
- Helps **prevent vanishing gradient**.
- May cause **"dying ReLU" problem**, where neurons output zero and never update (solved using variants like Leaky ReLU).

---

