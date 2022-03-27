
# Związek Harcerstwa Rzeczypospolitej
## Śpiewnik Duszpasterstwa w Opolu

### Autorzy
* Jan  Żaba [jan.zaba@zhr.pl](mailto:jan.zaba@zhr.pl)


### Instrukcja uruchomienia
1. Pobierz projekt
2. Zainstaluj środowisko [LaTeX](https://www.latex-project.org/get/)
3. Zainstaluj program do edycji plików tex (polecam [TexMaker](https://www.xm1math.net/texmaker/))
4. W programie do edycji otwórz plik `spiewnik.tex` i uruchom kompilację. Efektem powinien być wygenerowany plik .pdf


### Pomocne uwagi
#### Śpiewnik w wersji bez chwytów
Aby wyłączyć kompilowanie chwytów - odkomentuj polecenie `chordsoff`
```
% for music 
...
	\chordsoff
...
%%% ---------------------------------------------------
```

#### Rozmiar i orientacja strony
Formatem i orientacją można sterować w sekcji `for margins and paper size`.
Wystarczy zakomentować aktualny format i odkomentować oczekiwany

```
% for margins and paper size
	%A4 Portrait
		%\usepackage[top=0.5in, bottom=0.7in, left=0.5in, right=0.5in, paperheight=11.7in,paperwidth=8.3in]{geometry}
		
	%A4 Horizontal
		%\usepackage[top=0.5in, bottom=0.7in, left=0.5in, right=0.5in, paperheight=8.3in,paperwidth=11.7in]{geometry}	
	%A5
		\usepackage[top=0.3in, bottom=0.7in, left=0.1in, right=0.1in, paperheight=8.3in,paperwidth=5.8in]{geometry}
	\usepackage{marginnote}
% page size
```

#### Spisy treści
Po każdym dodaniu pieśni lub zmianie tytułu należy przegenerować indeksu (spisy). 
Mozna odświeżyć wszystkie spisy za pomocą skryptu:

```
sh ./reindex.sh
```
