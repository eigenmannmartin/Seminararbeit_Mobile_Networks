#TEMPLATE = template.tex
#TEMPLATE = ut-thesis.tex
CSL = elsevier-with-titles

.PHONY: all clean html pdf epub embed

pre:
	mkdir -p build

post:
	@echo POST

clean:
	rm -rf build

pdf: pre
	cat ./capters/*.md | pandoc -s -f markdown+yaml_metadata_block+hard_line_breaks+footnotes --filter pandoc-fignos -S -o ./build/out.pdf --chapters --bibliography=./Citer.bib --template=./template.tex --biblatex
	evince ./build/out.pdf

default: pdf
