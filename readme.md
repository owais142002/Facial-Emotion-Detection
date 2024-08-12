# Facial Emotion Detection using YOLOv8

This project is a Flask web application that detects facial emotions in real-time using a YOLOv8 model. The model can detect the following emotions:
- Disgusted
- Surprised
- Angry
- Sad
- Happy
- Scared
- Neutral

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Training Your Own Model](#training-your-own-model)
- [Project Structure](#project-structure)
- [License](#license)

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/owaisahmed142002/facial-emotion-detection.git
   cd facial-emotion-detection
   ```

2. **Set up a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
## Usage

1. **Run the Flask app:**
   ```bash
   python app.py
   ```
2. **Open your web browser and navigate to:**
   ```bash
   http://127.0.0.1:5000/
   ```
3. **Upload an image or start the webcam to detect emotions.**
   
## Training Your Own Model

If you want to train your own model, follow these steps:
1. **Prepare your dataset:**
Ensure your dataset is labeled and formatted correctly for YOLOv8.
2. **Train the model:**
   ```bash
   python train/train.py
   ```
The model after training will get stored in the runs directory, copy the .pt file of the model, and paste the file into the model directory.

## Project Structure

app.py: The main Flask application file.

requirements.txt: List of dependencies required for the project.

templates/: Directory containing HTML templates.

static/: Directory for static files like uploaded images.

models/: Directory containing the trained YOLOv8 model.

train/: Directory containing the training script.

README.md: This documentation file.

## Acknowledgments
Roboflow provided us with a platform for dataset annotation.

Ultralytics, for their pre-trained YOLOv8 weights.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

Feel free to contribute to this project by opening issues or submitting pull requests. Happy coding!
