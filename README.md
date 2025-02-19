# American Sign Language Detection

A real-time American Sign Language (ASL) detection system using computer vision and machine learning.

## Features

- Real-time ASL detection through webcam
- Static image processing for ASL signs
- REST API for sign language prediction
- GUI interface for easy interaction
- Supports both Python and Go clients

## Technical Stack

- Python 3.x
- OpenCV for video processing
- MediaPipe for hand, face, and pose detection
- Flask for API endpoints
- scikit-learn for machine learning
- Go for client implementation

## Project Structure

- `script.py`: Main script for video processing and landmark detection
- `asl_api.py`: Flask API for sign language prediction
- `asl_data_collector.py`: Data collection utility
- `asl_model_trainer.py`: Model training script
- `gui.py`: Graphical user interface
- `client.go`: Go client for the API
- `models/`: Directory containing trained models
- `asl_dataset.csv`: Dataset for training

## Setup and Installation

1. Clone the repository:
```bash
git clone https://github.com/mesutoezdil/American-Sign-Language-Detection.git
cd American-Sign-Language-Detection
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install opencv-python mediapipe numpy flask scikit-learn
```

## Usage

1. For real-time webcam detection:
```bash
python script.py
```

2. To start the API server:
```bash
python asl_api.py
```

3. To use the GUI:
```bash
python gui.py
```

## API Endpoints

- POST `/predict`: Send an image file to get ASL prediction
  - Request: Multipart form with 'image' field
  - Response: JSON with prediction or error message

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.