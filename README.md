# Background Extractor – Foreground Object Remover

**Background Extractor** is a Python-based desktop application that removes moving foreground objects from video footage, revealing the static background. It can be particularly useful in applications like **air traffic monitoring**, where the goal is to isolate and study environmental patterns without interference from moving aircraft or vehicles.

---

##  Key Features

-  Record real-time video using your webcam.
-  Extract frames and navigate through them using a GUI.
-  Apply **Singular Value Decomposition (SVD)** to isolate and reconstruct the static background.
-  Display the reconstructed background in a visually interactive matplotlib viewer.
-  Built with `Tkinter` and `ttkbootstrap` for an enhanced UI experience.

---

##  Use Cases

- **Air Traffic Monitoring:** Filter out moving aircraft to analyze runway conditions or background weather patterns.
- **Surveillance:** Isolate static background from foot traffic to monitor fixed environmental changes.
- **Research & Education:** Demonstrates real-world application of **Truncated SVD** and image matrix decomposition.

---

##  Technologies Used

- **Python**
- **OpenCV** (Video capture and image handling)
- **NumPy** (Numerical operations)
- **Matplotlib** (Visualization)
- **PIL (Pillow)** (Image processing)
- **tkinter** + **ttkbootstrap** (Graphical User Interface)
- **scikit-learn** (TruncatedSVD for dimensionality reduction)

---

##  How It Works

1. **Record Video**  
   Start recording via webcam. Press `q` to stop recording.

2. **Frame Extraction**  
   Captures each video frame as `.jpg` and stores locally (to store frames make path acc to your system).

3. **GUI Navigation**  
   Scroll through the captured frames using "<<" and ">>" buttons in a viewer.

4. **Background Extraction**  
   Uses **SVD** to decompose the frame matrix and reconstruct the dominant (static) background layer.

5. **Visual Output**  
   The reconstructed background is displayed using Matplotlib inside a tkinter window.

---
