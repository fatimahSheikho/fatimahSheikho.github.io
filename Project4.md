# TED TALKS
# Purpose 
Building a system that recommend TED talks to users based on ratings and transcript of talks using a clustering model.

# Data-set Description
I worked on two seperate data frames both containing the 2250 rows, same TED-talks but different columns.
- First DF
I only used transcript column to apply NLP.

- Second DF
I used ratings column which is people reaction on talks, I converted this column into separate DF containing ratings and their values. 

# NLP Workflow
- Preprocessing
1- Word Tokenization
2- Stop words  and punctuation removal
3- Repeated words in each talk
4- Non-English words removal 
5- Stemming

- Count Vectorizer 

- Dimensionality Reduction
1- Latent Semantic Analysis (LSA)
- Normalizing  the data
To eliminate redundant data and ensure a good quality clusters are generated.

 Before normalizing the data you could notice that there is a huge difference between sizes of clusters.
 
 - Clustering 
 I used K-Mean clustering technique.
 
 - Recommender
I builded a recommender that recommends talks based on clusters. 

# NLP Clustering Results 
The number of clusters were 4 based on elbow and silhouette test.
-UMAP


And to know more about what is inside each clusters, I builded a word cloud. I concluded that first cluster contains talks that are about sounds, and second one contains talks that motivate people. 

# Ratings Clustering Results 
The number of clusters were 4 based on elbow and silhouette test.
- UMAP 

And to dig into these clusters the table below shows highest ratings in each cluster

# Recommender 
I builded a recommender that takes the index of a talk and returns the most popular three talks in the same cluster based on transcript and ratings



