all: Deterministic\ Population\ Dynamics.pdf

Deterministic\ Population\ Dynamics.pdf: Deterministic\ Population\ Dynamics.tex ../resources.tex $(shell find contents/ -type f | sed 's/ /\\ /g')
	mkdir -p aux/
	pdflatex --aux-location=aux/ --output-directory=aux/ --interaction=nonstopmode Deterministic\ Population\ Dynamics.tex
	pdflatex --aux-location=aux/ --output-directory=aux/ --ubteraction=nonstopmode Deterministic\ Population\ Dynamics.tex
	cp aux/Deterministic\ Population\ Dynamics.pdf Deterministic\ Population\ Dynamics.pdf
	rm -rf aux/

clean:
	rm -rf *.pdf aux/ *.log *.aux
