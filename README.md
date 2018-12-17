# PUBG Finish Placement Prediction

<img src="./src/FinalRun/PUBG Inlay.jpg" alt="Drawing" style="width: 500px;"/>

This repository is our solution for Kaggle Competition: [PUBG Finish Placement Prediction](https://www.kaggle.com/c/pubg-finish-placement-prediction) (Kernel Only)

### Contributors:

[@yansun1996](https://github.com/yansun1996) [@xufanxiong](https://github.com/xufanxiong)

### Motivation
Recently, the battle royale-style game has become a very popular online game. One of the most famous game is called PlayerUnknown's BattleGrounds (PUBG). At beginning of each play, nearly 100 people parachute onto an island without any equipment. In order to win the game, you need to scavenge for weapons and available equipment to eliminate the other people and survive to the end.

Hence, if you want to see ‘Winner Winner Chicken Dinner!’ on your display, it’s very esscnetial to make some reasonable strategies based on actual condition. For example, a suitable location of parachuting can help you collect the equipment faster, the path you escape from the continuously shrinking blue circle (out of the circle players will get damage continuously until they die) can help you avoid some dangerous enemies and find a suitable location to hide in the last circle is helpful get the ‘Chicken Dinner’.

Based on these reasons, collect the PUBG’s data and analyze it is a meaningful work to help the player to survive at last. Kaggle hold an interesting competition which try to predict the final ranking percnetile based on the data collected through the PUBG developer API. This dataset has 28 features such as, number of enemy player killed, duration of the match, and so on. According to these data, we try to find the best model to predict the final percentile winning placement.

### Objective
Given previous players' statistical data during each match and ranking information in training data, we need to train a model predict the ranking of the player in testing set based on their statitical data during each match. The target label ranking will be a percentage value between 0 and 1, higher percentage indicates higher ranking in that match.

### Dataset
The dataset is provided by Kaggle, you could go to the [official website](https://www.kaggle.com/c/pubg-finish-placement-prediction/data) to get access to it. You could also create a kernel for the conpetition to get access to it. If you ewant to run our code locally, make sure that all the csv files located in ```../input/``` folder.

### File Description
In the ```./src/Solution.ipynb```, all the exploratory data analysis (EDA), preprocess and feature engineering result are included. As for the model building and test part, it is also included but the result is not directly run by this notebook. This is a kernel only test so that the running time has limitation. We run different models separately in different kernels and then collect all the results and paste them into this notebook. Here are the links to our kernels:
* Linear Regression: https://www.kaggle.com/yansun1996/baseline-linearregression
* Neural Network: https://www.kaggle.com/xufanxiong/artificial-neural-network
* Gradient Boost Regression Tree: https://www.kaggle.com/yansun1996/gbr-ipynb
* LightGBM: https://www.kaggle.com/xufanxiong/light-gbm

### How to Run
1. Fork our kernel on Kaggle to reproduce our results or modify for further exploration.
2. Download the dataset, download our code and reproduce our result.
3. This is a kernel only competition, in order to get the submission score you must submit the prediction through kernels.
