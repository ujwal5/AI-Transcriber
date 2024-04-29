# Transcriber
This Python script utilizes the WhisperX library to perform transcription and speaker diarization on audio files. It defines a Transcriber class with methods to transcribe audio files and extract speaker information. The script utilizes a pre-trained model (large-v2) from WhisperX for transcription and speaker diarization.
# WhisperX Transcriber

## Overview
WhisperX Transcriber is a Python script for performing transcription and speaker diarization on audio files using the WhisperX library. This script utilizes pre-trained models for accurate transcription and speaker segmentation.

## Features
- Transcription of audio files
- Speaker diarization to identify speakers in the audio
- Support for batch processing
- Flexible GPU memory management

## Installation
1. Install the required libraries using pip:
   ```bash
   pip install git+https://github.com/m-bain/whisperx.git
   pip install pyannote.audio
   
## Clone this repository:
git clone https://github.com/yourusername/whisperx-transcriber.git

## USAGE

## Import the Transcriber class from transcriber.py
from transcriber import Transcriber

## Create an instance of the Transcriber class:
transcriber = Transcriber()

## Set the path to your audio file:
transcriber.audio_file = "path/to/your/audio/file.mp4"

## Obtain transcription results:
result = transcriber.get_transcribe_dict()

## Access transcription segments and speaker information from the result dictionary:
for segment in result['segments']:
    print("Text:", segment.get('text'))
    print("Speaker:", segment.get('speaker'))


## Dependencies
- Python 3.x
- WhisperX
- Pyannote.audio



Further you can edit in the code and add a line where if you want to save the output in .txt file 
# Set the output file name
output_file = "transcript.txt"

# Save the transcript to a text file
transcriber.save_transcript(result, output_file)

print(f"Transcript saved to: {output_file}")



## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

Replace `"path/to/your/audio/file.mp4"` with the actual path to your audio file. Also, update the GitHub repository link (`https://github.com/yourusername/whisperx-transcriber.git`) to point to your repository. This README file provides users with instructions on how to install, use, and contribute to your WhisperX Transcriber project.

