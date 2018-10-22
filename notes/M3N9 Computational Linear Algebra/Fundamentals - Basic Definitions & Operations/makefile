all: Fundamentals\ -\ Basic\ Definitions\ &\ Operations.pdf

Fundamentals\ -\ Basic\ Definitions\ &\ Operations.pdf: Fundamentals\ -\ Basic\ Definitions\ &\ Operations.tex ../resources.tex $(shell find contents/ -type f | sed 's/ /\\ /g')
	mkdir -p aux/
	pdflatex --aux-location=aux/ --output-directory=aux/ --interaction=nonstopmode Fundamentals\ -\ Basic\ Definitions\ &\ Operations.tex
	pdflatex --aux-location=aux/ --output-directory=aux/ --ubteraction=nonstopmode Fundamentals\ -\ Basic\ Definitions\ &\ Operations.tex
	cp aux/Fundamentals\ -\ Basic\ Definitions\ &\ Operations.pdf Fundamentals\ -\ Basic\ Definitions\ &\ Operations.pdf
	rm -rf aux/

clean:
	rm -rf *.pdf aux/ *.log *.aux
