---
layout: container
name:  "quay.io/biocontainers/bioconductor-gcspikelite"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gcspikelite/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gcspikelite/container.yaml"
updated_at: "2022-10-29 18:11:00.913075"
latest: "1.32.0--r41hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-gcspikelite"
aliases:
 - ".bioconductor-gcspikelite-post-link.sh"
 - ".bioconductor-gcspikelite-pre-unlink.sh"
versions:
 - "1.32.0--r41hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-gcspikelite"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gcspikelite", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gcspikelite", "latest": {"1.32.0--r41hdfd78af_1": "sha256:0ec23b2d8a7bd2bd6c478e185b3b7c80d30cfe84b7fa32f027a01287861422f8"}, "tags": {"1.32.0--r41hdfd78af_1": "sha256:0ec23b2d8a7bd2bd6c478e185b3b7c80d30cfe84b7fa32f027a01287861422f8"}, "docker": "quay.io/biocontainers/bioconductor-gcspikelite", "aliases": {".bioconductor-gcspikelite-post-link.sh": "/usr/local/bin/.bioconductor-gcspikelite-post-link.sh", ".bioconductor-gcspikelite-pre-unlink.sh": "/usr/local/bin/.bioconductor-gcspikelite-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gcspikelite.
shpc-registry automated BioContainers addition for bioconductor-gcspikelite
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gcspikelite
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gcspikelite:1.32.0--r41hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gcspikelite/1.32.0--r41hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-gcspikelite/1.32.0--r41hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gcspikelite-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gcspikelite-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gcspikelite-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gcspikelite-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gcspikelite-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gcspikelite-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-gcspikelite-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-gcspikelite-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-gcspikelite-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-gcspikelite-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-gcspikelite-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-gcspikelite-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-gcspikelite-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-gcspikelite-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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