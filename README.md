# Linear Regression with a Simple Neural Network

A Python implementation of a basic neural network designed to solve a linear regression problem. This project demonstrates the core concepts of machine learning, including **Feed Forward**, **Backpropagation**, and **Gradient Descent**, built from scratch without high-level ML frameworks like TensorFlow or PyTorch.

## 📌 Project Objective
The goal of this neural network is to learn the linear relationship:

$$y = 3x_1 + 4x_2$$

Given the inputs $x_1=3$ and $x_2=2$, the target output is **17**. The network starts with random weights and iteratively learns the correct weights ($w_1 \approx 3$, $w_2 \approx 4$) to minimize the error.

## ⚙️ Features
* **From Scratch:** Implements gradient descent logic manually using NumPy.
* **Activation Functions:** Includes definitions for Sigmoid, Tanh, and ReLU (for educational reference).
* **Visualization:** Uses Matplotlib to plot the Error progression and Prediction convergence over epochs.
* **Configurable:** Easy to adjust learning rates and epochs to observe different training behaviors.

## 🛠️ Technologies Used
* **Python 3.x**
* **NumPy** (for numerical operations)
* **Matplotlib** (for data visualization)

## 🚀 How to Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/linear-regression-neural-net.git](https://github.com/YOUR_USERNAME/linear-regression-neural-net.git)
    cd linear-regression-neural-net
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the script:**
    ```bash
    python main.py
    ```

## 📊 Methodology

The training process follows these steps:

1.  **Initialization:** Weights $w_1$ and $w_2$ are initialized randomly between 1 and 10.
2.  **Feed Forward:** The network predicts the output:  
    $y_{pred} = (x_1 \cdot w_1) + (x_2 \cdot w_2)$
3.  **Error Calculation:** Squared Error is computed:  
    $Error = (y_{actual} - y_{pred})^2$
4.  **Backpropagation:** Gradients are calculated to find the direction of steepest descent.
5.  **Weight Update:** Weights are adjusted using the **learning rate** ($\eta$):  
    $w_{new} = w_{old} - (\eta \cdot \text{gradient})$

## 📈 Sample Results
After training for 20 epochs, the network typically converges:

| Epoch | Predicted Value | Error |
| :--- | :--- | :--- |
| 1 | 36.50 | High |
| ... | ... | ... |
| 20 | 17.05 | ~0.002 |

*(Note: Exact values vary due to random weight initialization)*

## 🤝 Contributing
Feel free to fork this repository and submit pull requests. You can experiment by adding bias units, changing the learning rate, or implementing non-linear activation functions.