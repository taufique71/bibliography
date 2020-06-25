# bibliography

Personal bibliographic database in Bibtex format.

## How to use in LaTeX documents?
The bibliography style is set with `\bibliographystyle{stylename}` and the bibliography file is imported with `\bibliography{bibfile}`.
Here `bibfile` is the name of the bibliography `.bib` file, without the extension and `stylename` is one of the following:
- abbrv
- acm
- alpha
- apalike
- ieeetr
- plain
- siam
- unsrt

```tex
\documentclass[12pt]{article}

\bibliographystyle{alpha}

\title{Some Document}

\begin{document}

    \maketitle

    \section{Hello}
    Hello World

    \bibliography{bibfile}

\end{document}
```

After that compiling is done with following four steps -
1. `pdflatex document.tex`
2. `bibtex document.aux`
3. `pdflatex document.tex`
4. `pdflatex document.tex`
