# Text-Retrieval-Using-Pretrained-Embedding - AI Viet Nam
## Text Retrieval (TR) (also called as Document Retrieval):
- A branch of information Retrieval (IR) where the system matching of some stated user search query against a set of texts.
  + Refs:
    * https://en.wikipedia.org/wiki/Document_retrieval
    * https://nlp.stanford.edu/IR-book/html/htmledition/an-example-information-retrieval-problem-1.html
## Basic Text Retrieval Pipeline:
- ![pipeline](https://drive.google.com/uc?export=view&id=1B45bwK4r_ddJztCf5l1yY7d1jnPxs3-R)
## Dataset:
- With MSMARCO Dataset, create a simple text retrieval program using Vector Space Model.
- ![Description](https://drive.google.com/uc?export=view&id=1Huoo3rq4-9QQTJB2aGJmDTC5P1HAnkwO)
- Dataset: https://huggingface.co/datasets/ms_marco
## Vector Space Model
- ![vectorspacemodel](https://drive.google.com/uc?export=view&id=1YOHgf2O7ipbuO2m29dJSoi7Qx27WrBsm)
## Project Pipeline:
- ![pipeline](https://drive.google.com/uc?export=view&id=16xT9AleEJC-Q0V8LKieE0Ix2Gi1sIbGQ)
  + Step 1: Install datasets.
  + Step 2: Load MS_MARCO
  + Step 3: Extract text:
    * only use sample with type == entity (you can change optionally).
    * Load text and append to corpus.
  + Step 4: Text Normalization
  + Step 4: Create a Bag-of-Words
    * ![bagofword](https://drive.google.com/uc?export=view&id=1TtkXaA3VeAJvDbaCmzw9Xr_IQ1xHQh0z)
      * Create Dictionary: concludes unique words in corpus.
      * Vectorize: Based on Weighting (term-frequency) to transform each doc_n in the Corpus into vectors
      * ![vectorizer](https://drive.google.com/uc?export=view&id=1FCqT0pSc2oebXPHyUIIn96c7l54IGHwv)
  + Step 5: Indexing: The process of organizing and structuring a collection of documents or data to facilitate efficient retrieval of information. It involves creating an index that enables quick access to relevant documents based on search queries or specific attributes.
    * We can use document-term matrix as a database to indexing documents
    * Document-term Matrix: A mathematical matrix that describes the frequency of terms that occur in a collection of document.
    * ![DocumentTermMatrix](1rTOcgVaSqxuIaOvTjAnUvsWg1YDKqKhR)
  + Step 6: Ranking based on Cosine Similarity
# The end.
