MAIN = main
TEX_SOURCES = $(wildcard ./sections/*.tex)
SOURCES = $(TEX_SOURCES) assets/preamble.tex

$(MAIN).pdf: $(MAIN).tex $(SOURCES)
	latexmk $(MAIN).tex

clean:
	@for extension in aux toc fls bbl blg nav snm vrb log out fdb_latexmk; do \
		find -type f -name "*.$$extension" -exec rm {} \; ; done

