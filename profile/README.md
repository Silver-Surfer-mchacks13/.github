# 🏄‍♂️ Silver Surfer

> *Empowering the elderly to navigate the digital world with confidence and ease*

[![McHacks 13](https://img.shields.io/badge/McHacks-13-blue)](https://mchacks. ca/)
[![Built with Plasmo](https://img.shields.io/badge/Built%20with-Plasmo-blueviolet)](https://www.plasmo.com/)
[![Next.js](https://img.shields.io/badge/Next.js-16-black)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![LangChain](https://img.shields.io/badge/🦜🔗-LangChain-green)](https://www.langchain.com/)

## 🌟 About

**Silver Surfer** is a comprehensive browser extension solution developed at McHacks 13 that makes navigating the web a breeze for the elderly. We recognize that the digital divide affects older adults significantly, and our mission is to bridge that gap with intuitive, accessible, and AI-powered tools. 

### The Problem

Older adults often face challenges when navigating the web:
- 🔍 Small text and buttons are difficult to see and click
- 🧩 Complex interfaces can be overwhelming
- 🔒 Security concerns and scam detection
- 📱 Modern web design often prioritizes aesthetics over accessibility
- 🤖 Information overload makes finding relevant content difficult

### Our Solution

Silver Surfer provides a suite of AI-powered accessibility features directly in the browser, helping elderly users:
- ✨ Simplify complex web pages with AI summarization
- 🔍 Enhance readability with customizable text sizes
- 🎯 Navigate with confidence using guided assistance
- 🛡️ Stay safe online with intelligent security features
- 🤖 Get contextual help powered by LangChain and OpenAI

## 🏗️ Architecture

Our project consists of two main repositories:

### 1. 🎨 [Frontend:  Silver-Surfer-Plasmo-Extension](https://github.com/Silver-Surfer-mchacks13/Silver-Surfer-Plasmo-Extension)

The browser extension interface built with modern web technologies: 

**Features:**
- 📱 Side panel interface for easy access to tools
- 🎨 Content scripts for real-time page enhancement
- 💾 Storage management for user preferences
- 🔗 Tab and activeTab permissions for seamless integration
- ⚡ Real-time communication with backend services

**Tech Stack:**
- **Framework:** Plasmo (Browser Extension Framework)
- **UI Library:** React 18
- **Language:** TypeScript
- **Styling:** TailwindCSS
- **Build Tool:** Plasmo Build System

**Permissions:**
- Side Panel API
- Storage API
- Tabs & Active Tab
- Identity API
- Offscreen API
- Host permissions for secure communication

### 2. 🔧 [Backend: Silver-Surfer-Main](https://github.com/Silver-Surfer-mchacks13/Silver-Surfer-Main)

AI-powered backend service located in the `test-backend` folder:

**Features:**
- 🤖 LangChain integration for intelligent content processing
- 🧠 OpenAI API integration for advanced language understanding (Speech to text)
- 💬 ElevenLabs for Text to Speech
- ✨ Agentic Development and Conversation using page and image context with Gemini 3.0 Preview through OpenRouter
- 📝 Content simplification and summarization
- 🔍 Web page analysis and accessibility improvements
- 🎯 Context-aware assistance

**Tech Stack:**
- **Framework:** Next.js 16
- **Language:** TypeScript
- **AI/ML:** LangChain, OpenAI, Gemini 3.0 Preview Model, OpenRouter
- **Runtime:** Node.js

**API Endpoints:**
- Content simplification
- Page summarization
- Accessibility analysis
- Security assessment

## ✨ Features

### Core Functionality
- 🔠 **Text Enhancement**: Increase font sizes and improve contrast
- 📖 **AI-Powered Simplification**: Convert complex pages to reader-friendly formats using LangChain
- 🎨 **Visual Adjustments**: Customize colors, spacing, and layouts
- 🗣️ **Voice Assistance**: Text-to-speech for web content
- 🔐 **Security Alerts**: Can find items on websites and adds to cart as well as magnfies, highlights, and can book reservations at ease. 
- ⚡ **Quick Actions**: Streamlined common tasks with one-click access
- 💾 **Personal Preferences**: Save and sync settings across devices
- 🆘 **Ask for help** : SOS button that can send automated messages when things go wrong to a discord server.

### AI-Powered Features
- 🤖 **Smart Summaries**:  Get concise summaries of long articles
- 💬 **Contextual Help**: Ask questions about the current page
- 🎯 **Content Focus**: Automatically highlight important information
- 🔍 **Enhanced Search**: Better search results tailored for elderly users

## 🚀 Getting Started

### For Users

1. Download the Silver Surfer extension *(coming soon to Chrome Web Store)*
2. Pin the extension to your browser toolbar
3. Click the Silver Surfer icon to open the side panel
4. Customize your preferences and start browsing with confidence! 

### For Developers

#### Prerequisites
- Node.js 18+
- pnpm or npm (preferably pnpm - for frontend)
- Git
- OpenAI API Key (for backend)/ Gemini Key + OpenRouter Key 

#### Frontend Setup

1. **Clone the extension repository:**
```bash
git clone https://github.com/Silver-Surfer-mchacks13/Silver-Surfer-Plasmo-Extension.git
cd Silver-Surfer-Plasmo-Extension
```

2. **Install dependencies:**
```bash
pnpm install
# or
npm install
```

3. **Start development server:**
```bash
pnpm dev
# or
npm run dev
```

4. **Load the extension:**
   - Open Chrome and navigate to `chrome://extensions/`
   - Enable "Developer mode"
   - Click "Load unpacked"
   - Select the `build/chrome-mv3-dev` directory

#### Backend Setup

1. **Clone the main repository:**
```bash
git clone https://github.com/Silver-Surfer-mchacks13/Silver-Surfer-Main.git
cd Silver-Surfer-Main/test-backend
```

2. **Install dependencies:**
```bash
npm install
```

3. **Configure environment variables:**
```bash
cp .env.local.example .env.local
# Edit .env.local and add your OpenAI API key
```

4. **Start the development server:**
```bash
npm run dev
```

The backend will be available at `http://localhost:3000`

#### Connecting Frontend and Backend

Update the extension's manifest to point to your local backend: 
- Frontend communicates with backend via API calls
- Ensure CORS is properly configured
- Backend runs on `localhost:3000` by default

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|------------|---------|
| Plasmo | Browser extension framework |
| React 18 | UI component library |
| TypeScript | Type-safe development |
| TailwindCSS | Utility-first styling |
| Chrome Extension APIs | Browser integration |

### Backend
| Technology | Purpose |
|------------|---------|
| Next.js 16 | React framework with API routes |
| LangChain | LLM orchestration framework |
| OpenAI/ Gemini via OpenRouter | Advanced language models |
| TypeScript | Type-safe development |

## 👥 Team

Silver Surfer was created by a passionate team at McHacks 13:
- **Andrew** - Fullstack & AI integration
- **Joyal** - Frontend Development * UI/UX + Testing
- **Thomas** - Backend Development + End to End Voice Training AI model for Speech to Text and Text to Speech
- **Bryan** - Fullstack & AI Integration

## 📂 Repository Structure

```
Silver-Surfer-mchacks13/
├── Silver-Surfer-Plasmo-Extension/    # Browser Extension (Frontend)
│   ├── src/                           # Extension source code
│   ├── assets/                        # Images and icons
│   ├── public/                        # Public assets
│   └── package.json                   # Frontend dependencies
│
└── Silver-Surfer-Main/                # Main Repository
    └── test-backend/                  # Next.js Backend
        ├── src/                       # Backend source code
        ├── package.json              # Backend dependencies
        └── . env.local. example        # Environment template
```

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

1. Fork the relevant repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Follow TypeScript best practices
- Write meaningful commit messages
- Test your changes thoroughly
- Update documentation as needed
- Ensure accessibility standards are met

## 📝 License

This project is currently unlicensed. All rights reserved by the Silver Surfer team.

## 🎯 Roadmap

### 🔮 Future Plans
- [ ] Multi-language support
- [ ] Mobile companion app
- [ ] Chrome Web Store publication
- [ ] Firefox and Edge support
- [ ] Advanced personalization features
- [ ] Offline mode with caching
- [ ] Community-driven presets
- [ ] Security and Fraud prevention with harmful ads.

## 🔗 Quick Links

- **Frontend Repository**: [Silver-Surfer-Plasmo-Extension](https://github.com/Silver-Surfer-mchacks13/Silver-Surfer-Plasmo-Extension)
- **Backend Repository**: [Silver-Surfer-Main](https://github.com/Silver-Surfer-mchacks13/Silver-Surfer-Main)
- **Demo Video**: [Video](https://www.youtube.com/watch?v=HM00RuoAPd4&t=1s)
## 📧 Contact

Have questions or feedback?  Reach out to us: 
- **GitHub**: [@Silver-Surfer-mchacks13](https://github.com/Silver-Surfer-mchacks13)
- **Project Link**: [Silver Surfer](https://github.com/Silver-Surfer-mchacks13)

## 🙏 Acknowledgments

- **McHacks 13** for providing the platform to build this project
- **Plasmo Team** for their excellent browser extension framework
- **LangChain** for powerful AI orchestration tools
- **OpenAI** for advanced language model capabilities
- The elderly community for inspiring this solution
- All testers and contributors who helped make this project better

---

<p align="center">
  <strong>Made with ❤️ at McHacks 13</strong><br>
  <em>Empowering seniors, one click at a time</em>
</p>

<p align="center">
  <a href="https://github.com/Silver-Surfer-mchacks13/Silver-Surfer-Plasmo-Extension">Frontend</a> •
  <a href="https://github.com/Silver-Surfer-mchacks13/Silver-Surfer-Main">Backend</a> •
  <a href="https://github.com/Silver-Surfer-mchacks13">Organization</a>
</p>
