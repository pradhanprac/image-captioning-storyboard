
# 🎬 The Substance: Possession

**Presented by:** Haunted Algorithms Studios  


---

## 📌 Project Overview

**The Substance: Possession** is a supernatural horror short film concept developed by Group 6. Originally conceived as a psychological thriller, the story was reimagined to incorporate supernatural elements, possession, and ancient evil. The film revolves around Sophie, a chemist whose discovery of a mysterious drug unleashes sinister forces. 

This project combines creative storytelling with technical implementation using Python, Jupyter Notebooks, and CSV data handling to script dialogue, automate formatting, and simulate screenplay logic.

---

## 🎥 Storyline Flow

1. **Discovery of the Substance** – Sophie finds an ancient compound during research.
2. **Testing the Drug** – Administered to Sophie and Emma, triggering supernatural hallucinations.
3. **Possession** – Spirits take over minds, leading to erratic behavior and horror.
4. **Investigation and Conflict** – Sophie and Samir uncover the origins and nature of the elixir.
5. **Final Confrontation** – Characters try to destroy the drug as spirits resist.
6. **Open-Ended Ending** – Leaves space for a sequel or continued horror.

---

## 🧠 Code Overview & Flow Explanation

This notebook acts as a **visual dialogue renderer**, converting raw scene images and dialogue CSVs into a polished, stylized storyboard. Here's a breakdown of libraries and logic:

### 📦 Python Libraries Used

| Library | Purpose |
|--------|---------|
| `cv2 (OpenCV)` | Read, resize, cartoonize, and border images |
| `numpy` | Handle image matrix operations |
| `PIL (Pillow)` | Draw text on images, apply transparency layers |
| `pandas` | Read dialogues from CSV |
| `IPython.display` | Display final images inside the notebook |
| `fpdf`, `os`, `tempfile` | (Optional) Handle file saving or PDF export |

---

### 🔁 Code Flow

#### 1. **Image Compression**
```python
imgcompress_mem(path_in, k)
```
- Resizes an image using OpenCV for efficient processing.

#### 2. **Cartoonization + Text Overlay**
```python
cartoonizeblt_mem_nb(path_in, k, blur, line, text)
```
- Converts the image into a cartoon style using blur + edge detection.
- Draws multiline text on the bottom with transparent overlay.

#### 3. **Process a Row of Frames**
```python
simple_row(folder, text_csv, list_nlines, font='Inkfree')
```
- Reads images from a folder and dialogues from CSV.
- Applies cartoonization and text overlay to all.
- Resizes and adds white borders.

#### 4. **Display Full Storyboard**
```python
display_images(images)
```
- Stacks images in rows of 4.
- Adds final black border and shows the storyboard as one scrollable output.

---

## 📁 Project Files

```
📁 The-Substance-Possession
├── Assignment_Final.ipynb              # English version screenplay logic
├── Assignment_Final_Hindi.ipynb        # Hindi version for bilingual presentation
├── dialogues_2.csv                     # Dialogue data used in both notebooks
├── Group 6 Poster.png                  # Film poster
├── Oscars Project Group 6.pdf          # Full story, cast, and scene documentation
├── README.md                           # You're here :)
```

---

## 👥 Cast & Roles

| Actor             | Role        | Description |
|------------------|-------------|-------------|
| **Samiksha Gupta** | Sophie      | Chemist, central protagonist, becomes possessed |
| **Atharva Chonkar** | Dr. Samir   | Rational scientist, friend and helper |
| **Prachi Pradhan** | Emma        | Best friend, first to be possessed |
| **Divyans Jemini** | Spirits     | Antagonists, supernatural entities |

---

## 🎭 Key Highlights

- **Genre**: Supernatural Horror  
- **Tools**: Python, Jupyter Notebook, Google Colab  
- **Data Handling**: CSV-based dialogue simulation  
- **Poster Design**: Visual storytelling and branding  
- **Bilingual Execution**: Hindi & English versions  
- **Creative Writing**: Genre transformation, character development

---

## 🚀 How to Use

1. Clone or download this repository.
2. Open `Assignment_Final.ipynb` or `Assignment_Final_Hindi.ipynb` in Jupyter/Colab.
3. Run all cells to view the visual storyboard with dialogues.
4. Check `Oscars Project Group 6.pdf` for full concept explanation.
5. Use `Group 6 Poster.png` for visual branding or presentation.

---

> *"You belong to us now." — The Spirits*  
> *A tale of curiosity, consequence, and the creeping dark that follows.*

---
