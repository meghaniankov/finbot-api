# FINBOT - API

This repo contains the API for a chatbot, Ubb, teaches users about personal finance. The API is built using Django, receving user inputs as POST requests and returning chatbot responses to the user as GET requests. The code also contains the logic for a model that trains a bot using Natural Language Processing (NLP)/machine learning. 

Built as a group for the final project at Makers Academy. You can access the frontend of the project [here](https://github.com/meghaniankov/finbot).

The project came about as a result of wanting to build a tool to increase financial literacy as well as the interest to learn a new language (Python) and machine learning.

## Learning Journey

This was the team's first experience with Python, Django, Natural Language Processing, Tensorflow, and NLTK. It was also the team's first time 

## Bot/A.I. Model

The bot logic was built using [NLTK](https://www.nltk.org/), a Python library for NLP, which we used to [tokenize](https://nlp.stanford.edu/IR-book/html/htmledition/tokenization-1.html) and [stem](https://nlp.stanford.edu/IR-book/html/htmledition/stemming-and-lemmatization-1.html) a set of intents. We trained the bot by passing that pre-proccessed data through a neural net using Tensorflow/[TFLearn](http://tflearn.org/).

We could then predict the correct intent based on a user input. The user input would be tokenized/stemmed (i.e. create a 'bag of words') and then the model would return the intent that most closely matched the input.

Finally, the bot returned a response related to that intent.

## The Team

[Meghan Iankov](https://github.com/meghaniankov) | [Niki Manoledaki](https://github.com/nikimanoledaki) | [Bassel Al-Sayed](https://github.com/basselalsayed) | [Shadi Khazaei](https://github.com/shadz22) | [Emily Spencer](https://github.com/emilyjspencer)

## Deployed App

Frontend: https://finbot-fe.herokuapp.com/ 
API: https://finbot--api.herokuapp.com/

## Getting Started

### 1. Install Python 3.6

### 2. Install all other dependencies

After cloning the repo, run:

```
pip install
```

## Running the program

### Start Server

```sh
$ python3 manage.py runserver
```

## Built With

* Python
* Django
* Tensorflow
* TFLearn
* NLTK (Natural Language Toolkit)
* Pytest (testing)
