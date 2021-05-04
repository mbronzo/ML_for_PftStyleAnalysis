# ML_for_PftStyleAnalysis

This repository contains a simple Jupyter Notebook to apply some Machine Learning tools available on scikit-learn to Sharpe's Portfolio Style Analysis.
It progressively build a more sophsticated approach, starting from simple regressions building up to Support Vector Machines, Trees, Ensemble Models and ultimately Neural Networks.

I would like to point out this was developed as a final project for a Machine Learning class, so it has limitations, nevertheless the main objective is to provide an initial framework for time series analysis and a good starting point for understanding the many options available on scikit-learn (with some ready-to-use receipts).

While this can be an interesting framework to start an analysis it definitely doesn't constitute a rigorous approach and can be improved. Results overall are in line with what can be achieved by a tradional approach to Sharpe's Portfolio Style Analysis.

One of the major limitation of such analysis is indeed the size of the datasets, unfortunately I only had 5 years of daily returns, from which weekly returns are calculated. This is actually a double-edge sword, as it reduces the overall noise on data as well as the size of the training set.
The methodology applied was to train the models on 4 years of data (208 weekly returns) and test them on 1 years of weekly returns (52 weekly returns). Most of the models tested, especially more sophisticated ones requires a much larger sample to yield reasonable results. This can be seen especially in Ensemble models and NN which can easily lead to overfit if the training set is not large enough. Unfortunately this is exactly what happened and the promising results in the training set were not achieved in the test set.
Overall I believe this to be one of the major issue of this project.

NB: It is not intended as legal, financial or investment advice and should not be construed or relied on as such. Before making any commitment of a legal or financial nature you should seek advice from a qualified and registered legal practitioner or financial or investment adviser.
