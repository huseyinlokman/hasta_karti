# Hasta Kartı Uygulaması

## Overview
This Flask web application processes uploaded `.docx` files, extracts specific data, and generates new `.docx` documents based on predefined templates. The generated documents are then packaged into a `.zip` file for download. The application is designed to handle Turkish character conversions and document classification based on doctor names.

## Features
- Upload `.docx` files via a web interface.
- Process document tables and extract specific information.
- Generate customized `.docx` files using templates.
- Organize output files into categorized subfolders.
- Compress generated files into a `.zip` for easy download.
- Automatic cleanup of uploaded and generated files.

## Installation
### Prerequisites
- Python 3.8+
- Flask
- python-docx

### Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/hasta-karti.git
   cd hasta-karti
   ```
2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows, use venv\Scripts\activate
   ```
3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
1. Start the Flask application:
   ```sh
   python app.py
   ```
2. Open a web browser and navigate to:
   ```
   http://127.0.0.1:5000/
   ```
3. Upload a `.docx` file and process it.
4. Download the generated `.zip` file containing the processed documents.

## API Endpoints
### `GET /`
- Loads the upload page.

### `POST /upload`
- Accepts a `.docx` file upload and processes it.
- Returns a `.zip` file containing the generated documents.

### `POST /cleanup`
- Deletes all uploaded and generated files.

## File Structure
```
/
├── uploads/        # Temporary storage for uploaded files
├── outputs/        # Processed document storage
├── templates/      # HTML templates for the web interface
├── app.py          # Main Flask application
├── requirements.txt # Required Python packages
└── README.md       # Project documentation
```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.


## Author
Developed by huseyinlokman.

