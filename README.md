# Project: Deep Parametric PDE Method

## Overview
This project contains a discussion and a toy implementation of the method presented in the research paper "[<i>The deep parametric PDE method and applications to option pricing</i>](https://doi.org/10.1016/j.amc.2022.127355)" of K. Glau and L. Wunderlich. We solve the problem of pricing a European basket put (and call) option for $d=2$ assets, based on a highway neural network. A short summary of our work, used for our project defense, is available in the file [slides](slides.pdf).

## Features
- Implementation of a highway neural network using `keras` and `tensorflow`.
- Definition of the loss and training procedure based on a least squares approach and integration of a no-arbitrage bound.
- Visualization n°1: option price, residual (option price minus no-arbitrage bound), and error (compared to a reference pricer) surfaces based on the two assets spot prices.
- Visualization n°2: comparison of option price vs. reference option price for randomly sampled points in the domain.

## Requirements
- See [requirements.txt](requirements.txt) for the list of required packages.

## Running the Algorithm
Open the file [notebook.ipynb](notebook.ipynb) and follow these steps:
1. Set up parameters and run the notebook.
2. You can either load a pre-trained model for a call/put available in the folder [models](models/) by setting `load_model=True` or train a new model by setting `load_model=False`. If `save_model=True`, the model will be saved in the [models](models/) folder.

## To go Further
Look at the [report](report.pdf) for a detailed investigation of the Deep Parametric PDE Method and a literature review.

### Authors
- [MICHAL Tangui](https://github.com/mtangui)
- [PÉCHEUL Ronan](https://github.com/Dracdarc)
- [SANGLIER Nathan](https://github.com/Nathan-Sanglier)