# Covid_19 Action Items
Research Paper Text Analysis for COVID-19 papers on Kaggle Competition

# Solved Items
Successful lower-casing, word-tokenization, stopword-removal, punctuation stripping, numeric stripping, and lemmatization of individual abstracts. 

Function created for aforementioned text processing pipeline: doc_proc. Tested, and seems to work. I have **not** yet run it on the whole dataset because it takes a while, wanted to check with team before running it on the whole dataset. 

# Pending Items
Deciding on next steps for text processing and modeling. I personally am still pretty set on starting with some kind of TF-IDF model to really distill out the common language across this type of scientific literature. For example, the word virus might be somewhat rare in normal conversation, but it is extremely common in these academic papers. If we do TF-IDF across all papers in this dataset, then we can mitigate the importances of those words. Open to anything though. Potentially address some formal tasks as well.


-Address abbreviation ambiguity (same abbreviation, different meanings)
-Address if abbreviations (post lowercasing) are stopwords (if something like ARE or AND mean something)
    +Comment out lowercasing code
-Workaround for appending every single unique possible symbol (exclude everything that isn't alpha numeric?)
-Run doc_proc on the entire datasets
