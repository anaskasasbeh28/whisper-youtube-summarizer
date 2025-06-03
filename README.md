# YouTube Transcriber & Summarizer

This project is a simple but powerful Python tool that:

* Downloads audio from a YouTube video
* Transcribes the audio using OpenAI's Whisper model
* Generates two summaries:

  * An English bullet-point summary
  * A life-coach-style Arabic summary with a title and conclusion

## 🔧 Features

* 🎥 Download best-quality audio using `yt-dlp`
* 🧠 Transcribe with OpenAI Whisper (`whisper-1`)
* 📝 Summarize using `gpt-3.5-turbo` in both English and Arabic
* 📂 Saves transcript to a `.txt` file automatically

## 🚀 How It Works

1. **Install Requirements:**

   ```bash
   pip install yt-dlp openai
   sudo apt install ffmpeg -y  # (For audio conversion)
   ```

2. **Run the Script:**

   ```bash
   python youtube_transcriber_summarizer.py
   ```

3. **Follow Prompts:**

   * Paste a YouTube video URL when asked.
   * The script will download the audio, transcribe it, and summarize it.

4. **Outputs:**

   * `transcript-<video-title>.txt` — original transcript
   * Console output — English & Arabic summaries

## 📁 File Structure

```
.
├── youtube_transcriber_summarizer.py
├── transcript-أحمد الشقيري ｜｜ ردد دائماً!.txt
├── Youyube video link .txt
├── أحمد الشقيري ｜｜ ردد دائماً!.mp3
├── README.md

```

## 🔐 API Key

This script requires an OpenAI API key. Set it as an environment variable inside the script:

```python
os.environ['OPENAI_API_KEY'] = 'your-api-key-here'
```

Or manage it securely using `.env` files in future versions.

## ✅ Requirements

* Python 3.8+
* OpenAI account with API access
* `yt-dlp`, `ffmpeg`, `openai` Python libraries

## 📌 Example Use Cases

* Transcribing educational videos
* Summarizing long podcasts or interviews
* Generating Arabic self-development summaries from English content

## 📬 Future Ideas

* Export summaries to PDF
* Support for multiple languages
* Streamlit or Web UI

---

Made with ❤️ by \[Anas+ChatGPT] — your friendly Generative AI Engineer.
