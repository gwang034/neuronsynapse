# neuronsynapse

**Grace Wang** and **Didi Zhou**

Code for ELEC 478 Neuron Synapse Final Challenge.

Synaptic connections allow neurons to send signals to one another, forming the foundation of understanding neural behavior and patterns.The present work outlines a machine learning approach to assess whether neurons within axonaldendritic proximity will form a synapse. The guiding principles behind our method were (1) to engineer biologically interpretable features and (2) to build a model selection process resistant to overfitting. The process began with data cleaning and preprocessing, followed by feature engineering based on an understanding of neural structures. Then, the data was split into training and query sets; with bootstrap subsamples of the training set, hyperparameters were selected for eXtreme Gradient Boosting, Random Forest, and Logistic Regression models. Finally, selected models were tested via a public and private kaggle leaderboard where our final placements were 14th and 45th respectively.

Code walkthrough:

* **ml_process.ipynb** - a jupyter notebook containing the final machine learning process used to train and tune ML models for the competition
* 
