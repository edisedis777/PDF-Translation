# PDF-Translation

## Easily extract text from PDFs while preserving formatting, translate the content accurately, and convert it back into a well-structured, professional PDF.

### Features
This program provides the following functionalities:

- Extracts text from PDFs while attempting to preserve formatting
- Detects and formats headers
- Preserves bullet points
- Maintains paragraph breaks
- Splits the content into files of 100 pages each
- Adds page separators between pages
- Includes error handling and progress feedback

## **PDF Extraction**
### **Requirements**
To use this program, install the required library:
sh
pip install pdfplumber

Modify the `pdf_path` and `output_dir` variables in the script to match your needs.

### **Key Improvements**
- Original indentation is now preserved using leading spaces
- Empty lines are kept exactly as they appear in the source
- Headers are detected more accurately based on positioning and style
- List formatting is preserved while maintaining original indentation
- Page breaks are more clearly marked with separator lines
- Added parameter to better handle column detection
- Improved header detection
- Better handling of list items and indentation
- Enhanced exception handling for better debugging

---

## **Translation**
### **Requirements**
Install the required translation library:
sh
pip install deep-translator


### **Key Features**
- Preserves all markdown formatting, including:
  - Headers
  - Code blocks
  - Inline code
  - Links
  - Line breaks
- Handles large files by splitting them into chunks
- Includes a retry mechanism with exponential backoff
- Preserves original file names with an "_english" suffix

**Note:** The script uses the free `deep_translator` library, which is more stable and does not require async handling.

---

## **Markdown to PDF Conversion**
### **Requirements**
To convert translated markdown text into a professional-looking PDF, install:
sh
pip install markdown weasyprint PyPDF2


#### **WeasyPrint Dependencies**
Depending on your operating system, additional dependencies may be required:

- **macOS:**
  sh
  brew install cairo pango
  
- **Ubuntu/Debian:**
  sh
  sudo apt-get install build-essential python3-dev python3-pip python3-setuptools python3-wheel python3-cffi libcairo2 libpango-1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 libffi-dev shared-mime-info
  
- **Windows:**
  Follow WeasyPrint's [installation guide](https://weasyprint.org/) for Windows.

### **Key Enhancements in PDF Formatting**
#### **Document Structure**
- Professional margins and page size
- Page numbers centered at the bottom
- Proper spacing between elements
- Automatic page breaks before new sections

#### **Typography**
- **Body text:** Times New Roman (optimized for readability)
- **Headings:** Arial (better contrast)
- Optimized font sizes and line heights
- Justified text alignment with hyphenation

#### **Headings**
- Clear visual hierarchy
- Proper spacing before and after
- No page breaks immediately after headers

#### **Lists**
- Proper indentation
- Different bullet styles for nested levels
- Consistent spacing
- Improved line height for readability

#### **Tables**
- Full-width design
- Subtle borders
- Proper cell padding
- No page breaks within tables

#### **Code Blocks**
- Monospace font
- Light background
- Rounded corners
- Proper padding
- Overflow handling
- No page breaks within blocks

#### **Additional Features**
- Styled blockquotes
- Proper link colors
- Responsive images
- Horizontal rules

---

## **License**
Distributed under the MIT License. See `LICENSE` for more information.

## **Authors**
- **edisedis777** - *Initial work* - [GitHub](https://github.com/edisedis777)

## **Acknowledgments**
- pdfplumber Library
- deep-translator library
- weasyprint PyPDF2 library

## **Support**
For support, please create an issue in the GitHub repository or contact the maintainers.
