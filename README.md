# Data-Driven Optimization of Semiconductor Processes and Forecasting

![ChipPerformance](https://github.com/user-attachments/assets/a5630c4f-df22-4c74-ab9c-af50e12b0b76)

![FeatureSelection](https://github.com/user-attachments/assets/ecae7c7d-e49a-4a2b-aae7-42f9d4a2a10f)

![WaferFaultRates](https://github.com/user-attachments/assets/224e7935-4888-4de5-b444-5cac5e2122c8)

![SemiconductorShortage](https://github.com/user-attachments/assets/0d2a8eec-2e0d-42e6-a54d-8071f3c5dc41)

## Project Overview

This project focuses on enhancing semiconductor manufacturing efficiency by applying data mining techniques across four distinct datasets. Each dataset corresponds to a unique aspect of semiconductor manufacturing and analysis, including performance benchmarking, manufacturing analysis, wafer fault detection, and economic forecasting related to semiconductor shortages.

The project employs the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology combined with Agile-Scrum practices to ensure a structured yet flexible approach. The main objective is to identify key factors influencing outcomes such as oxide thickness, yield, and defect rates, ultimately improving production processes and strategic decision-making.

## Datasets

### 1. **Trend Analysis and Performance Benchmarking of Semiconductor Chips**
   - **Objective**: Analyze development trends of CPUs and GPUs, validate against hypotheses like Moore's Law, and forecast future trends.
   - **Dataset Overview**: Historical data of semiconductor chips, focusing on metrics like process size, transistor counts, and energy efficiency.
   - **Key Techniques**: Time Series forecasting, Regression analysis, RandomForestClassifier for trend prediction.

### 2. **Feature Selection and Prediction for Manufacturing Analysis**
   - **Objective**: Identify key features impacting semiconductor yield and develop predictive models for quality control.
   - **Dataset Overview**: The dataset includes 1567 rows and 592 columns with various numerical features and a binary target variable 'Pass/Fail'.
   - **Key Techniques**: Exploratory Data Analysis (EDA), Feature Engineering, Logistic Regression, and Correlation Analysis.

### 3. **Wafer Fault Detection Analysis**
   - **Objective**: Improve fault rate prediction in wafer production, enhancing manufacturing flexibility and dependability.
   - **Dataset Overview**: Contains sensor data with 591 features and a target variable 'Good/Bad' for classification.
   - **Key Techniques**: Distribution analysis, Correlation heatmaps, Random Forest Classifier, SMOTE for class imbalance handling.

### 4. **Economic Forecasting Related to Semiconductor Shortages**
   - **Objective**: Analyze the impact of semiconductor shortages on economic indicators like PPI, and forecast future trends.
   - **Dataset Overview**: Time-series data related to economic factors such as PPI, Import/Export price indexes.
   - **Key Techniques**: Time Series forecasting using Prophet, Feature Engineering for lag and rolling window statistics.

## Setup and Installation

This project uses Python 3.12.4 and is managed with a virtual environment to ensure that all dependencies are correctly isolated.

### Creating a Virtual Environment

To create and activate the virtual environment, run the following commands in your terminal:

```bash
python3.12 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### Installing Dependencies

After activating the virtual environment, install the required packages using `pip`:

```bash
pip install -r requirements.txt
```

### Requirements

The `requirements.txt` file includes the following dependencies with specific versions:

```
absl-py==2.1.0
anyio==4.4.0
argon2-cffi==23.1.0
argon2-cffi-bindings==21.2.0
arrow==1.3.0
asttokens==2.4.1
astunparse==1.6.3
async-lru==2.0.4
attrs==24.2.0
Babel==2.15.0
beautifulsoup4==4.12.3
bleach==6.1.0
certifi==2024.7.4
cffi==1.17.0
charset-normalizer==3.3.2
cmdstanpy==1.2.4
colorama==0.4.6
comm==0.2.2
contourpy==1.2.1
cycler==0.12.1
Cython==3.0.11
debugpy==1.8.5
decorator==5.1.1
defusedxml==0.7.1
executing==2.0.1
fastjsonschema==2.20.0
flatbuffers==24.3.25
fonttools==4.53.1
fqdn==1.5.1
gast==0.6.0
google-pasta==0.2.0
grpcio==1.65.5
h11==0.14.0
h5py==3.11.0
holidays==0.54
httpcore==1.0.5
httpx==0.27.0
idna==3.7
imbalanced-learn==0.12.3
importlib_resources==6.4.3
ipykernel==6.29.5
ipython==8.26.0
ipywidgets==8.1.3
isoduration==20.11.0
jedi==0.19.1
Jinja2==3.1.4
joblib==1.4.2
json5==0.9.25
jsonpointer==3.0.0
jsonschema==4.23.0
jsonschema-specifications==2023.12.1
jupyter==1.0.0
jupyter_client==8.6.2
jupyter-console==6.6.3
jupyter_core==5.7.2
jupyter-events==0.10.0
jupyter-lsp==2.2.5
jupyter_server==2.14.2
jupyter_server_terminals==0.5.3
jupyterlab==4.2.4
jupyterlab_pygments==0.3.0
jupyterlab_server==2.27.3
jupyterlab_widgets==3.0.11
keras==3.5.0
kiwisolver==1.4.5
libclang==18.1.1
Markdown==3.7
markdown-it-py==3.0.0
MarkupSafe==2.1.5
matplotlib==3.9.0
matplotlib-inline==0.1.7
mdurl==0.1.2
meson==1.5.1
mistune==3.0.2
ml-dtypes==0.4.0
namex==0.0.8
nbclient==0.10.0
nbconvert==7.16.4
nbformat==5.10.4
nest-asyncio==1.6.0
ninja==1.11.1.1
notebook==7.2.1
notebook_shim==0.2.4
numpy==1.26.4
opt-einsum==3.3.0
optree==0.12.1
overrides==7.7.0
packaging==24.1
pandas==2.2.2
pandocfilters==1.5.1
parso==0.8.4
patsy==0.5.6
pillow==10.4.0
pip==24.2
platformdirs==4.2.2
pmdarima==2.0.4
prometheus_client==0.20.0
prompt_toolkit==3.0.47
prophet==1.1.5
protobuf==4.25.4
psutil==6.0.0
pure_eval==0.2.3
pycparser==2.22
Pygments==2.18.0
pyparsing==3.1.2
python-dateutil==2.9.0.post0
python-json-logger==2.0.7
pytz==2024.1
pywin32==306
pywinpty==2.0.13
PyYAML==6.0.2
pyzmq==26.1.0
qtconsole==5.5.2
QtPy==2.4.1
referencing==0.35.1
requests==2.32.3
rfc3339-validator==0.1.4
rfc3986-validator==0.1.1
rich==13.7.1
rpds-py==0.20.0
scikit-learn==1.5.1
scipy==1.14.0
seaborn==0.13.2
Send2Trash==1.8.3
setuptools==72.1.0
six==1.16.0
sniffio==1.3.1
soupsieve==2.5
stack-data==0.6.3
stanio==0.5.1
statsmodels==0.14.0
tensorboard==2.17.1
tensorboard-data-server==0.7.2
tensorflow-intel==2.17.0
termcolor==2.4.0
terminado==0.18.1
threadpoolctl==3.5.0
tinycss2==1.3.0
tornado==6.4.1
tqdm==4.66.5
traitlets==5.14.3
types-python-dateutil==2.9.0.20240316
typing_extensions==4.12.2
tzdata==2024.1
uri-template==1.3.0
urllib3==2.2.2
wcwidth==0.2.13
webcolors==24.6.0
webencodings

==0.5.1
websocket-client==1.8.0
Werkzeug==3.0.3
wheel==0.43.0
widgetsnbextension==4.0.11
wrapt==1.16.0
xgboost==2.1.1
```

> **Note**: If newer versions of any packages are released and cause compatibility issues, the versions listed here should be used as a reference for the working environment.

## Methodology

The project adheres to the CRISP-DM framework, which is particularly suitable for handling complex datasets from various sources. The six stages of CRISP-DM—Business Understanding, Data Understanding, Data Preparation, Modeling, Evaluation, and Deployment—are iteratively followed to ensure the project addresses the critical challenges in semiconductor manufacturing.

### Tools and Technologies

- **Programming Language**: Python 3.12.4
- **Data Analysis**: Pandas, NumPy
- **Machine Learning**: Scikit-learn, RandomForestClassifier, Logistic Regression
- **Time Series Analysis**: Prophet
- **Data Visualization**: Matplotlib, Seaborn
- **Data Preparation**: StandardScaler, SMOTE, Yeo-Johnson transformation

## Results

The project successfully developed predictive models and insights that can improve semiconductor manufacturing efficiency, forecast economic trends, and optimize production processes. Key findings include the validation of Moore's Law in performance benchmarking, identification of critical features impacting yield, and sensors crucial for fault detection in wafers.

## Future Work

Further exploration could involve refining the models by incorporating more external factors, addressing class imbalance more effectively, and extending the economic forecasting models to include additional economic indicators.

## Dataset References

The following datasets were used in this project, and their respective authors are credited below:

1. **ChipPerformance.csv**:
   - Original Dataset: [CPU and GPU Product Data](https://www.kaggle.com/datasets/michaelbryantds/cpu-and-gpu-product-data)
   - Renamed in this project as `ChipPerformance.csv`.

2. **FeatureSelection.csv**:
   - Original Dataset: [UCI Semcom](https://www.kaggle.com/datasets/paresh2047/uci-semcom)
   - Renamed in this project as `FeatureSelection.csv`.

3. **WaferFaultRates.csv**:
   - Original Dataset: [Wafer Dataset](https://www.kaggle.com/datasets/bhushanbhawarkar/wafer-dataset)
   - Renamed in this project as `WaferFaultRates.csv`.

4. **SemiconductorShortage.csv**:
   - Original Dataset: [Semiconductor Shortages (1985-2021)](https://www.kaggle.com/datasets/ramjasmaurya/semiconductor-shortages19852021)
   - Renamed in this project as `SemiconductorShortage.csv`.
