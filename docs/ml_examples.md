# Machine Learning Examples

Here is a summary of our results. Remark that from one seed to the other, results of the different notebooks may vary. Please look in the different notebooks for details.

| Model               | Dataset                                                   | Metric                            | Clear | Quantized | FHE    |
| ------------------- | --------------------------------------------------------- | --------------------------------- | ----- | --------- | ------ |
| Linear Regression   | Synthetic 1D                                              | R2                                | 0.876 | 0.863     | 0.863  |
| Logistic Regression | Synthetic 2D with 2 classes                               | accuracy                          | 0.90  | 0.875     | 0.875  |
| Poisson Regression  | [OpenML insurance (freq)](https://www.openml.org/d/41214) | mean Poisson deviance             | 0.61  | 0.60      | 0.60   |
| Gamma Regression    | [OpenML insurance (sev)](https://www.openml.org/d/41215)  | mean Gamma deviance               | 0.45  | 0.45      | 0.45   |
| Tweedie Regression  | [OpenML insurance (sev)](https://www.openml.org/d/41215)  | mean Tweedie deviance (power=1.9) | 33.42 | 34.18     | 34.18  |
| Decision Tree       | [OpenML spams](https://www.openml.org/d/44)               | precision score                   | 0.95  | 0.97      | 0.97\* |
| XGBoost             | [Diabetes](https://www.openml.org/d/37)                   | MCC                               | 0.48  | 0.52      | 0.52\* |

In this table, * means that accuracy in FHE is assumed to be the same than the one in quantized, by just checking that 10 samples behave the same way between FHE and quantized (because things are too slow to be exhaustively launched on the full dataset).

## **Concrete-ML** models

- [LinearRegression.ipynb](https://github.com/zama-ai/concrete-ml-internal/tree/main/docs/advanced_examples/LinearRegression.ipynb)
- [LogisticRegression.ipynb](https://github.com/zama-ai/concrete-ml-internal/tree/main/docs/advanced_examples/LogisticRegression.ipynb)
- [PoissonRegression.ipynb](https://github.com/zama-ai/concrete-ml-internal/tree/main/docs/advanced_examples/PoissonRegression.ipynb)
- [DecisionTreeClassifier.ipynb](https://github.com/zama-ai/concrete-ml-internal/tree/main/docs/advanced_examples/DecisionTreeClassifier.ipynb)
- [XGBClassifier.ipynb](https://github.com/zama-ai/concrete-ml-internal/tree/main/docs/advanced_examples/XGBClassifier.ipynb)
- [GLMComparison.ipynb](https://github.com/zama-ai/concrete-ml-internal/tree/main/docs/advanced_examples/GLMComparison.ipynb)

## Comparison of classifiers

- [ClassifierComparison.ipynb](https://github.com/zama-ai/concrete-ml-internal/tree/main/docs/advanced_examples/ClassifierComparison.ipynb)

## Kaggle competition

- [KaggleTitanic.ipynb](https://github.com/zama-ai/concrete-ml-internal/tree/main/docs/advanced_examples/KaggleTitanic.ipynb)