# Information-Retrieval-using-Multi-Phased-Genetic-Algorithm

This project aims to enhance query weight optimizations in search engines using genetic algorithm.  


There are 3 stages involved:  
```
1. Create a tf-idf vectorizer.
2. Preprocess the query, use the vectorizer on the query and every document, and find the cosine similarities - for baseline comparison.    
3. Use genetic algorithm with niching to find the best search results while adding a bit of diversity:  
  a. Use k-mean clusters to group documents - used as a niching technique to add diversity (punishes results for being too close to each other).
  b. In each cluster, evaluate fitness functions of all documents with query.
  c. Select best parents using tournament selection.  
  d. Perform single point crossovers.
  e. Perform random mutations.
  f. Use generational replacement for the new population.
  g. Evaluate new fitness functions.
```
