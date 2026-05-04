# IT23748408 - Transliteration Accuracy Testing

## Assignment Details

**Module:** IT3040 - Information Technology Project Management  
**Assignment:** Assignment 1 - Option 1  
**Student Registration Number:** IT23748408  
**Testing Type:** Chat Sinhala Transliteration Accuracy Testing  
**Website Tested:** https://www.pixelssuite.com/chat-translator  
**Repo Link:** https://github.com/Methyachayangi/IT23748408-testing-playwright.git

## Project Description

This project tests the accuracy of the Chat Sinhala transliteration function in the PixelSuite Chat Translator web application.
The purpose of this assignment is to identify negative test scenarios where the application fails to correctly convert chat-style Singlish input into Sinhala output.
The automation script reads test data from the Excel file, enters each Singlish input into the website, captures the actual Sinhala output, compares it with the expected output, and records the final status in the Excel sheet.

## Scope of Testing

This project tests only:

- Chat-style Singlish to Sinhala transliteration
- Negative transliteration accuracy scenarios
- Common informal Sinhala typing patterns

This project does not test:

- Standard Sinhala transliteration
- Backend APIs
- Performance
- Scalability
- Security
- Other PixelSuite tools such as PDF editing, image conversion, resizing, cropping, compression, or meme generation


## Installation Steps

Open VS Code Terminal inside the project folder and run:
- python -m pip install -U pip
- python -m pip install playwright openpyxl
- python -m playwright install

## If Playwright browser installation is slow or fails, install only Chromium:

- python -m playwright install chromium

## Run the Automation

- python .\test_automation\test_automation.py --excel ".\test_automation\IT23748408.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 20 --slow-mo-ms 100 --save-every 1 --keep-open


