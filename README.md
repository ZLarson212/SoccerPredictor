# Soccer Match Predictor
This notebook focuses on the sourcing and cleaning of data, engineering of features, and construction and tuning of a neural network with the goal of predicting the result of soccer matches in the English Premier League during the 2008-2016 seasons.

Analytics in the sporting world have become increasingly paramount in importance as computational, as well as monetary, resources have expanded. Sports teams and leagues have never had a larger stake in predictive power of data to optimize matchups, prevent injuries, and maintain conditioning. 

In this project, we'll be taking a look at a different side of sport: gambling. I've chosen to use data from a sportsbook because, while perhaps morally dubious, it offers a tangible treshold against which to compare the results of the model. The sports data sandbox is a wide one, with many insights and advantages to be found. The outcome of a game is the obvious first answer to provide and I'd be remiss not to use all the data at my disposal. Since there are three outcomes to a soccer match (win, draw, lose), one might think a correct prediction rate higher than 33% to be a success (in fact draws occur less frequently so that would not be completely accurate). But we will be going one step further by attempting to beat the book itself.

The sportsbook odds have a success rate as well, with the added advantage of the book's own predictive models weighted by public knowledge and opinion. As we'll see in the notebook, this is skewed a bit by having many matchups with a heavy favorite. I chose to limit my dataset to matches that did not have a favorite according to the book. In this case, the result with the best odds according to the book was correct about 41% of the time. Since we have that data point for each match, we can incorporate it into our model and thus should never predict outcomes at a worse rate. The question then becomes, can we add value to the model in order to have a higher success rate than the book? 

Ultimately, the answer is yes; we create a dataset and model that yield a 48% success rate. In the world of sports gambling, a 50% success rate on this data would guarantee a profit so perhaps that is a goal to aim for in the future. Just for fun, at the end of the notebook we find that our model would in fact have profited over the course of our dataset, however that result is mostly down to semantics. 

Thank you for reading me!
