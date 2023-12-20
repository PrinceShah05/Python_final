# Python_final

**Overview**
In this assessment I wish to conduct a preliminary study of Islamophobia and it's links to stereotypical vocabularies of terrorism. My focus is on sources on news and the social media. To the same extent my study has included English news sources and tweets from 2023. It is important to note that this is a preliminary study and is essentially a test of attitudes. A deeper look at the same would incorporate frameworks of discriminatory analysis into it's research. The tools that I have used are a 'WordCloud', Named Entity Recognition and Sentiment Analysis.

This study covers the primary sources of media, as well as the most popular. Orientalist narratives produce biased information about Muslims in many spheres of life, in this study the term of "terrorism" has been selected to look at the prejudicial profiling of Muslims as terrorists in popular media. Oriental narratives harm communities not just in shaping their popular understandings, but also, getting reproduced in alternate sources of media reinforces foundational biases against communities. These narratives strip attacked communities of agency over their viewership. They damage their collective self-esteem and shape self-hatred ([Vilchis, 2023]([url](https://oxfordre.com/religion/display/10.1093/acrefore/9780199340378.001.0001/acrefore-9780199340378-e-1102))). 

On the outside, these narratives also shape an unfair dehumanization of an entire community, which justifies acts of violence against them. As an international community, we must strive to question popular narratives of hate that act as political vehicles death for communities, far be they from us, geographically, but the success of such models guarantees their replication. 

**Word cloud**
The word cloud generation was done using the code published by [Geeks for Geeks]([url](https://www.geeksforgeeks.org/generating-word-cloud-python/)https://www.geeksforgeeks.org/generating-word-cloud-python/). The inputs are using 'everything' in [News API]([url](https://newsapi.org)https://newsapi.org) and searching for the key word (q) "terrorism". The results were then cleaned and organized in a dataframe to be formed into a WordCloud. The final outcome of the WordCloud looked like this.  !

[Unknown-3](https://github.com/PrinceShah05/Python_final/assets/117305770/07c938e8-61f3-4c85-8302-dc770a3b6af3) 

The words 'Israel' and 'Gaza' are understandable due to the aggressive media attention around the ongoing war, however, the word 'Palestinian', in the context of the same war present a potentially worrying case of profiling. 

**Sentiment Analysis**
For this exercise I used a data set from Kaggle called "[Twitter on Islamophobia]([url](https://www.kaggle.com/datasets/nassimeidrissi/twitter-dataset-islamophobia-updated/)https://www.kaggle.com/datasets/nassimeidrissi/twitter-dataset-islamophobia-updated/)" (2023) which is a compilation of almost 7 months of tweets on Islamophobia on Twitter. The aim of the process was to understand the perceptions of Islamophobia prevailing on Twitter. Islamophobia denial, support or other manipulative arguments to the same end distort a prevailing form of discrimination and deny the lived experienced of millions. The analysis encountered a snag however, due to the dates being in a 'MM/DD/YYY, 00:00:00, +/- TimeZone' format for the same cell across a column. So a sample for 500 was chosen for which I manually corrected the dates so they could be read by my code. 

The mean scores ([Krisel, 2023]([url](https://github.com/rskrisel/sentiment_analysis_workshop))) for the same were recorded at around '-0.24' indicating unfavourable sentiments towards 'Islamophobia', however, the coded unfavourism here would indicate unpleasant reactions and perhaps even denialism to the same. Vitriolic conversations around 'Islamophobia' being a form of 'self-victimisation' are a part of this dataset, that may potentially explain this score. However, it is very much possible that the same sentiment can be expressed in text that is expressing disdain at practices of Islamophobia, which is indicated by several tweets in the dataset. The point remaining, that popular dialogue on islamophobia can at least be considered divisive 

**Named entity recognition** 
This exercise was aimed at establishing more direct correlations between coded biases in racial profiling of the Muslim identity. Using the same parameters mentioned above for pulling news articles from NewsAPI, I performed a named entity recognition ([Krisel, 2023]([url](https://github.com/rskrisel/NER_workshop)https://github.com/rskrisel/NER_workshop)) to examine the commonalities or usage of vernacular in articles that discuss "terrorism". The most curious finding, from the analysis on 7,041 articles, is that on running 'nationalities or religious or political groups' (NORP) the code returns "Romanian and Muslim" as the only responses. Hinting at a bias in reportage, potential profiling or a coded bias in selective authorship. The naming of one religious community from 7,041 articles on "terrorism" highlights a crystal clear bias in reportage. The definition of terrorism can thus be considered defined via a global digital archive of journalism. Which then casts doubt upon similar violence in states through a religious or ethnic lens. 
