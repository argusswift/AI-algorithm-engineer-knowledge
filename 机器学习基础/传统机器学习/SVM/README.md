## SVM
- 寻找一个超平面，超平面与最近数据点之间的距离称为边距，可以将两个类分开的最佳超平面是具有最大边距的超平面
<div align=center><img width="500" height="400" src="https://github.com/ethan-sui/AI-algorithm-engineer-knowledge/blob/main/image/svm01.PNG"/></div>

- ==优点==：可以解决高维问题，即大型特征空间；解决小样本下机器学习问题；能够处理非线性特征的相互作用；泛化能力笔记强
- ==缺点==：当观测样本很多时，效率并不是很高；对非线性问题，没有通用解决方案，有时候很难找到一个合适的核函数；常规SVM只支持二分类；对缺失数据敏感
