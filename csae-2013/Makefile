bare_conf.pdf:
	pdflatex bare_conf.tex
	pdflatex bare_conf.tex

figures: example1.png example2.png christmas-dataflow.png

example1.png: example1.dot
	dot -Tpng -o $@ $^

example2.png: example2.dot
	dot -Tpng -o $@ $^

christmas-dataflow.png: christmas-dataflow.dot
	dot -Tpng -o $@ $^