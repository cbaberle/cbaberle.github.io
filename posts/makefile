TAR = $(wildcard *.html)

.PHONY: all clean

all: $(TAR)

%.html : sources/%.md ../styles/default.css ../elements/postheader.html ../elements/footer.html
	pandoc $< -s --mathjax -o $@ -c ../styles/default.css -B ../elements/postheader.html -A ../elements/footer.html

clean:
	rm -f $(TAR)