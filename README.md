[![Build Status](https://travis-ci.org/augusto-garcia/onemap.svg?branch=master)](https://travis-ci.org/augusto-garcia/onemap) [![Development](https://img.shields.io/badge/development-active-blue.svg)](https://img.shields.io/badge/development-active-blue.svg)

<!-- [![Build Status](https://travis-ci.org/mmollina/onemap.svg?branch=master)](https://travis-ci.org/mmollina/onemap) -->

# OneMap

`OneMap` is a software for constructing genetic maps in experimental
crosses: full-sib, RILs, F2 and backcrosses. It was developed by
Gabriel R A Margarido, Marcelo Mollinari and A Augusto F Garcia. Later on, Rodrigo R Amadeu and Cristiane H Taniguti joined the project.

It has been available on CRAN for several years
(http://cran.r-project.org/web/packages/onemap/index.html). Its last
version was updated on 2017-10-18. CRAN has OneMap's stable version,
which is recommended for most users.

This github page has its version under development. New functions will
be added (experimental work) and, once it is done, we will synchronize
the repositories and add it to CRAN.

We are working very hard to release a new stable version allowing
users to analyze data sets with markers based on sequencing
technologies, such as Illumina, GBS, etc.

`OneMap` comprises a set of functions that allows users to build a
linkage map. Some functions are used internally by the package, and
should not be used directly.

# How to install

## From CRAN (stable version)

It is easy, just type (within R):

```R
setRepositories(ind = 1:2)
install.packages("onemap", dependencies=TRUE)
```

Some Linux users reported the error message below:

```R
ERROR: dependency ‘tkrplot’ is not available for package ‘onemap’
```

To fix it, in a terminal (outside R), install `r-cran-tkrplot`:

```R
sudo apt-get install r-cran-tkrplot
```

Then, go back to `R` and install `OneMap` as mentioned above.

You also can use the console menus: _Packages -> Install
package(s)_. After clicking, a box will pop-up asking you to choose
the CRAN mirror. Choose the location nearest to you. Then, another box
will pop-up asking you to choose the package you want to install.
Select _onemap_ then click _OK_. The package will be
automatically installed on your computer.

`OneMap` can also be installed by downloading the appropriate files
directly at the CRAN web site and following the instructions given in
the section `6.3 Installing Packages` of the
[R Installation and Administration](http://cran.r-project.org/doc/manuals/R-admin.pdf)
manual.

## From github (version under development)

Within R, you need to install and load the package `devtools`:

```R
install.packages("devtools")
library(devtools)
```

This will allow you to automatically build and install packages from
github. If you use Windows, first install
[Rtools](https://cran.r-project.org/bin/windows/Rtools/). If you are facing problems with Rtools installation, try to do it by selecting *Run as Admnistrator* option with right mouse button. On a Mac,
you will need Xcode (available on the App Store). On Linux, you may need to install `r-cran-tkrplot` (see above).

Then, to install `OneMap` from github (this very repo):

```R
install_github("augusto-garcia/onemap")
```

# Tutorials

You can read _OneMap_ tutorials going to the vignettes of the
installed package, or clicking below. Please, start with the overview,
that will guide you through other chapters.

1. [Overview](http://augusto-garcia.github.io/onemap/vignettes_highres/Overview.html)

2. [Introduction to R](http://augusto-garcia.github.io/onemap/vignettes_highres/Introduction_R.html)

3. [How to build a linkage map for inbred-bases populations (F2, RIL and BC)](http://augusto-garcia.github.io/onemap/vignettes_highres/Inbred_Based_Populations.html)

4. [How to build a linkage map for outcrossing populations](http://augusto-garcia.github.io/onemap/vignettes_highres/Outcrossing_Populations.html)
