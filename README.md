# Nyan AI – Your Catgirl Chrome Assistant for Conversational Task Automation 🐾
Nyan AI is a Chrome Extension that brings a smart, interactive, and adorable catgirl-style AI assistant to your browser. More than just a desktop pet, Nyan AI combines Live2D animations, natural conversation, and goal-oriented task automation to help you navigate the web, complete daily tasks, and enjoy a more personalized digital experience — all based on your unique profile and preferences.

![Nyan AI Banner](https://user-images.githubusercontent.com/your-username/your-repo/assets/placeholder_banner.png)

<!-- We recommend you replace this link with a real project banner -->

**Nyan AI is more than just a desktop pet. She is a smart browser assistant powered by Live2D and large language models (LLMs). She can express vivid emotions, understand your voice commands, chat naturally, and even assist you with browsing tasks.**

[![GitHub issues](https://img.shields.io/github/issues/your-username/ai-nyan-extension)](https://github.com/your-username/ai-nyan-extension/issues)
[![GitHub forks](https://img.shields.io/github/forks/your-username/ai-nyan-extension)](https://github.com/your-username/ai-nyan-extension/network)
[![GitHub stars](https://img.shields.io/github/stars/your-username/ai-nyan-extension)](https://github.com/your-username/ai-nyan-extension/stargazers)
[![License: Apache-2.0](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0)

## ✨ Key Features

* **Dynamic Live2D Interaction**:

  * Real-time emotion-driven expressions and animations.
  * Supports multiple character models, each with unique personality traits (`roles.json`).

* **Voice Control & Dialogue**:

  * Integrated browser-based speech recognition (STT) and synthesis (TTS).
  * Supports high-quality external TTS services like Unreal Speech.
  * Custom lip-sync engine for realistic speaking animations.

* **Smart Browser Assistant**:

  * Natural language understanding (NLU) + LLM for intent conversion.
  * **Web actions**: navigate pages, click elements, manage tabs, scroll.
  * **Search & summarization**: find and summarize web content.

* **Multimodal AI Capabilities**:

  * **Vision (OCR)**: reads and understands text from images.
  * **DOM Structure Understanding**: faster and more accurate than OCR for structured automation.

* **🧩 Core Feature: Nyan Card System**:

  * Modular expansion system using JSON "Nyan Cards" to define appearance, personality, and complex behaviors.

* **Personalization & Memory**:

  * Lightweight memory system stores your nickname and preferences.
  * Remembers past websites you've analyzed for contextual conversations.

* **Highly Customizable**:

  * Detailed settings panel to manage LLM keys, TTS services, Nyan Cards, etc.

## 🎬 Demo

*Catgirl interacting with user GIF animation*

![Nyan AI Demo](https://user-images.githubusercontent.com/your-username/your-repo/assets/demo.gif)

*Settings Panel Screenshot*

![Nyan AI Settings](https://user-images.githubusercontent.com/your-username/your-repo/assets/settings_popup.png)

## 🚀 Installation & Usage

### 👤 For Regular Users

1. Go to the [Chrome Web Store]() to install. <!-- Add your link here -->
2. Click the Nyan AI icon in the top-right corner of the browser.
3. Sign in with your Google account.
4. Configure your LLM API key (OpenRouter or others recommended).
5. Click the "Show/Hide Nyan AI" toggle to summon the assistant.
6. Start interacting with your catgirl assistant!

### 🧑‍💻 For Developers

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/ai-nyan-extension.git
   ```
2. Open Chrome and go to `chrome://extensions`
3. Enable **Developer Mode** (top right)
4. Click **Load unpacked** and select the project folder.
5. Follow regular user steps from step 2 onward.

### 🎤 How to Interact

* **Voice input**: Click the mic icon next to Nyan.
* **Text input**: Use the chat input field under the dialogue bubble.
* **Install Nyan Cards**: Drag from the [Nyan Card Market & Generator](https://your-website-url.com) <!-- Replace with your site --> directly onto Nyan.

## 🛠️ Architecture & Tech Stack

```
[ User ] <--> [ Content Script ] <--> [ Background Script ] <--> [ APIs (LLM, TTS, Firebase) ]
   (DOM interaction)         (state/memory)                  (external services)
```

* **Language**: JavaScript
* **Rendering**: PIXI.js + pixi-live2d-display
* **Backend-as-a-Service**: Firebase
* **OCR**: Tesseract.js

## 🧩 Core System: Nyan Card

JSON-based modular definitions that customize:

* `modelPrompt`: change appearance/model
* `personalityPrompt`: change tone/personality
* `missionPrompt`: define task-oriented workflows

Visit: [https://your-website-url.com](https://your-website-url.com) <!-- Replace with your website -->

## 🤝 Contributing

1. Fork the repository
2. `git checkout -b feature/AmazingFeature`
3. `git commit -m 'Add some AmazingFeature'`
4. `git push origin feature/AmazingFeature`
5. Submit a pull request

## 📜 License

Licensed under the [MIT License](https://opensource.org/licenses/MIT).

## ❤️ Acknowledgments

* Live2D model creators (listed in `roles.json`)
* PIXI.js / pixi-live2d-display
* Tesseract.js
* The open-source community for their continued support
