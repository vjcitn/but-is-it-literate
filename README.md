# but-is-it-literate

## historical reflection on the literature of literate statistical computing

A [2001 paper in CHANCE](https://amstat.tandfonline.com/doi/abs/10.1080/09332480.2001.10542284#.W6uA-hNKh0s) described the use of
[noweb](https://www.cs.tufts.edu/~nr/noweb/) for literate
statistical software development.

It was just literate programming applied to programming
for a simple simulation task.

This predated Sweave but not by much.  See [Leisch 2002](https://cran.r-project.org/doc/Rnews/Rnews_2002-3.pdf), and its reference to work by
Tony Rossini.

## purpose of this repo

The CHANCE paper is not readily available.  The noweb
associated with the paper goes beyond defining a function.
It demonstrates how a complete checkable package can be defined
in a single noweb file.  

With a proper installation of noweb, the following commands
generate a very lightly modified HTML version of the paper:
```
notangle -t8 -R"AdminMakefile" Rpack.nw > AdminMakefile
make -f AdminMakefile Rpack.html
```

The following commands create and check the package.
```
notangle -t8 -R"AdminMakefile" Rpack.nw > AdminMakefile
make -f AdminMakefile package
```


## real use of noweb in statistical software development

Extensive use of noweb in advanced R software development
is found at Luke Tierney's [software projects site](http://homepage.divms.uiowa.edu/~luke/R/regexp.html).  Here the

![](first.png)
![](mid1.png)
![](mid2.png)
![](last.png)
