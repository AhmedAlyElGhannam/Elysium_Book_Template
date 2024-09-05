# Elysium_Book_Template
This is the LaTeX book template I have "created"---more like assembled XDD---for my graduation project documentation. This repository's purpose is to keep it in a functional state and to make it easier for myself to reuse it cuz I will probably forgot how I made it XDD.

# Main Document Components
1. `main.tex`: Main file in the document; the file that you will compile.
2. `settings.tex`: Contains settings for `elysium.sty`, page geometry, and title/subtitle.
3. `IDidItForTheMemes.tex`: Auto-generates memes in text form.
4. `FrontMatter.tex`: Contains `TitlePageListOfAuthors.tex`, `acknowledgement.tex`, `abstract.tex`, `tableofcontents.tex`, `listoffigures.tex`, `listoftables.tex`, `listoflistings.tex`, and `nomenclature.tex`.
5. `MainMatter.tex`: Contains parts and chapter files.
6. `BackMatter.tex`: Contains `References.bib`, appendices, and `Colophon.tex`.
7. The folder `606-ShadowRealm` is for banishing ChatGPT-generated text written by your colleagues!

# Front Matter

## Page Numbering
1. Title page is not numbered.
2. Rest of front matter pages are numbered using Roman numerals.

## Title Page
1. Found in `01-FrontMatter/TitlePageListOfAuthors.tex`.
2. Both `\@title` and `\@subtitle` can be changed in `settings.tex`.
3. I left an example for how to fill the name/id table + the other fields.

## Acknowledgement
1. Found in `01-FrontMatter/acknowledgement.tex`.
2. Simply write what you want in whatever format you want.

## Abstract
1. Found in `01-FrontMatter/abstract.tex`.
2. Simply write what you want in whatever format you want.

## Table of Contents
1. It will be auto-generated for you so you do not have to worry about that.

## List of Figures
1. It will be auto-generated for you so you do not have to worry about that.

## List of Tables
1. It will be auto-generated for you so you do not have to worry about that.

## List of Listings (Code Snippets)
1. It will be auto-generated for you so you do not have to worry about that.

## Nomenclature
1. Found in `01-FrontMatter/nomenclature.tex`.
2. Add abbreviations and symbols as shown in the example.

# Main Matter

## Page Numbering
1. Main matter and Bibliography pages are numbered using Arabic numerals.
1. Appendices' pages are numbered in the format `A5` where `A` is the appendix index and `5` is the page number in appendix `A`.
1. Colophon is not numbered.

## Parts
1. Parts can be edited or deleted altogether. The commands to create a part in Main Matter can be found in `FrontMatter.tex`.
2. Adding chapters is done as shown in the example. Upon adding/deleting a chapter, make sure to keep the directory hierarchy consistent to avoid errors.

## Chapter Commands Example (As I Prefer to Write Them)
1. Code snippets can be shown with syntax highlighting for the following languages: MATLAB `CodeStyleMatlab`, C `CodeStyleC`, C++ `CodeStyleCpp`, Python `CodeStylePython`, Bash `CodeStyleBash`, JSON `CodeStyleJSON`, Javascript `CodeStyleJavaScript`, PHP `CodeStylePHP`, XML `CodeStylePHP`. The command below is used to show a code snippet. Make sure to put the correct code style instead of the field `CODE_STYLE` and write the code snippet location correctly.
   ```
   \lstinputlisting[style=CODE_STYLE, caption=DESIRED_CAPTION label=cd:label, firstline=21, lastline=69]{./CodeSnippets/example.h}
   ```
   
2. Hyperlinks are added using the following command:
   ```
   \href{https://dudetrustme.org}{\color{blue2}CLICK HERE}.
   ```

3. Photos are added using this command. Make sure to write the photo/figure location correctly. Size can be freely adjusted using `scale` field.
   ```
   \begin{figure}[h!]
       \centering
       \includegraphics[scale=0.5]{./Figures/HW/powerDiagram-drawio.png}
       \caption{The Block Diagram for Power Management.}
       \label{fig:hw-power-blk1}
   \end{figure}
   ```

# Back Matter

## Bibliography
1. Add your references in `bibTeX` form to the file `References.bib`.
2. Cite your added references using `\cite{ref-nickname}`.
3. **VIMP**: Make sure to NOT use an underscore in any of the labels/commands cuz it makes LaTeX go nuts.

## Appendices
1. They can be found in `03-BackMatter`.

## Colophon
1. Can be found in `03-BackMatter/Colophon.tex`.
2. It can be either a publisher info or a meme as I wrote.
