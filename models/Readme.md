Some of the ready to use trained model artifacts are here.

Code to load these models in Python
```python
import pickle
with open('model.pkl', 'rb') as f: #Remeber you need to replace 'model.pkl' with your own pickled classifer file like 'logistic_regression_classifier.pkl'
    clf = pickle.load(f)
```
