# Video Description and Voiceover Generator

This Python script processes a video file, generates a compelling description, creates a voiceover script in the style of David Attenborough, and synthesizes the voiceover using OpenAI's Text-to-Speech API.

## Features

- Extracts frames from a video file
- Generates a video description using GPT-4 Vision
- Creates a voiceover script in David Attenborough's style
- Synthesizes the voiceover using OpenAI's Text-to-Speech API

## Prerequisites

Before running the script, make sure you have the following installed:

- Python 3.x
- OpenCV (`opencv-python`)
- OpenAI Python library
- Requests library

Clone the Repo:

```
git clone https://github.com/RaheesAhmed/video_description_generator.git
```

Navigate to the Directory:
```
cd video_description_generator
```


You can install the required libraries using pip:

```
pip install opencv-python openai requests
```

## Setup

1. Clone this repository or download the script.
2. Set up your OpenAI API key as an environment variable in `.env` file :
   ```
   OPENAI_API_KEY='your-api-key-here'
   ```

## Usage

1. Place your video file in the `data` directory and name it `bison.mp4`, or modify the script to use a different file path.
2. Run the script:
   ```
   python main.py
   ```

The script will:
1. Extract frames from the video
2. Generate a video description
3. Create a voiceover script
4. Synthesize the voiceover audio

## Output

The script will print:
- The number of frames extracted from the video
- The generated video description
- The voiceover script

The synthesized audio will be available as a binary object, which can be saved to a file or played using appropriate audio libraries.

## Note

This script uses OpenAI's GPT-4 Vision model and Text-to-Speech API, which may incur costs. Make sure you're aware of the pricing and your usage limits.
