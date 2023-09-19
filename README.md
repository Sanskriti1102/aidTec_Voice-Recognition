# Voice Recognition 

🔗[Voice-Recognition](https://github.com/Sanskriti1102/aidTec_Voice-Recognition/blob/main/Voice%20Recognition.ipynb)

This Python script allows you to perform voice recognition using the Google Web Speech API. 
It records audio from your microphone and then transcribes the spoken words into text. 
This can be a useful tool for various applications, including voice commands, speech-to-text conversion, and more.

## Getting Started

1. Before running the script, make sure to install the required Python packages using pip:
!pip install SpeechRecognition
!pip install pyaudio

## Code Explanation
**Importing Libraries:** We start by importing the necessary library, speech_recognition, which provides us with the tools for speech recognition.<br>
**Initializing the Recognizer:** We create a Recognizer object named recognizer to work with speech recognition.<br>
**Recording Audio:** With the help of the Microphone context manager, we capture audio from the computer's microphone. During this step, we also adjust for ambient noise to ensure accurate recognition. The timeout parameter specifies how long to record audio (in this case, 60 seconds).<br>
**Recognizing Speech:** We attempt to recognize the speech using the Google Web Speech API provided by the SpeechRecognition library. If the recognition is successful, we print the recognized text.<br>
**Handling Errors:** We handle two types of exceptions:

1. **sr.UnknownValueError:** This exception is raised if the recognizer couldn't understand the speech due to excessive noise or unclear pronunciation. <br>
2. **sr.RequestError:** This exception is raised if there's an issue with the request to the Google Web Speech API, such as a lack of internet connectivity.<br>

## Usage
You can use this script to experiment with voice recognition. It's a simple example of how to capture and convert speech to text in Python. Customize it as needed for your projects and applications.

#
Task By Info aidTech
--
