# Long-Term Investment Prediction Project

## Introduction

The Portuguese Bank has identified a revenue decline due to customers not making long-term deposits. The purpose of the model is to identify existing customers that have a higher chance to subscribe for a long term deposit and develop marketing campaigns to target them. The dataset used in this project is the Portuguese Bank dataset.

The data is related to direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be subscribed ('yes') or not ('no') subscribed.

## Dataset

The dataset contains train and test data. Features of train data are listed below:

-   age: age of a person
-   job: type of job ('admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')
-   marital: marital status ('divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)
-   education: ('basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')
-   default: if has credit in default ('no','yes','unknown')
-   housing: has housing loan ('no','yes','unknown')
-   loan: has personal loan ('no','yes','unknown')
-   contact: contact communication type ('cellular','telephone')
-   month: last contact month of year ('jan', 'feb', 'mar', ..., 'nov', 'dec')
-   dayofweek: last contact day of the week ('mon','tue','wed','thu','fri')
-   duration: last contact duration, in seconds affects the output target (e.g., if duration=0 then y='no')
-   campaign: number of contacts performed during this campaign and for this client
-   pdays: number of days that passed by after the client was last contacted from a previous campaign (999 means client was not previously contacted)
-   previous: number of contacts performed before this campaign and for this client
-   poutcome: outcome of the previous marketing campaign ('failure','nonexistent','success')
-   deposit: has the client subscribed a term deposit? ('yes','no')

## Models

The following models were used in this project:

-   Nearest Neighbors
-   Logistic Regression
-   Random Forest

## Results

The following results were achieved after training the models and making predictions:

| Classifier          | Accuracy | Precision | Recall   | F1 Train | F1 Test  | Train Time |
|-----------|-----------|-----------|-----------|-----------|-----------|-----------|
| Nearest Neighbors   | 0.921131 | 0.742643  | 0.440753 | 0.553191 | 0.400000 | 0.075835   |
| Logistic Regression | 0.899014 | 0.622159  | 0.225000 | 0.330483 | 0.327409 | 0.035240   |
| Random Forest       | 0.889605 | 1.000000  | 0.003425 | 0.006826 | 0.007547 | 0.585027   |

## Usage

To use this project, you can clone the repository and run the `long-term_investment_prediction.ipynb` notebook in Jupyter Notebook or JupyterLab.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.