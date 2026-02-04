# MLOps Introduction: Final Project Description

## Overview
The final project for the "Introduction to MLOps" course consists of comprehensive tasks covering Machine Learning model development and serving.

### Goals
* **Adhere to the ML Lifecycle:** Use the standard ML lifecycle as a continuous reference for all activities.
* **Software Excellence:** Apply essential software development knowledge (version control, modularity) to the ML lifecycle.
* **Engineering Best Practices:** Implement ML engineering practices for development, deployment, and serving.
* **MLOps Adoption:** Apply and integrate core MLOps concepts throughout the project.


## Final Work Definition
The following sections detail the requirements and steps for the final project:

### A) Problem Definition
* **Define an AI/ML Use Case:** Identify a specific problem that can be solved via ML/AI models.
    * Describe the problem context, constraints, goals, benefits, and expected results.
    * **Optional:** Define high-level success metrics (i.e., what results must be achieved to consider the ML solution a success).
* **Data Acquisition:** Identify, define, describe, and analyze your raw dataset(s).

### B) ML Experimentation
* **Execution:** Conduct experiments via Jupyter Notebooks and/or Python scripts.
* **Data Preparation:** Apply data transformations (if needed) to generate your training dataset.
* **Model Selection:** Choose and train your ML models.
* **Evaluation:** Analyze and evaluate the performance results.
* **Model Selection:** Identify your "champion" (best) model.
* **Optional:** Use **MLflow** to track and register your experiments.

### C) ML Development Activities
* **Project Preparation:**
    * Create a **public GitHub repository** in your account. 
    * Suggested naming convention: `uni_mds_ciclo3_ml_project`.
    * Establish a clean project structure and work within a dedicated implementation branch.
    * Clone your repository locally for development.
* **Data Engineering:**
    * Save your raw dataset in a structured directory (e.g., `/data/raw/`).
    * Implement transformations in a modular Python script (e.g., `data_preparation.py`).
    * *Note: If transformations are not required, provide a justification using graphics or analysis.*
    * Describe the features (variables) of the final training dataset.
    * **Expected Result:** A final training dataset saved in a designated folder (e.g., `/data/training/` or `/data/features/`).
* **Model Training Implementation:**
    * Implement training logic in a Python script (e.g., `train.py`).
    * Include **model serialization** (saving the model in `.pkl`, `.joblib`, or other standard formats).
    * **Expected Result:** A serialized trained model saved in a folder (e.g., `/models/<model_name>.pkl`).
* **Model Registry (Optional):**
    * Register your model in a registry, such as **MLflow Model Registry**.

### D) Model Deployment & Serving
* **Model Serving Strategy:** Implement one of the following two approaches:
    1.  **Web/REST API:** Use the **Flask** or **FastAPI** library. (Example filename: `serving/app.py`).
    2.  **MLflow Serving:** Serve the model locally using the `mlflow models serve` command.
* **Model Inference:**
    * Launch your model API from the previous step.
    * **Perform Predictions:** Use a REST client (`curl`, a Python script, or `Postman`) to request predictions by passing inputs to your API.
    * Document/register your results.
    * **Expected Result:** Successful generation of prediction values (class, label, or numerical output).
