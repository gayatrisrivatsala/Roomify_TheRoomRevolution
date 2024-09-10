# Flask Image Generation API

This project is a Flask-based web application that provides an API for generating images based on user prompts and uploaded sketches. It also includes a feature to retrieve items from a database based on room type and cost range.

## Features

- Image generation using Stability AI API
- Database integration for item retrieval
- CORS support for cross-origin requests


## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.6+
- pip (Python package manager)
- Stability AI API key

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd <project-directory>
   ```

2. Install the required dependencies:
   ```
   pip install flask flask-cors requests
   ```

3. Set up your Stability AI API key:
   - Create a `.env` file in the project root
   - Add your API key: `STABILITY_KEY=your_api_key_here`

## Configuration

1. Folders:
   - The script will automatically create `uploads/images` and `static/images/generated` folders

## Usage

1. Start the Flask server:
   ```
   python app.py
   ```
2. API Endpoints:
   - GET `/items`: Retrieve items based on room type and cost range
     - Query parameters: `room` and `range`
   - POST `/generate`: Generate an image based on a prompt and uploaded sketch

## File Structure

- `app.py`: Main Flask application file
- `templates/index.html`: HTML template for the web interface
- `uploads/images/`: Directory for uploaded sketch images
- `static/images/generated/`: Directory for generated images
