### Docoment once, include anywhere

 * When writing a note, report, manual, etc., do you find it difficult to choose the typesetting format? That is, to choose between plain (email-like) text, wiki, MS Word or OpenOffice, LaTeX, HTML, reStructuredText, Sphinx, XML, Markdown, etc.? Would it be convenient to start with some very simple text-like format that easily converts to the formats listed above?

 * Do you find it problematic that you have the same information scattered around in different documents in different typesetting formats? Would it be a good idea to write things once, in one place, and include anywhere?

You should take a look at Doconce if any of these questions are of interest.

*Users are strongly encouraged to use the most recent software in the [GitHub repository](https://github.com/hplgit/doconce) and not the tarballs!*

### Highlights

 * Minimally tagged markup language (like Markdown) with strong support for small and large scale projects involving much math and code in the text.

 * For documents with math and code, you can generate clean plain LaTeX (PDF), HTML (with MathJax and pygments - embedded in your own templates), Sphinx for nice web layouts, Markdown, IPython notebooks, HTML for Google or Wordpress blogging, and MediaWiki. LaTeX output is in the ptex2tex format for very flexible typesetting of computer code. Doconce can output other formats (with no support for nicely typeset math and code): plain untagged text, Google wiki, Creole wiki, and reStructuredText. From Markdown or reStructuredText you can go to XML, DocBook, MS Word, and many other formats.

 * The document source is first preprocessed by preprocess and mako, which gives you full programming capabilities in the text. For example, with mako it is easy to write a book with all computer code examples in both Matlab and Python, and you determine at compile time of the Doconce document whether the book features Matlab or Python.

 * Doconce extends Sphinx, Markdown, and MediaWiki output such that LaTeX align environments with labels work for systems of equations.

 * One source for the text can be used for different media: traditional books, ebooks in PDF, ebooks in PDF for phones, ebooks in HTML with various layouts, and blogs.

 * Doconce makes it very easy to write slides with nice math and code. Both LaTeX Beamer and HTML5 slides (reveal.js and deck.js) are supported. Slide elements can be arranged in cells to easily control the layout.

### Installation

Doconce is a pure Python package and installed by


```Bash
Terminal> sudo python setup.py install

```

However, Doconce has *a lot* of dependencies, depending on what type of
formats you want to work with. On Debian/Ubuntu it is fairly straightforward
to get the packages you need. See the [Installation Guide](http://hplgit.github.io/doconce/doc/pub/manual/html/manual.html#installation-of-doconce-and-its-dependencies) for
details.

### Demo

A [short scientific report](http://hplgit.github.io/teamods/writing_reports/index.html) demonstrates the many formats that Doconce can generate and
how mathematics and computer code look like.

<!-- Note: local links does not work since this README file is a source -->
<!-- code file and not part of the published gh-pages. Use full URL. -->

There is also a demo of how Doconce can
be used to [create slides](http://hplgit.github.io/doconce/doc/pub/slides/demo/index.html) in various formats.

### Documentation

 * Tutorial: [Sphinx](http://hplgit.github.io/doconce/doc/pub/tutorial/html/index.html),
   [HTML](http://hplgit.github.io/doconce/doc/pub/tutorial/tutorial.html),
   [PDF](http://hplgit.github.io/doconce/doc/pub/tutorial/tutorial.pdf)

 * Manual: [Sphinx](http://hplgit.github.io/doconce/doc/pub/manual/html/index.html),
   [HTML](http://hplgit.github.io/doconce/doc/pub/manual/manual.html),
   [PDF](http://hplgit.github.io/doconce/doc/pub/manual/manual.pdf)

 * Quick Reference: [Sphinx](http://hplgit.github.io/doconce/doc/pub/quickref/html/index.html),
   [HTML](http://hplgit.github.io/doconce/doc/pub/quickref/quickref.html),
   [PDF](http://hplgit.github.io/doconce/doc/pub/quickref/quickref.pdf)

### License

Doconce is licensed under the BSD license, see the included LICENSE file.

The files `doc/manual/figs/streamtubes.*` and
`doc/manual/figs/wavepacket.*` was made by the Doconce author and is
released under the same conditions as doconce.

The file `doc/manual/figs/mjolnir.mpeg` was made by Dr. Sylfest
Glimsdal, University of Oslo and is, with his permission, released
under the same conditions as doconce.

