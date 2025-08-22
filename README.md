README.txt

# Emotion Detection Web Application

## Overview

This project is a web-based application designed to detect and analyze emotions from user-provided text. Utilizing a Flask backend and integrating with an external sentiment analysis API, the application processes input text to identify emotions such as anger, joy, sadness, fear, and disgust. The system then determines the dominant emotion and displays the results to the user.

## Features

* Emotion Analysis: Processes input text to identify and quantify emotions.
* Dominant Emotion Detection: Determines the primary emotion expressed in the text.
* Error Handling: Manages blank or invalid entries by providing appropriate feedback.
* User Interface: Simple and intuitive web interface for user interaction.

## Technologies Used

* Backend: Python with Flask framework
* Emotion Detection API: Integration with an external sentiment analysis API
* Frontend: HTML templates rendered by Flask
* Version Control: Git for source code management

## File Structure

EmotionDetection/
├── **init**.py
├── emotion\_detection.py
server.py
templates/
├── index.html
test\_emotion\_detection.py
README.txt
.gitignore

* EmotionDetection/: Contains the module responsible for emotion detection logic.
* server.py: The main Flask application file that handles routing and user requests.
* templates/: Directory containing HTML templates for the user interface.
* test\_emotion\_detection.py: Test suite for validating the emotion detection functionality.
* README.txt: This file, providing an overview of the project.
* .gitignore: Specifies files and directories to be ignored by Git.

## Setup Instructions

1. Clone the Repository:

```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

2. Install Dependencies:

It's recommended to use a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

Then, install the required packages:

```bash
pip install -r requirements.txt
```

3. Run the Application:

Start the Flask development server:

```bash
python server.py
```

The application will be accessible at `http://127.0.0.1:5000/` in your web browser.

## Usage

* Navigate to the application in your browser.
* Enter a statement or text into the provided input field.
* Submit the form to receive an analysis of the emotions expressed in the text.
* If the input is blank or invalid, the system will prompt you to "Please try again!".
* The results will display the detected emotions and the dominant emotion.

## Error Handling

The application includes error handling for blank or invalid entries:

* Blank Input: If the input field is empty, the system will return a message prompting the user to try again.
* API Errors: If the external sentiment analysis API returns an error, the system will handle it gracefully and inform the user.

## Testing

Unit tests are provided in `test_emotion_detection.py` to ensure the functionality of the emotion detection logic. To run the tests:

```bash
pytest test_emotion_detection.py
```

## Deployment

For deployment in a production environment, consider using a WSGI server like Gunicorn and a reverse proxy such as Nginx. Ensure that environment variables and configurations are set appropriately for the production environment.


## Acknowledgments

Primary Instructors

* Abhishek Gagneja

* Sina Nazeri

Other Contributors and Staff 

* Project Lead: Rav Ahuja

* Instructional Designers: Andrew Pfeiffer, Bethany Hundutt

* Lab Authors: Abhishek Gagneja, Sina Nazeri, Vicky Kuo, Shivam Kumar

Production Team

* Publishing: Grace Barker, Jada Harrison

* QA: Mary Stenberg, Mercedes Schneider, Steve Hord

* Project Managers: Chaitra Nama, Simranjit Singh

* Narration: Bella West, Sarah Ruth

Video Production: Anmol Soni, Emily Lewis, Prayas Gupta, Sachin Kumar, Sanjay Soni, Tori Sleeper, Vaishali Rani
* Flask documentation and community for their support and resources.
