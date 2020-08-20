# Information_Extraction

## Problem Statement

To build an Al/ML model to extract data from the rental agreements.
The rental agreements will be in different data formats and available in
the form of PDFs to perform the extraction.

* ML Domain: `NLP`

## Solution Approach

Look into Custom_NER.ipynb for results
We have to extract 6 fields from the document Agreement_value, Renewal_Notice, Party_One, Party_Two, Agreement_Start_Date, Agreement_End_Date.
We shall use Spacy Custom NER model for training, due to lack of time I have done only for one field the same process goes for rest 5 fileds. 


## What else could have tried and what could have done better
Use a better sentence tokenizer instead of getting paragraphs from text and they try evaluation model on that data.



### ML Techniques
* Text Extraction
* spacy NER

### Programming languages

* Python 3.7 - For Machine Learning



