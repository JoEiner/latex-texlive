# latex-texlive
Docker container with full latex texlive distribution based on Debian 8 (jessie). Fork of https://github.com/schickling/dockerfiles/tree/master/latex

## Usage
```sh
$ docker run --rm -it -v $(pwd):/source joeiner/latex-texlive
```
Mount your local source folder to the container and run it inside the container.

#### Compiling a latex document
```sh
$ pdflatex my-document.tex
```

#### Compiling a xetex document
```sh
$ xelatex my-document.xtx
```
