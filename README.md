## Drat usage within the Platypus package

This repository is a fork of the template repository drat by Roman Hornung and Dirk Eddelbuettel.
Following the vignette here (https://eddelbuettel.github.io/drat/vignettes/dratstepbystep/) it contains tarballs of the packages SeuratWrappers (satijalab/seurat-wrappers), ProjecTILs (carmonalab/ProjecTILs) and monocle3 (cole-trapnell-lab/monocle3)
Using the Additional_repositories in the DESCRIPION of Platypus, we are able to use these packages within the newest CRAN release of Platypus, even though these packages are not available in any mainstream repository.
!!! The tarballs in this repo where compiled from the git repos of all packages on 07.08.22 and not updated since. 
We do not plan to update this repo with new builds of each package regulary. To install any of the three packages, please fetch the newest version on their respective Git repos !!!

Big thanks to Roman Hornung and Dirk Eddelbuettel for making this available as well as to the Satja, Carmona and Trapnell labs! 


## `drat` Repository for easy forking

`drat` ([CRAN](https://cran.r-project.org/package=drat), [GitHub](https://github.com/eddelbuettel/drat), [docs](https://eddelbuettel.github.io/drat)) makes it easy to host your own
CRAN-like repositories for packages (or [data](https://journal.r-project.org/archive/2017/RJ-2017-026/index.html)).

Many users have started their own `drat` repo by forking the original [GitHub
repo](https://github.com/eddelbuettel/drat) -- but as time passes this _code_ repo
accumulates more _code_ for `drat`, as well as
[documentation](https://eddelbuettel.github.io/drat)
 making it less of an ideal place to start for _your own_ repo.  So this repo offers an alternative:

- Just fork this repo into your own domain, and you have a working `drat`
 repo.
- Enable [GitHub Pages](https://docs.github.com/en/github/working-with-github-pages)
 with the `docs/` folder in the main branch:

 ![](https://github.blog/wp-content/uploads/2016/08/47c2ecc4-6533-11e6-828a-91980daa7297.gif)

Note, however, that you currently **must** use the `drat` package directly
from its [GitHub repo](https://github.com/eddelbuettel/drat) in order to use
GitHub Pages off `docs/` in the main branch---and you need to enable this,
e.g. via `options(dratBranch="docs")` as the _released_ version only supports
a `gh-pages` branch.  So in a sense this repo is currently "experimental" as
is the support in the not-yet-released `drat` version.

This repo was initiated (using command `dratPackage()`) with the source and
windows binary of the last CRAN release of `drat`. You can delete either or
both (for example via command `pruneRepo()`) and then
add your own (via `insertPackage()`). 

### Author

Dirk Eddelbuettel

### License

GPL (>= 2)
