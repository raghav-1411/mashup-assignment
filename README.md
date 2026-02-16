# Mashup

A YouTube mashup generator that downloads videos from any artist, extracts audio, trims clips, and merges them into a single mashup track.

## Student Details
- **Name:** Raghav Chhabra  
- **Roll Number:** <102303580> 

## Programs

### Program 1 - Command Line Tool

A Python CLI that creates audio mashups from YouTube videos.

**Features:**
- Download N videos for any artist from YouTube
- Convert videos to MP3 audio
- Trim first Y seconds from each track
- Merge all clips into one output file
- Automatic cleanup of temporary files

**Quick Start:**
```powershell
cd program1
pip install -r requirements.txt
python 102303557.py "Arijit Singh" 15 25 output.mp3
```

### Program 2 - Web Application

A Streamlit web interface that provides the same mashup functionality with email delivery.


> **Note:** Due to YouTube's strict anti-bot policies, the deployed version may encounter `403 Forbidden` or "Sign in to confirm you’re not a bot" errors. It is highly recommended to **run the app locally** for reliable performance.

**Features:**
- User-friendly web interface
- Same mashup generation as CLI
- Email delivery of completed mashup as ZIP file
- Powered by Mailjet for email

**Quick Start:**
```powershell
cd program2
pip install -r requirements.txt
streamlit run app.py
```

## Environment Setup

Copy `sample .env` to `.env` in the root folder and fill in your Mailjet credentials (required for Program 2):

```
SENDER_NAME=Your Name
SENDER_EMAIL=your-verified-email@example.com
MJ_APIKEY_PUBLIC=your-mailjet-public-api-key
MJ_APIKEY_PRIVATE=your-mailjet-private-api-key
```

## Requirements

- Python 3.10+
- Internet connection for YouTube downloads
- Mailjet account (for web app email delivery)

## License

MIT License
