# Computational Neuroscience Final Project

Elizabeth Frey

PSYC 40 / COSC 16

Fall 2023


## File Descriptions

* ` data-en-hi-de-fr.csv` is a database downloaded from [Kaggle](https://www.kaggle.com/datasets/rajnathpatel/multilingual-spam-data)
* `LICENSE` is the standard MIT license
* `main.ipynb` contains my actual project, which used the dataset to train and test a GRU model using various different types of embeddings.
* `README.md` is this file
* `requirements.txt` is a file that contains all the libraries needed in `main.ipynb`. At the beginning of `main.ipynb`, I use `pip` to install all the necessary dependencies
* `tutorial-requirements.txt` is a file that contains all the libraries needed in `tutorial.ipynb`. At the beginning of `tutorial.ipynb`, I use `pip` to install all the necessary dependencies
* `tutorial.ipynb` is a notebook that walks through [this tutorial](https://pythonalgos.com/2022/01/02/build-a-gru-rnn-in-keras/)

## Learning Reflection

To see my analysis of the accuracy, confusion matrices, and other metrics from the kaggle dataset, please see the `tutorial.ipynb` file itself. 

Overall, this project helped me learn a few main things:

1. Implementing various embeddings was a lot more difficult than I anticipated. Specifically, I spent a very long time trying to implement skip vector embeddings. I tried using this git repository and this tutorial to no avail because of a conflict in `python` versions. These were the two main resources that I was able to find on skip vectors, but they turned out to be written by the same person who used Python 2.7. This was very unfortunate. 

2. The differences between different embeddings. I choose two main types of vector embeddings: Word2Vec embeddings using the tokens themselves as a training set and BERT embeddings. I chose Word2Vec initially because they seemed the easiest to implement, and I wanted to try out the different BERT embeddings to better understand how they worked as we had done a little bit of them in part 3 of the project, and I thought they were super interesting. I've added more notes on this in the `main.ipynb` file comparing the differences between the confusion matrices. 

3. The GRU model. When I was trying to figure out how to implement this, I learned a lot about how the GRU model works. Specifically, I found the comparisons between GRU and LSTM algorithms 