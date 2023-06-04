# A Differential Machine Learning Approach for Calculating Deltas under the Heston Model

Project by: Elain Balderas, Nina McClure, Akash Yadav 

## Abstract 

This project introduces a novel technique called "differential machine learning" to estimate option prices and their deltas under the Heston model. Although option pricing under the Heston model has been done in the past, predicting sensitivities like deltas is not as straightforward, as it involves computing the derivatives of an estimated price function, which are historically not good approximates. Differential machine learning aims to remedy this issue with the aim of approximating the shape of the underlying function, by training on differentials of the target variable with respect to the input variables. Using a twin network architecture, we find that training on pathwise differentials and option price labels yields significantly  better results compared to training on price labels alone. Moreover, the performance of the differential twin network surpasses standard training whether we use a train-test split on a dataset generated by Monte Carlo simulations, or a noisier training set generated via the least squares Monte Carlo method. Notably, our network is capable of computing both prices and deltas much faster in a single pass.

## Previous work

a) Lui, S., Oosterlle, C. W. and Bohte, S. M. Pricing Options and Computing Implied Volatilities Using Neural Networks, Risk, 2019

b) Ruf, J. and Wang., W. Neural networks for option pricing and hedging: a literature review, Journal of Computational Finance, 2020

c) Huge, V and Savine, A. Differential Machine learning, Risk, 2021

_This repository is part of a master project submitted to fulfill the requirements of the Master of Program in Data Science Methodology at the Barcelona School of Economics._
