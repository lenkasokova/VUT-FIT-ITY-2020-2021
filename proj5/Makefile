PROJEKT=proj5
LOGIN=xsokov01

pdflatex: $(PROJEKT).tex
	pdflatex $^
	pdflatex $^

zip:
	zip $(LOGIN)-fit.zip *.tex binary_tree.png binary_tree_terminology.png BST.png algorithm2e.sty Makefile

clean:
	rm -f $(PROJEKT).{aux,dvi,log,pdf,ps,out} $(LOGIN)-fit.zip
