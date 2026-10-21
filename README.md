# Scripts

A personal collection of utility scripts for downloading, converting, transcribing, and OCR'ing media and text, pulled out of individual project repos so they live in one place.

## Structure

```
downloaders/
├── youtube/                 yt-dlp wrappers: audio, transcripts
├── wise/                    WISE course video/drive downloaders
├── turathio/                Turath.io manuscript downloaders
└── islamicpearls/           Islamic Pearls downloader/helpers
transcription/
└── whispercpp/              whisper.cpp wrappers for audio transcription
ocr/                         Mistral and Tesseract OCR for scanned docs/manuscripts
audio/                       ffmpeg-based audio/video conversion (mov→wav, etc.)
extractors/                  Text/Arabic extraction from PDFs
lecture-title-renamer/       Batch renaming for lecture files
combine-lesson-text.py       Merge lesson transcript text files
create-lesson-notes.py       Build lesson notes from transcripts
```

## Requirements

- Python 3 (`pip install -r requirements.txt`)
- Node.js (for the Turath.io and WISE `.js`/`.mjs` scripts — `npm install`)
- `ffmpeg`, `yt-dlp`, and a built `whisper.cpp` on `PATH` for the relevant scripts

Most scripts are standalone — read the top of each file for required env vars (e.g. `MISTRAL_API_KEY`) and usage.
