# latex-texlive
Docker container with full latex texlive distribution based on Debian 8 (jessie). Fork of https://github.com/schickling/dockerfiles/tree/master/latex

## Usage
```sh
$ docker run --rm -it -v $(pwd):/source joeiner/latex-texlive
```
Mount your local source folder to the container and run it inside the container.

#### Compiling a latex document
From inside the container:
```sh
$ pdflatex my-document.tex
```
From the host OS:
```sh
$ docker run --rm -it -v $(pwd):/source joeiner/latex-texlive pdflatex my-document.tex
```

#### Compiling a xetex document
From inside the container:
```sh
$ xelatex my-document.xtx
```

From the host OS:
```sh
$ docker run --rm -it -v $(pwd):/source joeiner/latex-texlive xelatex my-document.tex
```

#### Compiling with a build script
From inside the container:
```sh
$ ./my-build-script.sh
```

From the host OS:
```sh
$ docker run --rm -it -v $(pwd):/source joeiner/latex-texlive ./my-build-script.sh
```
