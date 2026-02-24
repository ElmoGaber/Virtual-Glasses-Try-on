# Virtual Glasses Try-On

![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-yellow)
![HTML5](https://img.shields.io/badge/HTML5-Ready-orange)
![CSS3](https://img.shields.io/badge/CSS3-Ready-blue)

**Try on glasses virtually in your browser** — no app download, no installation, just open your camera and see how different glasses frames look on your face instantly.

---

## ✨ Features

- Real-time face tracking and glasses overlay using webcam  
- Supports multiple glasses models (upload your own or use built-in ones)  
- Adjustable scale, rotation, and position of glasses  
- Works entirely client-side — zero server processing  
- Responsive design — looks great on desktop, tablet, and mobile  
- Simple and clean user interface  
- Easy to extend with new 3D glasses models  
- No login or data collection required  
- Fully open-source under MIT license  

---

## 🚀 Live Demo

You can try it right now:  
https://elmogaber.github.io/Virtual-Glasses-Try-on/

*(or open `index.html` directly in your browser after cloning)*

---

## 🛠 Tech Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript  
- **Face Detection & Tracking**: MediaPipe Face Mesh (Google)  
- **3D Rendering**: Three.js  
- **Glasses Models**: GLTF / GLB format (located in `/3dmodel`)  
- **Build Tools**: npm / package.json (no heavy bundler required)  
- **Assets**: Static images, styles, and 3D models in dedicated folders  

---

## 📥 Quick Start (Local)

```bash
# Clone the repository
git clone https://github.com/ElmoGaber/Virtual-Glasses-Try-on.git
cd Virtual-Glasses-Try-on
```

# Install dependencies (only needed if you want to modify/extend)
```
npm install
```

# Just open the file in browser (recommended for quick testing)
# Double-click index.html or use any local server
Easiest way:
```
Open index.html directly in Chrome / Edge / Firefox.
```
```
🖼 Project Structure
textVirtual-Glasses-Try-on/
├── 3dmodel/            # GLTF / GLB glasses models
├── images/             # Reference images, icons, backgrounds
├── js/                 # JavaScript logic (main.js, face tracking, rendering)
├── style/              # CSS files
├── .github/
├── .gitattributes
├── .gitignore
├── LICENSE
├── README.md
├── index.html
├── package.json
├── package-lock.json
└── ...
```
📸 Screenshots
(Place your screenshots in /images folder and update paths below)
<img src="images/demo1.jpg" alt="Virtual Try-On Demo 1">
<img src="images/demo2.jpg" alt="Virtual Try-On Demo 2">
<img src="images/multiple-frames.jpg" alt="Multiple Frames">

🔧 How to Add Your Own Glasses

Prepare a 3D model in GLTF/GLB format (Blender export works great)
Place it in the 3dmodel/ folder
Update the model selection array in js/main.js (or create UI buttons)
Adjust scale/position/rotation values if needed

Example code snippet:
```
JavaScriptconst glassesModels = [
    { path: '3dmodel/glasses1.glb', scale: 0.6, offsetY: -0.1 },
    { path: '3dmodel/your-new-glasses.glb', scale: 0.65, offsetY: -0.08 }
];
```



📄 License
MIT License — see the LICENSE file for full details.
You are free to use, modify, distribute, and even sell products based on this project.

🙏 Acknowledgments

MediaPipe by Google — amazing face mesh solution
Three.js — best WebGL library
Original inspiration from Benson Ruan's virtual try-on projects
Everyone who tested and gave feedback


Made with ❤️ by ElmoGaber
