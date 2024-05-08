# AvA-1.0
# Automated Virtual Assistant (Ava)

This is a Python program that creates a virtual assistant named Ava. Ava can perform various tasks such as playing songs on YouTube, telling the current time and date, introducing itself, providing information about people from Wikipedia, and responding to basic questions like "How are you?".

## Prerequisites

Before running the program, make sure you have the following Python libraries installed:

- `speech_recognition`
- `pyttsx3`
- `pywhatkit`
- `datetime`
- `wikipedia`

You can install these libraries using `pip`:

## Usage

To run the virtual assistant, simply execute the Python script. The program will listen for your voice input and perform the corresponding action based on your instructions.

Here are the available voice commands:

- "Play [song name]": Plays the specified song on YouTube.
- "Time": Tells the current time.
- "Date": Tells the current date.
- "How are you?": The assistant responds by saying it's doing good and asking about you.
- "What's your name?": The assistant introduces itself as Ava.
- "Who is [person]?": The assistant provides a brief summary about the specified person from Wikipedia.

If the voice input is not recognized, the assistant will ask you to provide the instruction again.

## Functions

The program consists of the following functions:

1. `talk(text)`: This function uses the `pyttsx3` library to convert text to speech and play the audio output.

2. `input_instruction()`: This function listens for voice input using the `speech_recognition` library and converts it to text using Google's speech recognition service. It returns the recognized instruction as a string.

3. `play_ava()`: This is the main function that handles the user's voice instructions. It calls the `input_instruction()` function to get the user's input, and then performs the appropriate action based on the instruction.

## Note

Please note that this program requires an active internet connection to use the Google speech recognition service and access Wikipedia. Additionally, the program assumes that your system has a working microphone for voice input.
