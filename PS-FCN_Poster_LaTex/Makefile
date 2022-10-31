l_file=poster_landscape
p_file=poster_portrait

landscape: ${l_file}.tex
	rm -f ${l_file}.pdf
	pdflatex --enable-write18 $< &&	pdflatex $< && pdflatex $<
portrait: ${p_file}.tex
	rm -f ${p_file}.pdf
	pdflatex --enable-write18 $< &&	pdflatex $< && pdflatex $<
mshow_l:
	open -a skim ${l_file}.pdf
mshow_p:
	open -a skim ${p_file}.pdf
show_l: 
	xdg-open ${l_file}.pdf
show_p: 
	xdg-open ${p_file}.pdf
macshow_l: 
	open ${l_file}.pdf
macshow_p: 
	open ${p_file}.pdf
clean:
	rm -f *.aux	*.bbl	*.blg	*.log poster_*.pdf
