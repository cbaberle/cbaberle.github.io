TAR = $(wildcard *.html)

.PHONY: all clean

all: $(TAR)

%.html : sources/%.md
	pandoc $< -s --mathjax -o $@ -c ../styles/default.css -B ../elements/header.html -A ../elements/footer.html

clean:
	rm -f $(TAR)