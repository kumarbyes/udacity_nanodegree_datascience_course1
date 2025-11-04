# Predict GDP Growth rate using Supervised Machine learning

![GDP Growth](GDP_Groth.png)

## Table of Contents

- [Project Motivation](#project-motivation)
- [Dataset](#dataset)
- [Requirements](#Requirements)
- [Installations](#Installations)
- [File description](#File Description)
- [Result summary](#Result summary)

### Project Motivation

For this project, I was motivated to do something related to finance using machine learning. I was interested on how news channels and financial institutions make predictions about a country's projected growth rate based on economic, social and infrastructure factors. Two models were used for the prediction : linear regression and random forest. Linear regression was used initially so that i can undertsand how the predictions are made. Random forest was used later to check how much better it performs than the linear regression model.

### Dataset

[World Bank Databank Website](https://databank.worldbank.org/source/world-development-indicators)

The World Bank is an institution that provides much needed credit and economic management for countries around the world. As part of their duties, they have comprehensive forms of economic data on their partners.

From the above website, I selected some 30-35 developed and developing countries, series indicators and values ranging from the year 2000 till 2021. More about the selected indicators you can find in the **Project_Supervised_ML.ipynb** notebook.

### Requirements

-**Python Version**: 3.11.9<br/>
-Jupyter notebook was created with this python version. If it works in other versions feel free to use anything<br/>
-Check Requirements.txt file for all the libraries used in the project<br/>

### Installations

Install the required libraries for notebook using **requirements.txt** file:

```bash
pip install -r requirements.txt
```

### File Description

Following files are available in the github repository to succesfully run the code:

1. **Project_Supervised_ML.ipynb**: This is primary file containing all the relevant python code for project. At each point in the notebook, markdown cells are added to explain the process or inform about the inference.
2. **Requirements.txt**: Python libraries used in the project for pip install
3. **sample4.csv**: Csv file containing the data needed for the machine learning model

### Result Summary

After performing exploratory data analysis, we could see that gross capital formation has a direct relationship to GDP growth rate. This was further confimred by both the models. Out of the two, random forest seems to score better on evaluation metrics like mean square error and root mean square error. Especially, on root mean square error it does way better than linear regression. Out of the two, random forest comes out as a clear winner. More about the analysis you can find in this [Post](medium.com) on medium.
