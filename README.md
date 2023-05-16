# Sentence Similarity for PDF Text Analysis
This is a basic codebase on using marketing research paper to test two sentence transformer models 

**Sentence Similarity for PDF Text Analysis**
This project uses the SentenceTransformer library to find the paragraph in a set of PDF files that is most similar to a given question. The solution relies on sentence embeddings to calculate similarity scores between the question and each paragraph in the PDFs.

**Dependencies**
To run the project, you will need to install the following Python libraries:

**pdftotext: A library that converts PDF files into text.**
sentence-transformers: A library for training and using transformer models for generating sentence embeddings.
numpy: A library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.
Installation
Run the following commands in a Colab notebook to install the necessary packages:

!apt-get install -y libpoppler-cpp-dev
!pip install pdftotext
!pip install sentence-transformers numpy

**Usage**

Initialize the SentenceTransformer model. The 'all-MiniLM-L6-v2' model is used in this project.

Define the file paths for the PDF files you want to analyze.

Extract text from each PDF file, preprocess it into paragraphs, and encode each paragraph into an embedding.

Define a question that you want to find the most similar paragraph to in the PDF files.

Use the get_most_similar_paragraph function to find the paragraph in each PDF file that is most similar to the question.

The output will print the number of paragraphs in the PDF file, the shape of the embeddings matrix, and the paragraph that is most similar to the question.

