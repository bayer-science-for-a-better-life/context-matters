Context Matters
===============


## :bangbang: Disclaimer:
These ideas have made it into **TypeDB ML** by now. Please Use that.
https://github.com/vaticle/typedb-ml
https://blog.vaticle.com/link-prediction-knowledge-graph-pytorch-geometric-f35917320806

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

update env (while having context-matters active):

```
conda env update -f environment-local.yml --prune
```

Setup upstreams for all sub-repos correctly:

```
cd typedb-pytorch-example
git checkout main
cd ../grakn-pytorch-geometric
git checkout main
cd ../kglib
git checkout master
```

This is just for local development with CPU, because context matters.