# Elysium_Book_Template
LaTeX book template combining elements of Ricardo Langner's Clean Thesis, Daan Zwaneveld's tudelft-report-thesis-template, and adding my own wicked mix to fit my needs.

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

## Chapter Commands Example
1. Code snippets can be shown with syntax highlighting for the following languages: MATLAB `CodeStyleMatlab`, C `CodeStyleC`, C++ `CodeStyleCpp`, Python `CodeStylePython`, Bash `CodeStyleBash`, JSON `CodeStyleJSON`, Javascript `CodeStyleJavaScript`, PHP `CodeStylePHP`, XML `CodeStylePHP`. The command below is used to show a code snippet. Make sure to put the correct code style instead of the field `CODE_STYLE` and write the code snippet location correctly.
   ```
   \lstinputlisting[style=CODE_STYLE, caption=DESIRED_CAPTION label=cd:label, firstline=21, lastline=69]{./CodeSnippets/example.h}
   ```
