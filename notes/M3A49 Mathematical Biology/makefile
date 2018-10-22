all: M3A49\ Mathematical\ Biology\ Notes.pdf

M3A49\ Mathematical\ Biology\ Notes.pdf: M3A49\ Mathematical\ Biology\ Notes.tex resources.tex $(shell find . -maxdepth 1 -type d -not -path . -exec find {} -type f -not -name makefile \; | sed 's/ /\\ /g')
	mkdir -p aux/
	pdflatex --aux-location=aux/ --output-directory=aux/ --interaction=nonstopmode M3A49\ Mathematical\ Biology\ Notes.tex
	pdflatex --aux-location=aux/ --output-directory=aux/ --interaction=nonstopmode M3A49\ Mathematical\ Biology\ Notes.tex
	cp aux/M3A49\ Mathematical\ Biology\ Notes.pdf M3A49\ Mathematical\ Biology\ Notes.pdf
	rm -rf aux/

clean:
	rm -rf *.pdf aux/ *.log *.aux
