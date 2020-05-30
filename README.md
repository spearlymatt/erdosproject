The inequalitydocuments_handcode.csv is the main dataset containing the documents, hand-coded document classifications, and other metadata.

The project.Rmd reads the data, cleans them, and preprocesses the documents to make a document-feature matrix for building a classifier. It then splits the document-feature matrix into training and test sets (~70/30) in a way that accounts for the different data sources (MTurk survey and lab experiment) as well as experimental conditions in the latter. Finally it makes a descriptive graphic for the presentation.

The dfm_train.csv and dfm_test.csv are the training and test document-feature matrices (with targets) to be loaded into Python.

The projectcode.ipynb builds, tunes, and tests all of the classifiers.
