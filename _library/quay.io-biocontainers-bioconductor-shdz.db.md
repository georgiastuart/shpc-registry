---
layout: container
name:  "quay.io/biocontainers/bioconductor-shdz.db"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-shdz.db/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-shdz.db/container.yaml"
updated_at: "2022-11-08 00:13:53.718104"
latest: "3.2.3--r41hdfd78af_9"
container_url: "https://biocontainers.pro/tools/bioconductor-shdz.db"
aliases:
 - ".bioconductor-shdz.db-post-link.sh"
 - ".bioconductor-shdz.db-pre-unlink.sh"
versions:
 - "3.2.3--r41hdfd78af_9"
description: "shpc-registry automated BioContainers addition for bioconductor-shdz.db"
config: {"url": "https://biocontainers.pro/tools/bioconductor-shdz.db", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-shdz.db", "latest": {"3.2.3--r41hdfd78af_9": "sha256:cc40f340e1321189a2df1670b7c9e7849e7e1494bc0b97923d536c0cf0dc8037"}, "tags": {"3.2.3--r41hdfd78af_9": "sha256:cc40f340e1321189a2df1670b7c9e7849e7e1494bc0b97923d536c0cf0dc8037"}, "docker": "quay.io/biocontainers/bioconductor-shdz.db", "aliases": {".bioconductor-shdz.db-post-link.sh": "/usr/local/bin/.bioconductor-shdz.db-post-link.sh", ".bioconductor-shdz.db-pre-unlink.sh": "/usr/local/bin/.bioconductor-shdz.db-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-shdz.db.
shpc-registry automated BioContainers addition for bioconductor-shdz.db
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-shdz.db
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-shdz.db:3.2.3--r41hdfd78af_9
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-shdz.db/3.2.3--r41hdfd78af_9
$ module help quay.io/biocontainers/bioconductor-shdz.db/3.2.3--r41hdfd78af_9
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-shdz.db-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-shdz.db-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-shdz.db-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-shdz.db-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-shdz.db-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-shdz.db-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-shdz.db-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-shdz.db-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-shdz.db-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-shdz.db-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-shdz.db-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-shdz.db-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-shdz.db-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-shdz.db-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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