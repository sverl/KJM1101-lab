# KJM1101 lab exerciese
This is the LaTeX source for the chemistry lab used in KJM1101 from 2017.

## Compiling
To compile the documents, run
```bash
xelatex labX.tex
```
or (make life easy)
```bash
texliveonfly --compiler=xelatex labX.tex
```

## Track changes
To track changes in document, run
```bash
git latexdiff --latexmk --latexopt "-xelatex" HEAD~1 --main ./labX/labX.tex
```
for diff of last and second to last commit in the current branch or
```bash
git latexdiff --latexmk --latexopt "-xelatex" --main ./labX/labX.tex branch1 branch2
```
for diff between branches.
