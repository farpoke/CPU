default: Stadgar Styrdokument

Stadgar: Stadgar.pdf
Styrdokument: Styrdokument.pdf

Stadgar.pdf: Stadgar.tex
	xelatex --mode=nonstop Stadgar.tex
	xelatex --mode=nonstop --src-specials Stadgar.tex

Styrdokument.pdf: Styrdokument.tex Stadgar.pdf
	xelatex --mode=nonstop Styrdokument.tex

clean:
	rm -f Stadgar.aux Stadgar.comments Stadgar.log Stadgar.pdf
	rm -f Styrdokument.aux Styrdokument.log Styrdokument.out Styrdokument.pdf
