.SUFFIXES: .tex .pdf 
.PHONY: clean

MAIN = main

$(MAIN).pdf: 
	latexmk $(MAIN).tex

clean:
	@for extension in aux toc fls bbl blg nav snm vrb log out fdb_latexmk; do \
		find -type f -name "*.$$extension" -exec rm {} \; ; done

