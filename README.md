# 统计学习导论

本仓库收录《统计学习导论》的课程作业和课堂练习。每份 Jupyter Notebook 包含数据说明、建模过程和运行结果。

| 作业 | 主题 |
| --- | --- |
| [作业 1](homework1_regression/hw1.ipynb) | 加州房价回归，比较线性模型、正则化方法和验证集表现 |
| [作业 2](homework2_discrete_choice/hw2.ipynb) | 离散选择模型，比较 Logit、Probit 和互补双对数，并完成多分类实验 |
| [作业 3](homework3_generative_bayes/hw3.ipynb) | 概率生成式分类，计算逐类后验并比较朴素贝叶斯、LDA、QDA 和 KNN |
| [课堂作业 1](classwork1_decision_tree/cw1.ipynb) | 鸢尾花决策树分类，展示混淆矩阵、树结构和特征重要性 |

## 运行

安装 Python 依赖后，在 JupyterLab 中打开对应的 Notebook，从上到下运行。外部数据放在相应作业的 `data/` 目录中，鸢尾花等小数据集由 scikit-learn 提供。

```bash
python -m pip install jupyterlab numpy pandas scipy "scikit-learn==1.7.2" matplotlib seaborn statsmodels threadpoolctl
python -m jupyterlab
```

作业 3 的交叉验证包含多次 KNN 距离搜索，运行时间取决于机器性能。也可以直接查看 Notebook 中保存的结果。

## 数据来源

- 作业 1 使用 [California Housing](https://scikit-learn.org/stable/datasets/real_world.html#california-housing-dataset)。
- 作业 2 使用 [UCI Bank Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing) 和 [scikit-learn 示例数据集](https://scikit-learn.org/stable/datasets/toy_dataset.html)。
- 作业 3 使用 Martyna Bator 的 [UCI Sensorless Drive Diagnosis](https://doi.org/10.24432/C5VP5F)。
- 课堂作业 1 使用 [Iris](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_iris.html)。
