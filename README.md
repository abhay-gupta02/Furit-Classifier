# Furit Classifier


## Overview
Fruit Classifier is a machine learning-based web application that identifies different fruit types from images. It utilizes a trained model integrated into a Flask backend, enabling real-time classification through API endpoints.

## Features
- **Machine Learning Integration**: Uses a trained model to classify fruit images.
- **REST API**: Provides endpoints for uploading images and receiving classification results.
- **Scalable Backend**: Developed using Flask for efficient request handling.
- **JSON Responses**: Returns structured classification results in JSON format.

## Tech Stack
- **Programming Language**: Python
- **Frameworks & Libraries**: Flask, TensorFlow/Keras, OpenCV, NumPy
- **Database**: SQLite (if needed for logging queries)
- **Developer Tools**: Postman (for API testing), Git, Visual Studio Code

## Installation
### Prerequisites
Ensure you have the following installed:
- Python (>=3.8)
- pip
- Virtual Environment (recommended)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/abhay-gupta/fruit-classifier.git
   cd fruit-classifier
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Flask application:
   ```bash
   python app.py
   ```

## API Endpoints
### 1. Upload Image
- **Endpoint**: `POST /classify`
- **Description**: Accepts an image file and returns the classification result.
- **Request Format**:
  ```bash
  curl -X POST -F "file=@apple.jpg" http://127.0.0.1:5000/classify
  ```
- **Response Format**:
  ```json
  {
    "fruit": "Apple",
    "confidence": 95.3
  }
  ```

## Future Enhancements
- Improve model accuracy with a larger dataset.
- Deploy on AWS or GCP for cloud-based inference.
- Add a frontend interface for easier usage.

## Contribution
Contributions are welcome! Fork the repo, create a new branch, and submit a pull request.

## Contact
For queries or contributions, reach out to:
- **Email**: ag770527@gmail.com
- **LinkedIn**: [Abhay Gupta](https://www.linkedin.com/in/abhay-gupta-30017021b/)

