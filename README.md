# 🧪 LaTeX Template for Scientific Writing 

This template serves as a basic structure for writing scientific, laboratory, or student papers in LaTeX.
It includes comments explaining basic commands and a sample document structure.
It is suitable even for beginners who are just starting with LaTeX.

⚙️ **How to use the template in Overleaf**

Create a new project:

* Log in at Overleaf.com.
* Click **"New Project" → "Upload Project".**
* Upload the entire downloaded `.zip` file or individual `.tex` files and images.

**Main file:**

`main.tex`.
This file is the **main control file** for the entire project. It contains:

* **Global settings:** package imports, language settings, fonts, page layout, and bibliography settings.
* **Chapter calls:** loads other files where the actual content is written.


### **Structure**

```
project/
│
├── main.tex               % Main file - packages, fonts, global settings
├── bibliography.bib       % Bibliography (BibTeX)
│
├── sections/
│   ├── 0firstcomponents.tex            % Acknowledgments, Abstract, Summary
│   ├── 1INTRODUCTION.tex               % Introduction
│   ├── 2THEORITICAL_PART.tex           % Theoretical background
│   ├── 3METHODS.tex                    % Materials and Methods
│   ├── 4RESULTS.tex                    % Results
│   ├── 5CONCLUSION.tex                 % Discussion and Conclusion
│   ├── 6lastcomponents.tex             % List of abbreviations
│   ├── 7appendix.tex                   % Appendices
│
└── figures/                % Images
    ├── example_1.png
    ├── example_2.png
```


### **Bibliography:**

The example file with citations is `bibliography.bib`.

It can be synchronized with **Zotero**.

In the text, cite using:

```
\cite{key}
```

At the end of the `main.tex` file, add the bibliography with:

```
\printbibliography
```


### **Compilation:**

* In Overleaf, select the **XeLaTeX** or **pdfLaTeX** compiler.
* Click **"Recompile"**.


LaTeX often throws errors. This is normal.
With time, you'll learn to recognize common mistakes in just a few seconds.
Don't be afraid to experiment and try again.

* Check **the top of the log**, where the compiler reports **"Error"** – this is usually the main problem.
* In Overleaf, click on the error message – it will show you the **exact line**.
* Look for words like **"missing"** (something is missing) or **"undefined"** (something doesn’t exist).


💡 **Tips for complete beginners**

* Each command in this template has a comment starting with `%`, explaining what it does.
* Start by changing the text and chapter titles. Just write your main text first.
  Then try tables, images, and citations.
* If you're stuck, ask your friend ChatGPT to help. 😉



✏️ **Basic text formatting in LaTeX**

```
\textbf{bold}   
\textit{italic}     
\underline{underlined}

\section{Title}
\subsection{Title}   
\subsubsection{Title}
\paragraph{Title} 

\newline   % line break
\newpage   % new page
```

A blank line in the code → new paragraph.


**Bullet list:**

```
\begin{itemize}
    \item First item
    \item Second item
\end{itemize}
```

**Numbered list:**

```
\begin{enumerate}
    \item First point
    \item Second point
\end{enumerate}
```

---

### **Equation**

```
\begin{equation}
E = mc^2
\end{equation}
```


### **Image**

```
\begin{figure}[H]
\centering
\includegraphics[width=0.5\textwidth]{figures/example.png}
\caption{Image caption}
\label{fig:example}
\end{figure}
```

### **Table**

```
\begin{tabular}{|l|l|}
\hline
Header 1 & Header 2 \\
\hline
Item A & Item B \\
\hline
\end{tabular}
```



## ❓ **Why use LaTeX instead of Word?**

 Advantages:
✅ Stable output (no images randomly shifting when formatting)
✅ Ideal for long documents (theses, dissertations, articles)
✅ Supports many languages and scientific fields (math formulas, chemical reactions, etc.)
✅ Citation management (BibTeX, biblatex) – automatic formatting according to journal styles
✅ Professional typography (consistent spacing, clean alignment, readable fonts)
✅ Automatic table of contents, list of figures, list of tables

Disadvantages:
⚠️ Higher learning curve (you learn to write code, not just click)

 Summary:
If you want full control over your document and you enjoy learning something new,
LaTeX is a great choice.
Word is fine for quick writing, but LaTeX will save you time during formatting and revisions.

