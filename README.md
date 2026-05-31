# SAGE Child Care Quick App - Vite Edition

A modern React app built with Vite for SAGE Apple Valley Child Care Center. Teachers can quickly capture photos, add development tags, and generate parent updates. Parents can securely view their child's updates.

## Features

- 📸 **Photo Capture**: Take photos directly via webcam or upload from device
- 🎯 **Smart Tags**: Quick-select developmental milestones (learning, social, character, creativity)
- 💬 **AI-Powered Updates**: Auto-generate warm, encouraging parent updates
- 🔒 **Secure Parent Portal**: PIN-protected access to individual child updates
- 🔊 **Audio Feedback**: Delightful sound effects for interactions
- 🌙 **Dark Mode**: Full dark mode support with Tailwind CSS

## Getting Started

### Prerequisites

- Node.js 16+ and npm

### Installation

1. Clone the repository:
```bash
git clone https://github.com/ldvareckas426/ChildCareQuickApp.git
cd ChildCareQuickApp
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

The app will open at `http://localhost:5173`

### Build for Production

```bash
npm run build
```

This creates an optimized build in the `dist` directory.

### Preview Production Build

```bash
npm run preview
```

## Project Structure

```
ChildCareQuickApp/
├── src/
│   ├── App.jsx           # Main React component
│   ├── main.jsx          # Entry point
│   └── index.css         # Global styles & Tailwind
├── index.html            # HTML entry point
├── vite.config.js        # Vite configuration
├── tailwind.config.js    # Tailwind CSS config
├── postcss.config.js     # PostCSS config
└── package.json          # Dependencies & scripts
```

## Configuration

### Firebase Setup

To enable Firestore integration, add Firebase config as global variables in your HTML:

```html
<script>
  window.__firebase_config = JSON.stringify({
    apiKey: "YOUR_API_KEY",
    authDomain: "your-app.firebaseapp.com",
    projectId: "your-project-id",
    storageBucket: "your-bucket.appspot.com",
    messagingSenderId: "YOUR_ID",
    appId: "YOUR_APP_ID"
  });
  window.__app_id = "your-app-identifier";
</script>
```

### Gemini API Setup

To enable AI sentence generation, add your Gemini API key in the `handleAIGenerateSentence` function in `src/App.jsx`.

## Technologies Used

- **React 18** - UI framework
- **Vite** - Lightning-fast build tool
- **Tailwind CSS** - Utility-first styling
- **Firebase** - Backend & real-time database
- **Web Audio API** - Sound effects
- **Web Camera API** - Photo capture

## License

This project is part of SAGE Apple Valley Child Care Center.

---

Built with ❤️ for teachers and parents
