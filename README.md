# Elektrotechnik Fachschaft LaTeX Workshop

This repository contains the documentation for the introductory LaTeX workshop.

![TeXWorks Editor](pics/texworks.png)

Figure: Screenshot of TeXWorks under Linux with the sample document `samples/gauss-flux.tex`

## Goals

- Install LaTeX on your machine (ideally before the workshop takes place)
- Understand what is TeX, LaTeX, XeLaTeX, CTAN, etc.
- Learn the basics of LaTeX to typeset
    - Text documents
    - Mathematics
- Understand compiler errors
- Bibliography management
- Integration with version control / Write collaboratively
    - Contribute to https://github.com/HSR-Stud !

## Extras (if there is time)

- Create your own packages and classes
- Add source code listings
- Plots with pgfplots and
- Diagrams and figures with TikZ
- Diagrams with IPE

## Homeworks

### Try LaTeX without installing

You're not really convinced? Give LaTeX a try using a free online editor.
https://www.overleaf.com/project

### Install a TeX distribution

On the [Official Website](https://www.latex-project.org/get/#tex-distributions) of the LaTeX project there are always updated links to the various TeX Distributions. We recommend to pick one of these below depending on your operating system.

**Note: A full LaTeX distributions may need a few Gigabytes!** You should download and install this in advance before the seminar!
You _may_ also install a minimal version (such as TinyTeX), but beware that you may be missing some packages. Though most TeX distributions come with a package manager that will allow you to download some packages later.

**Note for Linux users:** You may install texlive through your package manager.
If you are using a Debian / Ubuntu derivate the `texlive` package should install most of what you need.

**Note for Windows users:** The default MikTeX installation only contains the minimal number of packages. MikTeX then offers a package management system to automatically downlad the missing packages as needed, but that means that your first document will take forever to compile. Be patient.

| Distrubition                   | OS                    | Homepage                              |
| ------------------------------ | --------------------- | ------------------------------------- |
| TeX Live                       | Linux                 | https://www.tug.org/texlive/          |
| MacTeX                         | MacOS                 | https://www.tug.org/mactex/index.html |
| MikTeX                         | Windows               | https://miktex.org/                   |
| TinyTex (feeling adventurous?) | Linux, MacOS, Windows | https://yihui.org/tinytex/            |

### Get a (La)TeX editor

_Note:_ Your TeX distribution may already include an editor (for ex. TeXShop for MacTeX).

| Name                     | Supported OS          | Homepage                                                           | PDF-Preview | Auto-completion | LSP     | Formatter | Spell-check | Free?                                           | Vim-mode |
| ------------------------ | --------------------- | ------------------------------------------------------------------ | ----------- | --------------- | ------- | --------- | ----------- | ----------------------------------------------- | -------- |
| (N)-Vim + vimtex         | macOS, Linux, Windows | [Click me](https://github.com/lervag/vimtex)                       | Yes \*2     | Yes \*5         | Yes \*5 | Yes \*5   | Yes \*6     | Yes                                             | Yes      |
| VS-Code + LaTeX-Workshop | macOS, Linux, Windows | [Click me](https://github.com/James-Yu/LaTeX-Workshop)             | Yes         | Yes             | Yes \*5 | Yes \*5   | Yes \*5 \*6 | Yes                                             | Yes \*5  |
| Intellij + TeXiFy-IDEA   | macOS, Linux, Windows | [Click me](https://hannah-sten.github.io/TeXiFy-IDEA/welcome.html) | Yes         | Yes             | Yes     | Yes       | Yes         | Yes                                             | Yes \*5  |
| Gummi                    | ⠀⠀⠀⠀⠀⠀⠀Linux          | [Click me](https://alexandervdm.github.io/gummi/)                  | Yes         | No              | No      | No        | Yes         | Yes                                             | No       |
| TeXstudio \*1            | macOS, Linux, Windows | [Click me](https://www.texstudio.org/)                             | Yes         | Yes             | No      | Yes \*5   | Yes \*6     | Yes                                             | No       |
| TeXworks                 | macOS, Linux, Windows | [Click me](https://www.tug.org/texworks/)                          | Yes         | No              | No      | No        | Yes         | Yes                                             | No       |
| Setzer                   | ⠀⠀⠀⠀⠀⠀⠀Linux          | [Click me](https://github.com/cvfosammmm/Setzer)                   | Yes         | Yes             | No      | No        | No          | Yes                                             | No       |
| Texifier                 | macOS                 | [Click me](https://www.texifier.com/)                              | Yes \*3     | Yes             | No      | No        | Yes         | No ([~30CHF](https://www.texifier.com/osx/buy)) | No       |
| TeXMaker                 | macOS, Linux, Windows | [Click me](https://www.xm1math.net/texmaker/)                      | Yes         | Yes             | No      | No        | Yes         | Yes                                             | No       |
| Compositor               | macOS                 | [Click me](https://compositorapp.com/)                             | Yes \*4     | No \*4          | No      | No        | ?           | No (~30CHF)                                     | No       |
| Overleaf                 | Online                | [Click me](https://www.overleaf.com/)                              | Yes         | Yes             | Yes     | No        | Yes         | Depends \*7                                     | Yes \*5  |

- **\*1**: It's essentially the successor to Texmaker.
- **\*2**: Works with an external PDF-viewer but supports features like "jumping back to the location in the code" and vice versa (unlike most others).
- **\*3**: Supports near real-time preview.
- **\*4**: The preview functions more like Obsidian's live preview (or a Word document?), allowing you to edit the rendered document directly.
- **\*5**: Requires configuration.
- **\*6**: Advanced spell-checking with Language Tool can be configured.
- **\*7**: Free for groups smaller than 3. For groups of 3 or more, it costs about [100 CHF](https://www.overleaf.com/user/subscription/plans?plan=student&period=annual) per year.

For those unsure which to choose, this answer found on [Reddit](https://www.reddit.com/r/LaTeX/comments/xu3yoi/texstudio_vs_texmaker/) may provide helpful guidance.

> The first question should always be "do you edit any other source?". If you program, you probably already have a favorite editor, and it probably has a LaTeX plugin. Use that.
>
> And even if you don't have a favorite editor, if you think you're likely to be picking programming up in the future (for instance of you're a first year engineering student), you'll anyway want to get comfortable in a general editor. Learning a specialized TeX editor is a waste of time in that case.
>
> If you decide to go that route, you then have to decide between a bare bones editor and an ide. Either will be fine, it's just a matter of running some command line commands and keeping a good (= non-adobe) pdf viewer open if you take the former.
>
> Personally, I use Vim, but if you don't already know it I don't recommend learning a lifestyle editor (Vim, Emacs, Ed, ...) at the same time as you're learning LaTeX.

Here is a (pretty old, but still relevant) comparison of various editors:
https://tex.stackexchange.com/questions/339/latex-editors-ides

## Looking for templates?

There are a lot of templates online, here's a few:

- [Mine (Naoki's)](https://github.com/NaoPross/Thesis)
- [Mimosis Thesis](https://github.com/Pseudomanifold/latex-mimosis)
- [Clean Thesis](http://cleanthesis.der-ric.de/)
- [Informatik OST Beamer template](https://github.com/ost-fh/Latex-Beamer-Theme)
- [Badertscher's OST beamer template](https://github.com/HBadertscher/OSTPresentation)

Of course on the internet there are a million other templates, however beware most although good looking may be messy to work with. Check that the source code is not spaghetti before using for the most important work you write at University!

- [Overleaf's LaTeX templates for theses](https://www.overleaf.com/latex/templates/tagged/thesis)

## Further readings and useful links

- [LaTeX tips and guidelines to avoid terrible typesetting (online)](https://github.com/HSR-Stud/Willkommen/blob/master/Guidelines.md)
- [Wikibooks LaTeX (online)](https://en.wikibooks.org/wiki/LaTeX#Contents)
- [Introduction to LaTeX (online)](https://web.mit.edu/rsi/www/pdfs/new-latex.pdf)
- [A not so short introduction to LaTeXe](references/lshort.pdf) ([online](https://tobi.oetiker.ch/lshort/lshort.pdf))
- [Detexify LaTeX handwritten symbols recognition (online)](http://detexify.kirelabs.org/classify.html)
- [LaTeX Mathematical Symbols (compact)](references/symbols-compact.pdf) ([online](https://www.caam.rice.edu/~heinken/latex/symbols.pdf))
- [A comprehensive LaTeX Symbol List](references/symbols-a4.pdf) ([online](http://tug.ctan.org/info/symbols/comprehensive/symbols-a4.pdf))
- [The LaTeX Font Catalogue (online)](https://www.tug.org/FontCatalogue/)
- _Advanced!_ [Graphics in LaTeX using TikZ (online)](https://www.tug.org/TUGboat/tb29-1/tb91walczak.pdf)
- _Advanced!_ [A very minimal introduction to TikZ (online)](http://cremeronline.com/LaTeX/minimaltikz.pdf)
- _Advanced!_ [CTAN Topic TikZ (online)](https://www.ctan.org/topic/pgf-tikz)
- _Advanced!_ [Manual for PGF and TikZ (online)](http://mirror.easyname.at/ctan/graphics/pgf/base/doc/pgfmanual.pdf)
- _Advanced!_ [Manual for Package PGFPLOTS (online)](http://mirror.easyname.at/ctan/graphics/pgf/contrib/pgfplots/doc/pgfplots.pdf)
- _Advanced!_ [Building a new LATEX document class is illustrated by developing a class forminutes of meetings (online)](http://tutex.tug.org/pracjourn/2005-4/hefferon/hefferon.pdf)
- _Advanced!_ [LaTeXe for class and package writers](references/clsguide.pdf) ([online](https://www.latex-project.org/help/documentation/clsguide.pdf))

## License

```
LaTeX-Workshop 2024 (c) by Naoki Pross

LaTeX-Workshop is licensed under a Creative Commons Attribution-ShareAlike 4.0
Unported License.

You should have received a copy of the license along with this
work.  If not, see <http://creativecommons.org/licenses/by-sa/4.0/>.
```
