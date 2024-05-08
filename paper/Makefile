BASENAME=congestion-control

#all: $(BASENAME).html $(BASENAME).pdf
all: $(BASENAME).pdf

$(BASENAME).html: $(BASENAME).adoc $(BASENAME).bib
	asciidoctor -v -r asciidoctor-bibtex $<

$(BASENAME).pdf: $(BASENAME).adoc $(BASENAME).bib
	asciidoctor-pdf -v -r asciidoctor-bibtex $<

clean:
	/bin/rm $(BASENAME).html $(BASENAME).pdf
