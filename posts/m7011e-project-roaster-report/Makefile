SRC=$(wildcard *.tex *.bib)
OUTDIR=_build
OPTS=--pdf --into=$(OUTDIR)


.PHONY: clean

all: $(patsubst %.tex,%.pdf,$(SRC))

%.pdf: %.tex
	@mkdir -p $(OUTDIR)
	@rubber $(OPTS) $<

clean:
	@rubber --clean $(OPTS) $(SRC)
