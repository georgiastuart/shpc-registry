---
layout: container
name:  "quay.io/biocontainers/bioconductor-hpaanalyze"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hpaanalyze/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hpaanalyze/container.yaml"
updated_at: "2022-11-07 23:56:32.272347"
latest: "1.8.1--r40hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-hpaanalyze"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "1.8.1--r40hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-hpaanalyze"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hpaanalyze", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hpaanalyze", "latest": {"1.8.1--r40hdfd78af_0": "sha256:4c8fdffe67ecd8b389c9c584c2348e8c7c219e086a1d91c8a7449f0d843c7733"}, "tags": {"1.8.1--r40hdfd78af_0": "sha256:4c8fdffe67ecd8b389c9c584c2348e8c7c219e086a1d91c8a7449f0d843c7733"}, "docker": "quay.io/biocontainers/bioconductor-hpaanalyze", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hpaanalyze.
shpc-registry automated BioContainers addition for bioconductor-hpaanalyze
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hpaanalyze
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hpaanalyze:1.8.1--r40hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hpaanalyze/1.8.1--r40hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-hpaanalyze/1.8.1--r40hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hpaanalyze-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hpaanalyze-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hpaanalyze-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hpaanalyze-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hpaanalyze-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hpaanalyze-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### x86_64-conda-linux-gnu-gfortran.bin

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
```



In the above, the `<container>` directive will reference an actual container provided
by the module, for the version you have chosen to load. An environment file in the
module folder will also be bound. Note that although a container
might provide custom commands, every container exposes unique exec, shell, run, and
inspect aliases. For anycommands above, you can export:

 - SINGULARITY_OPTS: to define custom options for singularity (e.g., --debug)
 - SINGULARITY_COMMAND_OPTS: to define custom options for the command (e.g., -b)
 - PODMAN_OPTS: to define custom options for podman or docker
 - PODMAN_COMMAND_OPTS: to define custom options for the command

<br>

### Install

You can install shpc locally (for yourself or your user base) as follows:

```bash
$ git clone https://github.com/singularityhub/singularity-hpc
$ cd singularity-hpc
$ pip install -e .
```

Have any questions, or want to request a new module or version? [ask for help!](https://github.com/singularityhub/singularity-hpc/issues)