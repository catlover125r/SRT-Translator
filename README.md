# SRT Translator

A client-side tool that translates **SRT subtitle files from English to Spanish** and auto-downloads the result.

## Features

- Drag-and-drop or click-to-upload `.srt` files
- Preserves SRT format — indices and timecodes are untouched
- Batches subtitle text for efficient API usage (max 4,500 chars/request with `|||` separators)
- Sends up to 3 concurrent requests for speed
- Real-time progress display ("batch X of Y")
- Auto-downloads translated file with `_spanish` suffix
- Fully client-side — subtitles only go to the translation API, nowhere else

## Tech Stack

- Vanilla JavaScript, HTML5, CSS3
- [MyMemory Translation API](https://mymemory.translated.net/) — free, no API key required

## How to Use

1. Open `index.html` in any modern browser
2. Drag and drop an `.srt` file onto the page (or click to browse)
3. Wait for translation to complete — progress is shown in real time
4. The translated file downloads automatically as `filename_spanish.srt`

Requires an internet connection for the MyMemory API.
