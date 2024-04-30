# Fast Food Marketing A/B Test

![image](https://github.com/jasondo-da/Fast_Food_Marketing_Campaign_AB_Test/assets/138195365/5dbb82c9-db2d-4b3b-99e6-4794a42ff113)

## Table of Contents

- [Project Introduction](#project-introduction)
    - [Fast Food Marketing A/B Test Jupyter Notebook](#fast-food-marketing-ab-test-jupyter-notebook)
    - [Fast Food Marketing Campaign A/B Test Dataset](#fast-food-marketing-campaign-ab-test-dataset)
- [Objective](#objective)
- [Analysis Outline](#analysis-outline)
- [Conclusion](#conclusion)

## Project Introduction

This is a Kaggle-sourced dataset used to refine my data analytics skills further and gain more data science experience. A quick growing fast-food chain is planning to add a new menu and is currently undecided between three possible marketing campaigns for their new product. To find the best marketing campaign for optimal sales growth, the new menu item is introduced to several locations in randomly selected markets. One of three marketing campaigns is randomly used at each location and the weekly total sales will be recorded for the first four weeks under the new campaign. To find the best marketing campaign we are going to conduct an A/B test to statistically find the optimal marketing campaign.

### Fast Food Marketing A/B Test Jupyter Notebook

All codes of Fast Food Marketing A/B Test in Jupyter Notebook

Link: [Fast Food Marketing A/B Test](https://github.com/jasondo-da/Fast_Food_Marketing_Campaign_AB_Test/blob/main/fast_food_ab_test.ipynb)

### Fast Food Marketing Campaign A/B Test Dataset

A fast-food chain plans to add a new item to its menu. However, they are still undecided between three possible marketing campaigns for promoting the new product. In order to determine which promotion has the greatest effect on sales, the new item is introduced at locations in several randomly selected markets. A different promotion is used at each location, and the weekly sales of the new item are recorded for the first four weeks.

Link: [Original Kaggle Dataset](https://www.kaggle.com/datasets/chebotinaa/fast-food-marketing-campaign-ab-test/data)

| Shopping Behavior Dataset Tables | Table Description |
| :------------- | :------------ |
| MarketID | unique market identifier |
| MarketSize | market area size by sales generated |
| LocationID | unique store location identifier |
| AgeOfStore | age of store in years |
| Promotion | one of three promotions that were tested |
| week | one of four weeks when the promotions were run |
| SalesInThousands | sales amount (in thousands) for a specific LocationID, Promotion, and week |

## Objective

The purpose of this project is to be part of an ongoing process to refine and develop my data analysis skills. To find the best marketing campaign we are going to conduct an A/B test to statistically find the optimal marketing campaign for sales growth.

## Analysis Outline

- The ANOVA test was used, and the established hypothesis is:

    - (H0): M0 = M1 = M2 (There is not a statistical difference in the promotion groups)
    
    - (H1): M0 != M1 != M2 (There is a statistical difference in the promotion groups)

- Shapiro-Wilk test resulted in the significance level being less than 0.05, leading us to reject the null hypothesis, indicating that the assumption of equality is not met and that it is not a normal distribution

- In the case of non-normal distribution, we used the Kruskal–Wallis Test a non-parametric test. For this scenario, we are going to use the Kruskal–Wallis Test

## Conclusion

Based on the results of this dataset, I uncovered that this fast food company should use promotion strategies A/1 and/or C/3 for their future primary marketing campaign for optimal sales performance.
