% author Michael Valentin Klammer
% date today

README
================================================================================

This is a project to write a scientific thesis. It specifically aims to help 
students of the FH JOANNEUM University of applied Science, to write a thesis 
which fulfills every formal aspect. 
The writing itself of the thesis, is done in pure markdown (pandoc dialect).

Prerequisites
--------------------------------------------------------------------------------

- install [pandoc](http://pandoc.org)
- install latex with lualatex engine
- on Unix-like platforms install the Calibri font: 
    ~~~bash
        wget http://plasmasturm.org/code/vistafonts-installer/vistafonts-installer
        chmod +x vistafonts-installer
        ./vistafonts-installer
    ~~~
- download this repository and execute topdf

Files
--------------------------------------------------------------------------------

This lists all the files to understand how the project works and what you have 
change to write your thesis.

Citation
--------------------------------------------------------------------------------

If you want to use a different citation style, alter the `--csl` option in the
`topdf` script. You can download all different kinds of csls from
[here](https://github.com/citation-style-language/styles)
