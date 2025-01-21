# Interpretable ML: Insights from World Happiness 2023
This notebook explores the **World Happiness Report 2023** dataset using interpretable machine learning models from the **imodels** library. The goal of the project is to predict happiness levels across countries and gain insights into the key factors influencing global happiness using transparent, interpretable models.

## Models Used:
1. **SkopeRulesClassifier** - A rule-based classifier that selects interpretable if-then decision rules for classification.
2. **BoostedRulesClassifier** - A boosting-based model that iteratively improves classification rules by reducing errors.
3. **GreedyTreeClassifier** - A decision tree classifier that builds interpretable trees by selecting the most informative features at each split.

## Key Features Identified:
- **GDP per capita**
- **Social Support**
- **Healthy Life Expectancy**

These features were found to have the highest predictive power in determining happiness categories.

## Methodology:
1. **Preprocessing**: Imputation of missing values, scaling of numeric features, and one-hot encoding of categorical features.
2. **Model Evaluation**: Models were evaluated using accuracy, precision, recall, and F1-score. Regularization techniques were applied to mitigate overfitting.
3. **Model Performance**: After regularization, all models achieved over 95% accuracy on the test set, with strong generalization to unseen data.

## Results:
The models provided interpretable rules and insights that could assist in policy-making and further research in global well-being. **BoostedRulesClassifier** and **GreedyTreeClassifier** initially showed signs of overfitting, but regularization techniques ensured robust generalization.

## Dataset:
The dataset used is the **World Happiness Report 2023**, available on [Kaggle](https://www.kaggle.com/datasets/ajaypalsinghlo/world-happiness-report-2023).

## References:
- imodels library: [GitHub Repository](https://github.com/csinva/imodels)
- SkopeRulesClassifier: [Documentation](https://csinva.io/imodels/rule_set/skope_rules.html#imodels.rule_set.skope_rules.SkopeRulesClassifier)
- BoostedRulesClassifier: [Documentation](https://csinva.io/imodels/rule_set/boosted_rules.html#imodels.rule_set.boosted_rules.BoostedRulesClassifier)
- GreedyTreeClassifier: [Documentation](https://csinva.io/imodels/tree/cart_wrapper.html#imodels.tree.cart_wrapper.GreedyTreeClassifier)
- Dataset: [World Happiness Report 2023](https://www.kaggle.com/datasets/ajaypalsinghlo/world-happiness-report-2023)
