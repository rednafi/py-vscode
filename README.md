<div align="center">

# How to Python in VS Code 🦄

## An Opinionated Guide

<img src="/ext/logo.png" width="900" height="600">
</div>

Read the free guide at [py-vscode.readthedocs.io](py-vscode.readthedocs.io)

**This is an ongoing work. We need contributors. Specially, if are doing python with VS Code in MacOS and want to contribute, please hit me up in `redowan.nafi@gmail.com`.**

## Contribution Guidelines
* This guideline has been made with [Sphinx](http://www.sphinx-doc.org/en/master/) and served with [Read The Docs](https://readthedocs.org/).

* The pages are written in `markdown.md` format and are located in `docs/files/` folder. If you want to make an edit (You're awesome 👍)

    * Clone the repo
    * Make your changes to the files in `docs/files/`
    * And send me a pull request

* If you want to extend/add new pages to the guideline (Whoa, thanks 🔥)
    * Clone the repo
    * Make add new `newfile.md` in `docs/files` folder
    * Write your contents in markdown format
    * Add the new section in `docs/index.rst` file
    * And send me a pull request

* If you want to build the website locally after making an edit (Please Breed 🔱)

    * Make a python environment, activate it and install the requirements via:
    ```python
    pip install -r requirements.txt
    ```
    * Make your changes according to the above guildelines
    * From the root directory, run:
    ```python
    sphinx-build -b html docs/ docs/_build
    ```
    * Navigate to `docs/_build/files` to find your newly built html pages. Open them in your browser for inspection.
    * If you are satisfied with your edits, send me a pull request.
