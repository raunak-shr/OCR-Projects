# OCR-Projects
## Toolkit

<a href = "https://python.org/"><img src = "https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue"></a>
<a href = "https://jupyter.org/"><img src = "https://img.shields.io/badge/Jupyter-000000?style=for-the-badge&logo=jupyter&logoColor=orange"></a>
<a href = "https://pandas.pydata.org/"><img src = "https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white"></a>
<a href = "https://numpy.org/"><img src = "https://img.shields.io/badge/Numpy-FFFFFF?style=for-the-badge&logo=numpy&logoColor=blue"></a>
<a href = "https://chat.openai.com/"><img src = "https://img.shields.io/badge/chatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white"></a>
<a href = "https://www.latex-project.org/"><img src = "https://img.shields.io/badge/LaTeX-47A141?style=for-the-badge&logo=LaTeX&logoColor=white"></a>
<a href = "https://stackoverflow.com/"><img src = "https://img.shields.io/badge/Stack_Overflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white"></a>

---
# 1. Tamil Nadu Voter Information Extraction

This project demonstrates Optical Character Recognition (OCR) using Python and Pytesseract to convert voter information provided in Tamil language. OCR is a technology that extracts text from images or scanned documents. In this project, we leverage the power of Pytesseract, along with other essential libraries like Numpy, Pandas, PyPDF2, PIL (Python Imaging Library), and Google Translator, to perform OCR tasks in a Jupyter Notebook environment.

## Prerequisites

Make sure you have the following installed:

- Python: [Download Python](https://www.python.org/downloads/)
- Jupyter Notebook: [Installation Guide](https://jupyter.readthedocs.io/en/latest/install.html)
- Pytesseract: `pip install pytesseract`
- Tesseract OCR Engine: [Tesseract Installation Guide](https://github.com/tesseract-ocr/tesseract/wiki)

Additionally, install the required Python libraries:

```
pip install numpy pandas PyPDF2 googletrans==4.0.0-rc1
```

## Usage

1. **Image OCR:**
   - Place your images in the `images/` directory.
   - Run the Jupyter Notebook `OCR_with_Pytesseract.ipynb`.
   - The notebook will process the images using Pytesseract and display the extracted text.

2. **PDF OCR:**
   - Place your PDF files in the `pdfs/` directory.
   - Run the Jupyter Notebook `OCR_with_PDF.ipynb`.
   - The notebook will extract text from PDF files using PyPDF2 and perform OCR using Pytesseract.

3. **Language Translation (Optional):**
   - Modify the notebook to translate extracted text using Google Translator if multilingual support is needed.

## Example

```python
import pytesseract
from PIL import Image

# Read an image from file
image_path = 'images/sample_image.png'
image = Image.open(image_path)

# Perform OCR using Pytesseract
extracted_text = pytesseract.image_to_string(image)

# Print the extracted text
print("Extracted Text:")
print(extracted_text)
```

## Contributor

- [Shreeyansh Das](https://github.com/raunak-shr)

Feel free to contribute, open issues, or provide feedback.🚀
