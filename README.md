bookdown-equations, Convert LaTeX equation labels to bookdown compatible labels
==================================================================

[![GitHub build status][CI badge]][CI workflow]

bookdown-equations, Pandoc Lua filter for Converting LaTeX equation labels to [Bookdown Style equation labels](https://bookdown.org/yihui/bookdown/markdown-extensions-by-bookdown.html) in MathJax environment.
This filter also updates the equation references to [bookdown style references](https://bookdown.org/yihui/bookdown/markdown-extensions-by-bookdown.html).


[CI badge]: https://img.shields.io/github/workflow/status/Abhi-1U/bookdown-equations/CI?logo=github
[CI workflow]: https://github.com/Abhi-1U/bookdown-equations/actions/workflows/ci.yaml


Usage
------------------------------------------------------------------

LaTeX --> Markdown/R-markdown

The filter modifies the internal document representation to bookdown specified labelling/numbering
system. Hence it will work with documentation formats using [bookdown](https://bookdown.org/).

### Plain pandoc

Pass the filter to pandoc via the `--lua-filter` (or `-L`) command
line option.

    pandoc --lua-filter bookdown-equations.lua ...



License
------------------------------------------------------------------

This pandoc Lua filter is published under the MIT license, see
file `LICENSE` for details.
