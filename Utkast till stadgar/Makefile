
default: Stadgar Stadgar-Kommentarer Styrdokument

Stadgar: Stadgar.pdf
Stadgar-Kommentarer: Stadgar-Kommentarer.pdf
Styrdokument: Styrdokument.pdf

Stadgar.pdf: Stadgar.tex
	xelatex --mode=nonstop Stadgar.tex
	xelatex --mode=nonstop --src-specials Stadgar.tex

Stadgar-Kommentarer.pdf: Stadgar-Kommentarer.tex Stadgar.pdf
	xelatex --mode=nonstop --src-specials Stadgar-Kommentarer.tex

Styrdokument.pdf: Styrdokument.tex Stadgar.pdf
	xelatex --mode=nonstop Styrdokument.tex

clean:
	rm -f Stadgar.aux Stadgar.comments Stadgar.log Stadgar.pdf
	rm -f Stadgar-Kommentarer.aux Stadgar-Kommentarer.log Stadgar-Kommentarer.pdf
	rm -f Styrdokument.aux Styrdokument.log Styrdokument.out Styrdokument.pdf
