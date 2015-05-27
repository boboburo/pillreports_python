# pillreports_python
iPython notebooks for PyData Berlin Conference 2015
 
 
##### 1. Version and Library Check.ipynb
List of the library versions used in development. Must have library version equal or greater for notebooks to function as described.

##### 2. Web Scraping.ipynb
Initial scrape of data from website. Data is stored to a collection in a MongoDB. Must have instance of Mongo running. MongoDB can be downloaded from http://mongodb.org/downloads . Collection name is created in the format *pillreports_%d%b%y%* e.g (pillreports_31Mar15) 

##### 3. Data Cleansing.ipynb
Must have instance of MongoDB running. Data read from MongoDB collection. Specify name as above. Data is saved to .csv file (prReports.csv) . Remaining notebooks read from .csv file. Initial scrape of 5001 records is provided in Data/prReports.csv for replicating research presented.

##### 4. Data Visualisation.ipynb

##### 5. Classification.ipynb

##### 5. Clustering & PCA.ipynb

##### A. SparseMatrix.ipynb

##### B. Matplotlib_Subplots.ipynb
