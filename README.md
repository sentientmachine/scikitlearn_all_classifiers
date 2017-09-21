# scikitlearn_all_classifiers

# Python program output:

![Imgur](https://i.imgur.com/uYNKozw.png)


Demoed on Linux x86_64:

# Libraries to install

    pip install -U scikit-learn

# data sets used:

    sklearn.datasets: make_moons, make_circles, make_classification
    
    http://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_moons.html
    
    http://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_circles.html
    
    http://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_classification.html
    
    
# Run it: 

    python main.py

# How long does it take:

Between 10 and 20 seconds.

# Where is this from?

http://scikit-learn.org/stable/auto_examples/classification/plot_classifier_comparison.html

# Newbie help, what am I looking at?

All of these algorithms are supervised learning algorithms.

The feature data is coming in as the x, y points. The supervisory signal is yes or no, illustrated here as red and blue dots. The hazy background represents what the machine learning algorithm predicted for that area.

The rows are associated with each other in that the machine learning algorithm across the top is applyied to that data set.
For the top row, the ideal (perhaps overfit) machine learning algorithm for the job is decision tree or nearest neighbors. Poor algorithms are neural net and adaboost because they project bias that isn't there.

On the 2nd row, the ideal (perhaps overfit) machine learning algorithm is the niave bays or neural net. Bad ones are linear SVM and adaboost.

On the 3rd row decision tree or nearest neighbors is best, poorest are adaboost and linear SVM.
The machine learning algorithm doesn't have access to all the points when training, so that's how we know a positive result is good.

What this illustrates is the "no free lunch theorem" https://en.wikipedia.org/wiki/No_free_lunch_theorem
Which states that no single machine learning algorithm can optimally classify all input sets of data. Either your algorithm will be good at one or poor at another, or poor at one and good on the other. The only way to bypass the "no free lunch" algorithm is to develop an ensamble of machine learning algorithms which have introspective capabilities to look at its own poor performance relative to to the task at hand, and toss out and re-learning using a superior model.

When this is created, the age of humans being the intellectually dominant phenomenon in the world will be over, and take second place to giant buildings full of Titan X GPU's.
