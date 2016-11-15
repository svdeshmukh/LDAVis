# LDAVis
Business Analytics LDAvis 

                                               - VISUALISATION -  

(https://htmlpreview.github.io/?https://github.com/svdeshmukh/LDAVis/blob/master/ToolReviews/index.html)

-----------------------------------                                                  

*Siddhant Deshmukh*

*Business Analytics – Weekday Course*

*Assignment 8 – Text as Data*

                                                    - CASE - 

In this document, we fit an LDA Topic Model to the Amazon Home Improvement Tools Dataset found here. To fit the model, we used the R package lda and to visualise the output we used LDAvis.
Below I have pasted a few screenshots of the script used to create this visualisation – 

-	Loading the dataset and cleaning the corpus

![image](https://cloud.githubusercontent.com/assets/22182362/20296031/890c2aea-aad6-11e6-8725-d07cab00f270.png)

-	Fitting the model

![image](https://cloud.githubusercontent.com/assets/22182362/20296044/a11d3cfa-aad6-11e6-8cf2-49d87bc9fc86.png)

After fitting the model we are ready to create a JSON file and run the visualisation. In order to run the visualisation we need to first create a JSON object to feed our visualisation. 

![image](https://cloud.githubusercontent.com/assets/22182362/20296049/aaa9115e-aad6-11e6-920e-b2dd346f4eaa.png)

I have created a visualisation of the top 15 topics cross-referenced with the top 30 most salient terms. By hovering over different topics and different words, we can see that certain terms appear frequently in certain topics.

For example, looking at the top 30 most salient terms we can see that the word ‘light’ tops the list. By hovering over the word light we further see that this word appears in 3 topics, namely topic 2,10 and 12 as the most common word in each of these 3 topics. By further perusing the words appearing in these topics we see that even though the word ‘light’ appears frequently, the context it is used in varies from topic to topic. 

- Topic 2 suggests that it might have something to with flashlights, battery and intensity. 
- Topic 10 suggests it has more to do with home fittings such as CFL lamps and Wattage. 
- Topic 12 suggests that it has more to do with automated lighting fixtures such as motion sensing lights etc. 

As another example let us look at the 5th most used word that is 'blade'. Hovering over the word 'blade' we see that it most frequently appears in topics 8,7,6 and 1. By hovering over these topics we are able to identify the various contexts in which the term blade is being used.

- Topic 8 suggests that blade is used in the context of sanding or sharpening tools such as wood grinders etc.
- Topic 7 suggests that the word blade is used in the context of a multitool possessing pliers/blades/scissors etc.
- In Topic 1 the word blade is actually at the bottom of the top 30 used words. Here it is probably used in the context of clamping/adjusting equipment manufacted by companies such as Bosch, DeWalt etc.

In conclusion, by using the LDAvis package to create a visualisation of our model, we are able to assess the frequency and context of words and topics across an extremely large dataset. By setting topic parameters and relevance metrics, we are presented with a list of top 30 words that we may then cross reference across the most popular topics. Not only can we identify the overarching theme of various topics, but we can also identify the context in which certain terms appear within these topics.

------------------




