---
layout: container
name:  "quay.io/biocontainers/bioconductor-hgu2beta7"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hgu2beta7/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hgu2beta7/container.yaml"
updated_at: "2022-11-08 00:23:22.362400"
latest: "1.34.0--r41hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-hgu2beta7"
aliases:
 - ".bioconductor-hgu2beta7-post-link.sh"
 - ".bioconductor-hgu2beta7-pre-unlink.sh"
versions:
 - "1.34.0--r41hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-hgu2beta7"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hgu2beta7", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hgu2beta7", "latest": {"1.34.0--r41hdfd78af_1": "sha256:c7de83acbcbbecd7a11eba58710d25c8d3445d50c0580d1bd838e6d92e810e2b"}, "tags": {"1.34.0--r41hdfd78af_1": "sha256:c7de83acbcbbecd7a11eba58710d25c8d3445d50c0580d1bd838e6d92e810e2b"}, "docker": "quay.io/biocontainers/bioconductor-hgu2beta7", "aliases": {".bioconductor-hgu2beta7-post-link.sh": "/usr/local/bin/.bioconductor-hgu2beta7-post-link.sh", ".bioconductor-hgu2beta7-pre-unlink.sh": "/usr/local/bin/.bioconductor-hgu2beta7-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hgu2beta7.
shpc-registry automated BioContainers addition for bioconductor-hgu2beta7
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hgu2beta7
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hgu2beta7:1.34.0--r41hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hgu2beta7/1.34.0--r41hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-hgu2beta7/1.34.0--r41hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hgu2beta7-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hgu2beta7-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hgu2beta7-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hgu2beta7-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hgu2beta7-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hgu2beta7-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-hgu2beta7-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-hgu2beta7-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-hgu2beta7-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-hgu2beta7-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-hgu2beta7-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-hgu2beta7-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-hgu2beta7-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-hgu2beta7-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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