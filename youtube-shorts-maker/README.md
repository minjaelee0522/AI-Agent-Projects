# YouTube Shorts Maker Agent

## 🎯 Goal
Build a system that automatically produces YouTube Shorts videos from a given topic.

---

## 🤝 Cooperative Agents

### Content Planning Agent
Analyzes the topic and determines a detailed video scenario down to the second — including narration tone, visual concepts, and text overlays.

### Asset Generation Agent
Generates required images and narration according to the planned scenario.  
Uses OpenAI’s DALL-E for image creation, and a TTS model for voice narration.

### Video Editing Agent
Combines generated images and voice assets along a timeline, then renders a final 1080x1920 resolution video using FFmpeg.

### Image Production Agent
Converts optimized prompts into 9:16 image assets using the GPT-Image-1 model.

### Prompt Writing Agent
Creates optimized prompts based on scene descriptions and sends them to the Image Production Agent.

### Audio Generation Agent
Converts text-based narration scripts into high-quality audio files using the GPT-4o Mini TTS model.

---
