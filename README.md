Context Matters
===============

This repository hosts multiple submodules.


## Quickstart

Clone this repo, cd into it and run a submodule init followed by update to pull
all the subrepos:

```
git clone https://github.com/bayer-science-for-a-better-life/context-matters.git
cd context-matters
git submodule init
git submodule update
```


To create an environment with the correct dependencies
for the submodules run:

```
conda env create -f environment-local.yml
```

Setup upstreams for all sub-repos correctly:

```
cd grakn-pytorch-example
git checkout main
cd ../grakn-pytorch-geometric
git checkout main
cd ../kglib
git checkout master
```

This is just for local development with CPU, because context matters.