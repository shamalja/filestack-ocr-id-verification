# filestack-ocr-id-verification
Automated ID Verification with Filestack OCR: This repository demonstrates ID verification automation in JavaScript using Filestack's OCR API. Upload an ID document image, and the app extracts text for verification, streamlining data entry and enhancing security. Ideal for adding efficient identity checks in web applications.

Features
Image Upload: Users can upload an ID image for verification.
OCR Processing: The image is sent to Filestack for OCR processing, extracting text data from the uploaded ID.
Text Extraction: Displays the extracted text from the ID image, which can be used for further processing or verification.

Requirements
A Filestack API Key
Filestack Policy and Signature for secure access (generated in Filestack dashboard)

Setup
Clone this repository to your local machine or copy the HTML code into a file.
Replace placeholders in the code with your Filestack API credentials:
YOUR_API_KEY with your Filestack API key
YOUR_POLICY with the generated policy
YOUR_SIGNATURE with the generated signature

Usage
Open the HTML file in a web browser.
Click on the "Choose File" button to upload an ID image (passport, driver's license, etc.).
The uploaded image will be displayed, and the extracted text from the ID image will appear below it.

Code Explanation
The uploadAndExtractText function uploads the selected image to Filestack and retrieves the OCR data.
The fetch API is used to get the OCR results from Filestack, and the extracted text is displayed in the browser.

Example Output
After uploading an image, you should see:

The uploaded ID image displayed in the center.
Extracted text below the image, showing details captured from the ID (such as name, ID number, etc.).

Important Notes
Security: Make sure you generate the policy and signature server-side for security reasons in production applications.
Filestack Dashboard: Use the Filestack dashboard to create policies and signatures, and ensure that read, convert, and runWorkflow permissions are enabled for OCR functionality.

License
This project is open source and available under the MIT License.

Enjoy building with Filestack OCR!
