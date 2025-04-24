# Building the file from scratch

Thanks to @evanberkowitz, there is now a Makefile for building the pdf.  It assumes the user has pdflatex and biber available. The user should be able to do the following from the base directory:

1. `cd build` 
2. `make`

The many temporary TeX files are listed in `build/.gitignore`, so the repo still looks clean even if those files have changed, and won't tempt the user to commit them. `make clean` removes those temporary files from your local repo.

I left the old instructions below in case anyone wants to do this from scratch. But seriously, you don't need to!


~~This is a complex file, so building will take a little patience. It is assumed that you will have a full working LaTeX package installed on your machine. 

~~Here are the rough steps involved:

~~1. make sure the build directory contains *only* the `stat205.tex` file (and optionally the `stat205.pdf` file -- not needed in the build). 
~~2. in your terminal, run `pdflatex stat205` -- there will be a lot of errors for missing references during the first run.
~~3. run `biber stat205` -- this will add the references in!
~~4. run `pdflatex stat205` again -- this should build a PDF, but it won't be correct yet. Scroll up in your terminal output a bit and make sure there's no message about needing to run LaTeX again to fix page breaks.
~~5. run `pdflatex stat205` one more time~~

