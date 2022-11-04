# Stock Trading powered by Machine Learning
Algorithmic trading application that learns and adapts to new data and evolving markets


<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#purpose">Purpose</a>
      <ul>
        <li><a href="#inputs">Inputs</a></li>
        <li><a href="#outputs">Outputs</a></li>
      </ul>
    </li>
    <li>
      <a href="#modeling_techniques">Modeling Techniques</a>
      <ul>
        <li><a href="#pandas">Pandas</a></li>
        <li><a href="#sklearn">sklearn</a></li>
        <li><a href="#standardscaler">Standard Scaler</a></li>
        <li><a href="#stochastic-gradient-descent">Stochastic Gradient Descent -SGD</a></li>
        <li><a href="#ada-boost">ADA Boost</a></li>
        <li><a href="#accuracy-evaluation">Accuracy Evaluation</a></li>
      </ul>
    </li>
    <li><a href="#how-to-run">How to run</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#report-and-evaluation-of-tested-model">Report and evaluation of tested model</a></li>
        <ul>
        <li><a href="#training-the-model">Training the model</a></li>
        <li><a href="#supervised-learning-methods-and-models-used">Supervised Learning Methods used</a></li>
        </li>
            <a><li><a href="#1)-stochastic-gradient-descent-sgd">1)Stochastic Gradient Descent - SGD</a></li>
            <li><a href="#2)ada-boost">2)ADA Boost </a></li>
        <li><a href="#analysis">Analysis</a></li>
     </ul>   
    <li><a href="#version-release">Version Release</a></li>
    <li><a href="#contributors">Contributors</a></li>
    <li><a href="#license">License</a></li>
        <ul>
        <li><a href="#permissions">Permissions</a></li>
        <li><a href="#disclaimer">Disclaimer</a></li>
        </ul>
    </li>
    <li><a href="#aknowledgements">Aknowledgements</a></li>
</details>

---
<!--Purpose -->
## Purpose
This tool employs Supervised Machine Learning to model and identify creditworthiness of borrowers.


### Inputs
The application reads a data set of 34000 organizations that have recieved funding over the years. The CSV file contains a variety of information about each business including weather or not it became successful. 
We'll use this data to predict weather a business will be successful. The financial institution will use this to decide upon lending to the business.

    emerging_markets_ohlcv.csv
 
### Process:
1. Read historical business data in the CSV file.
2. Process data for Neural Network Modeling.
3. Compile and Evaluate a Binary Classification Model using a Nerural Network. 
4. Optimize the Neural Network Model using Tensorflow and Keras.
5. Define 2 deep neural network models from the original network model and 2 optimization attempts.
6. Obtain each model's Predictive Accuracy metrics. 
7. Predictive accuracy metrics will be saved as outputs that summarize each optimization attempt and model.

### Outputs:
1. HDF5 file named AlphabetSoup.h5 
File includes the initial model's data
2. AlphabetSoup_Model_1.h5
First attempt to evaluate the model using test data to determine the model's loss and accuracy.
3. AlphabetSoup_Model_2.h5
Second attempt to evaluate the model using test data to determine the model's loss and accuracy.

   
---
<!--Technologies -->
## Technologies
### Python:

    Phyton Version: **3.7.13**

## Libraries and Dependencies

### Pandas
[pandas](https://pandas.pydata.org/)

### Sklearn
[sklearn](https://scikit-learn.org/stable/)

### Standard Scaler
[standardscaler](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html)

### Stochastic Gradient Descent- SGD
[stochastic-gradient-descent](https://scikit-learn.org/stable/modules/linear_model.html#stochastic-gradient-descent-sgd) 

### ADA Boost
[ada-boost](https://scikit-learn.org/stable/modules/ensemble.html#adaboost)

### Accuracy Evaluation Metric
[accuracy-evaluation](https://pythonguides.com/adam-optimizer-pytorch/)



<!--How to run -->
## How to run
1. Clone the repository on a folder that will easy to open
2. File can run on a Jupyter notebook or Google Colab
3. Open the file with Jupiter using the Anaconda Navigator
4. Navigate open the folder where the files were cloned to
5. Open the file on JupyterLab
ANACONDA - Navigator
![jupyterlab](./images/anaconda_nav.png)
6. Make sure to import and install the required libaries and dependencies: 

        Install the required Supervised Learning libraries
            conda activate dev
            from pathlib import Path

        Import the required libraries and dependencies
            import tensorflow as tf
            from tensorflow.keras.layers import Dense
            from tensorflow.keras.models import Sequential
            from sklearn.model_selection import train_test_split
            from sklearn.preprocessing import StandardScaler,OneHotEncoder

---
<!--Version Release -->
## Version Release

### Version 1.0


---
<!--Usage -->
## Usage
### Data: Lending data
![lending_data](./images/lending_data.png)

### Applicant Data
![applicant_data](./images/applicant_data.png)

### Standard Scaler:
![standard-scaler](./images/standardscaler.png)

### Model Evaluation:
![model-evaluation](./images/model_evaluation.png)

### Alternative Models 1 and 2 results:

![model1and2](./images/model1and2.png)

---

<!--Report and Evaluation of tested model -->
## Report and evaluation of tested model

---

<!--Training the model -->
## Training the model
### Standard 3 month training
![Original 3 Month Training](/images/3months_model1_train_plot.png)
### Model trained 2 months 
![Original 2 Months Training](/images/2months_model2_train_plot.png)
### Model trained 6 months 
![Original 6 Months Training](/images/6months_model3_train_plot.png)
### Model trained 12 months 
![Original 12 Months Training](/images/12months_model4_train_plot.png)

---
<!--Supervised Learning Methods and Models used -->
## Supervised Learning Methods and Models used
## 1) Linear Models: SGD Classifier
## 2) Ensemble Methods: ADA Boost
---
<!--1)Linear Models: Stochastic Gradient Descent - SGD -->
## 1) Linear Models: Stochastic Gradient Descent - SGD
### SGD Classifer 3 Months
![SGD Classifer 3 months](./images/SGD3_plot.png)

### SGD Classifer 2 Months
![SGD Classifer 2 months](./images/SGD2_plot.png)

### SGD Classifer 6 Months
![SGD Classifer 6 months](./images/SGD6_plot.png)

### SGD Classifer 12 Months
![SGD Classifer 12 months](./images/SGD12_plot.png)

---
<!--2) ADA Boost -->
## 2) ADA Boost 

<!--Analysis -->
## Analysis

---
<!--Contributors -->
## Contributors

Jeremy Vargas

    Managing Director
    Resonant Solutions LLC
    email:    jeremyvargas@resonantsolutions.org
    linkedin: https://www.linkedin.com/in/jeremyvargas/

UW FinTech Bootcamp
- Startup code provided by institution

---
<!--License -->
## License
Tool is available under an MIT License.

Copyright (c) 2022 - Resonant Solutions, LLC

### Permissions
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
### Disclaimer
The Software is provided “as is”, without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the Software.

---
<!--Aknowledgements -->
## Aknowledgements
* [Markdown Guide](https://www.markdownguide.org/basic-syntax/#reference-style-links)


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->