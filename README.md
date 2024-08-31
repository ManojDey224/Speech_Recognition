# Speech_Recognition
# AssemblyAI Speech Recognition Demo

This repository demonstrates the capabilities of AssemblyAI's speech recognition API using Python.  The code shows how to transcribe audio from a URL, customize transcription settings, extract various insights from the transcript, and export subtitles.

## Getting Started

1. **Installation:** 
   - Make sure you have Python and the `assemblyai` library installed. You can install it using `pip`: 
      ```bash
      pip install assemblyai
      ```

2. **API Key:** 
   - Get your API key from AssemblyAI's website ([https://www.assemblyai.com/](https://www.assemblyai.com/)). 
   - Replace `"YOUR_API_KEY"` in the `speech_recognition.py` file with your actual API key:
      ```python
      aai.settings.api_key = "YOUR_API_KEY" 
      ```

## Usage 

The provided Python script (`speech_recognition.py`) includes examples of the following:

- **Basic Transcription:** Transcribe audio from a provided URL and display the text output.

- **Custom Transcription Configuration:**
    - **Speech Model Selection:** Choose a specific speech recognition model like `nano`, `conversational`, etc.
    - **Punctuation & Formatting:** Disable/Enable punctuation or text formatting.
    - **Language Detection:** Automatically detect the language spoken in the audio.
    - **Custom Spelling:** Correct commonly mispronounced words or define custom terminology.
    - **Word Boost:** Increase the likelihood of recognizing specific words or phrases (useful for technical jargon or domain-specific language). 
    - **Dual-Channel Transcription:**  Transcribe separate audio channels and distinguish speakers (requires dual-channel audio input). 
    - **Disfluencies:** Choose whether to keep disfluencies ("um", "uh", etc.) or have them removed. 
    - **Profanity Filtering:** Filter out profanity in the transcript output. 
    - **Audio Trimming:**  Select a specific segment of the audio file to transcribe.
    - **Speech Threshold:** Control the sensitivity for detecting speech (higher threshold means fewer false positives). 

- **Export Subtitles:** 
   - Generate subtitle files in SRT (SubRip) and VTT (WebVTT) formats, including options for character limits per caption. 

- **Extract Key Insights:**
   - **Sentences:** Get individual sentences from the transcript.
   - **Paragraphs:** Divide the transcript into meaningful paragraphs.
   - **Word Search:**  Count occurrences of specific words or phrases in the transcript. 

## Running the Demo

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/AssemblyAI-Speech-Recognition-Demo.git
2.Navigate to the directory:
cd AssemblyAI-Speech-Recognition-Demo
3.Execute the script:
python speech_recognition.py
