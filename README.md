# YouTube Shorts Maker Agent

## 🎯 Goal
Build a system that automatically produces YouTube Shorts videos from a provided topic.

---

## 🤝 Cooperative Agents

### 🎬 Content Planning Agent
Analyzes the topic and structures a detailed second-by-second scenario, including narration tone, visual concepts, and text overlays.

### 🖼️ Asset Generation Agent
Generates all required images and narration according to the planned scenario.  
Uses OpenAI’s DALL·E model for images, and a TTS model for generating narration.

### 🎥 Video Editing Agent
Combines the generated images and narration along a timeline, then renders the final 1080×1920 Shorts video (MP4) using FFmpeg.

### 🧩 Image Production Agent
Transforms optimized prompts into 9:16 vertical images using the GPT-Image-1 model.

### ✍️ Prompt Writing Agent
Creates optimized prompts based on scene descriptions that are easily understood by the image-generation AI, then provides them to the Image Production Agent.

### 🗣️ Audio Generation Agent
Processes text-to-speech narration scripts using the GPT-4o Mini TTS model to produce high-quality voice-over audio files.

---

## 📘 Workflow Diagram
<img src="youtube_shorts_maker_agent_diagram.png" alt="YouTube Shorts Maker Agent Diagram" width="50%" height="50%">
