"# featuretoolsdemo" 

The first method (with a helper function), plotstuff(dataset), is a computationally-inexpensive way to visualiza the data, and although it has not been fully polished I believe it handles the different quantitative and qualitative data types in an intuitive way. This would allow clients to get a good sense of what the feature matrix is telling them, making the actual data science part more palatable.

The second method, plotting2d(set), is a very rudimentary way to visualize the first-order relationships among the variables in the data. It just plots everything in 2D histograms, although it is only able to handle quantitative data types.

In this directory, there is included a demo of fitting some scipy.stats distributions to a given set of data (in this case, the duration newspaper subscriptions), and determining which are best from a comparison of Q-Q (quantile-quantile) plots and p values (the likelihood that the given data could be generated from a random distribution with the found parameters). These distributions could then be used to model the data, simulating what can be expected if something about the system were to be changed. This could be used to give client companies a way to "test out" new business strategies without needing to risk their actual business. The entire process can be automated very easily, and random samples can be generated even more easily. I could make this work for any data, fitting the different distributions and automatically selecting the best one. The simulation would be more difficult to automate, as depending on what a client wants simulated it may require different changes to an initial configuration (parameters, constraints), but getting a simulation "true-to-life" of their existing data should be quite simple. This was done with data other than the featuretools demo set because that data had a less interesting shape to showcase this process. This dataset was borrowed from ORIE 4580 at Cornell University.
