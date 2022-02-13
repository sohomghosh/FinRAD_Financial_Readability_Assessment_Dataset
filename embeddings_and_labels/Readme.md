The BERT and FinBERT embeddings extracted using sentence transformers of the entire data set (13,000+ definitions) and the assigned redability scores (i.e. target/labels) are here. [This notebook](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/FinRAD_Sentence_FinBERTembedding_Extraction_Modeling_13K.ipynb) has been used to extract the embeddings.

Python code to read the dataset, create train and validation splits is mentioned below.

```python
import pandas as pd
from sklearn.model_selection import train_test_split

X = pd.read_pickle('finbert_embeddings_of_definitions_13K.pickle')
y = pd.read_csv('assigned_redability_scores_13K.csv')

train_X, valid_X, train_y, valid_y = train_test_split(X, y, test_size=0.33, random_state=42)
```
