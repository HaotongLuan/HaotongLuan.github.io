# Bilingual CV

The English and Chinese CVs share `cv-template.sty`. The layout follows the supplied Haokai Ding CV: A4, two pages, red/gray accents, sans-serif typography, right-aligned dates and numbered publications. Personal content comes from Haotong Luan's existing CVs. AIR internship experience has been removed; the separate AIR summer-school admission remains.

## Build

Run from this directory with XeLaTeX (not pdfLaTeX):

```powershell
xelatex -interaction=nonstopmode -halt-on-error lht-CV-Eng.tex
xelatex -interaction=nonstopmode -halt-on-error lht-CV-Eng.tex
xelatex -interaction=nonstopmode -halt-on-error lht-CV-CN.tex
xelatex -interaction=nonstopmode -halt-on-error lht-CV-CN.tex
```

The Chinese CV uses Windows fonts Microsoft YaHei Light and Microsoft YaHei Bold. These system fonts are not included in the source package. Update `\setCJKmainfont` to an installed Chinese font if building on another platform.

## Files

- `lht-CV-Eng.tex` / `.pdf`: English source and PDF.
- `lht-CV-CN.tex` / `.pdf`: Chinese source and PDF.
- `cv-template.sty`: shared layout and typography.
- `cv-fonts/`: Source Sans Pro, Roboto, and Font Awesome fonts with their licenses.

Source Sans Pro comes from Adobe's `adobe-fonts/source-sans` repository, release `2.045R-ro/1.095R-it` (SIL Open Font License). Roboto comes from `googlefonts/roboto-2` (Apache License 2.0). Font files are unmodified.

The phone, email, and homepage icons use Font Awesome 6 Free Solid from `FortAwesome/Font-Awesome`, branch `6.x`. The font is licensed under the SIL Open Font License; the complete Font Awesome license is included in `cv-fonts/FontAwesome-LICENSE.txt`.
