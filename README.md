# Welfare AI 2.0 
This repository houses code for the welfare AI project done in collaboration with the McGill Animal Science Department.

## Folders

### Locomotion
This folder contains the excel files of the scaled coordinates passages. 

### Amanda_Notebooks
Models in these notebooks were trained by separating the data (25-75) BEFORE data augmentation. 

### Dylan_Notebooks
Models in these notebooks were trained by separating the data (25-75) AFTER data augmentation. 

### Results
This folder contains the final confusion matrices for the RF, CNN and LSTM trained by Amanda. 

 
 ## Running the code
 
### Configuration
To run this code, you will need an Anaconda environment prepackaged with Python 3. This code was tested using python version 3.8.3. Python libraries including matplotlib, scikit-learn, numpy, keras, tensorflow and pandas must be installed in your python environment. 

### Python version
* [python 3.7.11](https://www.python.org/downloads/release/python-3711/)

### Other libraries 
You can install these libraries using  `conda install`. 
* matplotlib 3.4.2
* scikit-learn 0.24.2
* numpy 1.19.2
* pandas 1.2.4
* keras-gpu 2.3.1
* tensorflow gpu 2.1.0

## Running this Code
Download all the files from the zip folder in this repository. Open a terminal and cd to the project folder (if you are using a python environment, make sure to activate it before). You can then open the jupyter notebook and run the cells during the tutorial. 

` ` ` git clone https://github.com/bioinfoUQAM/welfare_ai_2.0/ ` ` ` 

` ` `  cd welfare_ai_2.0  ` ` ` 
  
` ` `  python jupyter notebook  ` ` ` 
 
Then navigate to one of the jupyter notebooks using the Notebook Dashboard and click on it to open. 

Before running the notebooks, make sure to add the correct paths to the scores.csv files and Locomotion directories: 

```python
 
# Get the list of locomotion data files 
listLocomotionData = os.listdir("../Locomotion")

# Initialize the data dictionary
data = {}
# Get the list of sensor names
sensor_names = pd.read_excel("../Locomotion/" + listLocomotionData[0]).columns

 ``` 


 
