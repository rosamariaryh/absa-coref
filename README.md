# absa-coref

This repository includes material for aspect-based sentiment analysis experiments applying coreference resolution. The data is based on the English restaurant reviews from the SemEval-2016 ABSA task. AllenNLP's coreference resolution model was used to find coreferential links in the texts.

The following tasks are covered:

1. Opinion target extraction as a sequence labelling task
2. Opinion target extraction & aspect category detection as a sequence labelling task 
3. Aspect category detection as a multi-class classification task
4. Aspect category detection as a multi-label classification task

## 1-2. Sequence labelling 

### Sequence labelling notebook

### Data
The data folders hold train, development and test data in tsv format for both simple sequence labelling and sequence labelling with category detection. This type of data is provided for the original data, automatically resolved coreference data and manually resolved coreference data.

## 3. Multi-label classification

### Classification notebook

### Data formatting notebooks

### Data

## 4. Multi-label classification

### Classification notebooks
Multilabel classification experiments were carried out on BERT and RoBERTa, which both have slightly different scripts, hence the two different notebooks. These take as input two files: a train.csv file and a test.csv file, which have id’s, texts and one-hot encodings of labels as columns.

### Data formatting notebook
To get the correct format for the experiment, a data formatting notebook is provided. This takes as input the original ABSA dataset in .xml format to extract the categories and a file with only text, one sentence per row. The output will be a .csv file with id’s, texts and one-hot encodings.

### Data
The data folders include formatted data (original data, automatically resolved coreference data, manually resolved coreference data) for the multilabel classification models. These are called train.csv or test.csv. Also, files containing only texts are provided for all original, automatically resolved and manually resolved data. These are called <data-type>_texts_train-or-test.csv, for example, original_texts_train.csv.
