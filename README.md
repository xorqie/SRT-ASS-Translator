# 🎌 SRT/ASS Subtitle Translator v1.0.0

<div align="center">

**A powerful, AI-powered SRT/ASS subtitle translation tool designed for Localization/Subtitle Translation enthusiasts**

[Download Latest Release](https://github.com/xorqie/subtitle-translator/releases) • [Report Bug](https://github.com/xorqie/subtitle-translator/issues) • [Request Feature](https://github.com/xorqie/subtitle-translator/issues)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Download & Installation](#-download--installation)
- [Quick Start Guide](#-quick-start-guide)
- [Supported Languages](#-supported-languages)
- [Translation Engines](#-translation-engines)
- [Smart Logging](#-smart-logging)
- [System Requirements](#-system-requirements)
- [FAQ](#-faq)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)
- [Credits](#-credits)

---

## 🎯 Overview

**Subtitle Translator Pro** is a desktop application built in Python that makes translating subtitles effortless. Whether you're a fansub group, a language learner, localization company, freelancer or just want to translate your favorite show/anime/movie in your native language, this tool provides professional-grade translations on SRT/ASS subtitles with minimal effort using Gemini's Model.

### Why This Tool?

- 🚀 **Fast Batch Processing**: Translate hundreds of subtitle files in minutes
- 🤖 **AI-Powered**: Choose between Google Translate or advanced Gemini AI
- 🎨 **Beautiful Interface**: Modern, cyberpunk-inspired dark theme
- 📊 **Smart Filtering**: Only logs important translations, not common phrases
- 🔄 **Format Preservation**: Maintains timing, styling, and special formatting
- 🌍 **Multi-Language**: Supports 10+ languages including Serbian, Croatian, Japanese, and more

---

## ✨ Features

### Core Features

| Feature | Description |
|---------|-------------|
| Multiple Formats | Supports .srt, .ass, and .ssa subtitle formats |
| Batch Translation | Process multiple files simultaneously |
| Dual Translation Engines | Choose between Google Translate (free) or Gemini AI (advanced) |
| Smart Logging | Filters out common phrases, logs only meaningful translations |
| Video Extraction | Extract embedded subtitles from .mp4, .mkv, .avi files using FFmpeg |
| Language Labels | Automatically adds language name to translated files |
| Progress Tracking | Real-time progress with accurate ETA |
| Clipboard Support | Paste files directly using Ctrl+V |
| Statistics Dashboard | View detailed translation statistics |

### Advanced Features

- ✅ **Formatting Preservation**: Keeps ASS/SSA override tags, HTML formatting, and line breaks
- ✅ **Serbian Latin/Cyrillic**: Automatic conversion for Serbian translations
- ✅ **Rate Limit Protection**: Built-in rate limiting for Gemini API (1000 requests/day)
- ✅ **Session Logging**: Detailed logs of all translations with pattern detection
- ✅ **Drag & Drop** (if TkinterDnD2 is available)
- ✅ **Customizable UI Language**: English and Serbian interface

---

## 💾 Download & Installation

### Option 1: Download Pre-Built Executable (Recommended)

1. Go to the [Releases Page](https://github.com/xorqie/subtitle-translator/releases)
2. Download the latest `SubtitleTranslator.exe`
3. Run the executable - **no installation required!**

> ⚠️ **Windows SmartScreen Warning**: Windows may show a warning because the app is unsigned. Click "More info" → "Run anyway"

### Option 2: Build from Source

**Requirements:**
- Python 3.8 or higher
- pip package manager

**Installation Steps:**

```bash
# Clone the repository
git clone https://github.com/xorqie/subtitle-translator.git
cd subtitle-translator

# Install dependencies
pip install -r requirements.txt

# Run the application
python main.py
```

---

## 🚀 Quick Start Guide

### Step 1: Launch the Application

Double-click `SubtitleTranslator.exe` or run `python main.py`

### Step 2: Select Files

- Click **"Select Files"** button, or
- Use **Ctrl+V** to paste files from Windows Explorer

### Step 3: Choose Languages

- **From**: Select source language (or use "Auto Detect")
- **To**: Select target language

### Step 4: Configure Translation Engine

1. Click **"⚙️ Settings"**
2. Choose **Google** (free, no setup) or **Gemini** (better quality)
3. If using Gemini:
   - Get API key from [Google AI Studio](https://aistudio.google.com/apikey)
   - Paste it in the API Key field
   - Click **"💾 Save Settings"**

### Step 5: Start Translation

Click **"▶️ Start Translation"** and wait for completion!

**Output**: Find translated files in `Translated_to_[Language]_[Timestamp]` folder

---

## 🌍 Supported Languages

| Code | Language | Native Name |
|------|----------|-------------|
| `sr-Latn` | Serbian (Latin) | Srpski (latinica) |
| `sr-Cyrl` | Serbian (Cyrillic) | Српски (ћирилица) |
| `hr` | Croatian | Hrvatski |
| `bs` | Bosnian | Bosanski |
| `en` | English | English |
| `ja` | Japanese | 日本語 |
| `es` | Spanish | Español |
| `fr` | French | Français |
| `de` | German | Deutsch |
| `ru` | Russian | Русский |

---

## 🤖 Translation Engines

### Google Translate (Free)
- ✅ No API key required
- ✅ Fast and reliable
- ✅ Good for general translations
- ❌ Less accurate for idioms and slang

### Gemini AI (Advanced)
- ✅ Better context understanding
- ✅ Superior handling of anime-specific terms
- ✅ More natural translations
- ✅ Free tier: 1000 requests/day
- ⚠️ Requires API key (free from Google)

**Get Gemini API Key**: [https://aistudio.google.com/apikey](https://aistudio.google.com/apikey)

---

## 📊 Smart Logging

The app uses intelligent filtering to log only **important translations**:

### What Gets Logged:
- ✅ Anime-specific terms (jutsu, sensei, nakama, etc.)
- ✅ Long sentences (5+ words)
- ✅ Idioms and expressions
- ✅ Translations with significant length differences

### What Gets Filtered:
- ❌ Common phrases (yes, no, okay, etc.)
- ❌ Single punctuation marks
- ❌ Numbers only
- ❌ Duplicate translations

**Result**: Clean, readable logs focused on what matters!

---

## 💻 System Requirements

### Minimum Requirements
- **OS**: Windows 10 or later (64-bit)
- **RAM**: 4 GB
- **Storage**: 100 MB free space
- **Internet**: Required for translation APIs

### Recommended Requirements
- **OS**: Windows 11
- **RAM**: 8 GB or more
- **Storage**: 500 MB (for logs and output)
- **Internet**: Stable broadband connection

### Optional
- **FFmpeg**: Required only for video subtitle extraction
  - Download: [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html)

---

## ❓ FAQ

<details>
<summary><b>Is this app free?</b></summary>

Yes! The app itself is completely free and open-source. Translation services:
- **Google Translate**: Free, no limits
- **Gemini AI**: Free tier with 1000 requests/day
</details>

<details>
<summary><b>Do I need an internet connection?</b></summary>

Yes, translation requires internet access to communicate with Google/Gemini APIs.
</details>

<details>
<summary><b>Can I translate subtitles for commercial use?</b></summary>

The tool itself is MIT licensed. However, check Google's and Gemini's terms of service for commercial API usage.
</details>

<details>
<summary><b>What's the translation quality like?</b></summary>

- **Google**: Good for general dialogue, may struggle with idioms
- **Gemini**: Excellent context awareness, better for anime-specific terminology
</details>

<details>
<summary><b>Why does Windows block the .exe?</b></summary>

Because the app is unsigned. This is normal for indie software. Click "More info" → "Run anyway" to proceed safely.
</details>

<details>
<summary><b>Can I contribute translations or improvements?</b></summary>

Absolutely! See the [Contributing](#-contributing) section below.
</details>

---

## 🔧 Troubleshooting

### App Won't Start
```
Error: Missing DLL or Runtime Error
```
**Solution**: Install [Visual C++ Redistributable](https://aka.ms/vs/17/release/vc_redist.x64.exe)

### Translation Fails
```
Error: Failed to translate - API Error
```
**Solutions**:
1. Check internet connection
2. Verify Gemini API key (if using Gemini)
3. Check daily request limit (1000/day for Gemini)

### Subtitle Extraction Fails
```
Error: FFmpeg not found
```
**Solution**: Install FFmpeg and add to system PATH

### Settings Not Saving
**Solution**: 
1. Run as Administrator (right-click → Run as administrator)
2. Check if `settings.json` exists in app folder
3. Verify folder write permissions

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

### Reporting Bugs
1. Check [existing issues](https://github.com/xorqie/subtitle-translator/issues)
2. Create a new issue with:
   - Clear description
   - Steps to reproduce
   - Expected vs actual behavior
   - Screenshots if applicable

### Suggesting Features
Open an issue with the `enhancement` label and describe your idea!

### Pull Requests
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 xorqq

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software...
```

---

## 🙏 Credits

### Developer
- **xorqq** - [GitHub](https://github.com/xorqie)

### Technologies Used
- [Python 3](https://www.python.org/) - Core programming language
- [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) - Modern UI framework
- [Google Gemini AI](https://ai.google.dev/) - Advanced translation engine
- [Deep Translator](https://github.com/nidhaloff/deep-translator) - Google Translate wrapper
- [PySRT](https://github.com/byroot/pysrt) - SRT file parsing
- [PyASS](https://github.com/chireiden/pyass) - ASS/SSA file parsing
- [FFmpeg](https://ffmpeg.org/) - Video subtitle extraction

### Special Thanks
- **AniPiece** - Inspiration and testing
- All beta testers and contributors
- The open-source community

---

## 📞 Support

- 🐛 **Bug Reports**: [GitHub Issues](https://github.com/xorqie/subtitle-translator/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/xorqie/subtitle-translator/discussions)

---

## 🗺️ Roadmap

- [ ] **v1.1**: Add more languages (Polish, Turkish, etc.)
- [ ] **v1.2**: Real-time subtitle preview
- [ ] **v1.3**: Cloud backup for translation memory
- [ ] **v2.0**: Mac and Linux support
- [ ] **v2.1**: Browser extension for online streaming

---

<div align="center">

**Made with ❤️ for the anime community**

[⬆ Back to Top](https://github.com/xorqie/SRT-ASS-Translator?tab=readme-ov-file#-table-of-contents)

</div>
