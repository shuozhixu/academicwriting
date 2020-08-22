# Introduction

Writing a paper for a peer-reviewed scientific journal is not easy. Here, I share some of my experiences in writing one. A list of my publications can be found on [my Google Scholar page](https://scholar.google.com/citations?user=LhG5xZ4AAAAJ&hl=en).

# Text editor

First, what do we use to write? A text editor. Most people I know use either [Microsoft Word](https://en.wikipedia.org/wiki/Microsoft_Word) or [LaTeX](https://en.wikipedia.org/wiki/LaTeX). I recommend the latter. Similar to that multiple authors can collaborate on a Word document using [Google Docs](https://en.wikipedia.org/wiki/Google_Docs), people can do the same on a LaTeX document using [Overleaf](https://en.wikipedia.org/wiki/Overleaf). There are other LaTeX online services  but Overleaf is the one I use. Just go to [its website](https://www.overleaf.com) and create an account.

With Overleaf, you do not need to install any LaTeX-related software on your own computer. But if you want, you can. Follow [this page](https://www.latex-project.org/get).

If you are a beginner of LaTeX, these references may be helpful:

- [Learn LaTeX in 30 minutes](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes)
- [The Not So Short Introduction to LaTeX 2&epsilon;](http://ctan.math.washington.edu/tex-archive/info/lshort/english/lshort-letter.pdf)

# Structure of a paper

A scientific paper consists of five main parts: Introduction, Methods, Results, Discussion, and Conclusion. I usually write in that order. But some people write Methods, Results, Discussion first, before finishing Introduction and Conclusion. Some other people prefer having an outline first and/or having the figures/tables ready before they start writing. It is your choice.

There are already many good references on this topic, e.g.,

- [The art of writing science](https://doi.org/10.1002/pro.514)
- [How to write a first-class paper](https://doi.org/10.1038/d41586-018-02404-4)
- [Writing a scientific article: A step-by-step guide for beginners](https://doi.org/10.1016/j.eurger.2015.08.005)
- [11 steps to structuring a science paper](https://www.elsevier.com/connect/11-steps-to-structuring-a-science-paper-editors-will-take-seriously)
- [How to write a compelling (materials) science paper](https://doi.org/10.1016/j.mtla.2019.100339)
- [How to Write and Publish a Scientific Paper](https://www.amazon.com/How-Write-Publish-Scientific-Paper-dp-1316640434/dp/1316640434/ref=dp_ob_title_bk) - this is a book

# Writing style

The writing style varies greatly depending on the journal you want to submit your manuscrip to. Read the instructions carefully. Below are some examples:

- [Science](https://www.sciencemag.org/authors/science-information-authors)
- [Nature](https://www.nature.com/nature/for-authors)
- [PNAS](https://www.pnas.org/authors/submitting-your-manuscript)
- [Acat Materialia](https://www.elsevier.com/journals/acta-materialia/1359-6454/guide-for-authors)
- [JMPS](https://www.elsevier.com/journals/journal-of-the-mechanics-and-physics-of-solids/0022-5096/guide-for-authors)

For general writing style, I highly recommend [this book](https://www.amazon.com/Elements-Style-Fourth-William-Strunk/dp/020530902X). Chinese speakers may also be interested in [this book](https://www.amazon.com/English-Exposed-Mistakes-Chinese-Speakers/dp/9888390759).

## Main text

Below I give a list of some specific rules in writing the main text of an academic paper using LaTeX:

- Use one, not two, space after a period, [unless you are typing on an acutal typewritter](https://slate.com/technology/2011/01/two-spaces-after-a-period-why-you-should-never-ever-do-it.html) - even [APA changed their recommendation](https://apastyle.apa.org/style-grammar-guidelines/punctuation/space-after-period)
- Italicize all variables, but not non-variables. Follow this rule everywhere, including figures and tables. For example,
	- _x_ axis, _y_ axis, and _z_ axis 
	- elastic anisotropic index for cubic crystals: _A_<sub>c</sub>. _A_ is italic but the subscript c is not because it stands for cubic
	- however, if there is a vector _B_, which has three components and you use _a_, _b_, _c_ to denote each component, do italicize them, e.g., _B<sub>c</sub>_
	- do not italicize units, e.g., write `mJ/m$^2$` or `$\mathrm{mJ/m}^2$`, instead of `$mJ/m^2$`
- [Always use the Oxford comma](https://www.businessinsider.com/always-use-the-oxford-comma-2015-5).
- Be aware of [the lack of space after `\AA`](https://tex.stackexchange.com/questions/179625/in-text-mode-space-being-taken-away?noredirect=1&lq=1). A few tips:
	- write `\AA\` or `\AA{}`
	- if `\AA` is followed by a period or a comma, do not do anything special, i.e., just write `\AA.` or `\AA,`. If you use a backslash in front of a period or a comma, [it becomes a space](https://texblog.org/2014/04/09/whitespace-in-math-mode)
- Sometimes a period does not denote the end of a sentence. In this case, we need to use a backslash following the period, otherwise the space would be too wide, e.g.,
	- `Ref.\ [34]`
	- `Barack H.\ Obama II`
	- `Fig.\ [2]`
- For a short line over a number, use `\bar`, instead of `\overline`, e.g., `\bar{1}\bar{1}0`. `\overline` is too wide, especially when two are used sequentially.
- Add a space before the left bracket or the left parenthesis, e.g., `molecular dynamics (MD)` instead of `molecular dynamics(MD)`.
- Add a space before citing a reference, e.g., `I have a dream \cite{king1963}` instead of `I have a dream\cite{king1963}`.
- Add a space between the number and the unit, e.g., `10 nm` instead of `10nm`.
- Use [the correct units](https://www.nist.gov/pml/weights-and-measures/metric-si/si-units), e.g., 100 kelvin is written as `100 K` instead of `100 k`.
- To cite multiple references in the same place, use one `\cite`, e.g., write `\cite{king1963,obama2008}` instead of `\cite{king1963}\cite{obama2008}`. 
- When using an acronym, spell out the entire phrase once and once only and only when the phrase is used for the first time. Common mistakes include
	- write `molecular dynamics (MD)` on page 1, then write `molecular dynamics` on page 2
	- write `molecular dynamics (MD)` on page 1, then write `molecular dynamics (MD)` again on page 2
	- write `molecular dynamics` on page 1, then write `molecular dynamics (MD)` on page 2
	- write `MD` throughout the paper, without spelling out `molecular dynamics` at all
- For [dash](https://en.wikipedia.org/wiki/Dash) in text mode, use `-` for an ordinary hyphen, `--` for an en dash, and `---` for an em dash. For more on the dashes, read [this page](https://getitwriteonline.com/articles/en-dashes-em-dashes).
- A dash in math mode becomes the minus sign, e.g., `$-10$ degree Fahrenheit`. Do not write `-10 degree Fahrenheit`. Double check this in the main text and tables.
- If you use the full name of a chemical element, do not capitalize the first letter unless it is the first letter of a sentence, e.g., write `we study iron` instead of `we study Iron`. However, if you use the symbol of a chemical element, do capitalize the first letter, e.g., write `Fe` instead of `fe`.
- To create angular brackets in math mode, write `$\left<110\right>$` or `$\langle 110\rangle$` instead of `$<110>$` which yields less-than and greater-than signs. Note: `<` and `>` only works in math mode.
- Pay attention to the special letter(s) in people's names, e.g., `Schr\"{o}dinger` instead of `Schrodinger`. See [this page](https://en.wikibooks.org/wiki/LaTeX/Special_Characters) for special characters in LaTeX.

## Reference list

The reference style differs greatly among journals. Read their instructions carefully. In LaTeX, there are [two main ways to manage the reference list](https://www.overleaf.com/learn/latex/bibliography_management_with_bibtex): BibTeX and non-BibTeX. I strongly recommend the former. With BibTeX, simply write these two lines at the end of the paper (but before `\end{document}`):

- `\bibliographystyle{unsrt}`
- `\bibliography{ref}`

which would require two files: `unsrt.bst` and `ref.bib`. Most likely the first file is provided by the journal. In practice, however, Overleaf can retrieve a lot of `.bst` files from its server, so you may only need to provide the file `ref.bib`.

Double check the reference list for typos as if it were the main text. Pay attention to these :

- Write `$\left<110\right>$` and `\{110\}` instead of `<110>` and `{110}`.
- Write `dislocations in Mo` and `dilute Mg-based alloys` instead of `dislocations in mo` and `dilute mg-based alloys`. Unfortunately, in the article title, most BibTeX style automatically converts all uppercase letters to lowercase ones, except the very first letter. To enforce the usage of uppercase letters, add curly brakets around certain words/letters in your `.bib` file, e.g., `dislocations in {Mo}` or `dislocations in {M}o`.
- Use special letter(s) in authors' names, if any.
- When necessary, use math mode, e.g., `($\bar{1}10$)` instead of `(-110)`.
- In most cases, use abbreviated jouranl names, e.g., `Acta Mater.` instead of the full journal name, i.e., `Acta Materialia`.  Check [this webpage](https://woodward.library.ubc.ca/research-help/journal-abbreviations/) for the correct abbreviated journal names. Omit all articles (a, an, the) and prepositions (e.g., at, in, of, for, with). Also capitalize the first letter of each word. For example, write `J. Chem. Phys.`, instead of `The J. of Chem. Phys.` or `J. chem. phys.`  

