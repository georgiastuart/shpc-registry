---
layout: container
name:  "quay.io/biocontainers/bioconductor-mgu74cprobe"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-mgu74cprobe/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-mgu74cprobe/container.yaml"
updated_at: "2022-10-29 17:59:31.792393"
latest: "2.18.0--r41hdfd78af_8"
container_url: "https://biocontainers.pro/tools/bioconductor-mgu74cprobe"
aliases:
 - ".bioconductor-mgu74cprobe-post-link.sh"
 - ".bioconductor-mgu74cprobe-pre-unlink.sh"
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "2.18.0--r41hdfd78af_8"
description: "shpc-registry automated BioContainers addition for bioconductor-mgu74cprobe"
config: {"url": "https://biocontainers.pro/tools/bioconductor-mgu74cprobe", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-mgu74cprobe", "latest": {"2.18.0--r41hdfd78af_8": "sha256:d67e3e7247a52753cc3bebc9cfef4ef1b1ee5643108968249accc7cf3b7a7717"}, "tags": {"2.18.0--r41hdfd78af_8": "sha256:d67e3e7247a52753cc3bebc9cfef4ef1b1ee5643108968249accc7cf3b7a7717"}, "docker": "quay.io/biocontainers/bioconductor-mgu74cprobe", "aliases": {".bioconductor-mgu74cprobe-post-link.sh": "/usr/local/bin/.bioconductor-mgu74cprobe-post-link.sh", ".bioconductor-mgu74cprobe-pre-unlink.sh": "/usr/local/bin/.bioconductor-mgu74cprobe-pre-unlink.sh", "x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-mgu74cprobe.
shpc-registry automated BioContainers addition for bioconductor-mgu74cprobe
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-mgu74cprobe
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-mgu74cprobe:2.18.0--r41hdfd78af_8
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-mgu74cprobe/2.18.0--r41hdfd78af_8
$ module help quay.io/biocontainers/bioconductor-mgu74cprobe/2.18.0--r41hdfd78af_8
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-mgu74cprobe-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mgu74cprobe-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mgu74cprobe-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-mgu74cprobe-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-mgu74cprobe-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-mgu74cprobe-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-mgu74cprobe-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-mgu74cprobe-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-mgu74cprobe-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-mgu74cprobe-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-mgu74cprobe-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-mgu74cprobe-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-mgu74cprobe-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-mgu74cprobe-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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