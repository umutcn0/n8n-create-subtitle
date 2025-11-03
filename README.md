# 🎬 Subtitle Automation with n8n & ElevenLabs

This workflow automatically generates and embeds subtitles into videos using **n8n**, **ElevenLabs**, and **FFmpeg**.  
The user provides an audio file (extracted from a video), and the system handles transcription, subtitle creation, and video embedding — all automatically.

---

## ⚙️ Workflow Overview

![workflow](https://github.com/user-attachments/assets/7a89b933-7449-4ca4-969e-b2979911f7f3)


## ⚙️ Final Video Overview

https://github.com/user-attachments/assets/6389363a-f86a-4d37-8a9c-277235276faa

### Steps:
1️⃣ **Trigger:** Workflow starts manually (`When clicking 'Execute workflow'`).  
2️⃣ **Get Audio File:** Reads the audio file from disk.  
3️⃣ **Transcribe Audio:** Sends the audio to **ElevenLabs Speech-to-Text API** for transcription.  
4️⃣ **Create Subtitles:** Formats the transcription into `.ass` subtitle structure.  
5️⃣ **Save Subtitle:** Writes the generated `.ass` file to disk.  
6️⃣ **Execute Command:** Runs an **FFmpeg** command to embed the subtitles into the original video file.

---

## 🧠 Tech Stack
- **n8n** — Workflow automation  
- **ElevenLabs** — Speech-to-text conversion  
- **FFmpeg** — Subtitle embedding and video processing

---

## 🚀 How to Use
1. Clone this repository.  
2. Import the workflow JSON file into your n8n instance.  
3. Update your **ElevenLabs API key** in the HTTP Request node.  
4. Adjust input/output file paths as needed.  
5. Execute the workflow and enjoy automatically generated subtitles!

---

## 📁 Output
- `output.ass` — Generated subtitle file  
- `final_video.mp4` — Final video with embedded subtitles  

---

## 💬 Contact
If you’d like to try this workflow or have questions, feel free to reach out!  
📩 [Your LinkedIn Profile](https://www.linkedin.com/in/umutcn)

---

### ⭐ Bonus Tip
You can easily extend this workflow to:
- Automatically detect audio from uploaded videos  
- Translate subtitles into multiple languages  
- Upload the final video to YouTube or cloud storage automatically
