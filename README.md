# 02456 Deep Learning Project
This is repository for project 18F for the Course 02456 Deep Learning at DTU.

The purpose of the modal was to classify regions of origin from genotype data.

The project is split into different files. The content and purpose of each file is:

- `data_processing.py`: Preparing the data so that it can be used for training, validation, and testing.
- `model.py`: The Feed-Forward Neural Network created using Pytorch Lightning
- `18F_optuna.py`/`18F_optuna.ipynb`: The optuna code to find the optimized parameters used for the different input sizes. The code is available as a notebook and `.py` file.
- `18F_classification.py`/`18F_classification.ipynb`: The code for training the models. The code is available as a notebook and `.py` file.
- `18F_confusion_matrix.py`: Code for testing the models (after training). Here the confusion matrix for the test set is plotted.
- `18_F_plot.py`: The plots of the validation accuracy and loss.

The requirements for this project is listed in `requirements.txt`.

## The data

The dataset consists of two files:
1. `pcs.txt`: A `.txt` file with the PC's for the individuals
2. `v44.3_HO_public.anno`: The meta data for the individuals

The original file with the PC's consisted of 4000 PC's per individual. But due to the size of this file, only the first 100 PC's have been kept.

## Plots
The data for the plots can be found in the `wandb_csv`folder. We used the logger [WandB](https://wandb.ai) to gather the training metrics of the model.
