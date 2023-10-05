<!-- markdownlint-disable MD033 MD041 -->

<img
    src="https://kura.pro/audiotextpro/images/logos/audiotextpro.webp"
    alt="AudioTextPro logo"
    width="261"
    align="right" />

<!-- markdownlint-enable MD033 MD041 -->

# Python AudioTextPro

Convert audio to text accurately in real-time using our advanced AI speech
recognition technology.

## Overview 📖

AudioTextPro is a Python module designed to interact with the AssemblyAI API to
transcribe audio files. It provides a simple and efficient way to convert speech
into text using AssemblyAI's powerful transcription services.

## Features ✨

- [x] Uploads audio files to AssemblyAI.
- [x] Requests transcripts of uploaded audio files.
- [x] Processes and stores the resulting transcripts.
- [x] Simple API interaction through Python functions.
- [x] Extensible for future additions, such as more complex processing of
  transcripts.

## Requirements 📋

- Python 3.9 or higher
- The `requests`, and `python-dotenv` packages
- An AssemblyAI API key (get one [here](https://www.assemblyai.com/))

## Installation 🛠

1. Install the required packages:

```bash
pip install requests python-dotenv
```

1. Clone the audiotextpro repository:

```bash
git clone https://github.com/sebastienrousseau/audiotextpro.git
```

1. Add your OpenAI API key to a `.env` file in the project directory:

```bash

# API_TOKEN is used to authenticate with the AssemblyAI API.
# Replace with your actual API token from AssemblyAI.
API_TOKEN = ''

# FILENAME should be the path to the audio file you wish to transcribe.
# Replace with the path to your actual file.
FILENAME = ''

# TIMEOUT is the number of seconds to wait for the transcription to complete.
# Replace with the number of seconds you wish to wait.
TIMEOUT=""

```

## Usage 🚀

### Command Line Interface

To use AudioTextPro, navigate to the project directory in your terminal and
run the following command:

```bash
python3 -m audiotextpro
```

Ensure your audio file is accessible from the project and that the API key is
valid to avoid any request issues.

## File Structure 📁

```bash
.
├── LICENSE-APACHE
├── LICENSE-MIT
├── MANIFEST.in
├── Makefile
├── README.md
├── audiotextpro
│   ├── __init__.py
│   ├── __main__.py
│   ├── api.py
│   ├── file.py
│   ├── transcript.json
│   ├── transcript.txt
│   ├── transcript_processor.py
│   └── utils.py
├── pyproject.toml
├── requirements.txt
├── samples
│   └── call_from_a_customer.mp3
├── setup.cfg
├── setup.py
└── transcript.json

3 directories, 19 files
```

## License 📜

The project is licensed under the terms of both the MIT license and the
Apache License (Version 2.0).

- [Apache License, Version 2.0](https://opensource.org/license/apache-2-0/)
- [MIT license](https://opensource.org/licenses/MIT)