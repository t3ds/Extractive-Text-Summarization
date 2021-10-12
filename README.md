# Extractive-Text-Summarization

This project works on extractive text summarization.

More Specifically this uses the TextRank Algorithm which is based on the popular PageRank algortithm.

The Workflow of the project contains the following steps:

1. Read the PDF input

2. Use pdf2image to convert pdf pages to images

3. Use PyTesseract as an OCR to extract the text.

4. We employ sentence level tokenization to vectorize the text into sentences

5. We use preprocessing techniques to prepare the sentences by removing stopwords, special characters, numbers and converting everything to lowercase.

6. The next step is to create vectors from the sentences. We do that by going through each word in each sentence and assigning it a score to each word.

7. To score the words we use GloVe embedding vectors which are vectors obtained by training an  unsupervised learning algorithm on a large corpus of sentences and mapping words into a meaningful space based on  their semantic similarity.

You can read more about GloVe Embeddings Here: https://nlp.stanford.edu/projects/glove/

8. Now we have a matrix of vectors representing each sentence inthe input file, we run the textrank algorithm using the NetworkX package.

9. We then extract the top 'n' sentences('n' can be set by the user) as a summary.


PPT: Coming Soon
