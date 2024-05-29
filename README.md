# NLP---Sentiment-Analysis-and-Uniqueness-Score
Preprocessing , tokenisation and Sentiment Analysis using BERT on dataset of 1000 textual descriptions. Followed by calculation of a uniqueness score.

A. ​Preprocessing steps before tokenization using BERT.
      1.  Stemming
      2.  Remove special characters, extra spaces and numbers 
      3.  Convert to lower case 
      4.  Remove stop words
      5.  Remove rows with null values


B. Use BERT to tokenize the words in the description. Then use Cosine Similarity to calculate 
uniqueness of each description. BERT takes about 15 mins to do the tokenization on Colab. 


C. Now I would like to see how well the Uniqueness score works. So for that I used K-means to cluster the 
descriptions. I also used the elbow method and a few other metrics to tune the clustering method. After that 
I check the uniqueness score of the items in each cluster. 
***
D. A good way to determine how well  the uniqueness scores works is to see if the scores of the items in a cluster 
are similar. If they are fairly similar, then everything works fine. See the code and the visualizations. 
E. I also added code that will print the number of items in each cluster, the number of unique values, and the 
count of unique values that differ by a maximum of ±2.
(The last ±2 metric also helps check the effectiveness of K-means.)
