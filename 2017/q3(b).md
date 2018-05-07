## Term frequency (TF)
TF meausures how frequently a term occurs in a document.
```
TF(t) = (Number of times term t appears in a document) / (Total number of terms in the document).
```



## Inverse Document Frequency (IDF)
IDF measures how important a term is. While computing TF, all terms are equally important, however, words like `is, are, of, the, has ` may appear a lot of times but not really important, so we need to weight them down by computing IDF.  

```
IDF(t) = log_e(Total number of documents / Number of documents with term t in it).
```

Finally, we can calculate the TF-IDF weight by using the following formula
```
TFIDF(t) = TF(t) * IDF(t)
```

## Application
By using TFIDF method, we can rank document relevance give a specific term. Thus, this text-mining appproach is widely adopted in search engine such as Google, Yahoo and Bing, as they can rank document relevance based on user search query.
