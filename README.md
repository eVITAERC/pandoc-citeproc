Scholdoc-Citeproc
=================

### A fork of [Pandoc-Citeproc][pandoc-citeproc] for [Scholdoc][scholdoc]

**Current stable version:** 0.6

**Development build status** [![build status][scholarly-devel-travisimage]][travis_stat]  
**Stable build status** [![build status][scholarly-travisimage]][travis_stat]

This package is a fork of [Pandoc-Citeproc][pandoc-citeproc]. It is intended to
support the development of [Scholdoc][scholdoc], a fork of [Pandoc][pandoc]
that understands [ScholarlyMarkdown][scholmd]. It is mean to be used as a
filter with [Scholdoc][scholdoc] to resolve and format citations using a
bibliography file and a [CSL stylesheet][csl]. It can also be used (with
`--bib2yaml` or `--bib2json` options) to convert a bibliography to a YAML
format that can be put directly into a ScholarlyMarkdown document or to CSL
JSON. Bibliographies can be in any of several formats, but BibTeX/BibLaTeX
`.bib` database files are the best supported. For more information, consult the
original README file of `pandoc-citeproc`, which is moved to
[`README-pandoc-citeproc.md`][citeproc-readme-blob].

`scholdoc-citeproc` is currently just a trivial fork just so it can compile
against [Scholdoc-Types][scholdoc-types] and [Scholdoc][scholdoc] instead of
[Pandoc-Types][pandoc-types] and [Pandoc][pandoc], without polluting the
`pandoc-citeproc` package and executable namespace on the user's system. In the
future, enhancements and modifications made as part of the [Scholdoc][scholdoc]
project will be introduced here first.

The version number of this package is kept in sync with [pandoc-citeproc].

[scholmd]: http://scholarlymarkdown.com
[scholdoc]: https://github.com/timtylin/scholdoc
[scholdoc-types]: https://github.com/timtylin/scholdoc-types
[pandoc]: http://johnmacfarlane.net/pandoc/
[pandoc-types]: https://github.com/jgm/pandoc-types
[pandoc-citeproc]: https://github.com/jgm/pandoc-citeproc
[travis_stat]: https://travis-ci.org/timtylin/scholdoc-citeproc
[scholarly-devel-travisimage]: https://travis-ci.org/timtylin/scholdoc-citeproc.svg?branch=master
[scholarly-travisimage]: https://travis-ci.org/timtylin/scholdoc-citeproc.svg?branch=stable
[citeproc-readme-blob]: https://github.com/timtylin/scholdoc-citeproc/blob/master/README-pandoc-citeproc
[csl]: http://citationstyles.org
