# Jiangsu Ocean University Beamer Presentation Template

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub release](https://img.shields.io/github/release/TsekaLuk/JOU-Presentation-Beamer-Template.svg)](https://github.com/TsekaLuk/JOU-Presentation-Beamer-Template/releases/)
[![GitHub stars](https://img.shields.io/github/stars/TsekaLuk/JOU-Presentation-Beamer-Template.svg)](https://github.com/TsekaLuk/JOU-Presentation-Beamer-Template/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/TsekaLuk/JOU-Presentation-Beamer-Template.svg)](https://github.com/TsekaLuk/JOU-Presentation-Beamer-Template/network/members)
[![GitHub issues](https://img.shields.io/github/issues/TsekaLuk/JOU-Presentation-Beamer-Template.svg)](https://github.com/TsekaLuk/JOU-Presentation-Beamer-Template/issues/)
[![Overleaf Template](https://img.shields.io/badge/Overleaf-Template-brightgreen.svg)](https://www.overleaf.com/)
[![Last Commit](https://img.shields.io/github/last-commit/TsekaLuk/JOU-Presentation-Beamer-Template.svg)](https://github.com/TsekaLuk/JOU-Presentation-Beamer-Template/commits)

[简体中文](README_zh.md) | English

This template is a Beamer presentation template specifically designed for academic scenarios at Jiangsu Ocean University, providing a clean and professional layout.

## Preview Example

Here is a preview of the title page created using this template:

![JOU Beamer Template Preview](docs/slide_00.png)

## Features

* Based on the Beamer document class, with a clear structure for easy content management.
* Full Chinese language support through the `ctex` package, with XeLaTeX compilation recommended.
* Includes examples of commonly used mathematical formulas, charts, and code highlighting environments.
* Provides custom commands and color definitions for quick style modifications.
* Reserved fields for author, title, institution, advisor, and other information for easy customization.
* Integrated display of the Jiangsu Ocean University (JOU) logo.

## Usage Instructions

1. **Download the Template:** Obtain the template files (`.tex` files, `JOU.sty` file, `pic` folder, etc.).
2. **Install a LaTeX Distribution:** Ensure you have a complete LaTeX distribution installed on your computer, such as TeX Live or MiKTeX.
3. **Install the CTeX Package:** If you need good Chinese language support, ensure your LaTeX distribution includes the CTeX package.
4. **Open the Main File:** Use your preferred LaTeX editor to open `slide.tex` or a similar main `.tex` file.
5. **Fill in Information:** Modify the author, title, subtitle, institution, advisor name, and other information at the beginning of the document:
    ```latex
    \newcommand{\myinstitution}{Enter your institution name here}
    \newcommand{\advisorname}{Enter your advisor's name here}
    \author[Your short name]{Your full name \\ Advisor: \advisorname}
    \title{Enter your presentation title here}
    \subtitle{Enter subtitle here (optional)}
    \institute{\myinstitution}
    \date{Enter date here or \today}
    ```
6. **Add Content:** Add your presentation content between the `\begin{document}` and `\end{document}` environments. Use `\section{...}` to create new sections, and `\begin{frame}{...}\end{frame}` to create new slides.
7. **Insert Images:** Place image files (PDF or PNG formats recommended) in the `pic` folder, and insert them using the `\includegraphics` command:
    ```latex
    \begin{frame}{Example Image}
        \begin{figure}
            \centering
            \includegraphics[width=0.5\linewidth]{pic/your_image.png}
            \caption{Your image caption}
        \end{figure}
    \end{frame}
    ```
    Please update `pic/your_image.png` to your actual image path and filename.
8. **Manage References:** The template typically uses BibTeX or BibLaTeX to manage references. If using BibTeX, add your reference entries to the `ref.bib` file and use the `\cite{...}` command where you need to cite. Use `\bibliography{ref}` and `\bibliographystyle{...}` in the references section.
9. **Compile:** It is recommended to use the **XeLaTeX** compiler for compilation to achieve the best Chinese display effect. Multiple compilation passes (XeLaTeX -> BibTeX (if used) -> XeLaTeX -> XeLaTeX) are usually required to correctly generate the table of contents, cross-references, and references.

## Using with Overleaf

[Overleaf](https://www.overleaf.com/) is an online LaTeX editing platform that requires no local installation.

1. **Upload Template Files**: Create a new project and upload all template files (or upload as a ZIP package).
2. **Set Compiler**: Set the compiler to **XeLaTeX** in the menu for Chinese language support.
3. **File Structure**: Ensure `JOU.sty`, the main `.tex` file, the `pic` folder, and `ref.bib` (if any) are in the correct locations.
4. **Collaboration**: Invite others to collaborate through the "Share" feature.
5. **Compile and Download**: Click "Recompile" to generate the PDF, and download the PDF or source files when editing is complete.

If you encounter issues with Chinese characters, ensure the `ctex` package is loaded (`\usepackage{ctex}`).

## Template Structure

* `slide.tex` (or main `.tex` file): The main file for your presentation, containing content and layout settings.
* `JOU.sty`: Custom Beamer style file defining the template's appearance and some specific functions.
* `pic/`: Folder for storing images used in your presentation.
* `ref.bib`: (If using BibTeX) BibTeX file for storing reference entries.
* `example.tex`: Provides a real reference example for relevant academic competition presentations.

## Customization

You can modify the `JOU.sty` file to further customize the template's appearance, but this requires some knowledge of LaTeX Beamer. Simple customizations (such as modifying colors and font sizes) can be implemented in the `.tex` file using commands provided by Beamer.

If you need to replace the university logo, please update the image path in the `\includegraphics` command in `slide.tex`.

## Original Source and References

This template references Beamer template resources from the internet, especially related templates on Overleaf.
Original reference link: `https://www.latexstudio.net/archives/4051.html`

## Contributions

If you find bugs or have suggestions for improvements, please visit the GitHub project page to submit an Issue or Pull Request:
`https://github.com/TsekaLuk/JOU-Presentation-Beamer-Template`

## License

This project is licensed under the MIT License. Please see the license file for details.

---

**Note:** This template is designed to facilitate academic exchange and reporting for Jiangsu Ocean University students and faculty. Please comply with the relevant regulations of the university when using it. 