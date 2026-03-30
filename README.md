# 🎬 AI Video Generation Pipeline

This project is a custom-built AI pipeline that converts a simple user idea into a short video with visuals, captions, and background music.


## 🎥 Demo

![Demo](assets/demo.gif)


**Example Input:**
"AI in healthcare"

**Output:**
A short multi-scene video with captions, transitions, and music.

---


## ⚡ What This Does

Input:
"AI in healthcare"

**Output:**
- Structured story-based script
- Scene-wise captions
- Visual sequence (manual / API-ready)
- Final compiled video (MP4)

---

## 🚀 Features

- Takes a user topic as input
- Generates structured prompts (story-based)
- Supports manual or API-based image input
- Adds captions to each scene
- Combines images into a video with transitions and background music
- Designed for automation workflows


---

## 🧠 How it works

```
User Input (Topic)
        ↓
Prompt Generator (structured narrative)
        ↓
Image Source (manual / API-ready)
        ↓
Caption Overlay (PIL)
        ↓
Video Builder (MoviePy)
        ↓
Final Video Output
```

---


## 📌 Example

Input:

```
AI in healthcare
```

## 🌐 Flask API (Backend Simulation)

This project includes a Flask API layer to simulate how the pipeline can be deployed as a backend service.

**Endpoint:**
POST /generate

**Example Request:**
```json
{
        "topic": "AI in healthcare"
}
```

**Response:**
```json
{
  "status": "success",
  "output": "outputs/final_video.mp4"
}
```
## 📊 Results

- Generated 20+ test videos
- Avg generation time: ~15–30 seconds
- Supports multi-scene narrative structure
- Handles missing images with fallback logic

---

## 🛠 Tech Stack

- Python
- MoviePy (video processing)
- Pillow / PIL (image + captions)
- Requests (API-ready integration)
- Flask (API layer)

---

- 🎬 Format: MP4
- ⏱ Duration: ~30–60 seconds
- 🎞 Scenes: 4–6
- 📁 Output: `outputs/final_video.mp4`



## ⚙️ Setup

```bash
git clone https://github.com/YOUR_USERNAME/ai-video-generation-pipeline.git
cd ai-video-generation-pipeline
pip install -r requirements.txt
```

---

## ▶️ Run

```bash
python main.py

Then enter:

* Topic (e.g. "AI in healthcare")
* Mode: manual / api

---

## 🎯 Why this project?

This project demonstrates how real-world AI systems are built using pipelines that combine multiple components like prompting, media generation, and automation.

It reflects practical backend system design used in content generation tools.

## 🧠 System Design Highlights

- Modular pipeline architecture
- Separation of concerns (prompt → image → video)
- Extensible for API integrations (image generation, TTS)
- Designed for both manual and automated workflows


## ⚠️ Important Note

Currently, images are manually sourced for demonstration purposes.

The pipeline is designed to support full API-based image generation, making it easily extendable into a fully automated system.


## 📈 Future Improvements

- Full API-based image generation
- Text-to-speech (voiceover)
- Improved transitions and animations
- CLI support (--topic, --mode)
- Web interface for non-technical users


💡 Motivation

This project started as an experiment with no-code tools (n8n). It helped me quickly prototype the idea, but I realized I wanted more control and flexibility.

So I rebuilt the entire pipeline from scratch in Python, making it modular and extensible.


📬 Feedback


Open to suggestions and improvements!

Open to suggestions, improvements, and collaboration!


👨‍💻 Author

Vivek Devda
B.Tech Artificial Intelligence & Machine Learning

GitHub: https://github.com/vivek-devda
