# Class 17 – Fundamentals of Deep Learning

## 🧠 What is Deep Learning?
Deep Learning is a **subset of Machine Learning** that uses **neural networks with multiple layers** to learn complex patterns from data.

### Neural Networks
- Inspired by the **human brain**.  
- Made of **neurons (nodes)** connected by **weights**.  
- Learn by adjusting these weights using data.

### Why Use Deep Learning?
- Learns directly from **raw data**.  
- Automatically extracts **important features** (no manual feature engineering).  
- Widely used in:
  - **Image recognition**  
  - **Self-driving cars**  
  - **Speech recognition**  
  - **Natural Language Processing (NLP)**  

---

## ⚙️ Components of a Neural Network
1. **Input Layer** – Takes in raw data (features).  
2. **Hidden Layer(s)** – Applies weights + activation functions to process data.  
3. **Output Layer** – Produces predictions (e.g., classification label `0` or `1`).  

---

## 🔄 Backpropagation (Backward Pass)
The process of updating weights to minimize error.

1. **Receive Error** from the next layer.  
2. **Calculate Gradient** (example with ReLU activation):  
gradient = 1 if output > 0 else 0
3. **Update Weights** using Gradient Descent:  
new_weight = old_weight + (learning_rate × input × error_gradient)



---

## 📉 Gradient Descent
An optimization algorithm used to minimize the **loss (error)**.  

- **Initial Weight** → Current position.  
- **Derivative of Cost Function** → Direction of slope.  
- **Learning Step (α)** → How much to move each iteration.  
- **Convergence Point** → Minimum cost (best weights).  

---

## 🔁 Training Cycle of a Neural Network
1. **Input Features** → Forward pass → **Prediction**  
2. Compare with **Labels (Ground Truth)**  
3. Calculate **Loss**  
4. Perform **Backpropagation** (adjust weights)  
5. Repeat for multiple **epochs** until loss converges  

---

## 🧮 Example: Weight Shapes
If input layer has **3 neurons** and hidden layer has **4 neurons**:  

- Weight Matrix Shape: **(3, 4)**  
- Input Shape: **(1, 3)**  
- Output Shape: **(1, 4)**  

### Example Weight Connections
- From Input Neuron 1 → Hidden Neurons 1–4 → `[w11, w12, w13, w14]`  
- From Input Neuron 2 → Hidden Neurons 1–4 → `[w21, w22, w23, w24]`  
- From Input Neuron 3 → Hidden Neurons 1–4 → `[w31, w32, w33, w34]`  

This means **each input neuron connects to all hidden neurons**, forming a fully connected layer.