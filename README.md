## Supervised Learning Project Codes Instruction
#### hli736 (Gatech OMSCS CS7641)

This project is to develop 5 supervised learning methods (<em>Decision Tree, Neural Network, Boosting, Support Vector Machine and K-Nearest Neighbors</em>) to analysis two classification datasets.This document is the instructions of the codes development for **Supervised Learning** to solve the classification problems.

### Dataset
There are two datasets analyzed in this project. They are in teh root file as well as in file **Proj1_Healthinsurance/data** for cross_sell.csv and **Proj1_music/data** for music.csv.

The music.csv is retrieved from Spotify using Spotify’s API. It is published by id (GeorgeMcIntire) on Kaggle (https://www.kaggle.com/geomack/spotifyclassification). more details about the attributes: https://developer.spotify.com/documentation/web-api/reference/tracks/get-audio-features/

the cross_sell.csv is a new released competition on Analytics Vidhya, Janatahack: Cross-sell Prediction (https://datahack.analyticsvidhya.com/contest/janatahack-cross-sell-prediction). The dataset used in this competition is also published by Anmol Kumar on Kaggle (https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction?select=train.csv)

### The Structure of the Codes
There are two files under the root file: the **Proj1_music** and **Proj1_Healthinsurance**. The **Proj1_music** file include the codes for the analyses of Spotify dataset. And the **Proj1_Healthinsurance** includes the codes for the analyses of Health Insurance Cross Sell Prediction dataset.

The structure of the two files are very similar. There are:
* /Data: contains the music.csv
* Visualization.ipynb: the codes for data preprocessing and visualization
* DecisionTree_Boosting.ipynb: the codes for implementing of decision tree and Boosting (HistGradientBoosting and GradientBoosting)
* SVM_KNN.ipynb: codes for implementing of SVM and KNN
* NN.ipynb: codes for implementing of Neural Network
* decision_tree.png: the structure of decision after prunning

### The Package version
* pandas 1.0.5
* numpy 1.18.5
* matplotlib 3.1.3
* seaborn 0.11.0
* graphviz 0.14.1
* imageio 2.6.1
* tensorflow 2.3.0
* keras 2.4.0
* sklearn 0.22.2.post1

### Reference
Data normalization

* https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html

* https://www.kaggle.com/dietzschdaniel/who-should-you-sell-your-insurance-to

* https://seaborn.pydata.org/generated/seaborn.distplot.html

scikit-learn decision tree classifier:

* https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html

scikit-learn boosting classifier

* https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.HistGradientBoostingClassifier.html

SVM:

* https://scikit-learn.org/stable/modules/generated/sklearn.svm.NuSVC.html#sklearn.svm.NuSVC

KNN

* https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html

Keras:

* https://keras.io/api/layers/regularizers/
* https://keras.io/api/layers/regularization_layers/dropout/
* https://keras.io/api/models/sequential/
* https://keras.io/api/losses/

Deep learning post:

* https://machinelearningmastery.com/tutorial-first-neural-network-python-keras/
* https://towardsdatascience.com/evaluating-keras-neural-network-performance-using-yellowbrick-visualizations-ad65543f3174
Stack overflow:
* https://stackoverflow.com/questions/48118111/get-loss-values-for-each-training-instance-keras
