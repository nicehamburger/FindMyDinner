# Project Title

## Overview
A brief description of your project.

## Technologies Used

- **Google Cloud Storage (GCS)**: Used to store raw data files in a bucket.
- **Google Compute Engine**: Used for running the data processing pipeline.

## Project Structure

```
├── captions_extracted/              # Output file for extracted captions from posts
├── downloaded_images/               # Output file for downloaded posts
├── impfiles/                        # Folder containing raw data (JSON file from Apify Instagram Scrapper  API)
├── src/                             # Source code directory
│   ├── A_Main.py                    # Main script to run the project
│   ├── B_GoogleVisionExtraction.py  # Google Vision API OCR script
│   ├── C_GoogleAIAPI.py             # Google AI API Gemini Prompt script
│   ├── D_FinalProcessing.py         # Final Data Processing and Export script
│   ├── event.py                     # Event class definition
│   ├── eventcollections.py          # Event collection handling
│   ├── post.py                      # Post class definition
│   └── postcollections.py           # Post collection handling
├── texts_extracted/                 # Output file for OCR extracted text from posts
├── LICENSE                          # Project license file
├── all_events.txt                   # Output file for D_FinalProcessing.py
└── response.txt                     # Output file for C_GoogleAIAPI.py
