# authorship-verification
- University of Copenhagen
- IT and Cognition
- Language Processing 2
- Authorship Verification 2020 task

This repository contains the source code used to generate my model for the PAN 2020 authorship verification shared task: https://pan.webis.de/clef20/pan20-web/author-identification.html
This project is intented to decide whether two texts have been written by the same author based on comparing the texts' writing styles.

## Note
I developed all scripts in Jupyter Notebooks.
## Running the program:
- put the 'pan20-authorship-verification-training-small-truth.jsonl' and 'pan20-authorship-verification-training-small.jsonl' two files into data folder. Dataset can be dowloaded on https://pan.webis.de/data.html#pan20-authorship-verification
- run the dataread.ipynb first to read dataset.
- run feature_extract.ipynb. This script extracts all the features and saves them in the 'feature' folder. 
- run model.ipynb. This script read the features in feature folder, create feature matrix as input, train the models, make prediction using the trained models, and save the trained models in the 'model' folder.
- run new_text_predict_test.ipynb. This script loads the trained model in the 'model' folder and predicts two texts written by an author that does not belong to the training set.
## Features
- Average Sentence Length
- Average Word Length
- Noun
- Pronoun
- Adjective
- Numeral
- Verb 
- Adverb
- Period
- Comma
- Mispelling
- Bi-grams
- Tri-grams 
- Four-grams
- TF-IDF and cosine similarity
- Yule's K value
- Lexical Richness
- Tri-punctuations

npm838@alumni.ku.dk 
