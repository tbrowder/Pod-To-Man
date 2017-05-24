LSRC := corrupt.1
LSRC += corrupt.1perl6


all:
	for i in $(LSRC); do          \
		man -tl $$i > $$i.ps; \
		ps2pdf $$i.ps;        \
		rm $$i.ps;            \
	done

clean:
	rm *~
	for i in $(LSRC); do          \
		rm $$i.pdf;            \
	done
