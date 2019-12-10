# Personal CV
This is my resume, forked from [McDowell CV](https://github.com/dnl-blkv/mcdowell-cv) and modified to fit my needs.

The class is based on `article` class. The paper format is set to U.S. letterpaper by default.

The main modifications made are to the header, to format it as I like. I have also modified the header to better copy-paste into plain text documents to be easier for automated parsers.

## Layout
Each subsection is written in a file inside the details folder, and then imported into the main template using the `\input{}` directive.

 
## Environments
 - `\begin{cvsection}{sectionname}` - prints a section with a header consisting of the name in bold small caps and a page-wide horizontal line below.
 - `\begin{cvsubsection}[linesnum]{left}{center}{right}{content}` - prints a subsection with header consisting of the `left`, `center` and `right` titles. The optional `linesnum` argument defines the amount of lines in the header. The argument only affects the vertical spacing between the environment header and content thus eliminating the effect of *tabu* package vertical spacing bug.

## Build Instructions
- Make sure `lualatex` (see http://www.luatex.org/download.html) is installed on your machine and is available in the terminal or a command line client of your choice.
- In the terminal or a command line client of your choice, go to the folder containing `McDowell_CV_Template.tex` and `mcdowellcv.cls`, and run the following command: `lualatex McDowell_CV_Template.tex`.
