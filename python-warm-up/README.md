# python-warm-up
This repository hosts the teaching materials for python coding warm-up in the [UvA Data Science course](https://multix.io/data-science-book-uva/).

All the content in this repository is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

Credit: this teaching material is created by [Yen-Chia Hsu](https://github.com/yenchiah).

## Build this book

Below are the steps to update and build this book. First, clone this repository to your local machine. Assume that you already have [miniconda](https://docs.conda.io/en/main/miniconda.html) installed. Next, install the jupyter-book package:
```sh
$ conda create -n jupyterbook
$ conda activate jupyterbook
$ conda install python
$ pip install -U jupyter-book
$ pip install -U ghp-import
$ jupyter-book --help
```
Then, clone this repository and build the book:
```sh
$ git clone https://github.com/MultiX-Amsterdam/python-warm-up
$ cd python-warm-up
$ jupyter-book build .
```
To rebuild the entire book, use the following:
```sh
$ jupyter-book build --all .
```
Once it is done, you can view the book in the [html content](_build/html) folder using a web browser. To update the book online in this GitHub repository (in the gh-pages branch), run the following:
```sh
$ ghp-import -n -p -f _build/html
```
The above steps will update the gh-pages branch, which hosts the website. Finally, follow the normal git flow to commit the changes and push the code to the main branch in this repository.