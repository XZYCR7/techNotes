1. [\newcommand vs \DeclareRobustCommand](https://tex.stackexchange.com/questions/61503/newcommand-vs-declarerobustcommand)
2. [increment-the-section-number](https://tex.stackexchange.com/questions/73104/increment-the-section-number-with-1-not-0-1)
3. [line-spacing](https://texblog.org/2011/09/30/quick-note-on-line-spacing/)
4. [Align section with text body](https://tex.stackexchange.com/questions/405372/align-section-with-text-body)
5. [cleardoublepage](https://stackoverflow.com/questions/491904/how-do-i-remove-blank-pages-coming-between-two-chapters-in-appendix)
6. [New chapter top margin is large](https://tex.stackexchange.com/questions/149757/new-chapter-top-margin-is-large)
7. [remove-spacing-before-chapter-in-latex](https://stackoverflow.com/questions/3279194/remove-spacing-before-chapter-in-latex)
# 玄学问题

1. 标题加粗

```tex
\newcommand{\sanhao}{\fontsize{16pt}{\baselineskip}\selectfont\bfseries} 
\titleformat{\chapter}{\centering\sanhao}{\thechapter}{0em}{}
```

可以加粗

而

```tex
\newcommand{\sanhao}{\fontsize{16pt}{\baselineskip}\selectfont} 
\titleformat{\chapter}{\centering\sanhao\bfseries}{\thechapter}{0em}{}
```
不可以

参考 [Bold and italic subsection title with custom font size](https://tex.stackexchange.com/questions/165930/bold-and-italic-subsection-title-with-custom-font-size)

## 数学缩写

列表：https://en.wikipedia.org/wiki/List_of_mathematical_abbreviations

## matrix

https://tex.stackexchange.com/questions/153615/help-me-input-a-column-vector

http://latex.wikia.com/wiki/Matrix_environments

## Embed source files into the generated PDF

https://tex.stackexchange.com/questions/13187/is-there-some-way-to-embed-latex-source-code-in-a-pdf-file

## 章节内单独编号

1. https://tex.stackexchange.com/questions/356109/how-do-i-label-equations-without-the-chapter-number
2. https://tex.stackexchange.com/questions/28333/continuous-v-per-chapter-section-numbering-of-figures-tables-and-other-docume

## 编号问题

1. https://tex.stackexchange.com/questions/2597/how-do-i-turn-off-equation-auto-numbering
2. https://tex.stackexchange.com/questions/17528/show-equation-number-only-once-in-align-environment

## 文献

1. https://stackoverflow.com/questions/2765209/latex-bibliography-per-chapter
2. https://tex.stackexchange.com/questions/130228/two-styles-in-biblatex-with-textcite-author-year-and-author-year

3. https://tex.stackexchange.com/questions/369710/beamer-citation-coloring

每章从头开始

\renewcommand{\theequation}{\arabic{equation}}

独立于每章

\RequirePackage{chngcntr}
\counterwithout{equation}{chapter} % without chapter number

## page break

1. https://tex.stackexchange.com/questions/74296/to-have-no-pagebreak-before-bibliography
2. https://tex.stackexchange.com/questions/74296/to-have-no-pagebreak-before-bibliography?noredirect=1&lq=1


## others

1. https://tex.stackexchange.com/questions/8351/what-do-makeatletter-and-makeatother-do
2. https://tex.stackexchange.com/questions/246/when-should-i-use-input-vs-include
3. https://tex.stackexchange.com/questions/25701/bibtex-vs-biber-and-biblatex-vs-natbib
4. https://tex.stackexchange.com/questions/1050/whats-the-difference-between-newcommand-and-newcommand
5. https://tex.stackexchange.com/questions/250159/how-to-pass-title-or-other-parameter-to-class-file?rq=1

## 每章单独的参考文献

biblatex：
1. https://tex.stackexchange.com/questions/87414/per-chapter-bibliographies-in-biblatex

natbib:
1. https://stackoverflow.com/questions/2765209/latex-bibliography-per-chapter

## textcite 自定义

1. https://tex.stackexchange.com/questions/306801/different-comma-placement-in-textcite-and-parencite
2. https://tex.stackexchange.com/questions/359426/biblatex-using-and-within-textcite-within-parencite-within-bibliogr
3. https://github.com/plk/biblatex/issues/373

## table
1. https://tex.stackexchange.com/questions/19589/how-to-specify-the-row-height-in-latex-table/19594