![Version](https://img.shields.io/static/v1?label=manuscriptInOrg&message=0.7.1&color=brightcolor)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# Manuscript template in org-mode for the first submission 

## Background
The first submission of a research paper for peer review can be in a generic format as a PDF.
The advantage of a plain generic template is that it can be submitted to many different journals.

This is an org-mode variant of the main.tex file in the MooersLab/manuscriptInLaTeX [repo](https://github.com/MooersLab/manuscriptInLaTeX).
This template is for people who prefer to write research papers in org-mode because they do a lot of their other work in org-mode and do not want to switch to working in LaTeX.
They would rather spend all day in org-mode; it is that fun to use.
Org supports easy shuffling and other manipulations of document subtrees, very easy table generation, and literate programming.
You can also integrate manuscript writing with time management via org-agenda and knowledge management via org-roam more efficiently by staying in org-mode. 
These features are beyond what is readily possible in LaTeX without using extra packages.

If you are already a strong LaTeX user, there is plenty of tweaking of the preamble of this template that you can do to add your favorite packages and settings.
Org-mode recognizes many LaTeX commands directly.
LaTeX code can also be utilized inside of code blocks that can be evaluated on the fly.
See the [org-mode manual](https://orgmode.org/manual/).

```elisp
#+name: hello-world
#+BEGIN_SRC latex
\LaTeX code
#+END_SRC
```



## Sample title page

![Screenshot 2024-08-18 at 6 40 00 AM](https://github.com/user-attachments/assets/fbc7cbb8-4711-427b-864d-569178196adb)

## Sample second page

![Screenshot 2024-08-22 at 4 00 55 PM](https://github.com/user-attachments/assets/843aa28e-97ee-4a96-b151-1069e725d1c3)


## Default Features

- Line numbers.
- Block paragraphs. Reset the indent on the line `\setlength{\parindent}{0pt} `  if you indents.
- No numbering of the sections. This is suppressed in a org-mode setting in the header (i.e., num:\nil). Remove this setting to apply section numbering.
- Blank lines between paragraphs. This is set by the line `\usepackage{parskip}` in the preamble.
- Narrow margins to conserve paper in drafts. Edit the line `\usepackage[letterpaper, total={6.75in, 9in}]{geometry}` to change the margin width.
- Single-spaced abstract.
- Double-spaced main text.
- Wrapping of sentences written one per line for sane version control.
- Helvetica font.
- Page numbers in the upper right-hand corner.
- No page number on the first page.
- The LaTeX header is in a drawer so you do not have to look at it when working in Emacs.
- Comments are now in GUIDANCE drawers that can be closed with `Shift-TAB` in org-mode to reduce clutter. The contents of these drawers are not printed on export to PDF. 
- Running tiles to ease tracking printed copies.

## Installation

1. Git clone the repo `git clone https://github.com/MooersLab/manuscriptInOrg.git`.
2. Copy main.org to your project folder.
3. Load main.org file in Emacs via the File pulldown menu or `C-x C-f`.
4. Edit the file to customize to your manuscript.
5. Edit the paths to your global.bib file and your image files.
6. Enter `C-c C-e l o` to compile and open the resulting PDF in your default PDF viewer.

Compiling takes several seconds on a 2018 MacBook Pro with 32 GB of RAM. 
Org-mode is built into recent versions of Emacs. 
The main.org file will be compiled into the final PDF without any configuration.
Try `emacs -Q main.org` and then enter `C-c C-e l o`. 
The PDF will open in your default PDF viewer.


## Assumptions

1. LaTeX is installed with all of the required style files. However, my installation was missing the **break cities.sty** file. I installed this with the `sudo port install texlive-bibtex-extra` command.
2. You will use the LaTeX cite command and let LaTeX handle the generation of the literature cited section. This package *citar*, *helm-bibtex*, *ivy-bibtex*, or the like can help find the right citekey from inside Emacs.
3. You can edit org-mode files in other text editors. Many text editors support syntax highlighting for org-mode. VS Code has a package that provides additional support. To get the most out of utilizing org-mode, it is best to utilize it inside of Emacs. Org-mode is now built into GNU Emacs. You can utilize org-mode without any configuration of the `init.el` file. You can achieve the same effect by starting your current Emacs with the `-Q` flag, which skips reading your `init.el` file. The editing and building of a `init.el` file to extend the features of Emacs can be an activity trap. Frustration associated with errors late during the editing of this file led to Emacs having a reputation for being difficult to master.

## Postscript Oct 10, 2022
My approach was developed independently of another [solution](https://github.com/fangohr/template-latex-paper-from-orgmode/issues/4) found here. 

## Postscript May 16, 2023
I had upgraded my operating system to Ventura, but I had not properly migrated my MacPorts. I found that I was missing the breakcities.sty file.

## Postscript October 11, 2024

I often print manuscirpts before traveling to edit them while airborne.
The papers tend to get mixed up between projects.
I added a header that clarifyting which project a page belongs to.

## Related sites

- [Writing log template in Org-mode](https://github.com/MooersLab/writingLogTemplateInOrg)
- [Writing log template in LaTeX](https://github.com/MooersLab/writingLogTemplate)
- [LaTeX manuscript template](https://github.com/MooersLab/manuscriptInLaTeX/edit/main/README.md)
- [Org-mode manuscript template](https://github.com/MooersLab/manuscriptInOrg/edit/main/README.md)
- [Workbook for 2022 for tracking time spent and words written by project](https://github.com/MooersLab/writingProgress2022)
- [Slideshow template in LaTeX](https://github.com/MooersLab/slideshowTemplateLaTeX)
- [Annotated bibliography Template in LaTeX](https://github.com/MooersLab/annotatedBibliography)
- [Diary for 2022 in LaTeX](https://github.com/MooersLab/diary2022inLaTeX)
- [Diary for 2023 in LaTeX](https://github.com/MooersLab/diary2023inLaTeX)
- [latex-emacs profile](https://github.com/MooersLab/latex-emacs)
- [default Emacs profile](https://github.com/MooersLab/configorg)
- [snippets for latex-mode in Emacs](https://github.com/MooersLab/snippet-latex-mode)
- [Quizzes about Emacs to improve recall of keybindings](https://github.com/MooersLab/qemacs)
- [Slides from talk about GhostText, Data Science Workshop, July 2022](https://github.com/MooersLab/DSW22ghosttext)
- [Video link to talk about GhostText, Data Science Workshop, July 2022](https://mediasite.ouhsc.edu/Mediasite/Channel/python/watch/4da0872f028c4255ae12935655e911321d)
- [The writer's law](https://github.com/MooersLab/thewriterslaw)

Note that [latex-emacs profile](https://github.com/MooersLab/latex-emacs) has functions for converting LaTex lists into org-markdown lists.


## Update history

|Version      | Changes                                                                                                                                                   | Date                        |
|:-----------|:------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------|
| Version 0.2 |   Added badges, funding, and update table.                                                                                            | 2024 May 21          |
| Version 0.3 |   Updated main.org so it can compile without configuration from an init.el file.                                       | 2024 August 18      |
| Version 0.4 |   Fixed issues with preamble. Put comments in drawers.                                                                       | 2024 August 22       |
| Version 0.5 |   Put preamble in a drawer.                                                                                                                     | 2024 August 26       |
| Version 0.6 |   Put GUIDANCE drawers under subheadings with noexport tag.                                                         | 2024 August 26        |
| Version 0.7 |  Add urlx package to allow linebreaks in urls.                                                                                        | 2024 August 27        |
| Version 0.7.1 | Added short author list, running title, and page of N pages format to header                                    | 2024 October 11       |
## Sources of funding

- NIH: R01 CA242845
- NIH: R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel)
- NIH: P20 GM103640 and P30 GM145423 (PI: A. West)

