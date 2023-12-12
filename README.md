# neuronsynapse 🧠📈

**Grace Wang** and **Didi Zhou**

Code for ELEC 478 Neuron Synapse Final Challenge.

Synaptic connections allow neurons to send signals to one another, forming the foundation of understanding neural behavior and patterns.The present work outlines a machine learning approach to assess whether neurons within axonaldendritic proximity will form a synapse. The guiding principles behind our method were (1) to engineer biologically interpretable features and (2) to build a model selection process resistant to overfitting. The process began with data cleaning and preprocessing, followed by feature engineering based on an understanding of neural structures. Then, the data was split into training and query sets; with bootstrap subsamples of the training set, hyperparameters were selected for eXtreme Gradient Boosting, Random Forest, and Logistic Regression models. Finally, selected models were tested via a public and private kaggle leaderboard where our final placements were 14th and 45th respectively.

Code walkthrough:

* :page_facing_up:	**ml_process.ipynb** - a jupyter notebook containing the final machine learning process used to train and tune ML models for the competition
* :page_facing_up:	**create_figures.ipynb** - a jupyter notebook used to create the figures for the final report
* :file_folder:	**Data** - folder containing all of the necessary files for the project. Please note that **imputed_morph_embed.csv.zip** must be unzipped because the raw csv file was too large for Github.
* :file_folder:	**Submission** - folder containing information relevant to the XGBoost, Random Forest, and Logistic Regression models submitted to the kaggle leaderboard
  *   :file_folder:	**Hyperparameter Tuning** - folder containing files for the performance of XGBoost, Random Forest, and Logistic Regression across a grid of hyperparameters
  *   :file_folder:	**Predictions** - the predictions submitted to the Kaggle leaderboard. We selected the XGBoost and Random Forest predictions for the private leaderboard.
  *   :file_folder:	**Feature Importances** - the feature importances associated with XGB, RF, and LR model tuned to their best hyperparameters
* :file_folder:	**Revision** - folder containing information relevant to the XGBoost, Random Forest, and Logistic Regression models developed with adjustments to our process following the reveal of the private leaderboard results
  *   :file_folder:	**Hyperparameter Tuning** - folder containing files for the performance of XGBoost, Random Forest, and Logistic Regression across a grid of hyperparameters
  *   :file_folder:	**Predictions** - the predictions generated by the revised models on the submission set
