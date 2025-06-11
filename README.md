# Kingshot Map Editor & Planner

A dynamic, web-based isometric map planner designed for strategic visualization. This tool provides an interactive canvas for viewing and planning on a large grid, with features like dynamic zooming, panning, and object placement.

![image](https://github.com/user-attachments/assets/5190d976-12ca-4a71-aa46-346c1a6f0698)


---

## ✨ Features

*   **Isometric Grid:** A large 1200x1200 tile grid rendered on an HTML5 canvas.
*   **Dynamic Panning & Zooming:** Smoothly pan with mouse drag or keyboard arrows, and zoom using the mouse wheel, pinch gestures, or on-screen controls.
*   **Optimized Rendering:** Uses chunk-based rendering for high performance, only drawing what's visible on screen.
*   **Coordinate System:** Displays tile coordinates and building information interactively.
*   **Object Placement:** Load and display building footprints from external JSON data.
*   **Responsive UI:** User interface elements are designed to be intuitive and work across different screen sizes.

## 🕹️ Controls

| Action          | Method                                     |
| --------------- | ------------------------------------------ |
| **Pan**         | Drag with mouse, one-finger touch, or arrows |
| **Zoom**        | Mouse wheel, pinch-to-zoom, `+`/`-` keys   |
| **Select Tile** | Click or tap on a tile or building         |
| **Go to Tile**  | Enter X/Y coordinates and click "Go"       |

## 🚀 Local Development

To run this project on your local machine:

1.  Clone or download the repository.
2.  Ensure the following files are in the same directory:
    *   `map.html` (the main file)
    *   `baseMap.json`
    *   `patch_notes.json`
3.  Because the application uses the `fetch()` API to load local JSON files, you may need to run it from a simple local web server to avoid browser security (CORS) errors. A simple way to do this is with Python:
    ```bash
    # From your project directory, run:
    python -m http.server
    ```
    Then, open your browser to `http://localhost:8000`.

## ⚖️ License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.
