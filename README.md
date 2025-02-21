# PDF-Translation
## Translate PDF document by extraction to markdown, translation, and markdown to PDF conversion

### This program provides the following features:
##### - Extracts text from PDF while attempting to preserve formatting
##### - Detects and formats headers
##### - Preserves bullet points
##### - Maintains paragraph breaks
##### - Splits the content into files of 100 pages each
##### - Adds page separators between pages
##### - Includes error handling and progress feedback

### To use this program, you'll need to: 
- install the required library: pip install pdfplumber
- modify the pdf_path and output_dir variables to match your needs

#### Key points:
##### - Original indentation is now preserved using leading spaces
##### - Empty lines are kept exactly as they appear in the source
##### - Headers are detected more accurately based on positioning and style
##### - List formatting is preserved while maintaining original indentation
##### - Page breaks are more clearly marked with separator lines
##### - Added parameter to better handle column detection
##### - Improved header detection
##### - Better handling of list items and indentation
##### - Exception re-raising for better error debugging

### Translation

### To use this program, you'll need to: 
-install the required library: pip install googletrans

#### Key points:
##### -Preserves all markdown formatting including: 
Headers,
Code blocks,
Inline code,
Links,
Line breaks
##### - Handles large files by splitting them into chunks
##### - Includes retry mechanism with exponential backoff
##### - Preserves original file names with "_english" suffix

#### Note: The script uses the free deep_translator library which is more stable and doesn't require async handling.


### Translated Markdown Text to PDF conversion

#### To use this program, you'll need to: 
- install the required library: pip install markdown weasyprint PyPDF2
#### Note: WeasyPrint has some system dependencies:
- On macOS: brew install cairo pango
- On Ubuntu/Debian: sudo apt-get install build-essential python3-dev python3-pip python3-setuptools python3-wheel python3-cffi libcairo2 libpango-1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 libffi-dev shared-mime-info
- On Windows: Follow WeasyPrint's installation guide for Windows

#### Key points in the PDF conversion section:
##### -Document Structure:
Professional margins and page size,
Page numbers at bottom center,
Proper spacing between elements,
Automatic page breaks before new sections

##### -Typography:
Times New Roman for body text (more readable for long documents),
Arial for headings (better contrast),
Optimized font sizes and line heights,
Justified text alignment with hyphenation

##### -Headings:
Clear visual hierarchy,
Proper spacing before and after,
No page breaks after headers

##### -Lists:
Proper indentation,
Different bullet styles for nested levels,
Consistent spacing,
Better line height for readability

##### -Tables:
Full-width design,
Subtle borders,
Proper cell padding,
No page breaks within tables

##### -Code Blocks:
Monospace font,
Light background,
Rounded corners,
Proper padding,
Overflow handling,
No page breaks within blocks

##### -Additional Features:
Styled blockquotes,
Proper link colors,
Responsive images,
Horizontal rules

