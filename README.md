# LaTeX-Template for Project and Bachelor Theses at DHBW Mannheim / Business Informatics

This GitHub repository provides instructions, best practices, and a __template__ for writing a project or bachelor thesis at the Department of Business Informatics at DHBW Mannheim.

## General Notes
* __The template is just a sample!__ Please adapt it to your requirements which you agree upon with your scientific advisor. E. g. adapt citation style, page margins, etc.
* Always use the latest version of this template.
* The template is written for a thesis in German, but can be adapted easily to other languages.
* The template is written in pure LaTeX. It requires **basic knowledge of LaTeX**. Please get used to it *before* you start writing.
* If you prefer to work with other type setting systems, you should nonetheless consider the document **`master.pdf`** as guideline for the general structure of your project or bachelor thesis.

## Installation Instructions

### Prerequisites

First, you need a working LaTeX installation. Please find an appropriate one for your operating system, e. g.

* Windows, Mac, Linux: [TexLive](http://www.tug.org/texlive/) (included in most Linux distributions)
* Windows: [MikTex](http://www.miktex.org)
* Mac: [MacTex](http://www.tug.org/mactex/index.html)

Next, you need a LaTeX Editor. Any text editor (e.g. vi/vim, atom, sublime etc.) will do the job. However, there are some LaTeX editors which support writing LaTeX-domuments and which are tested with the template:

* [TexStudio](http://www.texstudio.org) (platform independent, recommended)
* [TexShop](http://pages.uoregon.edu/koch/texshop/) (Mac only)

Alternatively, you may choose the LyX graphical editor, which allows you to use all LaTeX features, but simplifies some tasks by its graphical user interface. This still needs a fully working LaTeX installation.

* [LyX](https://www.lyx.org) (platform independent)

### Template Installation

Clone/download the template or the complete GitHup repository to your local environment and unpack it to a directory of your choice. 

**Important:** Instead of BibTeX, the template uses the newer BibLaTeX/Biber combination. Please adjust your LaTeX environment accordingly when you get strange errors referring to the bibliography, since most editors default to BibTeX.

## Explanation of the LaTeX template

In the LaTeX directory, the file **`master.tex`** is the LaTeX root file which can be compiled directly. All other `.tex`-files are incuded there. 

The template files are commented in detail. Moreover, there is an instruction document **`anleitung.tex`** (in German) which explains the basic usage of the template.

Read the comments in all the `.tex`-files carefully, since you'll likely need to modify configurations and content, e.g. for disabling unused parts like the *List of Algorithms* etc. The file **`config.tex`** includes relevant packages and provides a great portion of configuration settings. Nearly every property or characteristic can be configured/modified/addee here, beginning from page layout, header and footer, citation style etc. *If needed read the LaTeX package documentations at [CTAN](http://www.ctan.org)!*

Adapt in the `.tex`-files, in particular in `master.tex` and `config.tex`, especially all parts which are marked with **`@stud`**.

Citation examples are included in the file **`bibliography.bib`** -- articles, books, online references, etc.

Acronyms will be maintained in file **`acronyms.tex`**.

The acronyms list will then be generated automatically from this file upon compilation with LaTeX. Also lists of figures, tables, coding sections, algorithms will be generated automaticvally during LaTeX compilation if these items are properly captioned in the running text of your thesis -- see LaTeX instructions for details. 

The GitHub bundle contains sample chapter and appendix files which may be adapted or extended. Additional chapter and appendix files can be provided and included in the `master.tex` file.

If you want to use a logo of your company replace the graphics file **`firmenlogo.jpg`** in folder `./img` by the logo of your company. Adjust the size of the logo by setting the scale factor of the image in **`titlepage.tex`**.

**Remark**
* The template **`master.tex`** will be used for the preparation of scientific theses
* Templates for other kinds of scientific papers, articles, monographs, etc. can be found in repositories of scientific journals or for instance here:
  * https://www.latextemplates.com/
  * https://www.overleaf.com/latex/templates
  * https://github.com/pmichaillat/latex-paper

## Explanation of the LyX template

For editing via the LyX graphical editor see the **`thesis.lyx`** template file in the LyX directory, which includes the acronyms and configs of above LaTeX template in the document and settings. 

The citations are included in the file **`bibliography.bib`** -- articles, books, online references, etc.
