# Stock-Performance-Predictor

## Topic

Predicting the stock price trend by interpreting the seemlychaotic market data has always been an attractive topic toboth investors and researchers. When it comes to trading inthe Stock Market, there are many different approaches tofind the right stock. Many forms of analysis have emergedto detect which stock is worth the money. **Technical Analysis**, **Sentimental Analysis** and **Fundamental Analysis** — observing a company’s financials like their Balance Sheet or Cash Flow Statement to determine if the company has valuerelative to their current stock price.

## Problem Statement

Building a Machine Learning model for classifying stocks as **BUY**, **SELL** or **HOLD** based on the Fundamentals.

## Models Trained

1. **Logistic Regression** is a statistical model that in its basic form uses a logistic function
1. **Decision Tree** is a type of supervisedlearning algorithm where the data is continuously split ac-cording to a certain parameter.
1. **Random Forest** is an ensemble of decision trees.
1. **XGBoost** is a decision-tree-based ensem-ble Machine Learning algorithm that uses a gradient boostingframework.

## Which Works the Best ?

Tree based algorithms worked well in our case, especially Random Forest. The same can be found in `Final_notebook.ipynb`.

## Evaluation Metrics

We used `classification_report` which consists of precision, recall, f1-score and accurary to get an indepth undersanding of how the model performs on various classes. Following is a sample evaluation

```
                precision    recall  f1-score   support

           0       0.52      0.64      0.57      6803
           1       0.45      0.41      0.43      5152
           2       0.40      0.23      0.29      2752

    accuracy                           0.48     14707
   macro avg       0.46      0.43      0.43     14707
weighted avg       0.47      0.48      0.47     14707
```

where,
`Precision = TruePositives / (TruePositives + FalsePositives)`

`Recall = TruePositives / (TruePositives + FalseNegatives)`

`F1-Score = (2 * Precision * Recall) / (Precision + Recall)`

## Results

## References

1. A. S. G. P. . Kohli P.P.S., Zargar S., “Stock prediction using machinelearning algorithms. in: Malik h., srivastava s., sood y., ahmad a.(eds) applications of artificial intelligence techniques in engineering.”[Online]. Available: https://doi.org/10.1007/978-981-13-1819-138
1. B. Jeevan, E. Naresh, B. P. V. kumar, and P. Kambli, “Share priceprediction using machine learning technique,” pp. 1–4, 2018.
1. J. Lee, D. Jang, and S. Park, “Deep learning-based corporate performanceprediction model considering technical capability,”Sustainability, vol. 9,no. 6, 2017. [Online]. Available: https://www.mdpi.com/2071-1050/9/6/899
1. T. pandas development team, “pandas-dev/pandas: Pandas,” Feb. 2020.[Online]. Available: https://doi.org/10.5281/zenodo.3509134
1. C. R. Harris, K. J. Millman, S. J. van der Walt, R. Gommers, P. Virtanen,D. Cournapeau, E. Wieser, J. Taylor, S. Berg, N. J. Smith, R. Kern,M. Picus, S. Hoyer, M. H. van Kerkwijk, M. Brett, A. Haldane, J. F.del R’ıo, M. Wiebe, P. Peterson, P. G’erard-Marchant, K. Sheppard,T. Reddy, W. Weckesser, H. Abbasi, C. Gohlke, and T. E. Oliphant, “Arrayprogramming with NumPy,”Nature, vol. 585, no. 7825, pp. 357–362, Sep.2020. [Online]. Available: https://doi.org/10.1038/s41586-020-2649-2
1. M. L. Waskom, “seaborn: statistical data visualization,”Journal of OpenSource Software, vol. 6, no. 60, p. 3021, 2021. [Online]. Available:https://doi.org/10.21105/joss.03021
1. F. Pedregosa, G. Varoquaux, A. Gramfort, V. Michel, B. Thirion, O. Grisel,M. Blondel, P. Prettenhofer, R. Weiss, V. Dubourg, J. Vanderplas, A. Passos,D. Cournapeau, M. Brucher, M. Perrot, and E. Duchesnay, “Scikit-learn:Machine learning in Python,”Journal of Machine Learning Research,vol. 12, pp. 2825–2830, 2011.
1. M. Feurer, A. Klein, K. Eggensperger, J. Springenberg, M. Blum, andF. Hutter, “Efficient and robust automated machine learning,” inAdvancesin Neural Information Processing Systems 28, C. Cortes, N. D. Lawrence,D. D. Lee, M. Sugiyama, and R. Garnett, Eds.Curran Associates, Inc.,
