
### **AWS SageMaker Flight Prices Prediction**

This repository contains the code and resources for predicting flight prices using machine learning models deployed on AWS SageMaker. The project is structured around several key stages: data cleaning, exploratory data analysis (EDA), data preprocessing, and model training.

#### **Project Structure**

- **`notebooks/`**: Contains Jupyter notebooks that guide you through different stages of the machine learning workflow.
  - **`1_Data_Cleaning.ipynb`**: 
    - Focuses on cleaning the raw dataset by handling missing values, correcting data types, and removing any irrelevant information.
    - Includes techniques for dealing with outliers and inconsistencies in the data.
  - **`2_EDA.ipynb`**: 
    - Performs exploratory data analysis to uncover patterns, trends, and relationships in the data.
    - Uses various visualization techniques to better understand the distribution of variables and their interactions.
  - **`3_Data_Preprocessing.ipynb`**: 
    - Involves feature engineering, such as encoding categorical variables, scaling numerical features, and creating new features.
    - Prepares the dataset for machine learning by splitting it into training and testing sets.
  - **`4_Model_Training.ipynb`**: 
    - Covers model selection, training, and evaluation.
    - Includes hyperparameter tuning using techniques like GridSearchCV or RandomizedSearchCV.
    - Demonstrates how to deploy the trained model on AWS SageMaker for inference.

- **`src/`**: Contains Python scripts that support the notebook workflows, allowing for scalable and reproducible pipelines.
  - `train.py`: Script for training the model using the processed data.
  - `inference.py`: Handles making predictions with the trained model.
  - `utils.py`: Utility functions for common tasks such as data loading, feature extraction, and model evaluation.

- **`data/`**: A directory intended for storing raw and processed datasets. (Datasets are not included in the repository due to size and privacy concerns.)

- **`models/`**: This folder stores trained models, including serialized versions (e.g., `.pkl` files) ready for deployment.

- **`vizpro.py`**: A custom Python module that includes various visualization functions to aid in exploratory data analysis (EDA). This module supports generating plots for outlier detection, bivariate relationships, and data transformations.

- **`requirements.txt`**: A file listing the Python dependencies required to run the project. These should be installed within a virtual environment.

- **`README.md`**: The main documentation file that provides an overview of the project, setup instructions, and usage guidelines.


3. **Running the Notebooks**:
   - Open Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Navigate to the `notebooks/` directory and start exploring the notebooks in the following order:
     1. `1_Data_Cleaning.ipynb`
     2. `2_EDA.ipynb`
     3. `3_Data_Preprocessing.ipynb`
     4. `4_Model_Training.ipynb`

4. **Deploying the Model on SageMaker**:
   - Follow the steps in `4_Model_Training.ipynb` to train and deploy your model on AWS SageMaker.

#### **Key Features**

- **Comprehensive Workflow**: Covers all steps from raw data cleaning to model deployment.
- **Scalable and Reproducible**: Uses modular scripts and notebooks that can be easily adapted for other datasets.
- **AWS Integration**: Seamless integration with AWS SageMaker for training and deploying machine learning models.
- **Visualization**: Includes custom visualization tools to enhance EDA and model interpretability.

#### **Contributing**

Contributions are welcome! If you would like to contribute to this project, please fork the repository and submit a pull request. Whether it's bug fixes, new features, or improvements to documentation, all contributions are appreciated.

