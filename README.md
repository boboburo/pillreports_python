# pillreports_python

iPython notebooks to accompany Chapter 5 of upcoming text book: <a href="http://www.amazon.co.uk/Text-Mining-Visualization-Open-Source-Knowledge/dp/1482237571/ref=sr_1_4?s=books&ie=UTF8&qid=1447346687&sr=1-4" target="_blank">Text Mining and Visualization: Case Studies Using Open-Source Tools</a> 
 
## Talks and Presentations
 
 Slides for PyData Berlin Conference May 2015 <a href="http://ibriancarter.github.io/berlin_pydata_2015/index.html#/" target="_blank">here</a> 

 Video of PyData Berlin Conference talk <a href="https://www.youtube.com/watch?v=ikxm_kFL9MA" target="_blank">here</a> 
 
 Slides for Python Ireland Meetup November 2015 <a href="http://ibriancarter.github.io/python_ireland_nov2015/index.html#/" target="_blank">here</a>

## Setup and Install
 
 Installation instructions where <a href="https://www.continuum.io/downloads" target="_blank">Anaconda</a>  and 
<a href="http://git-scm.com" target="_blank">Git</a> are installed on your machine. 
 
### Clone
 
 1. git clone https://github.com/iBrianCarter/pillreports_python
 2. cd pillreports_python
 
### Create Enviroment 

Downloads all the relevant packages, this can be done manually also. 

1. conda create -n pillreports_python --file package-list
2. activate pillreports_python
3. jupyter notebook

When you are complete don't forget to deactivate the environment in command line

4. deactivate


### Delete the Environment

1.conda env remove -n pillreports_python

## Notebook Descriptions 
 
##### 1. Version and Library Check.ipynb
List of the library versions used in development. Must have library version equal or greater for notebooks to function as described.

##### 2. Web Scraping.ipynb
Initial scrape of data from website. Data is stored to a collection in a MongoDB. Must have instance of Mongo running. MongoDB can be downloaded from http://mongodb.org/downloads . Collection name is created in the format *pillreports_%d%b%y%* e.g (pillreports_31Mar15) 

##### 3. Data Cleansing.ipynb
Must have instance of MongoDB running. Data read from MongoDB collection. Specify name as above. Data is saved to .csv file (prReports.csv) . Remaining notebooks read from .csv file. Initial scrape of 5001 records is provided in Data/prReports.csv for replicating research presented.

##### 4. Data Visualisation.ipynb
Data read from prReports.csv file - data exploration provided.

##### 5. Classification.ipynb
Data read from prReports.csv file. Naive Bayes and Stochastic Gradient Descent learning applied to predict *Warning:* field. Varying methods of vectorization applied to generate input features from *Description:* field. 

##### 6. Clustering & PCA.ipynb
Cluster and PCA applied to vector representation of the *User Report:* field. Scatterplot and wordcloud visualisastion of results.

##### 7. Extra_Topic_Models.ipynb
Quick implentation showing LDA Topic Models with *gensim* and visualisation with *pyLDAvis*.

##### A. SparseMatrix.ipynb
Appendix file illustrating the creation of sparse matrix representation of text data.

##### B. Matplotlib_Subplots.ipynb
Appendix file illustrating various methods of creating subplots with Matplotlib library.
