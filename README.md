# Airline

By using Tweets, we are trying to understand what is the problem, and how can we improve the service in the business. For this reason, we are trying to predict each sentiment as positive and negative feedback.
If it is negative feedback, the company will go deep and solve the problem for costumers.

We will restrict the reviews to the top 10,000 most common words and cut the reviews after only 20 words. 
Our network will simply learn 8-dimensional embeddings for each of the 10,000 words, turn the input integer sequences (2D integer tensor) into embedded sequences (3D float tensor), flatten the tensor to 2D, 
and train a single Dense layer on top for classification.
