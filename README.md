# Voxel World - A Minecraft Clone Demo

A simple Minecraft-inspired voxel game demo built using HTML, CSS, and Three.js. This project showcases procedural world generation, chunk loading, block interaction, a dynamic day/night cycle, and a handheld torch with particle effects, all running directly in the browser.

## ✨ Features

*   **Procedural World Generation:** Infinite terrain generated using Value Noise.
*   **Chunk System:** Loads and renders the world in manageable chunks based on render distance.
*   **First-Person Controls:** Standard WASD movement, mouse look (using PointerLockControls), jumping, and flying.
*   **Block Interaction:**
    *   Left-click to break blocks.
    *   Right-click to place selected blocks.
*   **Block Types:** Includes basic blocks like Grass, Dirt, Stone, Wood, and Leaves.
*   **Procedural Textures:** Block textures are generated on the fly using the Canvas API, reducing the need for external image assets.
*   **Dynamic Day/Night Cycle:**
    *   Simulated sun and moon movement.
    *   Changes in sky color, fog density/color, and directional light intensity/color based on the time of day.
    *   CSS-based starfield visible at night.
*   **Handheld Torch:**
    *   ViewModel torch rendered in the player's view.
    *   Dynamic point light attached to the torch.
    *   Flame particle system using Three.js Points.
    *   Subtle flickering effects on light and flame.
*   **Basic Collision Detection:** Simple Axis-Aligned Bounding Box (AABB) collision with world blocks.
*   **On-Screen Info:** Displays player position, current chunk, fly/ground status, and in-game time.

## 🛠️ Technology Stack

*   **HTML5:** Structure of the web page.
*   **CSS3:** Styling for the UI elements (blocker, crosshair, info text, stars).
*   **JavaScript (ES Modules):** Core game logic, rendering, and interactions.
*   **Three.js:** A powerful 3D graphics library for rendering the voxel world, handling camera, lighting, and geometry. Loaded via `importmap` from UNPKG.

## 🚀 Getting Started

This project is designed to be simple to run.

**Method 1: Direct File Access (Easiest)**

1.  Download the `index.html` file from this repository.
2.  Open the `index.html` file directly in a modern web browser (like Chrome, Firefox, Edge, Safari).

    *Note: While this often works for simple projects using external CDNs like UNPKG, complex browser security features (especially around file access or future local assets) might sometimes cause issues. If you encounter problems, try Method 2.*

**Method 2: Using a Local Web Server (Recommended)**

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
    cd YOUR_REPOSITORY_NAME
    ```
    *(Replace `YOUR_USERNAME` and `YOUR_REPOSITORY_NAME`)*

2.  **Start a simple local web server** in the project directory. Here are a few ways:
    *   **Using Python 3:**
        ```bash
        python -m http.server
        ```
    *   **Using Node.js (requires `http-server` installed globally):**
        ```bash
        npm install -g http-server
        http-server
        ```
    *   **Using VS Code:** Install the "Live Server" extension and click "Go Live" from the status bar.

3.  Open your web browser and navigate to the local address provided by the server (usually `http://localhost:8000`, `http://localhost:8080`, or similar).

## 🎮 Controls

*   **W, A, S, D:** Move Forward / Left / Backward / Right
*   **SPACE:** Jump (when on ground) / Fly Up (when in Fly Mode)
*   **SHIFT:** Fly Down (when in Fly Mode) / Crouch (TBD)
*   **MOUSE:** Look Around
*   **LEFT CLICK:** Break Block
*   **RIGHT CLICK:** Place Block (selected type shown in bottom-left)
*   **F:** Toggle Fly Mode
*   **1-5:** Select Block Type to Place (1: Stone, 2: Dirt, 3: Grass, 4: Wood, 5: Leaves)
*   **ESC:** Release mouse lock / Pause


