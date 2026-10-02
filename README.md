# Curriculum-Vitae

[![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat&logo=latex&logoColor=white)](https://www.latex-project.org/)
[![Build](https://github.com/leelening/curriculum_vitae/actions/workflows/latex.yml/badge.svg)](https://github.com/leelening/curriculum_vitae/actions/workflows/latex.yml)

Professional CV/Resume repository for Lening Li (郦乐宁).

## Overview

This repository contains the LaTeX source files for my professional curriculum vitae and resume, available in both English and Chinese.

## 📄 Documents

| Document | Source | Description |
|----------|--------|-------------|
| **English CV** | [`CV_English.tex`](./CV_English.tex) | Full academic and professional CV |
| **Chinese CV** | [`cv_Chinese.tex`](./cv_Chinese.tex) | 中文履历 |
| **Resume** | [`Resume.tex`](./Resume.tex) | Condensed one-page resume |

PDFs are not stored in this repository. Every `.tex` file is compiled by GitHub Actions on each push; download the built PDFs from the [latest workflow run](https://github.com/leelening/curriculum_vitae/actions/workflows/latex.yml) under **Artifacts**.

## Tech Stack

- **Typesetting**: LaTeX
- **Document Class**: Custom `resume.cls`
- **Bibliography**: BibTeX
- **Build Tool**: pdfLaTeX/XeLaTeX

## Features

- ✅ Professional academic CV format
- ✅ Multiple language support (English/Chinese)
- ✅ BibTeX integration for publications
- ✅ Clean, modern typography
- ✅ Easy to customize and extend

## Building from Source

### Prerequisites

- LaTeX distribution (TeX Live or MiKTeX)
- `resume.cls` class file (included)

### Build Instructions

```bash
# Clone the repository
git clone https://github.com/leelening/curriculum_vitae.git
cd curriculum_vitae

# Build English CV
pdflatex CV_English.tex
bibtex CV_English
pdflatex CV_English.tex
pdflatex CV_English.tex

# Build Chinese CV
xelatex cv_Chinese.tex

# Build Resume
pdflatex Resume.tex
```

## Project Structure

```
.
├── .github/workflows/
│   └── latex.yml        # CI: compiles every .tex, uploads PDFs as artifacts
├── CV_English.tex       # English CV source
├── cv_Chinese.tex       # Chinese CV source
├── Resume.tex           # Resume source
├── archive/             # Superseded sources, not built by CI
│   ├── CV_AGC_Associate_TMT.tex
│   └── CV_KPMG_Manager_AI.tex
├── resume.cls           # Custom LaTeX class
└── refs.bib             # Bibliography references
```

## Sections Included

- **Contact Information**: Email, phone, location
- **Research Interests**: Reinforcement Learning, Optimal Control, Game Theory, Formal Methods
- **Education**: Carnegie Mellon University (MBA), WPI (Ph.D., M.S.)
- **Professional Experience**: Yale University, Harvard University, Symbotic, Berkshire Grey
- **Publications**: Journal papers, conference papers, arXiv preprints
- **Teaching Experience**: Graduate courses at WPI
- **Honors & Awards**: Academic achievements
- **Skills**: Programming languages, tools, frameworks

## About the Author

**Lening Li**
- Research Affiliate at Yale University
- Robotic Lab Advisor at Harvard University
- Former Senior Software Engineer at Symbotic (Oct. 2022 – Sep. 2026)
- Ph.D. in Robotics Engineering (WPI)
- MBA Candidate at Carnegie Mellon University

## License

Feel free to use the LaTeX template for your own CV, but please customize the content for your own use.

## Contact

- Email: leningli@outlook.com
- GitHub: [@leelening](https://github.com/leelening)
- Website: [leelening.github.io](https://leelening.github.io)
