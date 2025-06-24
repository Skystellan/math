Jordan标准型（Jordan Normal Form）是线性代数中矩阵的一种特殊形式，它将矩阵通过相似变换化为一个块对角矩阵，其中每个块称为 Jordan块。Jordan标准型在研究矩阵的性质（例如特征值、特征向量、幂次行为等）时非常有用。

定义：
对于一个 $n \times n$ 的矩阵 $\mathbf{A}$，如果存在一个可逆矩阵 $\mathbf{P}$，使得： $$ \mathbf{P}^{-1} \mathbf{A} \mathbf{P} = \mathbf{J}, $$ 其中 $\mathbf{J}$ 是一个块对角矩阵，形式如下： $$ \mathbf{J} = \begin{pmatrix} \mathbf{J}_1 & 0 & \cdots & 0 \ 0 & \mathbf{J}_2 & \cdots & 0 \ \vdots & \vdots & \ddots & \vdots \ 0 & 0 & \cdots & \mathbf{J}_k \end{pmatrix}, $$ 每个 $\mathbf{J}_i$ 是一个 Jordan块，则 $\mathbf{J}$ 称为矩阵 $\mathbf{A}$ 的 Jordan标准型。

Jordan块的结构：
一个 $m \times m$ 的 Jordan块 $\mathbf{J}_i$ 对应一个特征值 $\lambda$，形式为： $$ \mathbf{J}_i = \begin{pmatrix} \lambda & 1 & 0 & \cdots & 0 \ 0 & \lambda & 1 & \cdots & 0 \ 0 & 0 & \lambda & \cdots & 0 \ \vdots & \vdots & \vdots & \ddots & 1 \ 0 & 0 & 0 & \cdots & \lambda \end{pmatrix}. $$ Jordan块的对角线元素全是特征值 $\lambda$，超对角线元素全是 $1$，其余元素为 $0$。

性质：
特征值：

Jordan标准型的对角线上的元素是矩阵的特征值。
每个特征值的重数等于对应 Jordan块的大小之和。
几何重数与代数重数：

几何重数是对应特征值的线性无关特征向量的个数。
代数重数是对应特征值的 Jordan块大小之和。
相似性：

任意矩阵都可以通过相似变换化为 Jordan标准型。
相似矩阵具有相同的 Jordan标准型。
计算步骤：
求特征值：

解矩阵的特征方程 $\det(\mathbf{A} - \lambda \mathbf{I}) = 0$，得到所有特征值。
求特征向量与广义特征向量：

对每个特征值 $\lambda$，求解 $(\mathbf{A} - \lambda \mathbf{I})^k \mathbf{x} = 0$，其中 $k$ 是特征值的代数重数。
构造 Jordan块：

根据特征值的代数重数和几何重数，构造对应的 Jordan块。
相似变换：

找到矩阵 $\mathbf{P}$，使得 $\mathbf{P}^{-1} \mathbf{A} \mathbf{P} = \mathbf{J}$。
示例：
设矩阵 $\mathbf{A} = \begin{pmatrix} 5 & 4 & 2 \ 0 & 5 & 2 \ 0 & 0 & 5 \end{pmatrix}$。

特征值：

解 $\det(\mathbf{A} - \lambda \mathbf{I}) = 0$，得到特征值 $\lambda = 5$。
特征向量与广义特征向量：

$(\mathbf{A} - 5\mathbf{I}) = \begin{pmatrix} 0 & 4 & 2 \ 0 & 0 & 2 \ 0 & 0 & 0 \end{pmatrix}$。
计算特征向量和广义特征向量。
Jordan块：

构造 Jordan块 $\mathbf{J} = \begin{pmatrix} 5 & 1 & 0 \ 0 & 5 & 1 \ 0 & 0 & 5 \end{pmatrix}$。
应用：
Jordan标准型在以下领域非常有用：

矩阵幂的计算：

如果 $\mathbf{A}$ 的 Jordan标准型为 $\mathbf{J}$，则 $\mathbf{A}^n = \mathbf{P} \mathbf{J}^n \mathbf{P}^{-1}$。
微分方程：

用于线性微分方程组的解。
矩阵分解：

用于研究矩阵的结构和性质。
Jordan标准型是矩阵理论中的重要工具，能够简化许多复杂的计算和分析。