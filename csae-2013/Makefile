bare_conf.pdf: bare_conf.bbl
	pdflatex bare_conf.tex
	pdflatex bare_conf.tex

bare_conf.bbl: bare_conf.aux
	bibtex bare_conf.aux

bare_conf.aux: bare_conf.tex figures
	pdflatex bare_conf.tex

figures: example1.png example2.png christmas-dataflow.png

example1.png: example1.dot
	dot -Tpng -o $@ $^

example2.png: example2.dot
	dot -Tpng -o $@ $^

christmas-dataflow.png: christmas-dataflow.dot
	dot -Tpng -o $@ $^

clean:
	rm -f *.pdf *.dvi *.aux *.bbl *.blg *.log *.png