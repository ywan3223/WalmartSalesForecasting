# WalmartSalesForecasting
The project focuses on **forecasting Walmart's department-wide sales** using historical data from 2010 to 2013, incorporating factors like promotional markdowns and economic indicators. Employing **Linear Regression**, **Random Forest**, and **Support Vector Machine** algorithms, the study cleans and prepares the data, emphasizing the significance of holiday periods on sales. Among the models tested, Random Forest outperformed others, showcasing its effectiveness in predicting weekly sales with the lowest **Mean Absolute Error**, demonstrating the potential for improving inventory management and strategic planning in retail operations.

## Dataset  
This historical information includes weekly sales from February 5, 2010, to July 26, 2013. The dataset is from the Kaggle dataset [Walmart Dataset - Regression Problem](https://www.kaggle.com/datasets/yasserh/walmart-dataset"悬停显示"). The dataset contains 6745120 data that have been categorized using 16 variables.

## Methodology
* *Data Cleaning*  
The methodology begins with data cleaning to ensure the integrity and usability of the dataset. The process involves merging features and store data into a single frame, addressing NaN values by filling them with averages for certain variables like Temperature, Fuel Price, and Unemployment, or zeroes for markdowns. This step is crucial for maintaining a robust dataset by removing extreme values and preparing it for analysis and modeling.  

* *Algorithms*  
The project utilizes Linear Regression, Random Forest, and Support Vector Machine (SVM) algorithms to forecast sales. Data is divided into training and testing sets, with weekly sales as the target variable. Each algorithm undergoes the same preparation, leveraging sklearn.linear_model for implementation. The quality of splits during sample division is critically evaluated, with the fit method used for training and the pre method for model predictions.  

* *Evaluation Procedure*  
Model performance is assessed through hold-out validation, using a pre-split dataset of Walmart's historical sales data into training and test sets. This approach allows for the evaluation of the model's efficacy on unseen data, providing a measure of the model's generalization capability. The primary metric for comparison is the Mean Absolute Error (MAE), which quantifies the average magnitude of errors in predictions, serving as a key indicator of model suitability and effectiveness.

## Result  
Results demonstrated the efficacy of various vectorization and optimization models in identifying suicidal ideation from online texts. MultiNB models with TfidVectorizer showed the highest performance and probability of distinguishing depression or suicidal ideation using this model reached 69.18% test accuracy with AUC score 0.77. 

<div>

|  | AUC score  | Train Accuracy  | Test Accuracy  |
| ---------- | -----------| -----------| -----------|
| cvec+ multi_nb  | 0.717 | 0.682| 0.628 |  
| tvec + multi_nb   | 0.754  | 0.687| 0.651| 
|hvec + multi_nb | 0.807 | 0.766| 0.659 | 

</div>
<img src="/image/result.png" width = "500" height = "200" alt="cmt" />

## Future Direction
1.Data Preprocessing: Apply advanced anomaly detection to identify and correct discrepancies, enhancing data quality.
2.Feature Engineering: Create sophisticated features, including customer sentiment from social media, to capture deeper insights.
3.Modeling Techniques: Explore deep learning, such as LSTM networks, for capturing complex data patterns.
4.Validation and Optimization: Use cross-validation and systematic hyperparameter tuning to refine model accuracy.
5.External Data: Incorporate broader factors like economic indicators and weather conditions to enrich the model's context.## Application  

The project's application encompasses the strategic refinement of retail operational frameworks by leveraging predictive analytics derived from machine learning algorithms. It empowers retailers to proactively manage inventory, tailor marketing campaigns, and streamline supply chain logistics based on anticipated sales trends. Additionally, this predictive approach facilitates data-driven decision-making, enabling retailers to dynamically adjust to market demands, optimize resource allocation, and enhance the overall customer experience through improved product availability and targeted promotions. By integrating such predictive models, retailers can significantly reduce operational costs, increase revenue through informed stocking decisions, and bolster customer loyalty by meeting consumer needs more effectively.
