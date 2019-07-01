# Spanish Word Embeddings
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3255001.svg)](https://doi.org/10.5281/zenodo.3255001)

Spanish words embeddings computed using [fastText](https://fasttext.cc) on the [Spanish Unannotated Corpora](https://github.com/josecannete/spanish-corpora).

## Pre-Processing

The data used was already preprocessed in [Spanish Unannotated Corpora](https://github.com/josecannete/spanish-corpora) to lowercase, remove multiple spaces, remove urls and others. We also used the script to split on punctuation included in the previous repository.

According to that tokenization, the 2.6B words corpus got into 3.4B tokens.

For **new L** we used the updated version of [Spanish Unannotated Corpora](https://github.com/josecannete/spanish-corpora) which has 3B words and applied same preprocessing of the other models.

## fastText Parameters

We set default parameters of fastText for *Skipgram* task except for *epochs* were we set 20 instead of 5.

## Evaluation

We evaluated our word embeddings in [SemEval-2017 Task 2 (Subtask 1)](http://alt.qcri.org/semeval2017/task2/index.php?id=task-details) using the script provided by [MUSE](https://github.com/facebookresearch/MUSE) library, getting these results:

|       | XS      | S       | M       | L           | new L   |
|-------|---------|---------|---------|-------------|---------|
| Score | 0.59150 | 0.67589 | 0.72345 | **_0.74676_** | 0.72940 |

Being **L** embedding model **the best one in Spanish** as far as we know in the date of publication.

## Download


- **XS (word vectors=1313423, dim=10)**: [model.bin](https://zenodo.org/record/3234051/files/embeddings-xs-model.bin?download=1), [model.vec](https://zenodo.org/record/3234051/files/embeddings-xs-model.vec?download=1)

- **S (word vectors=1313423, dim=30)**: [model.bin](https://zenodo.org/record/3234051/files/embeddings-s-model.bin?download=1), [model.vec](https://zenodo.org/record/3234051/files/embeddings-s-model.vec?download=1)

- **M (word vectors=1313423, dim=100)**: [model.bin](https://zenodo.org/record/3234051/files/embeddings-m-model.bin?download=1), [model.vec](https://zenodo.org/record/3234051/files/embeddings-m-model.vec?download=1)

- **L (word vectors=1313423, dim=300)**:[model.bin](https://zenodo.org/record/3234051/files/embeddings-l-model.bin?download=1), [model.vec](https://zenodo.org/record/3234051/files/embeddings-l-model.vec?download=1)

- **new L (word vectors=1451827, dim=300)**:[model.bin](https://zenodo.org/record/3255001/files/embeddings-new_large-general_3B_fasttext.bin?download=1), [model.vec](https://zenodo.org/record/3255001/files/embeddings-new_large-general_3B_fasttext.vec?download=1)
