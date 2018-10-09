all: Deterministic\ Populations.pdf

Deterministic\ Populations.pdf: Deterministic\ Populations.tex $(shell find contents/ -type f | sed 's/ /\\ /g')
	mkdir -p aux/
	pdflatex --aux-location=aux/ --output-directory=aux/ Deterministic\ Populations.tex
	cp aux/Deterministic\ Populations.pdf Deterministic\ Populations.pdf
	rm -rf aux/

clean:
	rm -rf *.pdf aux/ *.log *.aux
