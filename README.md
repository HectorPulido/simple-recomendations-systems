# Simple recomendations systems

This repository contains an implementation of a hybrid recommendation system combining both collaborative filtering and content-based filtering. This project contains examples of Collaborative Filtering, Content-Based Filtering and Hybrid models.

>[!WARNING]
> This is a proof-of-concept project and is not intended for production use. The code is provided as a reference for building recommendation systems using different techniques.

## Technologies
Python for the core logic.
Pandas, NumPy for data handling.
Scikit-learn for TF-IDF vectorization and cosine similarity.

## How It Works: Collaborative Filtering
Collaborative filtering is used to recommend items based on user-item interaction data (e.g., ratings). Users with similar preferences are grouped together, and their ratings are used to predict the user's ratings for unseen items. In this repository, we implemented user-based collaborative filtering with the cosine similarity between users.

### Key Steps:

1. Normalize user ratings by subtracting each user's average rating.
2. Calculate cosine similarity between users.
3. Predict ratings for unscored items based on the weighted sum of other users' ratings.

## How It Works: Content-Based Filtering
Content-based filtering recommends items based on the characteristics of the items themselves. Here, we use TF-IDF to vectorize the descriptions of items and calculate cosine similarities between item descriptions to recommend similar items to users.

### Key Steps:

1. Convert item descriptions into TF-IDF vectors.
2. Compute cosine similarity between items.
3. Recommend items that are similar to the ones the user has already interacted with.


## How It Works: Hybrid Model
The hybrid model combines both collaborative filtering and content-based filtering. The content-based information (item descriptions) is used to calculate item similarity scores, while the collaborative filtering information (user-item interactions) is used to calculate user-item similarity scores. The final recommendations are generated by combining the predictions of both models using a weighted average.

### Key Steps:

1. Use collaborative filtering to calculate the user-item similarity scores.
2. Use content-based filtering to calculate the item similarity scores.
3. Combine the predictions of both models using a weighted average to generate final recommendations.

## Future Improvements
* Incorporate additional generic metadata.
* Handling large-scale data: Explore optimizations for working with larger datasets, such as matrix factorization or distributed systems.
* A dockerized version of the project.
* More advanced deep learning models: Experiment with more complex neural network architectures like attention mechanisms, autoencoders, or graph-based networks.

## Future Improvements: Neural Networks
Neural networks are introduced to learn complex user-item interactions. Neural Collaborative Filtering (NCF) is implemented using Keras to model user-item relationships via embeddings and dense layers.

>[!WARNING]
> This is not implemented in this repository, but it is a potential future improvement.

### Key Steps:

1. Create embeddings for users and items.
2. Use a neural network with hidden layers to predict the interaction (e.g., ratings) between users and items.
3. Train the model using historical data and predict user preferences for new items.



## Contributing

Your contributions are greatly appreciated! Please follow these steps:

1. Fork the project
2. Create your feature branch `git checkout -b feature/MyFeature`
3. Commit your changes `git commit -m "my cool feature"`
4. Push to the branch `git push origin feature/MyFeature`
5. Open a Pull Request

## License

Every code made by me in this repo is under the MIT license.

## Contact

<div align="center">
<h3 align="center">Let's connect 😋</h3>
</div>
<p align="center">
<a href="https://www.linkedin.com/in/hector-pulido-17547369/" target="blank">
<img align="center" width="30px" alt="Hector's LinkedIn" src="https://www.vectorlogo.zone/logos/linkedin/linkedin-icon.svg"/></a> &nbsp; &nbsp;
<a href="https://twitter.com/Hector_Pulido_" target="blank">
<img align="center" width="30px" alt="Hector's Twitter" src="https://www.vectorlogo.zone/logos/twitter/twitter-official.svg"/></a> &nbsp; &nbsp;
<a href="https://www.twitch.tv/hector_pulido_" target="blank">
<img align="center" width="30px" alt="Hector's Twitch" src="https://www.vectorlogo.zone/logos/twitch/twitch-icon.svg"/></a> &nbsp; &nbsp;
<a href="https://www.youtube.com/channel/UCS_iMeH0P0nsIDPvBaJckOw" target="blank">
<img align="center" width="30px" alt="Hector's Youtube" src="https://www.vectorlogo.zone/logos/youtube/youtube-icon.svg"/></a> &nbsp; &nbsp;
<a href="https://pequesoft.net/" target="blank">
<img align="center" width="30px" alt="Pequesoft website" src="https://github.com/HectorPulido/HectorPulido/blob/master/img/pequesoft-favicon.png?raw=true"/></a> &nbsp; &nbsp;

