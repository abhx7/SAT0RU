## Description
SAT0RU is a cursed technique visualizer based on the popular anime series, Jujutsu Kaisen 呪術廻戦. It combines the mediapipe library with three.js to recreate cursed techniques from Jujutsu Kaisen. Powered by Gemini 3.

This project has been further extended with the addition of **Cursed Technique Lapse: Blue** and refined gesture logic using GPT-assisted development.

![Demo GIF](https://github.com/user-attachments/assets/8ad2b871-02c0-4b97-95f3-34682e745be0)

## Features

This project utilizes particles to render volume-based cursed techniques:

* **Cursed Technique Lapse: Blue**
    * **Visuals:** A gravitational singularity that compresses space inward with spiraling attraction.
    * **Trigger:** Closed fist (all fingers curled).
* **Secret Technique: Hollow Purple**
    * **Visuals:** A chaotic singularity combining attraction and repulsion.
    * **Trigger:** "Pinch" gesture (Thumb + Index touching, remaining fingers extended).
* **Domain Expansion: Infinite Void**
    * **Visuals:** A multi-layered celestial domain featuring a bright event horizon ring, a vertical stream of infinite information, and a deep cosmos background.
    * **Trigger:** "Cross" gesture (Index + Middle fingers crossed).
* **Cursed Technique Reversal: Red**
    * **Visuals:** A blinding white-hot core generating a violent, jagged sphere of repulsive force.
    * **Trigger:** Index finger pointing up.
* **Domain Expansion: Malevolent Shrine**
    * **Visuals:** A dark, ominous aura representing the King of Curses.
    * **Trigger:** Flat hand / Prayer gesture.


## Advanced Features

### Dual-Hand Tracking
- Each hand is tracked independently.
- Techniques render on the corresponding side of the screen.
- Particle systems dynamically offset based on real hand position.

### Red–Blue Convergence System
- When Red and Blue are active simultaneously, both particle systems render independently.
- As hands move closer together, particle offsets interpolate toward a midpoint.
- When distance falls below a threshold, techniques merge into Hollow Purple.

### Spatial Interaction
- Particle origin follows real-time hand movement.
- Effects respond dynamically to hand proximity.
- Smooth interpolation prevents snapping or flickering.

### Dynamic State Blending
- Separate states for:
  - Single-hand activation
  - Dual activation
  - Convergence state
  - Full merged state
- Visual transitions are continuous rather than instant swaps.

### Postprocessing Effects
- Adaptive bloom intensity based on technique.
- Camera shake for high-energy states.
- Rotation logic varies per technique.

---

## Getting Started

### Prerequisites
You need a modern web browser (Chrome, Edge, Firefox) and a webcam.

### Installation
1.  **Clone the repo**
    ```bash
    git clone [https://github.com/abhx7/SAT0RU.git](https://github.com/abhx7/SAT0RU.git)
    cd SAT0RU
    ```

2.  **Run the project**
    **VS Code:** Install the "Live Server" extension, right-click `index.html`, and select "Open with Live Server".

## Note 

This project was originally built and powered by **Google Gemini 3**, with additional feature development and gesture enhancements implemented using GPT-assisted development.
