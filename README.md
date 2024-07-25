# SkimLit-Abstract-NLP-Notebook

## Description
By following the practical of a course Deep Learning TensorFlow, I decided to write my own notebook in [Google Colab](https://colab.research.google.com/) introducing LNP SkimLit Abstract classification project.

## Content
This notebook is a practice of [**NLP**](https://medium.com/analytics-vidhya/an-introduction-to-nlp-explanation-and-examples-56035186197f) SkimLit (skim literature) classification of an abstract in research. For more specificially, I will be replicating the deep learning model behind the 2017 paper [*Neural Networks for Joint Sentence Classification in Medical Paper Abstracts*](https://www.google.com/url?q=https%3A%2F%2Farxiv.org%2Fpdf%2F1612.05251).

The paper presented a new dataset called [PubMed 200k RCT: a Dataset for Sequenctial Sentence Classification in Medical Abstracts](https://www.google.com/url?q=https%3A%2F%2Farxiv.org%2Fpdf%2F1710.06071) which consists of ~200,000 labelled Randomized Controlled Trial (RCT) abstracts.

The goal of the dataset was to explore the ability for NLP models to classify sentences which appear in sequential order...
* `BACKGROUND`
* `OBJECTIVE`
* `METHODS`
* `RESULTS`
* `CONCLUSIONS`
  
You can get the dataset from github  in [PubMed RCT200k](https://github.com/Franck-Dernoncourt/pubmed-rct).

I use pre-trained [BERT expert pubmed](https://www.kaggle.com/models/google/experts-bert/tensorFlow2/pubmed/2?tfhub-redirect=true) model as the main model for tokens dataset, with Bidirectional LSTM model for the characters dataset (see in model's paper), plus positional embeddings from each label (feature engineering data). With that in one big architecture [multi-models](https://en.wikipedia.org/wiki/Multimodal_learning) to maximize the highest accuracy. Not only make a prediction to the dataset but also test it with random abstract in public.

## Log
* 25 July 2024: First attempt, completed notebook.
