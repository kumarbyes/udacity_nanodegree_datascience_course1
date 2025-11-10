# Understanding which factors affect GDP Growth rate using sklearn

![GDP Growth](images/GDP_Growth.png)

## Table of Contents

- [Project Motivation](#project-motivation)
- [Dataset](#dataset)
- [Requirements](#Requirements)
- [Installations](#Installations)
- [File description](#file-description)
- [Result summary](#Result-summary)
- [Licensing, Authors, Acknowledgements](#Licensing-Authors-Acknowledgements)

### Project Motivation

I was interested on how news channels and financial institutions make predictions about a country's projected growth rate based on economic, social and infrastructure factors. I wanted to understand which factors contribute to the GDP growth rate. Two models were used in the process : linear regression and random forest. Linear regression was used initially so that i can undertsand how the predictions are made. Random forest was used later to check how much better it performs than the linear regression model. To understand which factros influence the GDP growth, SHAP plots were studied.

### Dataset

[World Bank Databank Website](https://databank.worldbank.org/source/world-development-indicators)

The World Bank is an institution that provides much needed credit and economic management for countries around the world. As part of their duties, they have comprehensive forms of economic data on their partners.

From the above website, I selected some 30-35 developed and developing countries, series indicators and values ranging from the year 2000 till 2021. More about the selected indicators you can find in the **Project_Supervised_ML.ipynb** notebook.

### Requirements

-**Python Version**: 3.11.9 was used for this project<br/>
-Jupyter notebook was used for the complete development of this project<br/>
-Check Requirements.txt file for all the libraries used in the project<br/>

### Installations

Install the required libraries for the project using **requirements.txt** file:

```bash
pip install -r requirements.txt
```

### File Description

Following files are available in the github repository to succesfully run the code:

1. **Project_Supervised_ML.ipynb**: This is primary file containing all the relevant python code for project. At each point in the notebook, markdown cells are added to explain the process or inform about the inference.
2. **Requirements.txt**: Python libraries used in the project for pip install
3. **sample4.csv**: Csv file containing the data needed for the machine learning models

### Result Summary

After performing exploratory data analysis, we could see that gross capital formation has a direct relationship to GDP growth rate. This was further confimred by both the models. Out of the two, random forest seems to score better on evaluation metrics like mean square error and root mean square error. Especially, on root mean square error it does way better than linear regression. Out of the two, random forest comes out as a clear winner when you want to make prediction. From the SAHP analysis, we can see that these features **Individuals using the internet, Domestic credit to private sector by banks, Gross capital formation and exports of goods & servcies** are imporatnt in the decision making process. More about the analysis you can find in this [Post](https://medium.com/@kumar.byes/understanding-which-factors-affect-gdp-growth-rate-using-sklearn-831874927d6f) on medium.

### Licensing, Authors, Acknowledgements

Thanks to the following websites :

- [Databank](https://databank.worldbank.org/) to provide the data for zero cost
- [SHAP documentation](https://shap.readthedocs.io/) for the explaining the concepts in detail
- Sklearn documentation
- Investopedia for this [blog](https://www.investopedia.com/ask/answers/112814/why-does-inflation-increase-gdp-growth.asp)
- [GeekfforGeeks](https://www.geeksforgeeks.org/data-science/detect-and-remove-the-outliers-using-python/) for the blogpost about outlier removal

No license attached to this jupyter notebook. Feel free to use the code as you would like! If in case you learned something, you give me credits or share the medium post.
