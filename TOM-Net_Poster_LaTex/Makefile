file=poster_landscape
ALL: clean ${file}.pdf 
%.pdf: %.tex Makefile
	pdflatex --enable-write18 $< &&	pdflatex $< && pdflatex $<

show: 
	  xdg-open ${file}.pdf
clean:
	  rm -f *.aux	*.bbl	*.blg	*.log	poster_*.pdf 
