all: M3N9\ Computational\ Linear\ Algebra\ Notes.pdf

M3N9\ Computational\ Linear\ Algebra\ Notes.pdf: M3N9\ Computational\ Linear\ Algebra\ Notes.tex resources.tex $(shell find . -maxdepth 1 -type d -not -path . -exec find {} -type f -not -name makefile \; | sed 's/ /\\ /g')
	mkdir -p aux/
	pdflatex --aux-location=aux --output-directory=aux/ --interaction=nonstopmode M3N9\ Computational\ Linear\ Algebra\ Notes.tex
	pdflatex --aux-location=aux --output-directory=aux/ --interaction=nonstopmode M3N9\ Computational\ Linear\ Algebra\ Notes.tex
	cp aux/M3N9\ Computational\ Linear\ Algebra\ Notes.pdf M3N9\ Computational\ Linear\ Algebra\ Notes.pdf
	rm -rf aux/

clean:
	rm -rf *.pdf aux/ *.log *.aux
