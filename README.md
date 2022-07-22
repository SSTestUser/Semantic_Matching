# Semantic_Matching

This project has methods to create word embeddings using the following means:

1. GLoVe embeddings
2. BeRt
3. TFiDF
4. TFiDF + GLoVe
5. Assorted text distance metrics (Jaccard distance, Sorensen dice, etc,)

And then aggregating the word embeddings additively or in other ways to generate sentance embeddings to find similarity using using the cosine similarity metric.

Other helper functions included are:
1. Convert PDFs/Docx files to raw text files
2. Tokenize and Convert to Embeddings (For the GLoVe embedding model) the text document
3. Load GLoVe model and a list of stopwords(frequently occuring words in the English Language) from Google Drive
4. Fetching the appropriate raw text file from the appropriate directory in the google drive from the list of candidates

In order to analyze the efficiency of the embedding methods and record other metrics we do the following:

1. Time the various embedding methods over a set number of iterations
2. Visualize the ranked values in the sort order of the candidate list
3. Save the ranked candidates and ranked values of the various embedding methods
4. Save the times over iterations of 10 candidates and the sum total of all candidates over various embedding methods
5. Compared similarity of the embedding methods using Rank Based Overlap, Kendell Tau and Bleu metrics 
