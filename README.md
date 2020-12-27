# Rollins_intern
The main purpose of this project is to predict Chemical_Materials_Applied, Product_Materials_Applied, Bait_Materials_Applied, Hardware_Materials_Applied, Equipment_Materials_Applied, service_Materials_Applied based on a random sample of data we have drawn from the database. 

Modeling: 
●	After preprocessing, I implement the train test splits to set aside a proportion of data for testing. Then, I deployed KNN algorithms to training the data. 
●	In order to optimize the result, I do try different parameters for the number of neighbors. In my findings, number 3 is the best among 1,3,5 and 7. 
●	But this is dependent upon datasets, therefore, this may vary among different datasets. 
●	After that, I also tried Random Forest Classifier into training the model. And I leave both in the notebook for further reference.

