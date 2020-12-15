# DataScienceFinal
Nathan Dunn, Paul Lussier Exploring the Big 5 personality test with Kmeans Clustering

#Introduction
	Personality--one's patterns of thinking, feeling, and behaving--determines one's satisfaction and success in almost every significant domain in life.
From friendships, to romantic relationships, to one's political leanings, the effects of personality are profound, according the literature referenced below. However, 
personality is still poorly understood. Though imperfect, The Big Five personality traits or OCEAN model is generally considered the most robust and is the most widely accepted
paradigm in personality psychometrics to date. This model consists of 5 traits on a spectrum which are Extraversion, Agreeableness, Neuroticism, Conscientiousness, and Openness. Extraversion is characterized by
reactivity to external activity/stimuli/situations. Those high in extraversion tend to be more group oriented, talkative, assertive, and outwardly energetic.
Neuroticism is essentially the volatility of a person's emotional state. High neuroticism is characterized by a tendency to experience negative emotions stronger and 
a lesser ability to deal with stress. Conscientiousness is a tendency towards self-discipline, duty, order, and an affinity for boundaries(in a variety of contexts). 
Agreeableness is a measure of concern for social harmony. Agreeable people are kind, trusting, warm, nurturing, and optimistic. Openness indicates an appreciation for novel
experiences, beauty, creative endeavor, new ideas. People high in openess are thought to be imaginative, curious, and willing to try new things. 
Though several of these traits sound exclusively positive or negative, none of them are, and being too high or low in any of them has both pros and cons. The goal of this 
project was to see if we could find personality 'types' or recurring configurations of these traits using some survey data from kaggle and kmeans clustering.
	The data used came from Kaggle and was collected through an online personality test. About half the dataset's columns was irrelevant for our purposes, with attributes
like the width and height of the screen on which the participant took the test and the time it took a participant to answer a question. Removing these, our plots showed that 
the vast majority of the participants were American, with other English speaking countries following. We took care to omit the responses from IP addresses that took the survey
more than once so as to prevent a single participant from submitting multiple observations. Some of the statements were put in the negative so as to indicate a lesser score in
the trait in question, so some feature engineering was required to make sure all numbers were on a uniform scale. The materials used for this analysis were, numpy, pandas, matplotlib
, seaborn, scikit, and yellowbrick, a python tool used to visualize the elbow method of finding the 
optimal number of clusters for a Kmeans model. The code was written in Jupytr Notebooks, and Google Colabs.
	One challenges was that the notebooks are run on the cloud and contrary to the expected ease of collaboration, getting the same things on two computers proved difficult.
Another was that our dataset was too large for some methods to handle and threw errors for infinite numbers.

#Findings
	Preliminary findings seem to indicate that conscientiousness and openness are often seen together when both values are 3 or above. 
This seems contradictary since mainstream academia defines Conscientiousness as liking order and boundries--characteristics that do not intuitively square with the definition
of Openness. Another interesting find was that there is an even distribution over the clusters made by the KMean model. Other than 0, all cluster combinations were fairly evenly
distributed. This means that there are an approximately even number of people who's personality can be tied to a single trait, two, three, four, and all five. Unsurprisingly, no
profile had extremely large or small values for any traits. Our most important finding is the 6 personality types, which proved our original hypothesis right that there would be
a small number of profiles relative to the size of the dataset, and also relative to other personality tests. Some qualifications must be made. The test is based on word associations,
specifically in English so there will likely be some variation across languages and levels of literacy that is unaccounted for. However, we believe that if a more comprehensive dataset
could be obtained, preferably with more information such as age and sex, our project could potentially be used in tandem with many other projects that were presented such as the spotify 
recommender, movie recommender, and twitter/sentiment analysis to improve results.


