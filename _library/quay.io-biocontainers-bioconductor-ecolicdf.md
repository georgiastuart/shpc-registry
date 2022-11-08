---
layout: container
name:  "quay.io/biocontainers/bioconductor-ecolicdf"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ecolicdf/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ecolicdf/container.yaml"
updated_at: "2022-11-08 00:10:11.674818"
latest: "2.18.0--r41hdfd78af_9"
container_url: "https://biocontainers.pro/tools/bioconductor-ecolicdf"
aliases:
 - ".bioconductor-ecolicdf-post-link.sh"
 - ".bioconductor-ecolicdf-pre-unlink.sh"
versions:
 - "2.18.0--r41hdfd78af_9"
description: "shpc-registry automated BioContainers addition for bioconductor-ecolicdf"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ecolicdf", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ecolicdf", "latest": {"2.18.0--r41hdfd78af_9": "sha256:23f59f4548e233697b6439dbe98d36143cf438ed8d8764f90e758df6bf41e6ec"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:23f59f4548e233697b6439dbe98d36143cf438ed8d8764f90e758df6bf41e6ec"}, "docker": "quay.io/biocontainers/bioconductor-ecolicdf", "aliases": {".bioconductor-ecolicdf-post-link.sh": "/usr/local/bin/.bioconductor-ecolicdf-post-link.sh", ".bioconductor-ecolicdf-pre-unlink.sh": "/usr/local/bin/.bioconductor-ecolicdf-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ecolicdf.
shpc-registry automated BioContainers addition for bioconductor-ecolicdf
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ecolicdf
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ecolicdf:2.18.0--r41hdfd78af_9
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ecolicdf/2.18.0--r41hdfd78af_9
$ module help quay.io/biocontainers/bioconductor-ecolicdf/2.18.0--r41hdfd78af_9
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ecolicdf-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ecolicdf-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ecolicdf-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ecolicdf-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ecolicdf-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ecolicdf-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-ecolicdf-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-ecolicdf-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-ecolicdf-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-ecolicdf-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-ecolicdf-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-ecolicdf-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-ecolicdf-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-ecolicdf-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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