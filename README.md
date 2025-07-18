# AI Personality Traits Analyzer

## Project Overview
This project features an AI-powered voice assistant named Ilana that analyzes a user's personality traits (or rather, their emotional tone) based on their speech. It then provides an emotion-based response, aiming to offer empathetic and relevant feedback. The system uses speech-to-text for understanding user input and tone analysis to classify emotions.

## Features
* **Greeting:** Ilana greets the user based on the time of day.
* **Voice Recording:** Records user's voice for a specified duration (8 seconds).
* **Emotion Classification:** Analyzes the recorded audio's pitch, energy, and tempo to classify the speaker's emotional tone into categories: "Excited / Happy", "Calm / Sad", "Angry / Aggressive", or "Neutral / Balanced".
* **Speech-to-Text:** Converts the user's spoken words into text using Google Speech Recognition.
* **Emotion-based Responses:** Provides diverse and empathetic responses tailored to the detected emotion.
* **Interactive Loop:** Continues to analyze and respond until the user chooses to exit.

## Technologies Used
* Python 3.x
* `gTTS`: Google Text-to-Speech for Ilana's voice output.
* `playsound`: To play the generated audio files.
* `sounddevice`: For recording audio from the microphone.
* `soundfile`: For reading and writing audio files.
* `librosa`: For audio analysis (pitch, energy, tempo extraction).
* `numpy`: For numerical operations on audio data.
* `SpeechRecognition`: For converting speech to text using Google Web Speech API.

## Setup and Installation

To run this project, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YourGitHubUsername/AI_Personality_Traits.git](https://github.com/YourGitHubUsername/AI_Personality_Traits.git)
    cd AI_Personality_Traits
    ```
    (Remember to replace `YourGitHubUsername` with your actual GitHub username.)

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On macOS/Linux
    # For Windows: venv\Scripts\activate
    ```

3.  **Install the required libraries:**
    ```bash
    pip install gTTS playsound sounddevice soundfile librosa numpy SpeechRecognition
    ```
    *Note: `playsound` might require additional system dependencies depending on your OS. Refer to its documentation if you encounter issues.*
    *For `sounddevice`, you might need PortAudio. On Ubuntu, for example: `sudo apt-get install libportaudio2`.*

## How to Run

1.  **Ensure your microphone is properly configured.**
2.  **Run the main script:**
    ```bash
    python AI_Personality_Traits.ipynb
    ```
    *Note: While `AI_Personality_Traits.ipynb` is a Jupyter Notebook, it seems designed to be run as a Python script directly from the terminal. If you prefer to run it as a Jupyter Notebook, you'll need to install `jupyter` (`pip install jupyter`) and then run `jupyter notebook` in your project directory and open the `.ipynb` file.*

## Usage
Upon running the script, Ilana will greet you. She will then prompt you to speak for 8 seconds. After you speak, she will classify your tone and provide an appropriate response. You will then be asked if you want to try again or exit.

## Code Structure
* `AI_Personality_Traits.ipynb`: The main script containing all the functions for TTS, emotion classification, greeting, emotion-based responses, and the main execution loop.
* `temp_audio.mp3`: (Temporary file) Used for playing Ilana's speech.
* `temp.wav`: (Temporary file) Used for recording and processing user's voice.
* `.gitignore`: Specifies files and directories to be ignored by Git.

## Future Enhancements
* More sophisticated emotion detection models (e.g., using machine learning with larger datasets).
* Integration with a more advanced conversational AI framework.
* Expand the range of personality traits analyzed.
* User profile creation to track emotional trends over time.

## Contributing
Feel free to fork this repository and contribute! Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is open source and available under the MIT License.

## Connect
[Linkedin](https://www.linkedin.com/in/anjankarthikchandra)
