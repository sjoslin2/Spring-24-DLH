# CS 598 DLH Final Project - Reproduction Study 
## Authors
* Team#: 97
* Team Members: Cody Talmadge(codytt2@illinois.edu), Seth Joslin (sjoslin2@illnois.edu), and Sree Alaparthi (sa68@illinois.edu)
* Paper: 33 - ScoEHR: Generating Synthetic Electronic Health Records using Continuous-time Diffusion Models[1]

## Introduction
This repository includes code for a reproduction study and additional ablations related to the paper titled 'Generating Synthetic Electronic Health Records using Continuous-time Diffusion Models' [1].<br/>
The original codebase was obtained from the GitHub repository of the paper's authors [2] 

For more details about our reproduction study, please refer to the following resources:

* Presentation [Video Presentation](https://drive.google.com/file/d/1-44eZ1X_3JA6lhmW0lIfsQZrf1oo_NGo/view)
* Final Report [Team_97.pdf](https://github.com/sjoslin2/Spring-24-DLH/blob/main/Team_97.pdf)

* [1] Paper Link: https://www.mlforhc.org/s/ID145_Research-Paper_2023.pdf
* [2] https://github.com/aanaseer/ScoEHR

## Requirements and Dependencies

Running the code requires Python 3. <br/>
All the requirements are documented in requirements.txt.<br/>
If you want to run the code directly on your local machine, install the required dependencies below:
```
$ pip3 install -r requirements.txt
```


## Manual Setup Needed
In order to run this notebook, you will need to:
1. Ensure that you downloaded it from the [github repository](https://github.com/sjoslin2/Spring-24-DLH).  This means that you should see the following folders:
- `./ablation_saved_models/` - This is where the saved Score Net models for the learning rate/epoch ablations live.
- `./ablation_synthetic_data/` - This is where the synthetic data generated by the ablation models live.
- `./additional_workbooks/` - This folder contains the additional notebooks that contains the data preprocessing and loading synthetic data using pyHealth.
 - `./mimic/` - Folder where you need to manually add the MIMIC-III data files (detailed instructions in Data sub-section).
 - `./saved_models/` - This is where the saved Autoencoder and Score Net model parametres live.
 - `./stats/` - This contains stats information around the model training.  If you train these models from scratch then your model trainings stats are displayed instead.
 - `./synthetic_data/` - This contains synthetic data generated by the model.  If you want to generate your own synthetic data you'll need ~30 minutes of GPU time.
2. Ensure you have added the MIMIC-III data files into the `./mimic/` folder (detailed instructions in the Data sub-section).

**Running This Notebook on Colab**

If you would like to run this notebook in Colab, place it and all of the files from the github repository into a "ScoEHR" folder in your Google Drive.

**Running This Notebook Without Colab**

Make sure this notebook is in the same folder as all of the other files from the github repository.

## Additional Instructions
Please review the 'Team_97.ipynb' notebook for sections covering data downloading, model training, and results analysis.
