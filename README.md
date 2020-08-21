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

Below I give a list of some specific rules in writing an academic paper using LaTeX:

- Use one, not two, space after a period, [unless you are typing on an acutal typewritter](https://slate.com/technology/2011/01/two-spaces-after-a-period-why-you-should-never-ever-do-it.html) - even [APA changed their recommendation](https://apastyle.apa.org/style-grammar-guidelines/punctuation/space-after-period)
- Italicize all variables, but not non-variables. Follow this rule everywhere, including figures and tables. For example,
	- _x_ axis, _y_ axis, and _z_ axis 
	- elastic anisotropic index for cubic crystals: _A_<sub>c</sub>. _A_ is italic but the subscript c is not because it stands for cubic
	- however, if there is a vector _B_, which has three components and you use _a_, _b_, _c_ to denote each component, do italicize them, e.g., _B<sub>c</sub>_
	- do not italicize units, e.g., write `mJ/m$^2$` or `$\mathrm{mJ/m}^2$`, instead of `$mJ/m^2$`
- [Always use the Oxford comma](https://www.businessinsider.com/always-use-the-oxford-comma-2015-5)
- Be aware of [the lack of space after `\AA`](https://tex.stackexchange.com/questions/179625/in-text-mode-space-being-taken-away?noredirect=1&lq=1). A few tips:
	- write `\AA\` or `\AA{}`
	- if `\AA` is followed by a period or a comma, do not do anything special, i.e., just write `\AA.` or `\AA,`. If you use a backslash in front of a period or a comma, [it becomes a space](https://texblog.org/2014/04/09/whitespace-in-math-mode)
- Sometimes a period does not denote the end of a sentence. In this case, we need to use a backslash in front of the period, otherwise the space would be too wide, e.g.,
	- `Ref.\ [34]`
	- `Barack H.\ Obama II`
	- `Fig.\ [2]`
- For a short line over a number, use `\bar`, instead of `\overline`, e.g., `\bar{1}\bar{1}0`. `\overline` is too wide, especially when two are used sequentially
- Add a space before the left bracket or the left parenthesis, e.g., `molecular dynamics (MD)` instead of `molecular dynamics(MD)`
- Add a space before citing a reference, e.g., `I have a dream \cite{king1963}`
- To cite multiple references in the same place, use one `\cite`, e.g., write `\cite{king1963,obama2008}` instead of `\cite{king1963}\cite{obama2008}` 
- When using an acronym, spell out the entire phrase once and once only and only when the phrase is used for the first time. Common mistakes include
	- write `molecular dynamics (MD)` on page 1, then write `molecular dynamics` on page 2
	- write `molecular dynamics (MD)` on page 1, then write `molecular dynamics (MD)` again on page 2
	- write `molecular dynamics` on page 1, then write `molecular dynamics (MD)` on page 2
	- write `MD` throughout the paper, without spelling out `molecular dynamics` at all
- For [dash](https://en.wikipedia.org/wiki/Dash) in non-math mode, use `-` for an ordinary hyphen, use `--` for an en dash, and use `---` for an em dash. For more on the dashes, read [this page](https://getitwriteonline.com/articles/en-dashes-em-dashes)
- A dash in math mode becomes the minus sign, e.g., `$-10$ degree Fahrenheit`. Do not write `-10 degree Fahrenheit`. Double check this in the main text and tables.