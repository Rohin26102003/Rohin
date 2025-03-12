# Smart Visitant Access

## Overview
Smart Visitant Access is a web-based visitor management system that allows visitors to check in and check out using QR codes. It also supports OCR-based identity proof extraction using Google Vision OCR. Visitors receive a QR code via SMS (using Twilio) and can use it to check in and check out.

## Features
- QR-based check-in and check-out system
- Identity proof extraction using Google Vision OCR
- Automatic data storage in a database
- Twilio integration for sending OTPs and QR codes via SMS
- Web-based interface for visitor registration

## Project Structure
```
SmartVisitantAccess/
│-- app.py                # Main application script
│-- database.sql          # SQL file for database setup
│-- from twilio.py        # Twilio integration for OTPs
│-- requirements.txt      # List of dependencies
│-- sample.py             # Sample testing script
│-- static/               # Static files (CSS, JS, images)
│-- templates/            # HTML templates
│-- testfolder/           # Testing files
│-- uploads/              # Directory for uploaded files
```

## Installation
1. Clone the repository:
   ```sh
   git clone <repository_url>
   ```
2. Navigate to the project directory:
   ```sh
   cd SmartVisitantAccess
   ```
3. Create a virtual environment:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use 'venv\Scripts\activate'
   ```
4. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
5. Set up the database:
   ```sh
   mysql -u root -p < database.sql
   ```

## Usage
1. Run the application:
   ```sh
   python app.py
   ```
2. Open your web browser and go to:
   ```
   http://localhost:8000
   ```

## Dependencies
- Python
- Flask
- Twilio
- OpenCV
- Tesseract OCR
- Google Vision OCR
- MySQL

## License
This project is licensed under the MIT License.

