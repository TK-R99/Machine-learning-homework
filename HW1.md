# HW1 线性模型

### 1 线性回归 Linear Regression（50）

#### 1.1 输入数据集 （10）

data1.txt为回归数据集，每一行为一个样本，前两列为特征，最后一列为目标值。按照7:3的比率划分训练集和验证集。

#### 1.2 线性回归（20）

建立线性回归模型，分别使用正规方程和梯度下降法求得参数解。

- 正规方程

$$
w=(X^TX)^{-1}X^Ty
$$



- 梯度计算

$$
g=\frac{1}{m}\sum^m_{i=1}(h_\theta(x^{(i)})-y^{(i)})x_j^{(i)}
$$

#### 1.3 可视化（20）

- 使用梯度下降法时请可视化loss曲线
- 请可视化验证集上所求回归直线

### 2 逻辑回归 Logitstic Regression/Percetron（50）

#### 1.1 输入数据集（10）

data2.txt为分类数据集，每一行为一个样本，前两列为特征，最后一列为目标值。按照7:3的比率划分训练集和验证集。

#### 1.2 逻辑回归（20）

建立逻辑回归模型，分别使用梯度下降法求得参数解。可尝试使用L2正则化。

- 梯度计算

$$
g=\frac{1}{m}\sum^m_{i=1}(h_\theta(x^{(i)})-y^{(i)})x_j^{(i)}
$$

- 梯度计算（L2正则化）

$$
g_j=\frac{1}{m}\sum^m_{i=1}(h_\theta(x^{(i)})-y^{(i)})x_j^{(i)}+2*\lambda*\theta_j
$$

#### 1.3 可视化（20)

- 使用梯度下降法时请可视化loss曲线
- 请可视化验证集上所求分类直线

### 3 Bonus：分析 （10）

- 对比正规方程和梯度下降法，基于实验结果比较两者之间的优劣。
- 基于实验结果，对比没有正则化的情况和L2正则化的逻辑回归模型。
- 分析特征归一化和不做归一化对模型训练的影响。
