# Completing Poetry with RNN

### This project aims to develop a deep learning model for generating poetry based on a given starting phrase.
Problem:
- Can I generate poetry given a few input words or a phrase?
- Can a machine generated poem be meaningful and coherent?
Approach:
- Model Architecture: Employ a recurrent neural network (RNN) which can write poetry.
- Evaluation Strategy: Evaluate the model's performance accuracy score as well as human evaluation of looking at the text generated.

## Source of data
I extracted the OkCupid dataset from [Kaggle](https://www.kaggle.com/datasets/johnhallman/complete-poetryfoundationorg-dataset/data) in CSV format.

The poem dataset has 15652 entries. Here is a breakdown of all the features:
- Author: The author of the poem
- Title: The title of the poem
- Poetry Foundation ID: This corresponds to the ID which can be used to find the same poem on the poetryfoundation website.
- Content: This is the main poem - the main content

## Missing Values
The data was fairly clean with only one missing value which was removed.
- Removed non alpha numeric characters with white space
- Used Tokenizer to break each poem into a sequence of characters, index characters by numbers, and map the sequence

## Modelling
For this project, the main modelling technique was RNN, both single layer and then multiple layers.
- Initial RNN model had 50% accuracy
    - Input Phrase: When to the session of sweet silent
    - Output Phrase: when to the session of sweet silentle narro rante  hond weave like her furtsty want  no tle spilies  and dy morn   mla da  for thee  u len the branchic ongel of the live  and tome  and  long with time hof on eshe ye flown wear on toil
- Second model had a very low accuracy:
    - Input Phrase: it is a lovely day
    - Output Phrase: it is a lovely day mine summers in murmuring thro among his lately blood this prevailing minds by the rang groan d but if a aidless perchance old shalott knightly strangers in the strength and horses him brightens d the earth camelot that as an and all to let that charge we lift he hangs


## Results
- RNNs for Poetry? This project explored if RNNs could generate poems.
- Simple RNN Struggles: Basic model couldn't create grammatically correct poems, but proved the concept.
- Deeper Network, Better Words: More complex model used better vocabulary, but struggled with meaningful poetry.
- AI Creativity Challenge: Project highlights the difficulty of AI-driven creative tasks like poetry generation.
- Room for Improvement: Refining the model architecture holds promise for better, more coherent text generation.