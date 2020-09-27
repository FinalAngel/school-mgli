# mgli

You need to save the `template.tex` file to regenerate the PDF. You can open the intergrated PDF Viewer from VSCode to see live updates.

## Installation

- Install a LaTeX distribution like [TeX Live](https://www.tug.org/texlive/)
- Install [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) for VSCode
- You may need to install [Latexmk](https://mg.readthedocs.io/latexmk.html)

You should be able to run `tlmgr` commands in your terminal if everything
is installed correctly.

### MacOS instruction

As I'm using MacOS as my primary system, I documented my installation procedure:

- `brew cask install mactex`
- make sure `"/usr/local/texlive/2020/bin/x86_64-darwin"` is in PATH and reload the Terminal
- `sudo tlmgr option repository ctan`
- `sudo tlmgr update --self`
- `sudo tlmgr install latexmk`
- `sudo tlmgr install latexindent`
- `sudo tlmgr install chktex`
- `code --install-extension James-Yu.latex-workshop`

I still get **Formatting failed** warnings when saving, even though the output
log shows no errors. Something to fix at some point ¯\\\_(ツ)\_/¯.
