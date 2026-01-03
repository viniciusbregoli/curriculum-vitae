# CV / Curriculum Vitae

LaTeX source files for my CV in multiple languages.

## Files

- `cv_en.tex` - English version
- `cv_pt.tex` - Portuguese (BR) version
- `cv_de.tex` - German version

## Requirements

- LaTeX distribution (e.g., TeX Live, MiKTeX)
- Required packages: `geometry`, `titlesec`, `enumitem`, `hyperref`, `xcolor`

On Arch Linux:
```bash
sudo pacman -S texlive
```

On Ubuntu/Debian:
```bash
sudo apt install texlive-latex-base texlive-latex-recommended texlive-fonts-recommended
```

## Building

Compile a single version:
```bash
pdflatex cv_en.tex
pdflatex cv_pt.tex
pdflatex cv_de.tex
```

Compile all versions:
```bash
for f in cv_*.tex; do pdflatex "$f"; done
```

## Cleanup

Remove auxiliary files:
```bash
rm -f *.aux *.log *.out
```
