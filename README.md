# Clustering products by using review data set
This repository is a revision of Machine Learning repository by Chay Thawaranont as part of a project in Machine Learning Spring 2021 class for Parsons School of Design,[learn more](https://github.com/Chayanitoey/machinelearning/tree/main/final_assignment_3).

## Data 

**Data: Amazon Fine Food Reviews**. The Amazon Fine Food Reviews dataset consists of 455,000 food reviews Amazon users left up to October 2012. Learn more about this [data set](https://github.com/Chayanitoey/GP3/blob/main/clusteringGraph.jpg)

Using [KMeans](http://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) clustering to create a **recommendation engine.** 
Objctive: Group the right features and number of clusters when the products in each cluster "seem" like they belong together. 


## Clustering with K-means: 

![results](https://github.com/Chayanitoey/GP3/blob/main/clusteringGraph.jpg)

Looking from the line graph above, '54'is shown as the optimal k-mean since the point represents the best evaluation of the data set. 
The point at '54' is the most descending one based on the range of 30 to 60 clusters and Intertia. Therefore, there will be 55. clusters in total

## Word Cloud : 

Cluster 1 : 
![wc1](https://github.com/Chayanitoey/GP3/blob/main/wordcloud_samples/WC1)

Cluster 2 : 
![wc2](https://github.com/Chayanitoey/GP3/blob/main/wordcloud_samples/WC2)

Cluster 3 : 
![wc3](https://github.com/Chayanitoey/GP3/blob/main/wordcloud_samples/WC3)

Cluster 4 : 
![wc4](https://github.com/Chayanitoey/GP3/blob/main/wordcloud_samples/WC4)

Cluster 5 : 
![wc5](https://github.com/Chayanitoey/GP3/blob/main/wordcloud_samples/WC5)


Generating wordcloud visualizatiion to depict all 54 clusters in a better view. The images above are the representation of the first 5 clusters and here are the first 10 example reviews from those first 5 clusters 
```
--------------------------------------------------
cluster:  1
cluster size:  (3445, 3)
         ProductId  cluster                                               Text
135940  B0014ATRV8        1  I wanted good quality, fresh chamomile tea.  T...
9372    B00020HHHC        1  After reading reviews from baby sites, I was r...
142460  B00188S3PM        1  I ordered this to serve at a "tea" where I was...
290334  B00412W76S        1  I've a difficult time drinking red raspberry l...
8935    B00020HHAO        1  I usually dont like black herbal tea, but this...
95350   B000M0F58U        1  In ayurvedic medidicne and in yoga exxercises ...
136094  B0014AUJII        1  Helped when I had a cold and soar throat and c...
8904    B00020HHAO        1  This is an outstanding product!! The test is g...
139706  B0016B7Z32        1  Helped when I had a cold and soar throat and c...
136321  B0014B0HWK        1  This is a good tasting tea at a great price. I...
--------------------------------------------------
cluster:  2
cluster size:  (1262, 3)
        ProductId  cluster                                               Text
102    7310172001        2  We have used Pro-Treat Beef Liver, Freeze Drie...
11783  B0002DGRPC        2  My dog enjoys these treats in moderation.  Bec...
11964  B0002DGRRA        2  I am a white, white Maltese. Before Mommy star...
11838  B0002DGRQ6        2  My 4 month old aussie loves these! Whenever he...
11981  B0002DGRRA        2  This is a great treat for dogs, but do read th...
11874  B0002DGRQ6        2  This a wonderful treat.  my 3 Labs just love t...
12352  B0002DGRZC        2  I've purchased several different brands of liv...
11751  B0002DGRPC        2  My dogs love this stuff! They will do anything...
12326  B0002DGRZC        2  Freeze dried liver has a hypnotic effect on do...
12368  B0002DGRZC        2  We have used Pro-Treat Beef Liver, Freeze Drie...
--------------------------------------------------
cluster:  3
cluster size:  (4097, 3)
         ProductId  cluster                                               Text
206239  B001RVFEP2        3  These are great to have around as a snack... i...
116769  B000VK8AVK        3  About 3 months ago I stayed at a hotel in Los ...
360565  B007M832YY        3  I was really excited to try these out as salt ...
116762  B000VK8AVK        3  I love potato chips and when I go at it I alwa...
215511  B0026KNQSA        3  So my cafe at work switch to a bunch of chips ...
215870  B0026KNQSA        3  I have said it once and I will say it again..T...
349317  B006HYLW32        3  I'm a little bit of Pop Chip addict, so was ve...
116664  B000VK8AVK        3  These taste like roasted marshmallows/sweet po...
349550  B006HYLW32        3  I have gained weight *not telling you how much...
215828  B0026KNQSA        3  Pop chips are great but you really have to be ...
--------------------------------------------------
cluster:  4
cluster size:  (1012, 3)
         ProductId  cluster                                               Text
148145  B001AHL6CI        4  True to the name, Food Should Taste This Good,...
124127  B000YSRK7E        4  I tried these for the first time about a year ...
147769  B001AHJ2D8        4  Love these chips. They taste great and I love ...
148125  B001AHL6CI        4  The Jalapeno tortilla chips have a great taste...
148033  B001AHJ2FQ        4  Was waiting for our airplane & wanted somethin...
124524  B000YSTIL0        4  These were a change of pace so to speak. I tho...
147800  B001AHJ2D8        4  This chip has a little tomato taste but the ja...
147665  B001AHFVHO        4  I bought these at a grocery store and I had al...
147915  B001AHJ2FQ        4  If you have to eat gluten-free and wonder what...
148141  B001AHL6CI        4  You won't find any MSG, hydrogenated oils, or ...
--------------------------------------------------
cluster:  5
cluster size:  (2059, 3)
        ProductId  cluster                                               Text
74007  B000H0ZJHW        5  My german shorthaired pointer, Tim loves prett...
74594  B000H1217M        5  Zuke's is a great natural mini treat. They are...
74889  B000H1217M        5  These treats may be great for some dogs, but m...
19207  B0007A0AQM        5  My 4 month old basenji Really likes these and ...
74168  B000H0ZJIG        5  Love these soft treats! Great size to use duri...
73856  B000H0ZJHW        5  My two "girls" love these training treats.  I ...
19554  B0007A0AQW        5  These dog treats are great for my new puppy an...
74222  B000H0ZJIG        5  Less than 24 hours after my four year old dog ...
73992  B000H0ZJHW        5  My dog and I both love Zuke's.  The mini natur...
19785  B0007A0AQW        5  my dog prefers the peanut butter ones. for som...
--------------------------------------------------
```



## Describe the Clusters: 

In order to describe what content the individual clusters stand for, having a description of the clusters will be benificial for further applications. To do this, the number of certain amount of samples, in this case, we'll be using 10 reviews per cluster. Those 10 reviews in each cluster will be used as an input for GPT3 itself to generate descriptions. I have decided to use the “davinci-instruct-beta-v3” model vom the [OpenAI API](https://beta.openai.com) because of its expressiveness.

Here is the function that was used to generate the cluster description : 

```
  def gettopic(self, n_samples):
        merged = self.merge_labels()
        num_clusters = self.model_instance.cluster_centers_.shape[0]
        for i in range(1, num_clusters): 
            print(f"Cluster {i} Topic:", end=" ")
            
            cluster = merged.loc[merged['cluster'] == i]
            reviews = cluster.sample(n_samples)
            response = openai.Completion.create(
                engine="davinci-instruct-beta-v3",
                prompt=f"What is the product that the following reviews talk about?\n\nReviews:\n\"\"\"\n{reviews}\n\"\"\"\n\nTopic:",
                temperature=0,
                max_tokens=64,
                top_p=1,
                frequency_penalty=0,
                presence_penalty=0,
                timeout = 60
            )
            print(response["choices"][0]["text"].replace('\n',''))
```
            


The prompt assigned for GP3 is **'What is the product that the following reviews talk about?'**, from the review input, GP3 will generate topic or product that is most relevant and best respresentation of that cluster. 

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
## Conclusion 

The topics that were generated by GP3 are clearly giving us the advantage and save time in manual labeling, however, there are some duplicates that would need human inteligence to support and further explore (for example 'tea' in cluster #28,#37 and #38). 
