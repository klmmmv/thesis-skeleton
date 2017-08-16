README
================================================================================

This is a project to write a scientific thesis. It specifically aims to help 
students of the FH JOANNEUM University of applied Science, to write a thesis 
which fulfills every formal aspect. 
The writing itself of the thesis, is done in pure markdown (pandoc dialect).

tl;dr:
--------------------------------------------------------------------------------

~~~bash
git clone https://github.com/klmmmv/thesis-skeleton.git
cd thesis-skeleton
./topdf
~~~

This creates an `output` folder where a html, epub and pdf version of your thesis will be created.
Write your thesis in chap1.md - chap**n**.md 

Prerequisites
--------------------------------------------------------------------------------

- install [pandoc](http://pandoc.org)
- install latex with lualatex engine
- Unfortunately, only proprietary fonts are allowed for writing a thesis at the institute of Informationmanagement. On Unix-like platforms install the Calibri font
    ~~~bash
        wget http://plasmasturm.org/code/vistafonts-installer/vistafonts-installer
        chmod +x vistafonts-installer
        ./vistafonts-installer
    ~~~
- download this repository and execute topdf

Files
--------------------------------------------------------------------------------

epub/

:   This folder contains static files for generating an e-book in the epub format.
    There is a sample cover picture and a gimp file for making your own.

html/

:   This directory is supposed to contain every static file needed for an HTML 
    export if needed

images/

:   Put all your images into this directory.

acm.csl

:   This is a citation style language file, which describes how citations are 
    formatted. The acm style is approved to be used in a master thesis. However, you can find other csls [here](http://citationstyles.org/styles).

bib.bib

:   This is your bibliography from which you can reference keys for a citation.

chap*.md

:   The `chap1.md` and following files, are you main working files. Write each 
    chapter into file. The script will order the chapters as they are named.
    Those are the only files which represent content.

frontmatter.md

:   Here you can find the english and german abstract, the "eidestattliche 
    Erklärung", the abbreviations and commandos for inputing list of table, list of figures and list of listing. Delete them if you dont want them.

header.tex

:   Pandoc uses latex for producing pdfs. Therefore it first creates tex files  
    from your markdown and then produces the pdf with latex. If you need to include latex packages to be used, add them here. For example activate the math package. Then you can write ordinary latexcode inside your markdown files.

references.md

:   This is only used for adding the references at the back of the thesis.
   

Citation
--------------------------------------------------------------------------------

If you want to use a different citation style, alter the `--csl` option in the
`topdf` script. You can download all different kinds of csls from
[here](https://github.com/citation-style-language/styles)
