---
layout: container
name:  "quay.io/biocontainers/bioconductor-predasampledata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-predasampledata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-predasampledata/container.yaml"
updated_at: "2022-11-19 02:26:02.056657"
latest: "0.34.0--r41hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-predasampledata"
aliases:
 - ".bioconductor-predasampledata-post-link.sh"
 - ".bioconductor-predasampledata-pre-unlink.sh"
versions:
 - "0.34.0--r41hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-predasampledata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-predasampledata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-predasampledata", "latest": {"0.34.0--r41hdfd78af_1": "sha256:2e1995bf7cfd99edbb719aa1d6cf3580f9729351110399851543e8d5a438e9f2"}, "tags": {"0.34.0--r41hdfd78af_1": "sha256:2e1995bf7cfd99edbb719aa1d6cf3580f9729351110399851543e8d5a438e9f2"}, "docker": "quay.io/biocontainers/bioconductor-predasampledata", "aliases": {".bioconductor-predasampledata-post-link.sh": "/usr/local/bin/.bioconductor-predasampledata-post-link.sh", ".bioconductor-predasampledata-pre-unlink.sh": "/usr/local/bin/.bioconductor-predasampledata-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-predasampledata.
shpc-registry automated BioContainers addition for bioconductor-predasampledata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-predasampledata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-predasampledata:0.34.0--r41hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-predasampledata/0.34.0--r41hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-predasampledata/0.34.0--r41hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-predasampledata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-predasampledata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-predasampledata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-predasampledata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-predasampledata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-predasampledata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-predasampledata-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-predasampledata-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-predasampledata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-predasampledata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-predasampledata-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-predasampledata-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-predasampledata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-predasampledata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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