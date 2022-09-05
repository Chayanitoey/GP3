# Clustering Product on Amazon by using a review data set
This repository is a revision of Machine Learning repository

## Data 

**Data: Amazon Fine Food Reviews**. The Amazon Fine Food Reviews dataset consists of 455,000 food reviews Amazon users left up to October 2012. 

Using [KMeans](http://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) clustering to create a **recommendation engine.** 
Objctive: Group the right features and number of clusters when the products in each cluster "seem" like they belong together. 


#### Clustering
https://github.com/Chayanitoey/machinelearning/blob/main/final_assignment_3/K_mean.jpg
Looking from the graph ![results](https://github.com/Chayanitoey/machinelearning/blob/main/final_assignment_3/K_mean.jpg)
'54'is shown as the optimal k-mean since the point represents the best evaluation of the data set. 
The point at '54' is the most descending one based on the range of 30 to 60 clusters and Intertia. Therefore, there will be 55. clusters in total

### Word Cloud : 

![results](https://github.com/Chayanitoey/machinelearning/blob/main/final_assignment_3/assignment3_1.jpg)

Generating wordcloud visualizatiion to depict all 54 clusters in a better view. 

### Describe the Clusters: 
In order to describe what content the individual clusters stand for, having a description of the clusters will be benificial for further applications. To do this, the number of certain amount of samples, in this case, we'll be using 10 reviews per cluster. Those 10 reviews in each cluster will be used as an input for GPT3 itself to generate descriptions. I have decided to use the “davinci-instruct-beta-v3” model vom the [OpenAI API] (https://beta.openai.com) because of its expressiveness.

The prompt assigned for GP3 is 'What is the product that the following reviews talk about?', from the review input, GP3 will generate topic or product that is most relevant and best respresentation of that cluster. 

Here are a list of products of all 50 clusters generated by GP3 : 
```
Cluster 1 Topic:  Throat Relief Tea
Cluster 2 Topic:  freeze-dried liver treats
Cluster 3 Topic:  Potato chips
Cluster 4 Topic:  Chips
Cluster 5 Topic:  Dog treats
Cluster 6 Topic:  Cliff Bar White Chocolate Macademia Nut Granola Bars
Cluster 7 Topic:  a lickable pet treat
Cluster 8 Topic:  Canidae dog food
Cluster 9 Topic:  coffee
Cluster 10 Topic:  canned cat food
Cluster 11 Topic:  Vita Coco Coconut Water
Cluster 12 Topic:  A type of food for cats
Cluster 13 Topic:  black tea
Cluster 14 Topic:  trail mix
Cluster 15 Topic:  KIND PLUS Pomegranate Blueberry Pistachio bars
Cluster 16 Topic:  Licorice Spice Tea
Cluster 17 Topic:  Hemp Seed
Cluster 18 Topic:  Kellogg's Crunchy Nut cereal
Cluster 19 Topic:  Cat food
Cluster 20 Topic:  potato chips
Cluster 21 Topic:  a dietary supplement
Cluster 22 Topic:  Beef jerky
Cluster 23 Topic:  Blue Diamond Almonds
Cluster 24 Topic:  Beef Jerky
Cluster 25 Topic:  coffee
Cluster 26 Topic:  coffee pods
Cluster 27 Topic:  KIND Fruit and Nut bars
Cluster 28 Topic:  Tea
Cluster 29 Topic:  Kitten food
Cluster 30 Topic:  bread
Cluster 31 Topic:  Vitamin Squeeze Energy Drink
Cluster 32 Topic:  Iced Tea
Cluster 33 Topic:  Wellness Core Natural Grain Free Dry Dog Food
Cluster 34 Topic:  coffee
Cluster 35 Topic:  Newman's Own Organics Adult Dog Food
Cluster 36 Topic:  Dog food
Cluster 37 Topic:  Tea
Cluster 38 Topic:  Tea
Cluster 39 Topic:  Hazelnut coffee
Cluster 40 Topic:  Spicy chips
Cluster 41 Topic:  green tea
Cluster 42 Topic:  facial moisturizer
Cluster 43 Topic:  gluten free pretzels
Cluster 44 Topic:  pouches of baby food
Cluster 45 Topic:  Temptations cat treats
Cluster 46 Topic:  coffee
Cluster 47 Topic:  Grain-free cat food
Cluster 48 Topic:  Keurig coffee
Cluster 49 Topic:  Bahlsen Delice Cookies
Cluster 50 Topic:  hot chocolate mix
Cluster 51 Topic:  canned cat food
Cluster 52 Topic:  energy bars
Cluster 53 Topic:  Butterscotch hard candies
Cluster 54 Topic:  toaster pastries
```
