# NLP_InvoiceScanner

## Project Description
This project contains a Python script that performs OCR on an invoice image and extracts key-value pairs from it. The script uses Tesseract for OCR and SpaCy for Named Entity Recognition (NER).

## Installation
Install Tesseract OCR: !apt-get install tesseract-ocr
Install libtesseract-dev: !apt-get install libtesseract-dev
Install pytesseract: !pip install pytesseract
Install spacy: !pip install spacy

## Usage
Import the necessary libraries:
pytesseract
cv2
imutils
spacy

Load the image using the Image module of the PIL library.
Perform OCR on the image using pytesseract.image_to_string() function.
Load the SpaCy model.
Process the OCR output using the SpaCy NLP model and extract entities and their labels.
Extract key-value pairs from the OCR output using regular expressions.

## Functionality
The script takes an invoice image as input and performs OCR on it using Tesseract.
It then extracts key-value pairs from the OCR output using regular expressions.
The script also uses SpaCy to perform Named Entity Recognition (NER) on the OCR output and extract entities and their labels.
## Example
The input invoice image is stored in "/content/invoice-trade@2x.png".
The output of the OCR is stored in the variable extractedInformation.
The output of the regular expression extraction is stored in the dictionary kv_pairs.
The output of the SpaCy NER is printed to the console.

License
This project is licensed under the MIT License.
