# LEXICON 3D STUDIO — LLM Pipeline & 3D Vector Embedding Space

An interactive, zero-dependency visualizer and tokenizer studio designed to explore and understand how Large Language Models (LLMs) preprocess text, tokenize inputs, and map semantic relationships in 3D embedding space.

---

## 🌟 Key Features

### 1. 🌐 Interactive 3D Vector Embedding Space
- **3D Shaded Spheres & Floating Labels:** Words rendered as glossy 3D spheres with specular lighting, vertical leader stems, and category-colored pill cards.
- **Spatially Separated Category Sectors:** Clear spatial clustering for **Objects** (Cyan), **Actions** (Green), **Emotions** (Amber), **Grammar** (Slate), and **Concepts** (Red).
- **Dynamic Word Synchronization:** The 3D space strictly reflects the active sentence. Removing a word from the sentence immediately removes it from 3D space.
- **Persistent Separate Additions:** Words injected separately via Quick Add or Manual Node Creator persist with distinct cyan highlight rings.
- **Gesture Navigation:** Click and drag to rotate the 3D space, and scroll the mouse wheel to zoom in/out smoothly.

### 2. ✂️ Multi-Strategy Tokenizer
- Switch between **Word Tokens**, **Subword (BPE Simulation)**, and **Character-level** tokenization.
- Live token badges with unique token IDs (`#0`, `#1`, ...) and sequence array mapping (`[0, 1, 2, ...]`).
- Full Token Mapping Table displaying positions, token strings, assigned IDs, and grammatical types.

### 3. ⚖️ Cosine Similarity & Vector Math (Analogy Lab)
- **Cosine Calculator:** Live computation of cosine scores, angular separation (`θ`), vector norms, and dot products.
- **Ranked Nearest Neighbors:** Instantly discover and fly to the closest semantic neighbors of any selected word.
- **Vector Word Math:** Semantic arithmetic lab (`Word A − Word B + Word C ≈ Target`) with presets like `dog − cat + playing`.

### 4. ▦ Attention Heatmap & 3D Beam Highlighting
- Pairwise token co-occurrence and attention matrix with dynamic intensity shading.
- Hovering over any matrix cell draws a glowing highlight beam between the two corresponding nodes in the 3D space.

### 5. 📊 Corpus Analytics & Zipfian View
- Real-time metrics including **Type-Token Ratio (Lexical Diversity)**, average word length, and embedding magnitude.
- Interactive vertical bar chart visualizing word frequency distributions according to Zipf's law.

### 6. ↔️ Interactive Draggable Splitter & Dual Themes
- **Resizable Workspace:** Drag the center splitter bar left or right to dynamically balance the content panel and 3D map.
- **Light & Dark Modes:** Seamlessly toggle between **Deep Black Dark Mode** and **Clean Light Mode**.

---

## 🛠️ Architecture & Philosophy

- **Single File:** Self-contained entirely in `index.html` (CSS in `<style>`, JavaScript in `<script>`).
- **Zero Dependencies:** No npm, no external frameworks, no CDNs, no backend, and no API keys required.
- **Vanilla Performance:** Pure HTML5 Canvas 3D projection math and standard Web APIs.
- **Beginner-Friendly:** Fully documented with `// WHAT THIS DOES:` comments throughout the codebase.

---

## 🚀 Getting Started

Simply open `index.html` in any modern web browser:

```bash
# Clone the repository
git clone https://github.com/ParagSanghavi2008/LLM-Pipeline.git

# Navigate to directory
cd LLM-Pipeline

# Open in browser (macOS)
open index.html
```
*(On Windows or Linux, double-click `index.html` or open it with Chrome, Firefox, Safari, or Edge).*
