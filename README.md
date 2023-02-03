# nlp-challenge

Given a list of product names, explore ml options for classification and text extraction.

For a detailed discussion see [nlp_challenge.ipynb](/source/nlp_challenge.ipynb)

In the case where high bias is present in a text classification model, techniques to consider for improving the model are:

- Data processing
  - Remove dependant variables or transform them (e.g. bin continuous features)
- Regularization
  - Introduce a penalty to the model to prevent it from settling in a local minima

When seeking to extract information from text, apply a supervised model that has learned on examples of the data that is to be extracted.

If a labelled dataset does not exist, two options can help get the training started.

- Transfer learning
  - Pre-trained models may be available that can be modified to learn the specific use case
  - Regular expressions can be used to automatically label clean samples of data. This initial dataset can be used to begin training
