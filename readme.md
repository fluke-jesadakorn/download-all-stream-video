# M3U8 Video Downloader

This project is a Python script that downloads video segments from an M3U8 playlist and saves them into a single `.ts` file. The script supports resuming the download from the last completed segment in case of interruptions.

## Features

- Fetches an M3U8 playlist and parses its segments.
- Downloads video segments and appends them to an output file.
- Resumes download from the last successfully downloaded segment in case of interruptions.
- Configurable via environment variables.

## Requirements

- Python 3.6+
- `requests` library
- `m3u8` library
- `python-dotenv` library

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/m3u8-video-downloader.git
    cd m3u8-video-downloader
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

3. Create a `.env` file in the root directory of the project and add the following content:
    ```env
    DOWNLOAD_URL=https://hlsp2p.xyz/files/c53af19e043341c85eb35d67e6b21ac9_1080p.txt
    OUTPUT_FILE=badboy.ts
    ```

## Usage

Run the script using Python:
```sh
python downloader.py
