![Version](https://img.shields.io/static/v1?label=manuscriptInLaTeX&message=0.2&color=brightcolor)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# Generic template in LaTeX for the first submission of an academic manuscript

## Tower of First-Submission Babel

A point of perpetual confusion for me is that the availability of style files for LaTeX for various Academic journals implies that you should prepare your first submission using the official template.
This is not true, and this is much more trouble than it is worth, especially if your manuscript is rejected, as most are.
Journal  configurations vary widely between journals: It can be much more challenging to reformat a manuscript than it may appear at first sight.

Instead, you only need to submit your first submission as a PDF.
You could use a format for that first submission that is easy for reviewers to read and edit when printed out.
It should also be simple for you to assemble.

(I know; you could format it for BioArxiv in LaTeX. 
This step is part of the workflow of many. 
It is not part of mine yet.)

## Solution: a generic template for the first submission

This GitHub repository is for a generic journal article template (main.tex) that I use to prepare my first manuscript submission as a LaTeX document.
I used one extra file for styling the bibliography, spbasic.bst.
The template includes examples of the following elements:

- figure
- tables
- equations
- code block
- bibtex file

Delete the boilerplate that you do not need and fill out the sections with your amazing results and submit.

### Note for org-mode users

Wouter Spekkink has written a detailed [blog post](http://www.wouterspekkink.org/academia/writing/tool/doom-emacs/2021/02/27/writing-academic-papers-with-org-mode.html) about writing an academic article in org-mode and then exporting it to LaTeX.
Org-mode users like to be able to fold sections.
You can do that to LaTeX sections in Overleaf.
He claims that LaTeX's markup is distracting.
He is right about that regarding tables, but I think the LaTeX markup is minimal for the vast majority of the document.
He is also right about seamlessly exporting from org through LaTeX to PDF because it requires one command.
However, in AUCTeX, this can be painless, too.
Nonetheless, I will develop an org variant for org-mode users.


## Features

The features of the template are as follows:

- A 7 x 9 inch geometry for the active text area.
- Double-spacing.
- Line numbers in the main document body.
- Automated page numbering.
- Generic Title page formatting with affiliations for multiple authors.
- Use a global.bib file rather than bibitems to assemble the bibliography.
- Use the booktabs library for pretty tables even if I have to downgrade them on the final submission with the journal's style file.
- A list of tables is autogenerated.
- Use the graphicx package to import images.
- Support for including figures in an old-fashioned Figure section rather than embedding them in the text. Hyperlinked labels allow you to navigate instantly to a figure. A list of figures is autogenerated.
- Support for including tables in a Tables section.
- Reminders (i.e., remember to spell out the hypothesis in the Introduction) of what should go where in a deleteable or foldable comment.
- Support for equation typesetting in a custom environment that supports captions.
- Support for syntax highlighting of code blocks and using captions for each code block.

After your manuscript is accepted, you can reformat it to comply with the Journal's style.
LaTeX template and style files can be found on the Journal's website.
The Overleaf.com site has a gallery of journal article templates that run on Overleaf.

## Complementary writing tools available at github.com/MooersLab

### Writing Log

See this [site](https://github.com/MooersLab/writingLogTemplate) for a template for a place to organize your thoughts and track your progress on your writing project.
I store the writing log in the same folder as all the files for my writing project.

### Annotated Bibliography

See this [site](https://github.com/MooersLab/annotatedBibliography) for a template to create an annotated bibliography in LateX. 
This is an excellent place to store your notes from reading the literature.
I store the annotated bibliography in a subfolder in the same folder as all the files for my writing project.

### Slideshow Template

See this [site](https://github.com/MooersLab/slideshowTemplateLaTeX) for a template to create a slideshow to advertise your manuscript.


### Diary for 2022 in LaTeX

[See](https://github.com/MooersLab/diary2022inLaTeX). Can serve many related purposes.

### Diary for 2023 in LaTeX

[See](https://github.com/MooersLab/diary2023inLaTeX). Can serve many related purposes.

### latex-emacs

See this [site](https://github.com/MooersLab/latex-emacs) for a latex-emacs configuration file.
This configuration allows you to run Emacs with LaTeX in isolation from your main configuration.

### snippet-latex-mode

See this [site](https://github.com/MooersLab/snippet-latex-mode) for a collection of yasnippet snippets for latex-mode in Emacs.
These extend the default set.

### emacs-quizzes

Improve your recall of Emacs commands in a few minutes a day thanks to spaced repetition. 
The [site](https://github.com/MooersLab/qemacs) has a set of fill-in-the-blank quizzes.

### LaTeX in Emacs

Learn how to use [LaTeX in Emacs](https://github.com/MooersLab/BerlinEmacsAugust2022) by watching the slides I presented at the Berlin Emacs Meetup on 31 August 2022.
This talk was not recorded.

### GhostText

Edit text areas in a web browser from your [favorite text editor](https://github.com/MooersLab/DSW22ghosttext).
The text area can be the opened tex file on Overleaf.
This talk was recorded: See the corresponding [video](https://mediasite.ouhsc.edu/Mediasite/Channel/python/watch/4da0872f028c4255ae12935655e911321d).

### The Writer's Law

Some [guidelines](https://github.com/MooersLab/thewriterslaw) to productive writing.

## Version History

|Version      | Changes                                               | Date            |
|:-----------:|:-----------------------------------------------------:|:---------------:|
| Version 0.2 | Added update table to README.md                       | 2024 April 7    |


## Sources of Funding

- NIH: R01 CA242845
- NIH: R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel)
- NIH P20GM103640 and P30GM145423 (PI: A. West)

