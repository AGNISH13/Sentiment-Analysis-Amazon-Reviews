# Sentiment Analysis of Amazon Fine Food Reviews"

## Project Description
This is a python-based project predicting the `Sentiment` of `Customer Reviews`. The Sentiment Analysis has been done using two approaches:
- Bag Of Words approach (NLTK's `SentimentIntensityAnalyzer` utlizing `VADER` (Valence Aware Dictionary and sEntiment Reasoner)) 
- Transformer approach (`RoBERTa` Pretrained Model from Hugging Face)

The entire coding workflow can be viewed in the ipynb file present in this repository.

## Dataset Description
Models are implemented using Pytorch and fitted on the [Amazon Fine Food Reviews](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews) Dataset.

This dataset consists of reviews of fine foods from amazon. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. Reviews include product and user information, ratings, and a plain text review. It also includes reviews from all other Amazon categories. All the data is present in the `Reviews.csv` file, which is the only file required for this project.

## Results
The data has been tested using the `VADER Sentiment Scoring` as well as the `RoBERTa pre-trained model`. Given below is the comparison of the results using both.

-     Pair Plot
     ![image](https://github.com/AGNISH13/Sentiment-Analysis-Amazon-Reviews/assets/84792746/38888cce-eb49-4789-a3df-728fb6cb1e8c)

We can infer from these plots that `RoBERTa` gives better sentiment scoreing than `VADER`, giving a skewer distribution for positive, neutral and negative reviews respectively.

## Dependencies
This entire project is based on `Python` programming language. The models have been trained and tested entirely using the resources `Google Colab`.
The Python libraries which are in use in this project are  `matplotlib`, `numpy`, `pandas`, `seaborn`, `nltk` and `tqdm`. The pre-trained transformer model `RoBERTa` has been loaded using [Hugging Face](https://huggingface.co/docs/transformers/model_doc/roberta).

## Acknowledgements
https://www.kaggle.com/code/robikscube/sentiment-analysis-python-youtube-tutorial/notebook

https://www.geeksforgeeks.org/python-sentiment-analysis-using-vader/
