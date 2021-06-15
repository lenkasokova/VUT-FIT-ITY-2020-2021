SHELL = /usr/bin/env bash
NAME = proj4
LOGIN = xsokov01

all: bibtex or biblatex

biblatex:
	pdflatex $(NAME).tex
	biber $(NAME).bcf
	pdflatex $(NAME).tex



bibtex:
	pdflatex $(NAME).tex
	bibtex $(NAME).aux
	pdflatex $(NAME).tex
	pdflatex $(NAME).tex


zip:
	zip $(LOGIN)-fit.zip *.tex  Makefile czechiso.bst proj4.bib

.PHONY: clean
clean:
	rm -f $(NAME).{aux,dvi,log,ps,out,bbl,blg,fls,fdb_latexmk} $(LOGIN)-fit.zip
