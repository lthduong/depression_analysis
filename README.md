# Depression Analysis

This is a project to analyse and predict depression states of patients. To run the code, simply install the requirements:
```
python pip install -r requirements.txt
``` 
Then the code can be ran. The recommened order to run the notebooks is `data_process.ipynb`, `individual_analysis.ipynb`, `group_analysis.ipynb`, and `prediction.ipynb`.

# Project structured
The data of the condtioned patients are stored in `data/condition`. Similarly, the data of the controlled patients are stored in `data/control`. The MADRS score data are stored in `data/scores.csv`

The code in `data_process.ipynb` performed data preprocessing, and the output are stored in `cleaned_data/`. For more information on the types of preprocessing.

The code in `individual_analysis.ipynb` and `group_analysis.ipynb` performed the individual and group analysis mentioned in the report. The results of the analysis are stored in `img/individual` and `img/group`, respectively

The code in `prediction.ipynb` implemented a Linear Regression model to predict the data in `cleaned_data/scores.csv`

The file `report.pdf` contains a full explaination on the dataset, the code, and the results obtained from the code
