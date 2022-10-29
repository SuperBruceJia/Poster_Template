file=poster_landscape

landscape: ${file}.tex
	rm -f ${file}.pdf
	pdflatex ${file}.tex
	#pdflatex --enable-write18 $< &&	pdflatex $< && pdflatex $<
show: 
	xdg-open ${file}.pdf
mshow:
	open -a skim ${file}.pdf
macshow: 
	open ${file}.pdf
clean:
	rm -f *.aux	*.bbl *.blg	*.log poster_*.pdf
