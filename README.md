
# Project README: Anomaly Prediction, Software Tracking, and Text Detection Scripts

## Overview
This project contains three distinct Python scripts that handle different aspects of anomaly detection, software tracking, and text recognition using OCR.

### 1. Classes Anomaly Prediction Script
This script is designed to predict software vulnerabilities by analyzing data from SCCV logs. It fetches log data from a MongoDB database and uses a Linear Regression model to predict vulnerability counts.

#### Features:
- **Data Processing**: Fetches data from Splunk and SCCV logs stored in MongoDB.
- **Linear Regression Model**: Utilizes a regression model to predict the number of vulnerabilities based on historical data.
- **Model Evaluation**: The script splits data into training and testing sets and evaluates the model using Mean Squared Error (MSE).

#### Requirements:
- `pandas`
- `sklearn`
- `pymongo`
- `certifi`

### 2. Software Tracking Anomalies Script
This script is used to track software anomalies across different sites by processing logs from various sources. It helps in identifying and recording incidents of software issues.

#### Features:
- **Anomaly Detection**: Tracks software issues across different sites by processing log data.
- **Log Processing**: Maintains a history of software incidents, helping in identifying recurring issues.

#### Requirements:
- `pandas`
- `pymongo`

### 3. Text Detection and OCR Script
This script is designed to detect and extract text from images using Optical Character Recognition (OCR). It preprocesses the image and extracts key information such as dates and times from the recognized text.

#### Features:
- **Image Preprocessing**: Enhances image properties like brightness and sharpness for better OCR accuracy.
- **OCR**: Uses the `pytesseract` library to extract text from images.
- **Date and Time Extraction**: Extracts specific date and time patterns from the OCR results.

#### Requirements:
- `pytesseract`
- `PIL` (Pillow)
- `re`

## Usage Instructions
1. **Classes Anomaly Prediction Script**:
   - Set up a MongoDB instance and provide a connection string.
   - Run the script to fetch log data, process it, and predict the number of vulnerabilities.

2. **Software Tracking Anomalies Script**:
   - Provide log data from various sources.
   - The script will process the data and maintain records of software anomalies across sites.

3. **Text Detection and OCR Script**:
   - Provide the image path where the text needs to be detected.
   - The script will process the image and return the extracted text, along with any detected dates and times.

## Additional Information
Each script is designed to operate independently, but they share common libraries such as `pandas` for data manipulation and processing. Make sure to install the required dependencies for each script before execution.

