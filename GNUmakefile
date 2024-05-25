.PHONY: all clean CLEAN rebuild
TARGETS:=Seminarnotizen-Betriebsrat-1.pdf Rangordnung-der-Normen.pdf

all: $(TARGETS)

%.pdf: %.tex
	latexmk -lualatex $<

Seminarnotizen-Betriebsrat-1.tex: Rangordnung-der-Normen.pdf

CLEAN: clean
	rm -f $(TARGETS)

clean:
	rm -f *.aux *.log *.out *.synctex.gz *.fdb_latexmk *.fls *.synctex*

rebuild: CLEAN all
