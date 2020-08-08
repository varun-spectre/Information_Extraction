# Information_Extraction

## Problem Statement

To build an Al/ML model to extract data from the rental agreements.
The rental agreements will be in different data formats and available in
the form of PDFs to perform the extraction.

* ML Domain: `NLP`

## Solution Approach

We have to extract 6 fields from the document Agreement_value, Renewal_Notice, Party_One, Party_Two, Agreement_Start_Date, Agreement_End_Date.
Since spacy is good with dates we can let spacy handle the Agreement_Start_Date, Agreement_End_Date. For the remaining 4 fileds I have divided each document into paragraphs and by considering each paragraph as context I have passed a set of questions to the BERT model. Questions are as follows ["what is the owner name?", "what is the tenant or resident name?", "what is the rent money?", "what is the notice period?"] I sorted the confidence scores and answers for the each paragraph in the document and this process is followed for all the documents. Results are filtered based on confidence scores.


## What else could have tried and what could have done better
There's is training data of 43 rental agreements available. I could have trained the Spacy custom NER model on that data.

From BERT QA model answer is accurate for paragraph if related data for question is present for the paragraph bit if it's not I am getting some random answer with good confidence scores, to handle these types of situation some regex can be done


### ML Techniques
* Text Extraction
* BERT QA
* spacy NER

### Programming languages

* Python 3.7 - For Machine Learning
* torch for running nlp pipelines



