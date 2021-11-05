
# Building The Framework For A Spotify Recommendation System

In this project, I took over 7,000 songs using the Spotipy API and a dataset from Kaggle, inspected, cleaned, and merged the data to create models and use machine learning methods with the intention of returning to create a recommendation system.







![Logo](https://storage.googleapis.com/pr-newsroom-wp/1/2018/11/Spotify_Logo_CMYK_Green.png)
## Methods
First, I combed through my own data obtained through Spotipy, the lightweight API for Spotify. I used several loops as well as various built in methods of the API to create a dataframe of my own music I could explore, clean, and eventually model. 

After this, I decided to use a playlist from Kaggle to sample from, and create models that could: 1) Differentiate between my music and the sample music from this secondary dataset, and 2) display and explore what makes the music I enjoy similar and different to the music randomly chosen from the other set.

Next, I merged all aspects of the information obtained from the API, which include genres, song popularity, and different audio features that could be compared to one another. I combined the two datasets on a binary feature: whether or not the music belonged to my liked songs. Here's a look at some of the things that jumped out during my exploratory data analysis: 

![Unknown-3](https://user-images.githubusercontent.com/55816424/140588917-ececfb79-cf93-4986-968e-e9bf1ddb387c.png)

![Unknown-4](https://user-images.githubusercontent.com/55816424/140588949-5c8b141b-8a05-4d1b-9088-e14e0362b51f.png)


## Modeling

I instantiated several models and created a function that would allow me to easily reproduce confusion matrices and accuracy for each model I used. My best performing models were the Ada Boost and XGB Boost Classifiers, with both models returning perfect accuracy and precision.

![Unknown](https://user-images.githubusercontent.com/55816424/140588970-b8cb5b42-48f9-4414-b596-180025906099.png)

![Unknown-2](https://user-images.githubusercontent.com/55816424/140588974-b6d21d04-e9d0-4869-87d4-7546e174ff72.png)


## Post Modeling EDA

There were a few things I considered after the modeling phase, which included different ways to visualize and compare the data that I had at my disposal. A few key features and their interactions jumped out:

![Unknown-5](https://user-images.githubusercontent.com/55816424/140589007-e951e9c1-84c8-4ee5-86ad-eae80db8d522.png)

![Unknown-6](https://user-images.githubusercontent.com/55816424/140589021-2ba28ab3-b4d5-4250-99bd-92e2cc2fc5b5.png)



The 1 in these graphs represents music that is in my liked songs, while a 0 represents those which are not.

## Summary / Next Steps

To improve this project in the future, I would take data from more sources as they become available, and look into more features to see what other insights could be drawn. I would additionally build a recommendation system that users could interact with to find new and exciting music based on things they already like!

