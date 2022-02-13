Some of the ready to use trained model artifacts are here. These have been trained on the entire dataset. They have been developed using [this notebook](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/FinRAD_Sentence_FinBERTembedding_Extraction_Modeling_13K.ipynb).

Code to load these models in Python and generate predictions is presented below.
```python
import pickle
with open('model.pkl', 'rb') as f: #Remeber you need to replace 'model.pkl' with your own pickled classifer file like 'logistic_regression_classifier.pkl'
    clf = pickle.load(f)

# For prediction
text = 'A mutual fund is a type of financial vehicle made up of a pool of money collected from many investors to invest in securities like stocks, bonds, money market instruments' #This is a sample text, feel free to write your own
from sentence_transformers import SentenceTransformer
model = SentenceTransformer('ProsusAI/finbert')
emd = model.encode([text])

if clf.predict(emd)==1:
    ans = 'readable'
else:
    ans = 'not readable'

print("Predicted Type:", ans)
print("Preidcted Score:", clf.predict_proba(emd)[0,1])

```
