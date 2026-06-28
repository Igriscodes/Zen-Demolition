# Zen Demolition

A relaxing, interactive 3D destruction experience built with **Three.js**. Witness blocks shatter into physics-based fragments and rebuild your tower with a single keystroke.

## How to Play

* **Shatter:** Click on any block in the tower to break it apart.
* **Rebuild:** Press the **R** key at any time to reset the tower to its original state.
* **Automatic:** If you clear the entire tower, it will automatically rebuild itself after a short delay.

## Technical Implementation

This project utilizes [Three.js](https://threejs.org/) to handle rendering and physics simulations:

* **Renderer:** Uses `WebGLRenderer` with `antialias: true` for smooth edges.


* **Physics:** A custom Euler integration loop handles velocity, gravity ($-15 m/s^2$), and floor collision damping.


* **Interaction:** Employs `Raycaster` to detect mouse clicks in 3D space.


* **Visuals:** Features a pastel color palette and a gentle camera sway to maintain a "Zen" aesthetic.

## Getting Started

1. Clone this repository.
2. Open the `game.html` file in any modern web browser.
3. Ensure your browser supports ES Modules (required for the `importmap` implementation).
