
```markdown
# MO903-T3-Final-Coursework

## Project: Optimization of Student Timetabling
Final academic coursework for **MO903** (UNICAMP). This document presents a formal study and optimization methodology for the Student Timetabling Problem, leveraging models developed during undergraduate research.

---

### 👤 Author
- **Luis Alberto Vásquez Vargas** (Master's Student @ IC-UNICAMP)
- **Professor:** Flávio Keidi Miyazawa

---

### 🛠️ Build Instructions (Arch Linux)

#### 1. Install dependencies
```bash
sudo pacman -S texlive-basic texlive-latexextra texlive-fontsrecommended \
               texlive-fontsextra texlive-bibtexextra texlive-plaingeneric \
               texlive-binextra texlive-science zathura zathura-pdf-mupdf \
               latexmk
```

#### 2. One-Line Build & Watch
Run this from the project root. It prepares the output directory and starts the live-recompile loop:
```bash
mkdir -p output && TEXINPUTS=./src//:./src/img//: \
latexmk -pdf -pvc -outdir=output src/main.tex
```

#### 3. Open Preview
Run this in a separate terminal:
```bash
zathura output/main.pdf
```

---

### ⚡ Workflow
* Edit modules in **Neovim** (e.g., `src/sections/methodology.tex`).
* Save file (`:w`).
* `latexmk` detects changes and updates the PDF in `output/`.
* **Zathura** refreshes the view instantly.

---

### 📂 Repository Structure
```text
.
├── output/             # Build artifacts and final PDF
│   └── main.pdf        # Rendered monograph
├── src/
│   ├── main.tex        # Entry point
│   ├── img/            # Static image assets (.png, .jpg)
│   ├── sections/       # Content modules (.tex)
│   └── structure/      # Preamble, metadata, and engine config
└── README.md
```

---

### 📋 Review Full Source
To dump the entire source code into the terminal in logical order for a final review:
```bash
find src -name "*.tex" -exec cat {} +
```

---

### ✅ Mandatory Requirements
- [ ] Font size 11pt + 1.5 Line Spacing
- [ ] Maximum 2 pages (excluding cover and references)
- [ ] At least 3 bibliographic references
- [ ] Final filename: `LuisAlberto-t3.pdf`
```
