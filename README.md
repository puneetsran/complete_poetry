# Completing Poetry with RNN

### This project aims to develop a deep learning model for generating poetry based on a given starting phrase.
Approach:
- Model Architecture: Employ a recurrent neural network (RNN) which can write poetry.
- Evaluation Strategy: Evaluate the model's performance accuracy score as well as human evaluation of looking at the text generated.

## Source of data
I extracted the OkCupid dataset from [Kaggle](https://www.kaggle.com/datasets/johnhallman/complete-poetryfoundationorg-dataset/data) in CSV format.

## Missing Values
The data was fairly clean with only one missing value which was removed.

## Modelling
For this project, the main modelling technique was RNN, both single layer and then multiple layers.

## Results
The initial single-layer RNN struggled to produce English-language poetry but it was a good starting point to see if a poem can be generated. The second deep neural network model performed better as it used more English words but still faced challenges in generating meaningful poems.
