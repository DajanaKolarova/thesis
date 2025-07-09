# 🧪 LaTeX šablona pro vědecké práce (CZ)

Tato šablona slouží jako základní kostra pro psaní **vědeckých, laboratorních nebo studentských prací v LaTeXu**. Obsahuje komentáře k základním příkazům a ukázku struktury dokumentu. Je vhodná i pro začátečníky, kteří se s LaTeXem teprve seznamují.

## ⚙️ Jak šablonu použít v Overleaf

1. Vytvoř nový projekt:

   * Přihlas se na [Overleaf.com](https://www.overleaf.com).
   * Klikni na **"New Project" → "Upload Project"**.
   * Nahraj celý stažený `.zip` soubor nebo jednotlivé `.tex` soubory a obrázky.

2. Hlavní soubor:

`main.tex`.
Tento soubor slouží jako hlavní řídící soubor celého projektu.
Obsahuje:
Globální nastavení: použití balíčků, nastavení jazyka, písma, vzhledu stránky, nastavení obsahu a citací.
Volání jednotlivých kapitol: načítá další soubory, kde je skutečný obsah práce.


3. Sekce
   
   ```
projekt/
│
├── main.tex               % Hlavní soubor - balíčky, fonty, základní globální nastavení
├── bibliography.bib       % Literární zdroje (BibTeX)
│
├── sections/
│   ├── 0firstcomponents.tex            % Poděkování, souhrn, summary
│   ├── 1INTRODUCTION.tex               % Úvod
│   ├── 2THEORITICAL_PART.tex           % Teoretická rešerše
│   ├── 3METHODS.tex                    % Seznam materiálů a metody
│   ├── 4RESULTS.tex                    % Výsledky
│   ├── 5CONCLUSION.tex                 % Diskuze a závěr
│   ├── 6lastcomponents.tex             % Seznam použitých zkratek
│   ├── 7appendix.tex                   % Přílohy
│
└── figures/                % Obrázky
    ├── example_1.png
    ├── example_2.png
   ```


5. Literatura:

   * Ukázkový soubor s citacemi je `bibliography.bib`.
   * Dá se synchronizovat se zotero
   * V textu cituješ pomocí:

     ```latex
     \cite{klic}
     ```
   * Na konci souboru `main.tex` je příkaz pro vypsání literatury:

     ```latex
     \printbibliography
     ```

6. Kompilace:

   * V Overleaf zvol jako kompilátor **XeLaTeX** nebo **pdfLaTeX**.
   * Klikni na **"Recompile"**.


## 🧠 Doporučení pro úplné začátečníky

* Každý příkaz má v této šabloně komentář začínající `%`, který ti vysvětlí, co dělá.
* Nejprve jen měň texty a názvy kapitol. Piš svůj hlavní text. Až potom zkoušej tabulky, obrázky a literaturu.
* Když nevíš, strejda ChatGPT ti pomůže


## Proč psát v LaTeXu a ne wordu?

% Výhody:
✅ Stabilní výstup (žádné posouvání obrázků při formátování)
✅ Vhodný pro dlouhé práce (bakalářky, diplomky, články, disertace)
✅ Podpora mnoha jazyků a vědeckých formátů (matematické vzorece, chemické rovnice,.. )
✅ Práce s citacemi (BibTeX, biblatex) – automatické formátování podle stylů časopisů
✅ Profesionální typografie (rovnoměrné mezery, kvalitní zarovnání textu, čitelné fonty)
✅ Automatická tvorba obsahu, seznamu obrázků a tabulek

Nevýhody:
⚠️ Vyšší vstupní náročnost (učíš se psát kód, ne jen klikání)

Shrnutí:
Pokud chceš mít nad svým dokumentem plnou kontrolu a zároveň Tě baví naučit se něco nového, LaTeX je skvělá volba.
Word je fajn pro rychlé psaní, ale LaTeX Ti ušetří čas při formátování a revizích.

