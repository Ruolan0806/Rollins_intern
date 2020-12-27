# Rollins_intern
The main purpose of this project is to predict Chemical_Materials_Applied, Product_Materials_Applied, Bait_Materials_Applied, Hardware_Materials_Applied, Equipment_Materials_Applied, service_Materials_Applied based on a random sample of data we have drawn from the database. 



# Transforming: 
●	After selecting the appropriate features, I need to preprocess the data in a proper way in order to fit the model. Since the two features are all categorical values, I need to transform them into numerical values. 

●	To do this, there are several options. The first one is one hot encoding. This method converts each category value into a new column and assigns a 1 or 0. For example, in the case of program, we have 59 different programs. If we use one hot encoding, then we will have an extra of 59 new columns to substitute the original column. Therefore, this option is not suitable in this case. 

●	Another option is the LabelEncoding method which is what I finally decide to use in the model. This method gives each unique category a number which means if we have 59 programs, we will have number 0 to 58 to replace the original column. Even though this method may introduce some misinterpretation in the algorithm, it is the best among the three options we have. 

●	The third option is the binary encoding and it is mentioned later in the discussion. After doing much research in this method, we can see that it is not a good choice. Just like the names indicated, this method yields two results, 0 or 1. For instance, if 1 represents ‘PC Standard - Monthly’, then 0 will represent all other programs beside ‘PC Standard - Monthly’. If we use this method, then the purpose of predicting products based on different regions and different programs will be highly impacted.

●	 In conclusion, LabelEncoding is the best fit for the situation. 

# Modeling: 
●	After preprocessing, I implement the train test splits to set aside a proportion of data for testing. Then, I deployed KNN algorithms to training the data. 

●	In order to optimize the result, I do try different parameters for the number of neighbors. In my findings, number 3 is the best among 1,3,5 and 7. 

●	But this is dependent upon datasets, therefore, this may vary among different datasets. 

●	After that, I also tried Random Forest Classifier into training the model. And I leave both in the notebook for further reference.

