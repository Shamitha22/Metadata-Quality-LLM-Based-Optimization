# Metadata-Quality-LLM-Based-Optimization
Metadata Generator
About the Project

This project focuses on automating metadata generation for historical documents from the University of North Texas Libraries (UNTL). Manually creating metadata for archival materials is time-consuming and error-prone, so the goal of this project was to simplify and speed up the process using OCR and large language models.

The system takes scanned documents such as pamphlets, letters, photographs, and images, extracts text using OCR, and then generates structured Dublin Core metadata that follows UNTL Metadata Input Guidelines.

What This Project Does

Extracts text from scanned historical documents using OCR

Uses a language model (via OpenRouter) to generate meaningful metadata

Produces standardized metadata fields in a clean CSV format

Supports multiple document types in a single workflow

Document Types Supported

Pamphlets

Letters

Photographs

Images

Each document type is handled with its own examples and prompts to improve metadata accuracy.

Technologies Used

Python

Tesseract OCR & pytesseract

OpenRouter API (LLaMA models)

Pandas

Pillow (PIL)

Google Colab

How It Works (Simple Flow)

Upload ZIP files containing document images

Images are extracted and resized if needed

Text is extracted using Tesseract OCR

The extracted text is sent to an LLM with examples

Metadata is generated following UNTL standards

Results are saved as CSV files

Metadata Fields Generated

For each document, the following fields are created:

Title

Creator

Contributor

Date

Content Description

Subject and Keywords

Coverage

If any information is missing, it is clearly marked as “Not provided.”

How to Run the Project

Open the notebook in Google Colab

Install required libraries (requests, pytesseract, pandas, Pillow)

Install Tesseract OCR

Enter your OpenRouter API key when prompted

Upload the ZIP files containing document images

Run all cells to generate metadata

Output

Metadata is saved as CSV files

Separate CSV files are generated for each document type

The output is ready for use in digital libraries or archival systems

Why This Project Matters

This project demonstrates how AI can be used responsibly in digital libraries to:

Reduce manual effort

Improve consistency in metadata

Support large-scale archival digitization

It also shows practical use of OCR, prompt engineering, and structured data generation.

Academic Context

This project was developed as part of INFO 5731 – Information Organization and follows UNTL metadata standards strictly.

Future Improvements

Add a web interface for easier uploads

Improve OCR accuracy for low-quality scans

Support additional metadata schemas

Add validation and confidence scoring

Contributors

Shamitha Reddy

INFO 5731 – Group 4
