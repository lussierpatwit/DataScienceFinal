# DataScienceFinal
Nathan Dunn, Paul Lussier
notebook exploring the big 5 personality test with machine learning

Personality--one's patterns of thinking, feeling, and behaving--determines one's satisfaction and success in almost every significant domain in life. From friendships, to romantic relationships, to one's profession, a personality that matches our engagements in life is a foundational condition on which our happiness depends. However, personality is very poorly understood. When most people attempt to describe a personality, particularly their own, typically they mention something that is really just a quirk, preference, or interest. Formally(or at least academically), personality The Big Five personality traits or OCEAN model is the most robust and widely accepted paradigm in personality psychometrics to date. 

This model consists of 5 traits on a spectrum which are Extraversion, Agreeableness, Neuroticism, Conscientiousness, and Openness. Extraversion is characterized by reactivity to external activity/stimuli/situations. Those high in extraversion tend to be more group oriented, talkative, assertive, and outwardly energetic. Neuroticism is essentially the volatility of a person's emotional state. High neuroticism is characterized by a tendency to experience negative emotions stronger and a lesser ability to deal with stress. Conscientiousness is a tendency towards self-discipline, duty, order, and an affinity for boundaries(in a variety of contexts). Agreeableness is a measure of concern for social harmony. Agreeable people are kind, trusting, warm, nurturing, and optimistic. Openness indicates an appreciation for novel experiences, beauty, creative endeavor, new ideas. People high in openess are thought to be imaginative, curious, and willing to try new things.
Though several of these traits sound exclusively positive or negative, none of them are, and being too high or low in any of them has both pros and cons. The goal of this project was to see if we could find personality 'types' or common configurations of these traits using some survey data from kaggle and kmeans clustering.

The data used came from Kaggle and was collected through an online take it yourself perosanlity test. Looking at the raw data you can glean some interesting information about who was actually taking this test. Our plots show that the vast majority of the participents were American, with the other english speaking countries following.

Materials used for this analysis were, numpy, pandas, matplotlib, seaborn, scikit, and yellowbrick, a python tool used to visualize the elbow intergeal to KMeans clustering. The code waws written in Jupytr Notebooks, and Google Colabs. 

An interesting article on Psycology today looks at a similar use of Kmenas clustering and concludes that there are a small number of personality profiles relatively speaking.
https://www.psychologytoday.com/us/blog/seeing-what-others-dont/201908/how-many-personality-configurations-exist
The tools used in this study were refined and had good documentation. However, the notebooks are run on teh cloud and contrary to the expected ease of collaboration, getting the same things on two computers proved difficult. Another challenge was that our dataset was too large for some methods to handle and threw errors for infinite numbers.

Preliminary findings seem to indicate that conscientiousness and openness are often seen together when both values are 3 or above. This seems contradictary since mainstreram academia defines Conscientiousness as liking order and boundries, characteristics that do not go with thier definition of Openness.
Another interesting find was that there is an even distribution over the clusters made by the KMean model. other than 0, all cluster combinatins were fairly evenly distributed. This means that there are an approximately even number of people whos personality can be tied to a single trait, two, three, four, and all five. Interesting is that the curve is slightly dipped in the middle as opposed to a more traditional normal distribution we would have thought to find.  


