# Makefile for asciidoc based presentation

SLIDES=slides.html

default: $(SLIDES)

%.html: %.adoc
	asciidoctor -T asciidoctor-reveal.js/templates/slim -b revealjs $<

open: $(SLIDES)
	"$(shell which xdg-open || which open || which x-www-browser)" $<

clean:
	rm -f *.html

serve: $(SLIDES)
	"$(shell which xdg-open || which open || which x-www-browser)" \
		http://localhost:8000/$<
	python -m SimpleHTTPServer 8000
