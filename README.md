# Estatuts de la Unió Musical del Bages

Aquest repositori conté un versionat dels estatuts de la
[Unió Musical del Bages](https://www.umbages.cat). S'utilitza *git*
per mantenir una mica d'historial dels canvis efectuats.

Utilitza LaTeX per a compilar-lo.

## Instal·lar dependències

Instruccions provades a un Ubuntu 24.04.

```sh
sudo apt update
sudo apt install texlive-latex-extra texlive-fonts-extra texlive-lang-spanish
```

Aquestes dependències instal·len `pdflatex`, els paquets LaTeX utilitzats pel
document, la font Source Sans Pro i el suport de llengua per al català.

## Generar PDF

```sh
pdflatex -interaction=nonstopmode -halt-on-error estatuts.tex
pdflatex -interaction=nonstopmode -halt-on-error estatuts.tex
```

La segona execució actualitza referències internes com el número total de
pàgines.
