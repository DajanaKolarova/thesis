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

3. Složka `/sections/`:

   * Obsahuje jednotlivé části textu (např. `experiment.tex` s příkladem materiálů a metod).
   * Můžeš si vytvořit vlastní soubory pro jednotlivé kapitoly a vložit je do `main.tex` pomocí:

     ```latex
     \input{sections/nazev_souboru}
     ```

4. Složka `/figures/`:**

   * Sem patří obrázky, které vkládáš do práce příkazem:

     ```latex
     \includegraphics[width=\textwidth]{figures/nazev_souboru.png}
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




## 📁 Struktura projektu

projekt/
│
├── main.tex               % Hlavní soubor - balíčky, fonty, základní globální nastavení
├── bibliography.bib       % Literární zdroje (BibTeX)
│
├── sections/              % Jednotlivé části dokumentu
│   ├── example.tex        % Ukázková kapitola
│   └── experiment.tex     % Ukázka experimentální části
│
└── figures/                % Obrázky
    ├── example.png


## 🧠 Doporučení pro úplné začátečníky

* Každý příkaz má v této šabloně komentář začínající `%`, který ti vysvětlí, co dělá.
* Nejprve jen měň texty a názvy kapitol. Piš svůj hlavní text. Až potom zkoušej tabulky, obrázky a literaturu.
* Když nevíš, strejda ChatGPT ti pomůže
