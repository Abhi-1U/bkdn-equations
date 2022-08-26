bookdown-equations, Convert LaTeX equation labels to bookdown compatible labels
==================================================================

[![GitHub build status][CI badge]][CI workflow]
[![GitHub Workflow Status][pages badge]][pages workflow]
[![Pandoc Version][Pandoc badge]][pandoc]
[![Lua Filter][Lua Filter]][Main Filter]
[![MIT][License]][License URL]

bookdown-equations, is a Pandoc Lua filter for Converting LaTeX equation labels to [Bookdown Style equation labels](https://bookdown.org/yihui/bookdown/markdown-extensions-by-bookdown.html) in MathJax environment.
This filter also updates the equation references to [bookdown style references](https://bookdown.org/yihui/bookdown/markdown-extensions-by-bookdown.html).

[pages badge]: https://img.shields.io/github/workflow/status/Abhi-1U/bookdown-equations/Publish%20Website?label=Pages&logo=github&style=for-the-badge
[pages workflow]: https://github.com/Abhi-1U/bookdown-equations/blob/main/.github/workflows/website.yml
[CI badge]: https://img.shields.io/github/workflow/status/Abhi-1U/bookdown-equations/CI?logo=github&style=for-the-badge
[CI workflow]: https://github.com/Abhi-1U/bookdown-equations/actions/workflows/ci.yaml
[pandoc]: https://pandoc.org/index.html
[Pandoc badge]: https://img.shields.io/badge/pandoc-2.9+-red?style=for-the-badge&logo=haskell
[Lua Filter]: https://img.shields.io/badge/lua-filter-darkblue?style=for-the-badge&logo=lua
[License]: https://img.shields.io/badge/license-MIT-black?style=for-the-badge
[License URL]: https://github.com/Abhi-1U/bookdown-equations/blob/main/LICENSE
[Main Filter]: https://github.com/Abhi-1U/bookdown-equations/blob/main/bookdown-equations.lua
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
