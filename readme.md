# 🧠 Simple Neural Network from Scratch (NumPy)

This is just an implementation while I tried to code up a neural network in numpy from scratch without standard libraries to get the hang of it.

## 📌 Project Overview

- **Input Layer:** 784 features (28x28 grayscale image)
- **Hidden Layer:** 40 neurons with ReLU activation
- **Output Layer:** 10 classes with Softmax
- **Loss Function:** Cross-Entropy
- **Optimization:** Gradient Descent

This network is designed to classify handwritten digits, similar to the [MNIST dataset](http://yann.lecun.com/exdb/mnist/).

---

## Workflow:

1. **Initialization**: Random weights and biases
2. **Forward Propagation**:
   - `Z1 = W1·X + b1`
   - `A1 = ReLU(Z1)`
   - `Z2 = W2·A1 + b2`
   - `A2 = softmax(Z2)`
3. **Loss**: Cross-entropy with one-hot encoded labels
4. **Backward Propagation**: Compute gradients for weights and biases
5. **Parameter Update**: Apply gradients using learning rate

