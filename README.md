# HabNet
The code and data are for reviewing paper 'Hierarchical Bi-directional Self-Attention Networks for Paper Review Rating Prediction'

## Code overview
There are two folders of code: HabNet is the code for the main task of predicting final acceptance decisions for papers; HabNet_MC is the code for the sub_task of predicting ratings for reviews. The steps for running them are the same as shown in following section "usage".

## Dataset
The open review datasets (processed) are already in the "data" folder of HabNet and HabNet_MC folder. "ICLR_Review_all_with_decision_processed.csv" is used for the main task of predicting acceptance decsions for papers, it is located in "data" folder of HabNet; "ICLR_Review_all_processed.csv" is used for the sub-task of predicting ratings for reviews, it is located in "data" folder of HabNet_MC.


## Code

## Requirements

- Python 3
- Tensorflow = 1.13.1
- Pandas
- Nltk
- Tqdm
- [Glove pre-trained word embeddings](http://nlp.stanford.edu/data/glove.6B.zip)

## Usage

First step: run script to prepare the data:

```bash
python data_prepare.py
```

Second step: train and evaluate the model:
<br>
*(make sure [Glove embeddings](#requirements) are ready before training), put glove.6B.50d.txt in HabNet, and put glove.6B.100d.txt in HabNet_MC*
```
wget http://nlp.stanford.edu/data/glove.6B.zip
unzip glove.6B.zip
```
```bash
python train.py
```




