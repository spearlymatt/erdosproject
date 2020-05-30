The inequalitydocuments_handcode.csv is the main dataset containing the documents, hand-coded document classifications, and other metadata.

The project.Rmd simply loads some packages, reads the data, cleans them (i.e. makes some of the features the correct class), and preprocesses the documents to make a document-feature matrix for building a classifier. It then splits the document-feature matrix into training and test sets (~70/30) in a way that accounts for the different data sources (MTurk survey and lab experiment) as well as experimental conditions in the latter. Please forgive the coding inefficiencies--no need or bandwidth to make it super elegant at this point. Finally, there's some commented-out code for building preliminary classifiers.

The spearly_boggs_vwb.pdf is a bad draft of a seminar paper I wrote using the lab data (coauthor credited, all deficiencies mine of course). It's only included here in case you want more context about the original project, data, and/or experimental manipulation in particular; all things considered, it's probably a better resource for this than I am at this point.

The dfm_train.csv and dfm_test.csv are the document-feature matrices to be loaded into Python. They only include the "left" target, the text features, and complete observations--so the matrices themselves should be ready to input into models. 
