PROJEKT=proj3
LOGIN=xsokov01

$(PROJEKT).pdf: $(PROJEKT).ps
	ps2pdf -sPAPERSIZE=a4 $^

$(PROJEKT).ps: $(PROJEKT).dvi
	dvips -sPAPERSIZE=a4 $^

$(PROJEKT).dvi: $(PROJEKT).tex
	latex $^
	latex $^

zip:
	zip $(LOGIN)-fit.zip *.tex oniisan.eps oniisan2.eps etiopan.eps algotithm2e.sty Makefile

clean:
	rm -f $(PROJEKT).{aux,dvi,log,pdf,ps,out} $(LOGIN)-fit.zip
