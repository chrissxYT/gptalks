all:
	@pandoc slides.md -f markdown -t beamer -o slides.pdf

clean:
	@rm -f slides.pdf

test:all
	@mupdf slides.pdf

present:test
