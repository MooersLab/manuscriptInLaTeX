# Template for the first submission of a manuscript

A point of perpetual confusion for me is that the availability of style files for LaTeX for various Academic journals implies that you should prepare you first submission using the official template.
This is not true, and this is much more trouble than it is worth, especially if your manuscript in rejected, as most are.
These configurations vary widely between journals: It can be much harder to reformat a manuscript than it may appear at first sight.

Instead, you only need to submit you first submission as a PDF.
You might as well use a format for that first submission that is easy for reviewers to read and edit when printed out.
It should also be simple for you to assemble.

(I know; you could format it for BioArvix in LaTeX. 
This step seems to be the part of the workflow of many. 
It is not part of mine yet.
It seems like too much extra work.)

This repo is for a generic template that I use to prepare my first submission of a manuscrpt.
The features of the template are as follows:

- A 7 x 9 inch geometry for the active text area
- Double-spacing
- Line numbers in the main document body
- Automated page numbering
- Generic Title page formatting
- Use of a global.bib file rather than bibitems to assemble the bibliography
- Use of the booktabs library for pretty table even if I have to downgrade them on the final submission with the journals style file.
- Use of the minted package for syntax highlighting of code blocks.
- Use of the graphicsx package to import images.
- Support for including figures in an old fashion Figure section rather than embedding the figures in the text. You can navigate instatnaly to a figure via hyperlinked labels.
- Support for including tables in a Tables section.
- Reminders (i.e., do not forget to spell out the hypothesis in the Introduction) of what should go where in a deletable or foldable comment.
- Support for equation typesetting.

After papers is accepted, you can reformat it to comply with the Journal's style file.

