# PDF Password Remover

This project provides a simple utility to remove passwords from protected PDF files using Python. It utilizes the `PyPDF2` library to handle PDF reading and writing.

## Features

- Decrypts password-protected PDFs.
- Saves the unprotected PDF as a new file.
- Handles errors gracefully with informative messages.

## Requirements

- Python 3.x
- PyPDF2 library

## Installation

You can install the required library using pip:


pip install PyPDF2


## Usage

1. Update the `INPUT_PDF`, `OUTPUT_PDF`, and `PASSWORD` variables in the `main` function of the `PDF Password Remover` script to match your file paths and password.
2. Run the script:


python PDF\ Password\ Remover.ipynb


## Example

```
def main():
    INPUT_PDF = "input.pdf"
    OUTPUT_PDF = "output.pdf"
    PASSWORD = "your_password_here"
    
    success = remove_pdf_password(INPUT_PDF, OUTPUT_PDF, PASSWORD)
    
    if success:
        print(f"Password removed successfully. Output saved as: {OUTPUT_PDF}")
    else:
        print("Failed to remove PDF password")
```

## License

This project is licensed under the MIT License.
