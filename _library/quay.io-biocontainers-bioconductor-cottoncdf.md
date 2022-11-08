---
layout: container
name:  "quay.io/biocontainers/bioconductor-cottoncdf"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-cottoncdf/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-cottoncdf/container.yaml"
updated_at: "2022-11-07 23:57:26.999536"
latest: "2.18.0--r41hdfd78af_9"
container_url: "https://biocontainers.pro/tools/bioconductor-cottoncdf"
aliases:
 - ".bioconductor-cottoncdf-post-link.sh"
 - ".bioconductor-cottoncdf-pre-unlink.sh"
versions:
 - "2.18.0--r41hdfd78af_9"
description: "shpc-registry automated BioContainers addition for bioconductor-cottoncdf"
config: {"url": "https://biocontainers.pro/tools/bioconductor-cottoncdf", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-cottoncdf", "latest": {"2.18.0--r41hdfd78af_9": "sha256:b8fbe87417052fd4f8f9bfa8d94107a1f266db1c3f8a32f116efefda1263752e"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:b8fbe87417052fd4f8f9bfa8d94107a1f266db1c3f8a32f116efefda1263752e"}, "docker": "quay.io/biocontainers/bioconductor-cottoncdf", "aliases": {".bioconductor-cottoncdf-post-link.sh": "/usr/local/bin/.bioconductor-cottoncdf-post-link.sh", ".bioconductor-cottoncdf-pre-unlink.sh": "/usr/local/bin/.bioconductor-cottoncdf-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-cottoncdf.
shpc-registry automated BioContainers addition for bioconductor-cottoncdf
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-cottoncdf
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-cottoncdf:2.18.0--r41hdfd78af_9
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-cottoncdf/2.18.0--r41hdfd78af_9
$ module help quay.io/biocontainers/bioconductor-cottoncdf/2.18.0--r41hdfd78af_9
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-cottoncdf-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cottoncdf-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cottoncdf-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-cottoncdf-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-cottoncdf-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-cottoncdf-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-cottoncdf-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-cottoncdf-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-cottoncdf-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-cottoncdf-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-cottoncdf-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-cottoncdf-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-cottoncdf-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-cottoncdf-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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