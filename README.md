# NA-404
AI Based Project that is used for Sentimental Analysis. 

# Introduction:
We are living in a very politically charged environment these days and in this environment, people can easily express their thoughts and opinions on the internet freely without any fear. People say things on the internet which they don’t usually say in person and that can be because of multiple reasons.
The sentiments of the people should predict what should happen in the future because all politicians try to appease the people at least till before elections. 
Our program takes these opinions from Twitter, learns the general opinion and can then try to find out how many people support which political party. This can be very helpful to the media people of these respective parties when they want to find out about what people are saying about the party. 


# Dataset:
The Data we are using is non-numeric. We initially wanted a dataset only related to specific Pakistani Politics. So, we had to create it on our own. We made our dataset from the scratch.

•	Initially total tweets extracted were 5000.
•	Manually removing the duplicates and empty ones we cut it down to approximately 4000 tweets.
•	After applying pre-processing techniques, we now have approximately 3000 tweets.
•	Total Keywords = 40
•	Total features = 8
•	Useful Features = 3
•	We had 2 output columns (Response & Party)
•	Response had three classes: Positive, Negative & Neutral
•	Party had 4 Classes that are: PTI, PMLN, PPP, Neutral

Step 1: We made a twitter developer account and waited for the access permission.
Step 2: We used the Tweety API that helps you in extracting tweets for specific keywords, hash tags or for specific dates.
Step 3: We decided approximately 40 keywords against which we extracted the tweets.
Step 4:Writing those tweets into CSV files.
Step5: We manually read each tweet and labeled the output columns of which party it belongs to or what type of sentiment it shows
Step 6: We manually cleaned the data, removed the extra words and quotation marks and images that were not useful.
Step 7: We applied built-in functions for cleaning that data. 

# PRE- PROCESSING STEPS:
1.	Remove Punctuations, Urls, stop words, converting it to lower case etc.
2.	Mapping Tweets to a Vector Space.
3.	Converted the Non-Numeric data into Numeric so we can process it and run it on our models.

# Baseline:
The Baseline of our project NA-404 was to do sentimental analysis.  It can provide you the bias free result that you want to see. Politics is always a hot topic to discuss so that is why we solely focused on it. We made two output columns (Response and Party). The User can just input the tweets he wants to look up for and can get the result that whether this tweet supports PTI, PMLN, PPP or is it just a normal or Neutral tweet. He/she can also check what emotion this tweet reflects.
Base line of NA-404 was using ML classificationmodels to classify the result correctly. We used six ML Models.They are “Linear SVM, Poly SVM, Decision tree, random forest classifiers, Naïve Bayes and Neural Networks “

# Result and Analysis:
Our Results were surprisingly very accurate. It not only gave correct results for English tweets but roman Urdu as well. 
Our main approach was to get the tweet classified in two features i.e. Party (having 4 classes) and Responses (having 3 classes). It not only classified testing data on basis of training data, but also figured out the overall result. 
We were first implementing SVM model on our raw dataset which gave us very low results. Then after implementing preprocessing steps, our accuracy increased from 59 to 70 percent which is a good ratio.
According to accuracy, Neural Network gives the best result up to 97.7% accuracy, which is due to our small dataset. By right accuracy, we mean that our input is rightly classified in terms of both response and party.

#REFERENCES :

https://thesai.org/Publications/ViewPaper?Volume=9&Issue=2&Code=IJACSA&SerialNo=26

https://www.researchgate.net/publication/323536661_Sentiment_Analysis_using_SVM_A_Systematic_Literature_Review

https://www.sciencedirect.com/topics/computer-science/evaluation-metric

https://towardsdatascience.com/decision-tree-in-machine-learning-e380942a4c96#:~:text=Decision%20Trees%20are%20a%20non,values%20are%20called%20classification%20trees.

https://www.analyticsvidhya.com/blog/2021/06/understanding-random-forest/

https://towardsdatascience.com/an-easy-tutorial-about-sentiment-analysis-with-deep-learning-and-keras-2bf52b9cba91
