# Introduction

Writing a paper for a peer-reviewed scientific journal is not easy. Here, I share some of my experiences in writing one. A list of my publications can be found on [my Google Scholar page](https://scholar.google.com/citations?user=LhG5xZ4AAAAJ&hl=en).

# Text editor

First, what do we use to write? A text editor. Most people I know use either [Microsoft Word](https://en.wikipedia.org/wiki/Microsoft_Word) or [LaTeX](https://en.wikipedia.org/wiki/LaTeX). I recommend the latter. Similar to that multiple authors can collaborate on a Word document using [Google Docs](https://en.wikipedia.org/wiki/Google_Docs), people can do the same on a LaTeX document using [Overleaf](https://en.wikipedia.org/wiki/Overleaf). There are other LaTeX online services  but Overleaf is the one I use. Just go to [its website](https://www.overleaf.com) and create an account.

With Overleaf, you do not need to install any LaTeX-related software on your own computer. But if you want, you can. Follow [this page](https://www.latex-project.org/get).

If you are a beginner of LaTeX, these references may be helpful:

- [Learn LaTeX in 30 minutes](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes)
- [The Not So Short Introduction to LaTeX 2&epsilon;](http://ctan.math.washington.edu/tex-archive/info/lshort/english/lshort-letter.pdf)

# Article type and journal selection

There are two [main types of academic papers](https://www.springer.com/gp/authors-editors/authorandreviewertutorials/writing-a-journal-manuscript/types-of-journal-articles/10285504): research articles and review articles. The former report original research while the latter provide a summary of research on a certain topic and perspective on where the field is heading. Some journals publish research articles only, some review articles only, some both.

## Research article

Depending on the length, there are two main types of research articles: full length articles and letters. 

A full length article consists of five main parts, each of which has a heading: Introduction, Methods, Results, Discussion, and Conclusion. However, this is not necessarily the order in which these sections appear in a paper because some journals, e.g., [_npj Computational Materials_](https://www.nature.com/npjcompumats), want you to put the Methods section at the end. Letters usually do not have any heading, but the structure is largely the same. Some letters, e.g., [_Nature_](https://www.nature.com/nature/for-authors/formatting-guide), want you to have a section with heading Methods at the end of the text.

Some journals publish full length article only, some letters only, some both. In some journals, e.g., [_Physical Review Materials_](https://journals.aps.org/prmaterials/authors), the letter-size paper is called Rapid Communication. To find out more about a jouranl, read the recently published work in it. Also read their instructions carefully. Below are some examples:

- [_Science_](https://www.sciencemag.org/authors/science-information-authors)
- [_Nature_](https://www.nature.com/nature/for-authors)
- [_PNAS_](https://www.pnas.org/authors/submitting-your-manuscript)
- [_Acat Materialia_](https://www.elsevier.com/journals/acta-materialia/1359-6454/guide-for-authors)
- [_JMPS_](https://www.elsevier.com/journals/journal-of-the-mechanics-and-physics-of-solids/0022-5096/guide-for-authors)

Once you select a journal, start writing. When I write a paper, I start with Introduction and end with Conclusion, before finishing the Abstract. But some people write Methods, Results, Discussion first, followed by Introduction, Conclusion, and Abstract. Some other people prefer having an outline first and/or having the figures/tables ready before they start writing. It is your choice. 

## Review article

Writing a review article is different from writing a research article. [This video from Elsevier](https://researcheracademy.elsevier.com/writing-research/technical-writing-skills/editor-guide-writing-review-article) may be useful.

Below is the list of some journals in my field that only publish review articles:

- [_Progress in Materials Science_](https://www.journals.elsevier.com/progress-in-materials-science)
- [_Annual Review of Materials Research_](https://www.annualreviews.org/journal/matsci) - by invitation only
- [_Materials Science and Engineering R: Reports_](https://www.journals.elsevier.com/materials-science-and-engineering-r-reports) - by invitation only
- [_Current Opinion in Solid State & Materials Science_](https://www.journals.elsevier.com/current-opinion-in-solid-state-and-materials-science)
- [_International Materials Reviews_](https://www.tandfonline.com/toc/yimr20/current)
- [_Critical Reviews in Solid State and Materials Sciences_](https://www.tandfonline.com/toc/bsms20/current)
- [_Archives of Computational Methods in Engineering_](https://www.springer.com/journal/11831)

# Writing style

The writing style varies greatly depending on the type of article you want to write and the journal you want to submit your manuscript to. For general writing style, I highly recommend [this book](https://www.amazon.com/Elements-Style-Fourth-William-Strunk/dp/020530902X). Chinese speakers may also be interested in [this book](https://www.amazon.com/English-Exposed-Mistakes-Chinese-Speakers/dp/9888390759).

There are also many good references on this topic, e.g.,

- [The art of writing science](https://doi.org/10.1002/pro.514)
- [How to write a first-class paper](https://doi.org/10.1038/d41586-018-02404-4)
- [Writing a scientific article: A step-by-step guide for beginners](https://doi.org/10.1016/j.eurger.2015.08.005)
- [11 steps to structuring a science paper](https://www.elsevier.com/connect/11-steps-to-structuring-a-science-paper-editors-will-take-seriously)
- [How to write a compelling (materials) science paper](https://doi.org/10.1016/j.mtla.2019.100339)
- [How to Write and Publish a Scientific Paper](https://www.amazon.com/How-Write-Publish-Scientific-Paper-dp-1316640434/dp/1316640434/ref=dp_ob_title_bk) - this is a book

## Main text

First, avoid plagiarism, including the words that come from prior published work by the same author(s). Pay special attention to the Introduction and Methods sections in your research articles and all sections in your review articles. Here are some useful resources:

- [What is plagiarism?](http://studentconduct.sa.ucsb.edu/academic-integrity)
- [Eight most common types of plagiarism](https://www.enago.com/academy/fraud-research-many-types-plagiarism)
- [Elsevier Publication Ethics Q&A](https://www.elsevier.com/editors/perk/questions-and-answers)
- [UCSB Academic Integrity](http://studentconduct.sa.ucsb.edu/academic-integrity)

Below I give a list of specific rules in writing the main text of an academic paper using LaTeX:

- Use one, not two, space after a period, [unless you are typing on an acutal typewritter](https://slate.com/technology/2011/01/two-spaces-after-a-period-why-you-should-never-ever-do-it.html) - even [Microsoft Word changed their mind](https://www.theverge.com/2020/4/24/21234170/microsoft-word-two-spaces-period-error-correction-great-space-debate). In practice, there is no need to type an additional space, because [LaTeX treats multiple, consecutive spaces as if they were a single space](http://www.ctex.org/documents/latex/latex2e-html/ltx-143.html).
- Italicize all variables, but not non-variables. Follow this rule everywhere, including figures and tables. For example,
	- _x_ axis, _y_ axis, and _z_ axis 
	- elastic anisotropic index for cubic crystals: _A_<sub>c</sub>. _A_ is italic but the subscript c is not because it stands for cubic
	- however, if there is a vector _B_, which has three components and you use _a_, _b_, _c_ to denote each component, do italicize them, e.g., _B<sub>c</sub>_
	- do not italicize units, e.g., write `mJ/m$^2$` or `$\mathrm{mJ/m}^2$`, instead of `$mJ/m^2$`
- When you want to italicize one or more words because you want to emphasize or quote something, use `\emph`, e.g., `\emph{I have a dream}` or `\emph{very} important`. Do not use the math mode. `$I have a dream$` would yield _Ihaveadream_.
- [Always use the Oxford comma](https://www.businessinsider.com/always-use-the-oxford-comma-2015-5).
- Be aware of [the lack of space after `\AA`](https://tex.stackexchange.com/questions/179625/in-text-mode-space-being-taken-away?noredirect=1&lq=1). A few tips:
	- write `\AA\` or `\AA{}`
	- if `\AA` is followed by a period or a comma, simply write `\AA.` or `\AA,`. If you use a backslash in front of a period or a comma, [it becomes a space](https://texblog.org/2014/04/09/whitespace-in-math-mode)
- Sometimes a period does not denote the end of a sentence. In this case, we need to use a backslash following the period, otherwise the space would be too wide, e.g.,
	- `Ref.\ [34]`
	- `Barack H.\ Obama II`
	- `Fig.\ [2]`
	- `Wang et al.\ [17]`
	- `Grant No.\ 123456`
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
- To create angular brackets in math mode, write `$\left<110\right>$` or `$\langle 110\rangle$` instead of `$<110>$` which renders less-than and greater-than signs. Note: `<` and `>` only works in math mode.
- Pay attention to [special character(s)](https://en.wikibooks.org/wiki/LaTeX/Special_Characters) in people's names, e.g., `Schr\"{o}dinger` instead of `Schrodinger`.
- There are two main citation styles: numberic and author-year:
	- The author-year style will take care of the authors' names automatically, regardless of how many authors there are. But for the numerical style, you need to explicitly write the authors' names, if presenting the names is desirable. Use their last names only. Note that some last names have more than one word, e.g., de Koning, van Gogh, Van der Ven, Van de Walle, and D&#237;az de la Rubia. When there is one author, e.g., King, write `King [34] has a dream`. When there are two authors, e.g., Lewis and Clark, write `Lewis and Clark [44] returned to St. Louis on September 23, 1806`. When there are more than two authors, e.g., Weiss, Barish, and Thorne, write `Weiss et al. [54] won the 2017 Nobel Prize in Physics`.
	- With the numberic style, add the citation at the end of the sentence, e.g., `I have a dream \cite{king1963}.` which would render `I have a dream [34].` An exception is when the author name is at the beginning of a sentence, e.g., `King \cite{king1963} has a dream` which renders `King [34] has a dream`. Sometimes the citation is a superscript, e.g., `I have a dream \cite{king1963}` becomes <code>I have a dream<sup>34</sup>.</code> In some cases, the superscript may be confused with the exponent, e.g., `2 \cite{obama2008}` would render <code>2<sup>35</sup></code>. In some other cases, the superscript is not desirable, e.g., `our results are compared against those in Ref.\ \cite{obama2008}` would render <code>our results are compared against thost in Ref.<sup>35</sup></code>. In these cases, write `2 [\citenum{obama2008}]` and `our results are compared against those in Ref.\ \citenum{obama2008}`, which would render `2 [35]` and `our results are compared against those in Ref. 35`, respectively.
	- With the author-year style, add the citation at the end of the sentence too, e.g., `I have a dream \citep{king1963}` which would render `I have a dream (King, 1963)`. Do not write `I have a dream \cite{king1963}` which would render `I have a dream King (1963)`. However, if the author name is at the beginning of a sentence, write `\cite{king1963} has a dream` which would render `King (1963) has a dream`. Do not write `\citep{king1963} has a dream` which would render `(King, 1963) has a dream`.

## Figures

Say that you are writing a paper A for journal B and you want to use a figure that is modified or taken directly from a paper C in journal D. You should cite paper C and add a few words such as `Reproduced with permission from Ref. [C]`. Refer to the published work or instructions in journal B for the exact words. In addition, obtain the permission from the copyrights holder of that figure, which is mostly like the publisher of journal D, to reuse the figure. Here are [guidelines from Elsevier](https://www.elsevier.com/about/policies/copyright/permissions). Other publishers have their own guidelines.

There may be some scenarios in which you do not need to obtain permission. For example, the image or figure has been substantially modified. In this case, you still need to cite journal D. However, if you use a TEM or SEM image or photo, you need to obtain permission from the copyrights holder even if you add in the caption that the image has been modified.

## Reference list

The reference style differs greatly among journals. Read their instructions carefully. In LaTeX, there are [two main ways to manage the reference list](https://www.overleaf.com/learn/latex/bibliography_management_with_bibtex): BibTeX and non-BibTeX. I strongly recommend the former. With BibTeX, simply write these two lines at the end of the paper (but before `\end{document}`):

- `\bibliographystyle{unsrt}`
- `\bibliography{ref}`

which would require two files: `unsrt.bst` and `ref.bib`. Most likely the first file is provided by the journal. In practice, however, Overleaf can retrieve a lot of `.bst` files from its server, so you may only need to provide the file `ref.bib`.

If you want to cite a paper, e.g., [this one](http://dx.doi.org/10.1016/j.actamat.2019.05.030), click on `Export`, then choose `Export citation to BibTeX`. Then you will get a `.bib` file. Open it, copy its content, and add it to your `ref.bib` file. Then in your main text, write `\cite{XU2019160}` to cite it. Do this for all other references to cite all of them.

Alternatively, use [reference management software](https://en.wikipedia.org/wiki/Comparison_of_reference_management_software). I use [Zotero](https://en.wikipedia.org/wiki/Zotero). Go to [its website](https://www.zotero.org/download/) and install Zotero and Zotero Connector. When you read a paper in your browser and want to cite it, [use the Zotero Connector](https://www.zotero.org/support/adding_items_to_zotero) to add the bibliographic information to Zotero, which should be already open. Read [this page](https://www.zotero.org/support/quick_start_guide) for more on Zotero. Then, in Zotero, select entries you want to export, right-click on them, choose `Export Items`, change Format to `BibTeX`, select `Use Journal Abbreviation`, then click on `OK`. The entries will be exported to a local `.bib` file. Again, open it and copy & add its content to your `ref.bib` file.

Double check the reference list for typos as if it were the main text. Pay attention to these :

- Write `$\left<110\right>$` and `\{110\}` instead of `<110>` and `{110}`.
- Write `dislocations in Mo` and `dilute Mg-based alloys` instead of `dislocations in mo` and `dilute mg-based alloys`. Unfortunately, in the article title, most BibTeX style automatically converts all uppercase letters to lowercase ones, except the very first letter. To enforce the usage of uppercase letters, add curly brakets around certain words/letters in your `.bib` file, e.g., `dislocations in {Mo}` or `dislocations in {M}o`.
- Use special character(s) in authors' names, if any.
- When necessary, use math mode, e.g., `($\bar{1}10$)` instead of `(-110)`.
- In most cases, use abbreviated jouranl names, e.g., `Acta Mater.` instead of the full journal name, i.e., `Acta Materialia`.  Check [this webpage](https://woodward.library.ubc.ca/research-help/journal-abbreviations/) for the correct abbreviated journal names. Omit all articles (a, an, the) and prepositions (e.g., at, in, of, for, with). Also capitalize the first letter of each word. For example, write `J. Chem. Phys.`, instead of `The J. of Chem. Phys.` or `J. chem. phys.`  

