all: Introduction.pdf

Introduction.pdf: Introduction.tex $(shell find contents/ -type f | sed 's/ /\\ /g')
	mkdir -p aux/
	pdflatex --aux-location=aux/ --output-directory=aux/ Introduction.tex
	cp aux/Introduction.pdf Introduction.pdf
	rm -rf aux/

clean:
	rm -rf *.pdf aux/ *.log *.aux
