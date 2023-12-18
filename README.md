# Programming and Experiments Repository

This repository is a collection of articles, research papers and experiments.

## Getting Started

To explore the content in this repository, clone it to your local machine:

```bash
git clone https://github.com/artem-burashnikov/articles.git
```

## How to use

* Recommended method: online tools such as [Overleaf](https://www.overleaf.com/) or [Papeeria](https://papeeria.com/)
* Upload the template files to your project, preserving the folder structure.
Choose XeTeX (or LuaTeX) as the compiler (for example, in Overleaf, go to Menu -> Compiler).
* Alternative method: install TeX locally on your machine (for example, [TeXLive](https://www.tug.org/texlive/))


## Building

If you are using a local TeX compiler, then simply navigate to a folder and use the command:
```sh
make
```

`make` can also be used with `clean` и `dist-clean` optional arguments.

`clean` deletes temporary files, `dist-clean` will also clean an output pdf.


### Additional notes

* A few external packages are required. Use `make depext` to install them (if you use local TeX distribution. No action is needed if you use online editors)
* File `ugost2008ls.bst` was adopted from [here](https://github.com/anlun/Russian-Phd-LaTeX-Dissertation-Template/tree/master/BibTeX-Styles) because original one from APT package `texlive-lang-cyrillic` gives a weird error:

    ```sh
    bibtex "\" can't start a style-file command- ...
    ```

