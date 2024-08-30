# END TO END ML PROJECT

1. VS Code
   - Python Extension Pack
   - Jupyter
   - Data Wrangler

E2E ML Project Session 01 Summary:

- IDE: VS Code setup
- Install VS Code Extensions
- Create folders and files

  - README.md
  - notebooks
  - data

- Data collection

  - Download data from Kaggle
  - Load data into pandas dataframe

- Automated EDA tools

  - Ydata Profiling
  - Dtale

- Git and GitHub
  - Git init
    - `git init`
    - Git add
    - Git commit
  - Create a new repository in github
  - Push changes to GitHub

Intstructions to clone the repository:

```bash
git clone https://github.com/meftaul/e2e-ml-housing-project.git
```

Open the project in VS Code and start working on the project.


## Session 02 Summary:

- Create train and test datasets
  - Random sampling
  - Stratified sampling
- Split the data into features and target based on `income_cat` - startified sampling

- Data Cleaning
  - Missing value visualization
  - Missing values imputation - mean, median
  - Missing values imputation - SimpleImputer

- Feature Scaling
  - Standardization
  - Min-Max Scaling
  - Normalization (Home work)

- Categorical Encoding
  - One Hot Encoding (Home work)
  - Ordinal Encoding

## Session 03 Summary:

- Create a pipeline for data preprocessing
  - Numeric features
    - Mean imputation
    - Standardization
  - Categorical features
    - Most frequent imputation
    - One Hot Encoding
- Create a pipeline for model training
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
- Save the model using joblib
- Load the model and make predictions

- Build a streamlit app
  - Install streamlit

# Next Session goals:
- Take the streamlit app to the docker container
- Experiment tracking with MLflow


# Share final application using dokcer:
- Build the docker image
  - Create a `Dockerfile`
  - Build the docker image
    - `docker build -t housing-app .` or `docker build -t meftaul/housing-app:v1 .`
    - Change tag name as per your username in the docker hub
    - `docker tag housing-app:latest meftaul/housing-app:v1`
- Push the docker image to docker hub
  - `docker push meftaul/housing-app:v1`

# How to use the docker image? 
- Install docker
- Pull the docker image
  - `docker pull meftaul/housing-app:v1`
- Run the docker image
  - `docker run -p 8501:8501 meftaul/housing-app:v1`
  - `docker run -p <host-machine-port>:<container-port> image-name:version`




## References and links

[Pandas read\_\* docucemntation](https://pandas.pydata.org/docs/getting_started/intro_tutorials/02_read_write.html)
[SQLAlchemy](https://www.sqlalchemy.org/)
[Ydata Profiling](https://docs.profiling.ydata.ai/latest/)

[Preprocessing](https://scikit-learn.org/stable/modules/preprocessing.html)

[Pipeline Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html)
[Streamlit](https://docs.streamlit.io/)
