## 逻辑回归
- 一种分类模型，常用于二分类
- Logistic分布：

&emsp;&emsp;分布函数:
$$F(x)=\frac{1}{1+e^{-\frac{x-\mu}{\sigma}}}$$
概率密度函数：
$$F(x)=\frac{e^{-\frac{x-\mu}{\sigma}}}{\sigma(1+e^{-\frac{x-\mu}{\sigma}})^{2}}$$
<div align=center><img width="500" height="160" src="https://github.com/ethan-sui/AI-algorithm-engineer-knowledge/blob/main/image/logistics01.png"/></div>

sigmoid函数就是logistics函数在 $\mu=0, \sigma=1 $的特殊情况
- 把线性回归的预测值转化为离散值(通过logistics函数)，所以是一种广义的线性回归
$$h_{\theta }(x)=g(\theta ^{T}x)$$
&emsp;&emsp;其中，$g(Z)=\frac{1}{1+e^{-Z}} ,\theta^{T}X=\theta_{0}+\theta_{1}x_{1}+\theta_{2}x_{2}$
- 优点：实施简单，非常高效(计算量小，存储占用低)，可以在大数据场景中用；可以使用在线的方式更新参数，不需要重新训练整个模型
- 缺点：因为本质上是一个分类器，所以处理不好特征之间相关的情况；特征空间很大时，性能不好；容易欠拟合，精度不高
