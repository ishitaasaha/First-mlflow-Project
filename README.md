MLflow Workflow
Install MLflow ↓ Initialize Project ↓ Prepare Dataset ↓ Train ML Model ↓ Start MLflow Tracking ↓ Log Parameters ↓ Log Metrics ↓ Log Model ↓ View MLflow UI ↓ Modify Model/Parameters ↓ Run Experiment Again ↓ Compare Runs ↓ Register Best Model
MLflow Commands
| **Command** | **Purpose** | **What it creates/affects** |
|---|---|---|
| `pip install mlflow` | Install MLflow | Installs MLflow on your system |
| `python training.py` | Run ML training script | Trains the ML model and creates an MLflow run |
| `mlflow.set_experiment("Salary Prediction")` | Create/select experiment | Creates or selects an MLflow experiment |
| `mlflow.start_run()` | Start an MLflow run | Creates a new experiment run |
| `mlflow.log_param("model", "LinearRegression")` | Log model parameter | Stores the model configuration |
| `mlflow.log_param("test_size", 0.2)` | Log hyperparameter | Stores the training configuration |
| `mlflow.log_metric("rmse", rmse)` | Log model metric | Stores RMSE performance |
| `mlflow.log_metric("r2_score", r2)` | Log model metric | Stores R² performance |
| `mlflow.sklearn.log_model(model, "model")` | Log trained model | Stores the trained model as an MLflow artifact |
| `mlflow.log_artifact("data.csv")` | Log additional file | Stores a file as an MLflow artifact |
| `mlflow.end_run()` | End MLflow run | Closes the current MLflow run |
| `mlflow ui` | Start MLflow UI | Starts the MLflow tracking dashboard |
| `python training.py` | Run experiment again | Creates a new MLflow run with new parameters/metrics |
| `mlflow.register_model(...)` | Register model | Registers a model in MLflow Model Registry |
| `mlflow models serve ...` | Serve model | Starts an API endpoint for model inference |

