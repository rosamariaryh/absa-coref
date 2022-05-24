# absa-coref

Experiments for aspect-based sentiment analysis with coreference resolution. Master's thesis 2022 for the Language Analysis and Processing programme at the faculty of Informatics at the University of the Basque Country.

This repository includes material for opinion target extraction and aspect category detection.

## Multi-label classification

### Classification notebooks
Multilabel classification experiments were carried out on BERT and RoBERTa, which both have slightly different scripts, hence the two different notebooks. These take as input two files: a train.csv file and a test.csv file, which have id’s, texts and one-hot encodings of labels as columns.

### Data formatting notebook
To get the correct format for the experiment, a data formatting notebook is provided. This takes as input the original ABSA dataset in .xml format to extract the categories and a file with only text, one sentence per row. The output will be a .csv file with id’s, texts and one-hot encodings.

### Data provided
The data folders include formatted data (original, automatically resolved, gold/manual) for the multilabel classification models. These are called train.csv or test.csv. Also, files containing only texts are provided for all original, automatically resolved and manually resolved data. These are called data-type_texts_train-or-test.csv, for example, original_texts_train.csv.

