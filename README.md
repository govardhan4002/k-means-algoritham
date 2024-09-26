Project Title: Customer Segmentation Using K-Means Clustering
Objective:
The goal was to group customers of a retail store based on their purchase history to help the store understand customer behavior and plan better marketing strategies.

Steps:
Data Loading: We started by loading a dataset with information like customers' age, gender, income, and spending score.

Data Preprocessing:

Gender Conversion: We converted gender from text (Male/Female) into numbers (1 for Male, 0 for Female) because algorithms work better with numbers.
Missing Data Check: We checked for any missing values to make sure the data was clean.
Feature Selection: We used three key features:

Age
Annual Income (in thousands of dollars)
Spending Score (a value from 1-100 showing how much a customer spends)
Data Normalization: Since the features had different ranges, we normalized them so that all features contributed equally to the clustering process.

Applying K-Means Clustering: We applied the K-Means algorithm to group customers into 5 clusters. Each cluster represents customers with similar age, income, and spending score.

Cluster Analysis: We analyzed each cluster to see how customers differed in age, income, and spending habits. We also checked the gender distribution in each cluster to see if certain groups had more males or females.

Visualizing the Clusters: We created a scatter plot showing customers' annual income and spending score. Each point was colored according to the cluster it belonged to, making it easy to see the different customer segments.

 explanation of the commands related to warnings and memory control:

  Suppressing Warnings:
  
What we did: We used a command to ignore certain warning messages from scikit-learn (the machine learning library we used).
Why we did this: Warnings are messages that let you know there could be a small issue, but it's not a big problem for your code right now. To keep the output clean and easy to read, we told Python to ignore these messages.

 Controlling Memory Usage:
 
What we did: We set a limit on how many processing units (threads) the computer uses while running the K-Means algorithm.
Why we did this: If too many threads run at once, it can use a lot of memory and slow down or crash your computer. By limiting the number of threads, we made sure the program runs smoothly without using too much memory.
