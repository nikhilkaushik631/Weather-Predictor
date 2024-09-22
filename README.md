# Weather Prediction Project

## Introduction
This project involves predicting whether it will rain tomorrow (`RainTomorrow`) based on weather observations from the past. The dataset used includes various weather metrics such as temperature, rainfall, humidity, and wind conditions, collected between 2008 and 2017. Several machine learning algorithms were implemented to build predictive models, utilizing Scikit-learn for preprocessing and evaluation.

## Algorithms Used
The following machine learning algorithms were used in this project:
- **Linear Regression**
- **K-Nearest Neighbors (KNN)**
- **Decision Trees**
- **Logistic Regression**
- **Support Vector Machines (SVM)**

## Metrics Used
To evaluate the performance of the models, we used several metrics:
- **Accuracy Score**
- **Jaccard Index**
- **F1-Score**
- **LogLoss**
- **Mean Absolute Error**
- **Mean Squared Error**
- **R2-Score**

## Scikit-learn
Scikit-learn (sklearn) is a widely used Python library in machine learning, which we utilized in our project for tasks like data preprocessing and implementing algorithms for classification and regression. Its efficient tools for model evaluation and selection made it essential for our workflow.

## Dataset Used
The original source of the data is the Australian Government's Bureau of Meteorology. The latest data can be gathered from [this link](http://www.bom.gov.au/climate/dwo/).

The dataset for this project includes two target columns:
- **`RainToday`**: Indicator of whether it rained today (Yes/No)
- **`RainTomorrow`**: Indicator of whether it will rain tomorrow (Yes/No), used as the target variable for prediction.

You can find the dataset at [Rattle's repository](https://bitbucket.org/kayontoga/rattle/src/master/data/weatherAUS.RData).

### Dataset Fields
| Field          | Description                                                            | Unit             | Type   |
|----------------|------------------------------------------------------------------------|------------------|--------|
| Date           | Date of the Observation in YYYY-MM-DD                                  | Date             | object |
| Location       | Location of the Observation                                            | Location         | object |
| MinTemp        | Minimum temperature                                                    | Celsius          | float  |
| MaxTemp        | Maximum temperature                                                    | Celsius          | float  |
| Rainfall       | Amount of rainfall                                                     | Millimeters      | float  |
| Evaporation    | Amount of evaporation                                                  | Millimeters      | float  |
| Sunshine       | Amount of bright sunshine                                              | hours            | float  |
| WindGustDir    | Direction of the strongest gust                                        | Compass Points   | object |
| WindGustSpeed  | Speed of the strongest gust                                            | Kilometers/Hour  | float  |
| WindDir9am     | Wind direction averaged over 10 minutes prior to 9am                   | Compass Points   | object |
| WindDir3pm     | Wind direction averaged over 10 minutes prior to 3pm                   | Compass Points   | object |
| WindSpeed9am   | Wind speed averaged over 10 minutes prior to 9am                       | Kilometers/Hour  | float  |
| WindSpeed3pm   | Wind speed averaged over 10 minutes prior to 3pm                       | Kilometers/Hour  | float  |
| Humidity9am    | Humidity at 9am                                                        | Percent          | float  |
| Humidity3pm    | Humidity at 3pm                                                        | Percent          | float  |
| Pressure9am    | Atmospheric pressure reduced to mean sea level at 9am                  | Hectopascal      | float  |
| Pressure3pm    | Atmospheric pressure reduced to mean sea level at 3pm                  | Hectopascal      | float  |
| Cloud9am       | Fraction of the sky obscured by cloud at 9am                           | Eights           | float  |
| Cloud3pm       | Fraction of the sky obscured by cloud at 3pm                           | Eights           | float  |
| Temp9am        | Temperature at 9am                                                     | Celsius          | float  |
| Temp3pm        | Temperature at 3pm                                                     | Celsius          | float  |
| RainToday      | If there was rain today                                                | Yes/No           | object |
| RainTomorrow   | If there is rain tomorrow (target variable)                            | Yes/No           | object |

Column definitions were gathered from [here](http://www.bom.gov.au/climate/dwo/IDCJDW0000.shtml).
