# Introduction to Statistical Learning

This repository contains homework and in-class exercises for the Introduction to Statistical Learning course. Each Jupyter notebook describes the data, explains how the models are fitted and evaluated, and includes the saved outputs.

| Assignment | Topic |
| --- | --- |
| [Homework 1](homework1_regression/hw1.ipynb) | California housing price prediction with linear regression and regularization |
| [Homework 2](homework2_discrete_choice/hw2.ipynb) | Discrete choice models using logit, probit, and complementary log-log links, plus multiclass classification |
| [Homework 3](homework3_generative_bayes/hw3.ipynb) | Generative classification and class posterior calculations, with a comparison of naive Bayes, LDA, QDA, and k-nearest neighbors |
| [Classwork 1](classwork1_decision_tree/cw1.ipynb) | Iris classification with a decision tree, including a confusion matrix, tree diagram, and feature importance |

## Running the notebooks

Install the Python packages and launch JupyterLab from the repository root.

```bash
python -m pip install jupyterlab numpy pandas scipy "scikit-learn==1.7.2" matplotlib seaborn statsmodels threadpoolctl
python -m jupyterlab
```

Open a notebook and run its cells from top to bottom. The external datasets are included in each assignment's `data/` directory, and scikit-learn provides the smaller datasets such as Iris. You can also view the saved outputs directly. Homework 3 takes longer to run because cross-validation repeats the nearest-neighbor search.

## Data sources

- Homework 1 uses the [California Housing dataset](https://scikit-learn.org/stable/datasets/real_world.html#california-housing-dataset).
- Homework 2 uses [UCI Bank Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing) and [scikit-learn example datasets](https://scikit-learn.org/stable/datasets/toy_dataset.html).
- Homework 3 uses Martyna Bator's [UCI Sensorless Drive Diagnosis dataset](https://doi.org/10.24432/C5VP5F).
- Classwork 1 uses the [Iris dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_iris.html).
