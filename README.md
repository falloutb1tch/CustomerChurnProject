# Churn Down For What
## Overview

(Client Redacted) approached our company, The Classification Station, to ascertain whether we could build a model to accurately predict whether a customer would "soon" stop doing business with (Client Redacted). When a customer withdraws their business, this is known as "churning".

## Business Understanding

While a certain amount of churn is unavoidable, businesses strive to bring churn to as low a level as possible. It is cheaper and thus more profitable to keep existing customers rather than lure in new ones. So, our company was employed to determined causes of churn and which of those causes had the most impact on (Client Redacted). Specifically, as we begin 2024, it is wise to keep in mind the changing social landscape around us. I do not know a single person without a cell phone unless they are a very young child, but I know many people without a landline, or only a cursory one that they got along with their internet or cable television package. Therefore, this project will continue under the assumption we are speaking of a cellular telephone company rather than one offering landline services.

## Data Understanding

This public dataset is provided by the CrowdAnalytix community as part of their churn prediction competition. The real name of the telecom company is anonymized. It contains 20 predictor variables mostly about customer usage patterns. There are 3333 records in this dataset, out of which 483 customers are churners and the remaining 2850 are non-churners. Thus, the ratio of churners in this dataset is 14%.

## Data Preparation

We removed unnecessary columns such as "phone number", then encoded our categorical variables and scaled our numerics. Then, we used class_weight to deal with the aforementioned class imbalance, and did a train/test split to prepare our data for modeling.

## Model Recommendation

After modeling, we found that a logistic regression with an L2 penalty and class_weight balance brought both our accuracy and our recall up around 75%. It is posisble that these numbers could improve with further time and/or resources.

## Conlusion and Next Steps

Though our final model was not our most accurate, it did have the highest recall we could facilitate. Recall was our most important metric because it measures, in this context, which customers actually churned versus predicted churns. A possible next course of action would be for (Client Redacted) to earmark customers with a certain threshold of customer service calls and use our model to predict those that will churn based upon that. Then, (Client Redacted) can take advantage of the proffered opportunity to prevent that customer from churning.

## Repo Structure
```
├── data
├── images
├── README.md
├── ChurnDown.pdf
└── Final.ipynb
```
