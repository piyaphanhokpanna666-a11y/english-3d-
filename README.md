# **Voxel English Quest 3D**

A lightweight, single-file 3D educational web game built with **Three.js** and **Tailwind CSS**. In this game, players navigate a voxel-style world, avoid enemies, collect score boxes, and answer English quizzes to earn stars. The game is completely self-contained within a single HTML file, requiring no external image or audio assets.

## **🎮 Features**

* **Single-File Architecture:** Everything (HTML, CSS, 3D Logic, UI, and Audio) is bundled into one index.html file.  
* **Voxel 3D Graphics:** Built with Three.js featuring procedural environment generation (randomized buildings, trees, and item spawns).  
* **Synthesized Sound Effects:** Uses the native Web Audio API (Oscillators) to generate all sound effects dynamically—no external .mp3 or .wav files needed.  
* **Interactive UI:** Responsive, modern user interface built with Tailwind CSS, including a dynamic 2D floating Name Tag that tracks the 3D player model.  
* **Educational Gameplay:** Integrated English quiz system. Answer correctly to earn stars, answer incorrectly to spawn an extra enemy as a penalty\!  
* **Cross-Platform Controls:** Supports Keyboard (WASD/Arrows), Mouse (Click-to-move), and Touchscreen (Tap-to-move) for mobile compatibility.

## **🕹️ How to Play**

### **Objective**

Your goal is to collect **10 Stars** by answering the yellow Quiz Boxes correctly while avoiding the dark, red-eyed enemies.

### **Controls**

* **Keyboard:** Use W, A, S, D or Arrow Keys to move.  
* **Mouse:** Click anywhere on the ground to make your character walk to that specific point.  
* **Touch (Mobile):** Tap anywhere on the ground to move.

### **Game Elements**

* **Player:** The humanoid voxel character.  
* **Enemies (Black Boxes with Red Eyes):** They slowly chase you. If they catch you, it's Game Over\!  
* **Orange Boxes (Score):** Walk into these to earn \+10 points.  
* **Yellow Boxes (Quiz):** Walk into these to open the English Quiz modal.  
  * Correct Answer: \+50 points, \+1 Star.  
  * Wrong Answer: \+0 points, spawns an additional enemy.

## **🛠️ Technologies Used**

* **HTML5 / JavaScript (ES6)**  
* **Three.js** (v0.128.0) \- For 3D rendering and raycasting.  
* **Tailwind CSS** (via CDN) \- For styling the 2D UI overlays and modals.  
* **Web Audio API** \- For procedural sound synthesis.

## **🚀 How to Run**

Since the game is a single HTML file with no external local assets, running it is extremely simple:

1. Download or copy the code into a file named index.html.  
2. Double-click index.html to open it in any modern web browser (Chrome, Firefox, Edge, Safari).  
3. Type in your player name, click **"เริ่มเกม" (Start Game)**, and enjoy\!

*(Note: An active internet connection is required only on the first load to fetch the Three.js and Tailwind CSS libraries from their respective CDNs).*

## **📝 Customization**

You can easily modify the game by editing the index.html file:

* **Add more questions:** Find the quizBank array in the JavaScript section and add your own questions.  
* **Change Colors:** Modify the THREE.Color or THREE.MeshLambertMaterial hex codes.  
* **Adjust Difficulty:** Change the speed (player speed) or enemySpeed variables.

*Created as a demonstration of combining 3D WebGL, Procedural Audio, and Modern CSS in a minimal footprint.*