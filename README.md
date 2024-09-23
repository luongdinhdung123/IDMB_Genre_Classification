# IMDB Genre Classification

This project focuses on classify the genres of movies, based on IDMB dataset, which is extracted from [Movielens dataset] (https://grouplens.org/datasets/movielens/10m/) by our professor. By using pretrained models and some algorithms, we come up with 4 methods of classifying movie genres.

1. `vgg19+hf.ipynb`: We think that the first kinds of data that we need to solve the problem are **images and titles** of the movies. This file is developed under that idea, so that given a new image and a new title, the model may know which kind of genre will have in that movie

2. `vgg19+mistral.ipynb`: We think that the title of the movie alone might not be enough for the model to learn.   That is why, we decided that instead of using the images and titles like the first method, we will use images and summaries of the movies, with the summaries could be taken from the given title.

3. `mistral+user.ipynb` : This method is fairly straightforward. We just use all the data that we could have, including **images, summaries** (we get this from the title, same from the second method), **users’ information and users’ rating** to guess what movies.

4. `recommender_st.ipynb` : During the experiment, we have another idea, which based on the recommender systems on lots of websites: Some websites could recommend the products we like, just by using the tags of the product we had previously bought or give positive comments about. So, what if we only use just the ratings? This module is developed under that idea
