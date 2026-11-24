MLflow Workflow
Install MLflow
↓
Initialize Python Project
↓
Prepare Dataset
↓
Train ML Model
↓
Start MLflow Tracking
↓
Log Parameters
↓
Log Metrics
↓
Log Model
↓
View Experiment in MLflow UI
↓
Modify Parameters / Model
↓
Run Experiment Again
↓
Compare Runs
↓
Register Best Model
MLflow Commands
Command	Purpose	What it creates/affects
pip install mlflow	Install MLflow	Installs MLflow on your system
python training.py	Train ML model	Trains the model and creates model artifacts
mlflow ui	Start MLflow UI	Opens MLflow experiment tracking dashboard
mlflow.set_experiment("Salary Prediction")	Create/select experiment	Creates or selects an MLflow experiment
mlflow.start_run()	Start an MLflow run	Creates a new experiment run
mlflow.log_param("model", "LinearRegression")	Log model parameter	Stores parameter used during training
mlflow.log_param("learning_rate", 0.01)	Log hyperparameter	Records training configuration
mlflow.log_metric("rmse", rmse)	Log model metric	Stores model performance metric
mlflow.log_metric("r2_score", r2)	Log evaluation metric	Stores R² score
mlflow.sklearn.log_model(model, "model")	Log trained model	Stores model artifact in MLflow
mlflow.log_artifact("data.csv")	Log additional file	Stores file as an MLflow artifact
mlflow.end_run()	End MLflow run	Closes the current experiment run
python training.py	Run experiment again	Creates another MLflow run
mlflow models serve ...	Serve MLflow model	Starts model inference API
mlflow.register_model(...)	Register model	Adds model to MLflow Model Registry
