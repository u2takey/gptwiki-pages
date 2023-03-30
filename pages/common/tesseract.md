# tesseract 
## chatgpt 
Tesseract is a command-line tool for optical character recognition (OCR), which means it takes an image file containing text and converts the text content into a digital format that can be copied and pasted, searched, or edited like any other text document. 

Usage:
tesseract [inputFile] [outputFile] [option]

[inputFile] is the image file that contains the text to be extracted.
[outputFile] is the file to store the extracted text.
[option] is optional and can be used to specify additional parameters such as the OCR engine mode, language, page segmentation mode, and other customizations.

Example:
tesseract image.png output.txt -l eng --psm 6

In this example, tesseract will use the English language (-l eng) and page segmentation mode number 6 (--psm 6) to process the input file image.png and output the extracted text into the file output.txt. 

Note that tesseract may require additional installation and setup of language data files and the OCR engine itself, depending on your operating system and environment. 

## tldr 
 
> OCR (Optical Character Recognition) engine.
> More information: <https://github.com/tesseract-ocr/tesseract>.

- Recognize text in an image and save it to `output.txt` (the `.txt` extension is added automatically):

`tesseract {{image.png}} {{output}}`

- Specify a custom language (default is English) with an ISO 639-2 code (e.g. deu = Deutsch = German):

`tesseract -l deu {{image.png}} {{output}}`

- List the ISO 639-2 codes of available languages:

`tesseract --list-langs`

- Specify a custom page segmentation mode (default is 3):

`tesseract -psm {{0_to_10}} {{image.png}} {{output}}`

- List page segmentation modes and their descriptions:

`tesseract --help-psm`
