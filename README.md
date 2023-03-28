# SMRampup
# SagMaker Ramup
2. Train a Machine Learning Model

Time: 45mins - 55 mins

Overview: For this tutorial users use a synthetically generated auto insurance claims dataset. The inputs are the training, validation, and test datasets. Each of the data sets contain details and extracted features about claims and customers along with a fraud column indicating whether a claim was fraudulent or otherwise.

Learning Objectives:

* Setup SM environment 
* Build, train, and tune model using Hyperparameter Tuner
* Detect bias in ML models and understand model predictions by using SM Clarify
* Deploy the trained model to a real-time inference endpoint for testing using SM Endpoints
* Evaluate the model by generating sample predictions and understanding feature impact

Notes for steps:

1. Create a new notebook in Studio and give it a file name
2. It will take time for hyper parameter tuning results - (5-10) minutes, you will see a .... working and ! at the end.
3. Clarify steps to 5-10 minutes- around 30 total
4. The total time was about 1hr
5. We need to review where to look for experiment results
6. We may need identify which commands have an output and that users will need to wait on it.



3. Automate Machine Learning Workflows

Time: 45-55 mins
In this tutorial, you build a pipeline with the following steps: Data Processing, Train a Model, Evaluate a Model, Conditional Step, Create a Model, Bias check step, Model Explainability, Register Model, Deploy Model.

Learning Objectives:

1. Run a SageMaker Processing job using the input raw data in S3 and outputs training, validation, and test splits to S3.
2. Train an XGBoost model using SageMaker training jobs with training and validation data in S3 as inputs, and stores the trained model artifact in S3.
3. Evaluate the model on the test dataset by running a SageMaker Processing job using the test data and the model artifact in S3 as inputs, and stores the output model performance evaluation report in S3.
4. Compare model performance on the test dataset against the threshold. Run a SageMaker Pipelines predefined step using the model performance evaluation report in S3 as input, and stores the output list of pipeline steps that will be executed if model performance is acceptable.
5. Run a SageMaker Pipelines predefined step using the model artifact in S3 as an input, and stores the output SageMaker model in S3.
6. Checks for model bias using SageMaker Clarify with the training data and model artifact in S3 as inputs and stores the model bias report and baseline metrics in S3.
7. Run SageMaker Clarify with the training data and model artifact in S3 as inputs, and stores the model explainability report and baseline metrics in S3.
8. Run a SageMaker Pipelines predefined step using the model, bias, and explainability baseline metrics as inputs to register the model in the SageMaker Model Registry.
9. Run a SageMaker Pipelines predefined step using an AWS Lambda handler function, the model, and the endpoint configuration as inputs to deploy the model to a SageMaker Real-Time Inference endpoint.

