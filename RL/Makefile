default: main.pdf

%.pdf : %.tex bib sec
	pdflatex $<
	pdflatex $<
	bibtex $*
	pdflatex $<
	pdflatex $<
	pdflatex $<
	$(MAKE) clean

clean:
	$(RM) *.aux *.bbl *.blg *.log *.dvi *.toc *~ *.gz

purge:
	$(RM) *.aux *.bbl *.blg *.log *.dvi *.toc *~ *.pdf */*~ *~ pst/*.pdf *.gz
