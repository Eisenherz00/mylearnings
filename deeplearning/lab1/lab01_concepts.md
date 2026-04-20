# Lab 1: Simple MLPs - Knowledge Points & Concepts (知识点总结)

## English
This lab focuses on understanding the fundamental capabilities and limitations of Multi-Layer Perceptrons (MLPs) using threshold activation functions to solve non-linear classification problems.

1. **Multi-Layer Perceptron (MLP)**: Understanding the basic architecture of neural networks, including input, hidden, and output layers.
2. **Limitations of Shallow Networks**: A neural network with a single hidden layer and a threshold activation function cannot perfectly separate certain complex, non-linearly separable regions (e.g., regions consisting of disjoint areas, similar to the XOR problem).
3. **Linear Decision Boundaries**: Neurons in the first hidden layer act as linear classifiers. Their weights and biases define linear decision boundaries (lines in a 2D space) that split the space into half-spaces.
4. **Logical "AND" Combinations**: Neurons in the second hidden layer can perform logical "AND" operations on the outputs of the first layer. This allows the network to intersect multiple half-spaces to form enclosed convex regions (such as triangles or polygons).
5. **Logical "OR" Combinations**: The output neuron can perform a logical "OR" operation on the outputs of the second hidden layer. This allows the network to combine disjoint regions into a single positive classification area.
6. **Threshold Activation Function**: Utilizing the threshold function ($\tau(x) = \mathbf{1}[x>0]$), which outputs 1 if the input is greater than 0 and 0 otherwise, to make hard classification decisions.
7. **Matrix Operations / Vectorization**: Grouping neuron weights and biases into weight matrices to compute the forward pass (layer outputs) efficiently via matrix multiplication.

---

## 中文 (Chinese)
本实验的重点是理解多层感知机（MLP）在解决非线性分类问题时的基本能力和局限性，特别是使用阈值激活函数的情况。

1. **多层感知机 (MLP)**：了解神经网络的基本计算和架构，包括输入层、隐藏层和输出层。
2. **浅层神经网络的局限性**：具有单隐藏层和阈值激活函数的神经网络无法完美分离某些复杂的、非线性可分的区域（例如，由不相交区域组成的图形，类似于经典的 XOR（异或）问题）。
3. **线性决策边界**：第一个隐藏层中的神经元充当线性分类器。它们的权重和偏置定义了二维空间中的线性决策边界（直线），将空间划分为不同的半空间。
4. **逻辑“与” (AND) 组合**：第二个隐藏层中的神经元可以对第一隐层的输出执行逻辑“与”操作。这使得神经网络能够将多个半空间相交组合，形成封闭的凸区域（例如三角形或多边形）。
5. **逻辑“或” (OR) 组合**：输出层神经元可以对第二隐藏层的输出执行逻辑“或”操作。这使得网络能够将多个不相交的局部区域组合成一个统一的正分类区域。
6. **阈值激活函数**：使用阶跃/阈值函数 ($\tau(x) = \mathbf{1}[x>0]$)，即如果输入大于 0 则输出 1，否则输出 0，以此来进行严格的二元分类决策。
7. **矩阵运算/向量化**：将各神经元的权重和偏置组合成权重矩阵，通过矩阵乘法高效地批量计算神经网络的前向传播过程（各层的输出）。
