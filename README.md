# HabNet
The code and data are for reviewing paper 'Hierarchical Bi-directional Self-Attention Networks for Paper Review Rating Prediction'

## Dataset
The open review datasets (processed) are already in the "data" folder of HabNet code folder, there are two files in "data" folder: "ICLR_Review_all_with_decision_processed.csv" is used for the main task of predicting acceptance decsions for papers; "ICLR_Review_all_processed.csv" is used for the sub-task of predicting ratings for reviews.

## Code

## Requirements

- Python 3
- Tensorflow = 1.13.1
- Pandas
- Nltk
- Tqdm
- [Glove pre-trained word embeddings](http://nlp.stanford.edu/data/glove.6B.zip)

## Usage

First step: run script to prepare the data (the default data file is: "ICLR_Review_all_with_decision_processed.csv"):

```bash
python data_prepare.py
```

Second step: train and evaluate the model:
<br>
*(make sure [Glove embeddings](#requirements) are ready before training)*
```
wget http://nlp.stanford.edu/data/glove.6B.zip
unzip glove.6B.zip
```
```bash
python train.py
```




