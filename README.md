# Depression Analysis

This is a project to analyse and predict depression states of patients. To run the code, simply install the requirements:

```
python pip install -r requirements.txt
```

The code can then be ran after installing requirements. To performed the full analysis from the beginning, run the notebooks in the order `data_process.ipynb`, `individual_analysis.ipynb`, `group_analysis.ipynb`, and `prediction.ipynb`.

**Note**: if you want to obtain the same results in `data/individual` and `report.pdf`, locate and set the following variables in `data_process.ipynb`:

```
condition_sample = [3]
control_sample = [27]
```

# Project structured

The data of the condtioned patients are stored in `data/condition`. Similarly, the data of the controlled patients are stored in `data/control`. The MADRS score data are stored in `data/scores.csv`

The code in `data_process.ipynb` performed data preprocessing, and the output are stored in `cleaned_data/`. For more information on the types of preprocessing.

The code in `individual_analysis.ipynb` and `group_analysis.ipynb` performed the individual and group analysis mentioned in the report. The results of the analysis are stored in `img/individual` and `img/group`, respectively

The code in `prediction.ipynb` implemented a Linear Regression model to predict the data in `cleaned_data/scores.csv`

The file `report.pdf` contains a full explaination on the dataset, the code, and the results obtained from the code
