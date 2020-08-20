# SCAtutorial
Supportnig material for the manuscript: 
Sparsely-Connected Autoencoder (SCA) for single cell RNAseq data mining
Alessandri L, Cordero F, Beccuti M, Licheri N, Arigoni M, Olivero M, Di Renzo F, Sapino A and Calogero RA

# Introduction

This vignette provides support to use Sparsely-Connected Autoencoder (SCA) in the analysis of single cell RNAseq data (scRNAseq).
SCA analysis was added as extention of [*rCASC*](https://pubmed.ncbi.nlm.nih.gov/31494672/).


## Installation

An extensive description of how rCASC works is provided at [*rCASC* vignette](https://kendomaniac.github.io/rCASC/articles/rCASC_vignette.html). Installation of rCASC including the SCA modules requires:

- A workstation/server running 64 bits Linux.

- Docker daemon installed on the machine, for more info see this document:

    [*https://docs.docker.com/engine/install/*](https://docs.docker.com/engine/install/).

- The functions in rCASC package require that user belongs to a group with the rights to execute docker. See the following document for more info: 

    [*https://docs.docker.com/engine/install/linux-postinstall/*](https://docs.docker.com/engine/install/linux-postinstall/)


To install the SCAtutorial in an R session write:

```
install.packages("devtools")
library(devtools)
install_github("kendomaniac/SCAtutorial", ref="master")

```
Then, after package installation execute in R:
```
library(SCAtutorial)
installing.rcasc()
library(rCASC)
downloadContainers(group="docker", containers.file="sca")
```

## web site

The vignette of the SCAtutorial can be also at [**vignette**](https://kendomaniac.github.io/SCAtutorial/articles/SCAvignette.html)



