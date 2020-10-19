# sentiment-analysis
In this project I have done the sentiment analysis on the reviews for different mobile phones on amazon.
### Execution
we will be training our model on the stanford sentiment treebank data.  
Note that you can recover the 5 classes by mapping the positivity probability using the following cut-offs:
[0, 0.2], (0.2, 0.4], (0.4, 0.6], (0.6, 0.8], (0.8, 1.0]
for very negative, negative, neutral, positive, very positive, respectively.
As the folder of sentiment treebank data has many files inside it so we need to generate our training  and testing data from it. 
1. generate data  
The code in file generate data.ipynb contains the code used for generation of train, test and val data in csv format.  
2. analyse the data and train the model  
The file training.ipynb contains the code used for training the model.I used different machine learning algorithms and checked the accuraccy.The best model was pickled for further use.  
3. Scrap the amazon website  
As of now our model is ready so our next target is to scrap the amazon website and get the data on which we have to perform sentiment analysis.For scrapping the website I have used scrapy and 
pycharm ide.The folder named amazon contains all the files related to scraping.The file named data1 contains the scrapped data it has names of mobiles and their reviews.  
4. Prediction  
Now we are all set for prediction of the sentiments of people. here all the reviews are passed to the model and the results were stored in final.csv and final.xlsx files.The code is in prediction.ipynb file     
5. Results  
Now in see results.ipynb file I have just ploted the bar graphs for the different classes of reviews for all mobiles.  
