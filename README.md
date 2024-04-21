# Wine Quality Analysis

## Introduction

The wine industry is experiencing significant growth due to the increasing popularity of social drinking. However, the current certification process, relying on human experts and physicochemical tests, is time-consuming and costly. The subjective nature of wine appreciation and variability in opinions among tasters further complicate the process. This project seeks to identify key indicators of wine quality by examining the relationship between human tasting preferences and physicochemical properties. The goal is to enhance and streamline the certification and quality assessment processes in the red wine market.

## Research Question

"How do different physicochemical properties, such as acidity, sulfur content, and alcohol, relate to the quality of wine?"

## Methods

In our group project, we undertook a comprehensive regression analysis on a cross-sectional dataset to explore the relationships between various properties and wine quality. We began with constructing a Linear Regression Model, which served as the foundation for predicting wine quality based on a range of predictor variables. To diagnose potential issues related to heteroscedasticity, we applied both the Breusch-Pagan Test and the White Test, with the former assessing constant variance in residuals and the latter investigating patterns involving squared and interaction terms. The RESET Test was utilized to evaluate the potential enhancement of our model by incorporating non-linear terms. In response to concerns related to varying residuals' variance, Robust Estimation techniques were collaboratively integrated.

### Results

#### Regression Analysis Results

```markdown
| term                  | estimate   | std.error  | statistic  | p.value     |
|-----------------------|------------|------------|------------|-------------|
| (Intercept)           | 21.9652084 | 21.1945750 | 1.0363599  | 0.3001921   |
| fixed.acidity         | 0.0249906  | 0.0259485  | 0.9630827  | 0.3356528   |
| volatile.acidity      | -1.0835903 | 0.1211013  | -8.9478019 | 0.0000000   |
| citric acid           | -0.1825639 | 0.1471762  | -1.2404449 | 0.2149942   |
| residual.sugar        | 0.0163313  | 0.0150021  | 1.0885992  | 0.2764960   |
| chlorides             | -1.8742252 | 0.4192832  | -4.4700697 | 0.0000084   |
| free sulfur dioxide   | 0.0043613  | 0.0021713  | 2.0086353  | 0.0447450   |
| total sulfur dioxide  | -0.0032646 | 0.0007287  | -4.4798298 | 0.0000080   |
| density               | -17.8811638| 21.6330999 | -0.8265650 | 0.4086079   |
| PH                    | -0.4136531 | 0.1915974  | -2.1589710 | 0.0310019   |
| sulphates             | 0.9163344  | 0.1143375  | 8.0142971  | 0.0000000   |
| alcohol               | 0.2761977  | 0.0264836  | 10.4290143 | 0.0000000   |
| R^2                   | 0.3605517  |            |            |             |

````

#### Heteroskedasticity Test Results

```markdown

| Test                | statistic | p_value |
|---------------------|-----------|---------|
| Breusch-Pagan Test  | 84.98902  | 0       |
| White Test (Full)   | 115.08705 | 0       |
| White Test (Special)| 115.08705 | 0       |

```

Certainly! Here's a markdown template for a README file that includes all the information together:

markdown

# Wine Quality Analysis

## Introduction

The wine industry is experiencing significant growth due to the increasing popularity of social drinking. However, the current certification process, relying on human experts and physicochemical tests, is time-consuming and costly. The subjective nature of wine appreciation and variability in opinions among tasters further complicate the process. This project seeks to identify key indicators of wine quality by examining the relationship between human tasting preferences and physicochemical properties. The goal is to enhance and streamline the certification and quality assessment processes in the red wine market.

## Research Question

"How do different physicochemical properties, such as acidity, sulfur content, and alcohol, relate to the quality of wine?"

## Methods

In our group project, we undertook a comprehensive regression analysis on a cross-sectional dataset to explore the relationships between various properties and wine quality. We began with constructing a Linear Regression Model, which served as the foundation for predicting wine quality based on a range of predictor variables. To diagnose potential issues related to heteroscedasticity, we applied both the Breusch-Pagan Test and the White Test, with the former assessing constant variance in residuals and the latter investigating patterns involving squared and interaction terms. The RESET Test was utilized to evaluate the potential enhancement of our model by incorporating non-linear terms. In response to concerns related to varying residuals' variance, Robust Estimation techniques were collaboratively integrated.

### Results

#### Regression Analysis Results

```markdown
| term                  | estimate   | std.error  | statistic  | p.value     |
|-----------------------|------------|------------|------------|-------------|
| (Intercept)           | 21.9652084 | 21.1945750 | 1.0363599  | 0.3001921   |
| fixed.acidity         | 0.0249906  | 0.0259485  | 0.9630827  | 0.3356528   |
| volatile.acidity      | -1.0835903 | 0.1211013  | -8.9478019 | 0.0000000   |
| citric acid           | -0.1825639 | 0.1471762  | -1.2404449 | 0.2149942   |
| residual.sugar        | 0.0163313  | 0.0150021  | 1.0885992  | 0.2764960   |
| chlorides             | -1.8742252 | 0.4192832  | -4.4700697 | 0.0000084   |
| free sulfur dioxide   | 0.0043613  | 0.0021713  | 2.0086353  | 0.0447450   |
| total sulfur dioxide  | -0.0032646 | 0.0007287  | -4.4798298 | 0.0000080   |
| density               | -17.8811638| 21.6330999 | -0.8265650 | 0.4086079   |
| PH                    | -0.4136531 | 0.1915974  | -2.1589710 | 0.0310019   |
| sulphates             | 0.9163344  | 0.1143375  | 8.0142971  | 0.0000000   |
| alcohol               | 0.2761977  | 0.0264836  | 10.4290143 | 0.0000000   |
| R^2                   | 0.3605517  |            |            |             |

```
Heteroskedasticity Test Results

```

| Test                | statistic | p_value |
|---------------------|-----------|---------|
| Breusch-Pagan Test  | 84.98902  | 0       |
| White Test (Full)   | 115.08705 | 0       |
| White Test (Special)| 115.08705 | 0       |

```

Robust Estimation Results

```
| Variable              | Model Coefficient | Robust Standard Errors | p-value    |
|-----------------------|-------------------|------------------------|------------|
| (Intercept)           | 21.9652084        | 24.7168339             | 0.3741783  |
| fixed acidity         | 0.0249906         | 0.0327063              | 0.4448135  |
| volatile acidity      | -1.0833903        | 0.1380015              | 0.0000000  |
| citric acid           | -0.1825639        | 0.1540859              | 0.2360890  |
| residual sugar        | 0.0163313         | 0.0195255              | 0.4029262  |
| chlorides             | -1.8742252        | 0.4897887              | 0.0001299  |
| free sulfur dioxide   | 0.0043613         | 0.0022685              | 0.0545361  |
| total sulfur dioxide  | -0.0032646        | 0.0007685              | 0.0000216  |
| density               | -17.8811638       | 25.2915763             | 0.4795660  |
| PH                    | -0.4136531        | 0.2153875              | 0.0547939  |
| sulphates             | 0.9163344         | 0.1367898              | 0.0000000  |
| alcohol               | 0.2761977         | 0.0292505              | 0.0000000  |


```

RESET Test and R-squared

```
| p-value    | r-squared   |
|------------|-------------|
| 0.0001189  | 0.3671343   |
```

Conclusion

In conclusion, our findings highlight the importance of considering both linear and non-linear terms in modeling wine quality. The robust estimation techniques addressed heteroskedasticity issues, enhancing the reliability of our results. Future research may explore additional factors or data sources to further refine our understanding of the complex interplay between physicochemical properties and wine quality in the evolving landscape of the wine industry.
