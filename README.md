# Spanish Word Embeddings

Spanish words embeddings computed using [fastText](https://fasttext.cc) on the [Spanish Unannotated Corpora](https://github.com/josecannete/unannotated-spanish-corpora).

## Pre-Processing

The data used was already preprocessed in [Spanish Unannotated Corpora](https://github.com/josecannete/unannotated-spanish-corpora) to lowercase, remove multiple spaces, remove urls and others. We also used the script to split on punctuation included in the previous repository.

According to that tokenization, the 2.6B words corpus got into 3.4B tokens.

## fastText Parameters

We set default parameters of fastText for *Skipgram* task except for *epochs* were we set 20 instead of 5.

Each model has 1313423 words vectors of the following dimensions:

## XS (dim=10)

*Download*: [model.bin](google.com), [model.vec](google.com)

## S (dim=30)

*Download*: [model.bin](google.com), [model.vec](google.com)

## M (dim=100)

*Download*: [model.bin](google.com), [model.vec](google.com)

## L (dim=300)

*Download*: [model.bin](google.com), [model.vec](google.com)
