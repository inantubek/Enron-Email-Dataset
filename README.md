# Enron-Email-Dataset
Project work done as part of Udacity's  Data Analyst Nanodegree course.

The [Enron Corpus](https://en.wikipedia.org/wiki/Enron_Corpus) is a large database of over 600,000 emails generated by 158 employees of the Enron Corporation and acquired by the Federal Energy Regulatory Commission during its investigation after the company's collapse.

Enron Email Dataset downloaded from : https://www.cs.cmu.edu/~enron/.  
And it is the __May 7, 2015 Version of dataset__.

Running the `startup.py` file present in this repository will automatically download the tarred and gzipped dataset and extract it for usage.  

***
 The email and finance data is combined into a single dataset, which is explored in this mini-project.

Getting started:

- Clone this [git repository](https://github.com/udacity/ud120-projects)
- Open the starter code from the cloned repo : ```datasets_questions/explore_enron_data.py```

The aggregated _Enron email + financial dataset_ is stored in a dictionary, where each key in the dictionary is a person’s name and the value is a dictionary containing all the features of that person.   
 
The _email + finance (E+F) data dictionary_ is stored as a _pickle file_, which is a handy way to store and load python objects directly. Use ```datasets_questions/explore_enron_data.py``` to load the dataset.

* Number of data points (people) in the dataset - 146
* Features in the Enron Dataset - 21  
* Finding numer of POIs(Person of Interest) in the Enron Data - 18
* Total number of POI's (Obtained from the list of all POI names ```(in ../final_project/poi_names.txt)```) = 35

### Querying the dataset
1.  total value of the stock belonging to James Prentice -- 1095040
2.  Number of email messages from Wesley Colwell to persons of interest -- 11
3.  The value of stock options exercised by Jeffrey K Skilling -- 19250000


The helper functions (```featureFormat()``` and ```targetFeatureSplit()``` in ___tools/feature_format.py__) that can take a list of feature names and the data dictionary, and return a numpy array.

***

The folder __My works__ contains the jupyter noptebook files which show the analysis done on the dataset.  
* ```My works/Dataset qtns/explore_enron_data_jn.ipynb``` - includes the initial analysis done on the datset.
* ```My works/regression/finance_regression_jn.ipynb```  - Regression analysis done on variables Bonus, salary and long_term_incentive.