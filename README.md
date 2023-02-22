# MLflow-project-template
MLflow project template

## STEPS -

### STEP 01- Create a repository by using template repository

### STEP 02- Clone the new repository

### STEP 03- Create a conda environment after opening the repository in VSCODE

```bash
conda create --prefix ./env python=3.7 -y
```

```bash
conda activate ./env
```
OR
```bash
source activate ./env
```

### STEP 04- install the requirements
```bash
pip install -r requirements.txt
```

### STEP 05- Create conda.yaml file
```bash
conda env export > conda.yaml
```


### STEP 06- commit and push the changes to the remote repository

### STEP 07 - Get data
```bash
1.create stage_01_get_data.py and update config.yaml file to fetch and create data file
2.write code unzip data in common.py as a function, stage_01_get_data.py file and config.yaml
3.create data_mgmt file to validate image and store bad images in bad folder, update cnfig.yaml file and stage_01_get_data
```

### STEO 08 - Model Creation
```bash
1. Create Stage_02_base_model_creation.py file and update required code
2. Update config file with params
3. This will create model folder with .h5 model
```

### Command to run the ML project file
```bash
mlflow run. --no-conda
```

### Run any specific entry point in the ML project files
```bash
mlflow run . -e get_data -P config=configs/your_config.yaml --no-conda
```

### Create stage_04_train.py file for training and stage_03_prepare_callbacks.py
```bash
update stage_04_train.py file for training and stage_03_prepare_callbacks.py with required code
update  MLproject file, main.py file, config.yaml file
```