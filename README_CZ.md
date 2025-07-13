# 🧪 LaTeX šablona pro vědecké práce (CZ)

Tato šablona slouží jako základní kostra pro psaní **vědeckých, laboratorních nebo studentských prací v LaTeXu**. Obsahuje komentáře k základním příkazům a ukázku struktury dokumentu. Je vhodná i pro začátečníky, kteří se s LaTeXem teprve seznamují.

CustomGPT kompatibilní s touto šablonou: https://chatgpt.com/g/g-6803582b37a8819190dd2132d148b86d-latex-thesis-code-tutor

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

     ```
     \cite{klic}
     ```
   * Na konci souboru `main.tex` je příkaz pro vypsání literatury:

      ```
     \printbibliography
     ```

6. Kompilace:

   * V Overleaf zvol jako kompilátor **XeLaTeX** nebo **pdfLaTeX**.
   * Klikni na **"Recompile"**.


LaTeX chybuje často. Je to normální. Časem si zvykneš rozpoznávat běžné chyby během pár sekund.
Neboj se experimentovat a zkusit to znovu.

        * Podívej se **nahoře v logu**, kde kompilátor hlásí **"Error"** – tam bývá hlavní problém.
        * Pokud máš Overleaf, klikni na chybu, ukáže ti **konkrétní řádek**.
        * Hledej „missing“ (něco chybí) nebo „undefined“ (něco neexistuje).


## 💡� Doporučení pro úplné začátečníky

* Každý příkaz má v této šabloně komentář začínající `%`, který ti vysvětlí, co dělá.
* Nejprve jen měň texty a názvy kapitol. Piš svůj hlavní text. Až potom zkoušej tabulky, obrázky a literaturu.
* Když nevíš, strejda ChatGPT ti pomůže


## ✏️ **Základní formátování textu v LaTeXu**
```
\textbf{tučný}   
\textit{kurzíva}     
\underline{podtržený}
\section{Název}
\subsection{Název}   
\subsubsection{Název}
\paragraph{Název} 
\newline
\newpage  
prázdný řádek v kódu  - nový odstavec  
```

#### **Odrážkový seznam:**

```
\begin{itemize}
    \item První položka
    \item Druhá položka
\end{itemize}
```

#### Číslovaný seznam:

```
\begin{enumerate}
    \item První bod
    \item Druhý bod
\end{enumerate}
```

###**Rovnice**
```
\begin{equation}
E = mc^2
\end{equation}
```


### **Obrázek**

```
\begin{figure}[H]
\centering
\includegraphics[width=0.5\textwidth]{figures/example.png}
\caption{Popisek obrázku}
\label{fig:example}
\end{figure}
```


### **Tabulka**

```
\begin{tabular}{|l|l|}
\hline
Nadpis 1 & Nadpis 2 \\
\hline
Položka A & Položka B \\
\hline
\end{tabular}
```


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

