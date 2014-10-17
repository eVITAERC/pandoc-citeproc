ALL=man1/scholdoc-citeproc.1
DATE=$(shell date "+%Y-%m-%d")
VERSION=$(shell ../dist/build/scholdoc-citeproc/scholdoc-citeproc --version | head -1 | awk '{print $$2;}')

.PHONY: all

all: $(ALL)
man1/%.1: %.1.md ../dist/build/scholdoc-citeproc/scholdoc-citeproc
	scholdoc $< -o $@ -s -f markdown -t man -Vfooter="${VERSION}" -Vdate="${DATE}"
