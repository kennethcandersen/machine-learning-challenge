# MACHINE LEARNING TO CLASSIFY NEWLY DISCOVERED CANDIDATE PLANETS
 
 <table style="width:100%">
  <tr valign="top">
    <th><img height="250" alt="Sample histogram" src="https://github.com/kennethcandersen/machine-learning-challenge/blob/main/images/example_histogram.png"></th>
    <th><img height="250" alt="Box Plot" src="https://github.com/kennethcandersen/machine-learning-challenge/blob/main/images/tensor_model_summary.png"></th>
    <th><img height="250" alt="Bar Chart With Code" src="https://github.com/kennethcandersen/machine-learning-challenge/blob/main/images/tensor_model_compile_fit_eval.png"></th>
  </tr>
</table> 

**EXECUTIVE SUMMARY**
**Mission:** Create a machine learning model that identifies possible new planets using data raw dataset NASA's Kepler space telescope.

**Conclusion:** A TensorFlow-Keras neural network achieved an accuracy of .75, the strongest of the various models that were tested. 

**REPOSITORY NAVIGATION**

* [*Jupyter Notebook*](https://github.com/kennethcandersen/machine-learning-challenge/blob/main/exoplanet_model.ipynb) with the data Extraction, Cleaning, Preparation, and Analysis. 
* [*Saved TensorFlow-Keras Model H5 File*](https://github.com/kennethcandersen/machine-learning-challenge/blob/main/exoplanet_prediction.h5) provides an exported version of the model that can be imported by other users. 
* [*Original data file from NASA*](https://github.com/kennethcandersen/machine-learning-challenge/blob/main/exoplanet_data.csv) with nearly 7,000 observations. 

** ASSUMPTIONS & RESULTS **
* Histograms of the 8 main data columns revealed that several of them mirrored each other and didn't have very interesting distributions. 5 columns were chosen as features for the models. 
* The KNN model, even after GridSearchCV tuning, returned an accuracy of .61.
* The SVC fit process took an excessive amount of time and the model was discarded. 
* The TensorFlow-Keras Neural Network, after experimenting with various quantities of layers, units and features, returned an Accuracy of .75. It was the most effective model tested, although it still did not result in a very high level of confidence. 

**STEPS, TOOLS & LANGUAGES USED**

1. Import CSV data with Pandas.
2. Remove unhelpful columns (numerous columns with error data)
3. Remove outliers using Numpy z scores. 
4. Explore the data with MatPlotLib Histograms, which were created for each of the remaining 8 data columns to view the distribution of the data. 
5. Of the 8 data columns, 5 appeared to have interesting distributions to use in a model.
6. Use sklearn to create a train-test split, and scale the data with MinMaxScaler.
7. Train and Test 3 different models: KNN, SVC, and TensorFlow-Keras Neural Network. 
8. Use GridSearchCV to tune the KNN model. 
9. Save the best model.


=======










