---
title: 'Keeping references in order with BibTeX'
summary: Why formatting a bibliography by hand is a losing game, and what to use instead.
date: 2026-08-20
authors:
  - me
tags:
  - Bibliography
  - LaTeX
  - Tools
---

My first school-style bibliography was five sources typed by hand at the bottom of a document. When a teacher asked me to add one source in the middle, I renumbered everything manually and got two citations wrong. That's the entire case for bibliography managers, told in one sentence.

The core idea: keep information about sources separate from the text. In the BibTeX format, each source is a small structured record in a `.bib` file:

```bibtex
@book{knuth1984,
  author    = {Donald E. Knuth},
  title     = {The {TeX}book},
  publisher = {Addison-Wesley},
  year      = {1984}
}
```

In the text you write only the key, `\cite{knuth1984}`, and LaTeX assembles the reference list itself: numbered, sorted and formatted in whatever style the venue requires. Add a source, remove a source, reorder chapters, and the numbering just stays correct. The renumbering problem I had at school simply cannot happen.

Styles matter more than I expected. The same book can be cited in APA style, IEEE style or the Russian GOST style, and they all look different in fussy little ways: initials before or after the surname, year in parentheses or not, italics here or there. Doing this by hand for thirty sources is a job for a robot. With a `.bib` file, changing style is one line.

Where do the records come from? Mostly not from typing. Google Scholar has a "cite" button that gives you ready BibTeX. Reference managers like Mendeley and Zotero go further: they store your PDF library, pull metadata automatically and export the `.bib` file. I've started keeping course papers in Mendeley, less because I have a huge library and more because I'd rather build the habit now, while the library is small.

For a first-year student this may look premature. But every coursework ends with a reference list, mine is due in December, and I'd rather fight LaTeX once in September than fight numbering forever.
