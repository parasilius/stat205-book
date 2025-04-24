TEX=pdflatex
BIB=biber

stat205.pdf: ../tex/*.tex
	$(TEX) stat205
	$(BIB) stat205
	$(TEX) stat205
	$(TEX) stat205

clean:
	$(RM) stat205.{aux,bbl,bcf,blg,log,out,run.xml,toc}
