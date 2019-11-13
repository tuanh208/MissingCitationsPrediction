# Missing Citations Prediction

In-class Machine Learning data challenge: https://www.kaggle.com/c/inf554-2018/. <br/>

Predict missing links in a citation network using textual features as well as topological features between two papers. 
## 1. Features
The extracted features are: <br/>
**Textual features**  <br/>
* (1) Cosine similarity of abstracts
* (2) Number of overlap words in abstract
* (3) Cosine similarity of titles
* (4) Number of overlap words in title
* (5) Number of overlap words between target’s title and source’s abstract

**Graphical features** <br/>
*Citation graph*  <br/>
* (6) Number of common neighbourhoods
* (7) Link-based Jaccard coefficient
* (8) Adamic-Adar index
* (9) Preference attachment
* (10) Difference in betweenness centrality
* (11) Difference in the number of in-links
* (12) Number of times target cited
* (13) Pagerank of source
* (14) Pagerank of target
* (15) Minimal distance*
* (16) Is the same cluster? <br/>

*Author collaboration graph*  
* (17) Number of common neighbourhoods
* (18) Link-based Jaccard coefficient
* (19) Preference attachment
* (20) Adamic-Adar index

**Other features** <br/>
* (21) Difference in publication year
* (22) Journal popularity of target
* (23) Is the same journal?
* (24) The number of common authors
* (25) Is self-cited?

## 2. Results
We have tried over different classifiers: *ExtraTree*, *Adaboost*, *LogisticRegression*, *LinearSVM*, *RandomForest*, and *NeuralNetwork*. <br/>
Our best submission on Kaggle was using NeuralNet: **0.97715 F1-score**.

## 3. Others
For more information of the project, please have a look at our report in the file report_ML1_2018.pdf. <br/>
The [data](https://www.kaggle.com/c/inf554-2018/data) should be correctly placed in the folder *data*.
