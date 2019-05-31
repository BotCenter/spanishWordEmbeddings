# Spanish Word Embeddings
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3234051.svg)](https://doi.org/10.5281/zenodo.3234051)

Spanish words embeddings computed using [fastText](https://fasttext.cc) on the [Spanish Unannotated Corpora](https://github.com/josecannete/unannotated-spanish-corpora).

## Pre-Processing

The data used was already preprocessed in [Spanish Unannotated Corpora](https://github.com/josecannete/unannotated-spanish-corpora) to lowercase, remove multiple spaces, remove urls and others. We also used the script to split on punctuation included in the previous repository.

According to that tokenization, the 2.6B words corpus got into 3.4B tokens.

## fastText Parameters

We set default parameters of fastText for *Skipgram* task except for *epochs* were we set 20 instead of 5.

Each model has 1313423 words vectors of the following dimensions:

## Download


- **XS (dim=10)**: [model.bin](https://zenodo.org/record/3234051/files/embeddings-xs-model.bin?download=1), [model.vec](https://zenodo.org/record/3234051/files/embeddings-xs-model.vec?download=1)

- **S (dim=30)**: [model.bin](https://zenodo.org/record/3234051/files/embeddings-s-model.bin?download=1), [model.vec](https://zenodo.org/record/3234051/files/embeddings-s-model.vec?download=1)

- **M (dim=100)**: [model.bin](https://zenodo.org/record/3234051/files/embeddings-m-model.bin?download=1), [model.vec](https://zenodo.org/record/3234051/files/embeddings-m-model.vec?download=1)

- **L (dim=300)**:[model.bin](https://zenodo.org/record/3234051/files/embeddings-l-model.bin?download=1), [model.vec](https://zenodo.org/record/3234051/files/embeddings-l-model.vec?download=1)
