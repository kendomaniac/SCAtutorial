# SCAtutorial
Supportnig material for the manuscript: 
Sparsely-Connected Autoencoder (SCA) for single cell RNAseq data mining
Alessandri L, Cordero F, Beccuti M, Licheri N, Arigoni M, Olivero M, Di Renzo F, Sapino A and Calogero RA

# Introduction

This vignette provides support to use Sparsely-Connected Autoencoder (SCA) in the analysis of single cell RNAseq data (scRNAseq).
SCA analysis was added as extention of [*rCASC*](https://pubmed.ncbi.nlm.nih.gov/31494672/).


## Installation

To simplify usage and to guarantee reproducibility the tools required for the SCA workflow are embedded in docker containers stored at docker.io/repbioinfo. For more info on the computational approaches used in SCAtutorial please see [*Kulkarni et al. BMC Bioinformatics 2018*](https://pubmed.ncbi.nlm.nih.gov/30367595/)

An extensive description of how rCASC works is provided at [*rCASC* vignette](https://kendomaniac.github.io/rCASC/articles/rCASC_vignette.html). Installation of rCASC including the SCA modules requires:

- A workstation/server running 64 bits Linux.

- Docker daemon installed on the machine, for more info see this document:

    [*https://docs.docker.com/engine/install/*](https://docs.docker.com/engine/install/).

- The functions in rCASC package require that user belongs to a group with the rights to execute docker. See the following document for more info: 

    [*https://docs.docker.com/engine/install/linux-postinstall/*](https://docs.docker.com/engine/install/linux-postinstall/)


To install the SCAtutorial, write in an R session:

```
install.packages("devtools")
library(devtools)
install_github("kendomaniac/SCAtutorial", ref="master")

```
Then, after package installation, execute in R:
```
library(SCAtutorial)
#check if docker daemon is  running and install rCASC package from github.
installing.rcasc()
```

This step checks that dockert daemon is running and downloads the dockert containers required for the tutorial. It might require sometime, between minutes to hours, depending on the available internet bandwidth.


## Web site

The vignette of the SCAtutorial is available at [**vignette**](https://kendomaniac.github.io/SCAtutorial/articles/SCAvignette.html)

The vignette is located in the folder *SCAtutorial/docs/articles*. The data produced by the building of the vignette using the command:

```
pkgdown::build_site()

```
 are instead located in *SCAtutorial/vignettes/setA* folder.

