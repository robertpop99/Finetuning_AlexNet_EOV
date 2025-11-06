# Finetuning AlexNet EOV #

To launch the notebook:
- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/robertpop99/Finetuning_AlexNet_EOV/blob/main/Finetuning_AlexNet_for_Volcanic_Deformation_Classification.ipynb) Recommended. After opening it, change the execution type to T4 GPU or any execution with a GPU.
- [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/robertpop99/Finetuning_AlexNet_EOV/main?labpath=Finetuning_AlexNet_for_Volcanic_Deformation_Classification.ipynb) Not recommended. Due to memory constrains, you need to set the batch size to 2.


## Install locally ##

### Instructions for Windows ###

1. Download the notebook: [Notebook](https://github.com/robertpop99/Finetuning_AlexNet_EOV)

2. Download Miniforge and install with the default settings: [Miniforge](https://conda-forge.org/download/). Open Miniforge Prompt from the search bar and navigate to the folder where you downloaded the notebook.

3. You can install the environment by running the following commands:
    ```bash
    conda create --name finetuning_alexnet python=3.12
    conda activate finetuning_alexnet
    pip install torch torchvision --index-url https://download.pytorch.org/whl/cu130
    pip install matplotlib jupyterlab scikit-learn
    ```

4. Download the dataset from here: [Dataset](https://zenodo.org/records/14161590/files/LiCS.zip). Unzip the dataset in the same folder where you downloaded the notebook. Make sure you have one folder named LiCS with two subfolders named background_noise and volcano_deformation.

5. You can activate the Jupyter Notebook by running the command:

    ```bash
    jupyter lab
    ```
    A new tab should open in your web browser.


### Instructions for Mac ###

1. Download the notebook: [Notebook](https://github.com/robertpop99/Finetuning_AlexNet_EOV)

2. Download and install Miniforge from here: [Miniforge](https://conda-forge.org/download/)

3. By default, conda is activated every time you open a terminal. If you want this to stop, run this command in a terminal:

    ```bash
    conda config --set auto_activate_base false
    ```
4. Now you can install the packages. Navigate tot the folder where you downloaded the notebook and run the next commands:

    ```bash
    CONDA_SUBDIR=osx-64 conda create --name finetuning_alexnet python=3.12
    conda activate finetuning_alexnet
    conda config --env --set subdir osx-64
    pip install torch torchvision
    pip install matplotlib jupyterlab scikit-learn
    ```

5. Download the dataset from here: [Dataset](https://zenodo.org/records/14161590/files/LiCS.zip). Unzip the dataset in the same folder where you downloaded the notebook. Make sure you have one folder named LiCS with two subfolders named background_noise and volcano_deformation.

6. You can activate the Jupyter Notebook by running the command:

    ```bash
    jupyter lab
    ```
    
    A new tab should open in your web browser.
