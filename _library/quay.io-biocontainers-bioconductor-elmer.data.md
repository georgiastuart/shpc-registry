---
layout: container
name:  "quay.io/biocontainers/bioconductor-elmer.data"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-elmer.data/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-elmer.data/container.yaml"
updated_at: "2022-10-29 18:21:59.808068"
latest: "2.8.0--r36_1"
container_url: "https://biocontainers.pro/tools/bioconductor-elmer.data"
aliases:
 - ".bioconductor-elmer.data-post-link.sh"
 - ".bioconductor-elmer.data-pre-unlink.sh"
 - "gio-launch-desktop"
 - "c89"
 - "c99"
versions:
 - "2.8.0--r36_1"
description: "shpc-registry automated BioContainers addition for bioconductor-elmer.data"
config: {"url": "https://biocontainers.pro/tools/bioconductor-elmer.data", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-elmer.data", "latest": {"2.8.0--r36_1": "sha256:7b9ea7716d40a1d8062505afc59b1c78f0033dc40212c77bf08a0744079cc5da"}, "tags": {"2.8.0--r36_1": "sha256:7b9ea7716d40a1d8062505afc59b1c78f0033dc40212c77bf08a0744079cc5da"}, "docker": "quay.io/biocontainers/bioconductor-elmer.data", "aliases": {".bioconductor-elmer.data-post-link.sh": "/usr/local/bin/.bioconductor-elmer.data-post-link.sh", ".bioconductor-elmer.data-pre-unlink.sh": "/usr/local/bin/.bioconductor-elmer.data-pre-unlink.sh", "gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-elmer.data.
shpc-registry automated BioContainers addition for bioconductor-elmer.data
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-elmer.data
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-elmer.data:2.8.0--r36_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-elmer.data/2.8.0--r36_1
$ module help quay.io/biocontainers/bioconductor-elmer.data/2.8.0--r36_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-elmer.data-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-elmer.data-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-elmer.data-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-elmer.data-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-elmer.data-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-elmer.data-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-elmer.data-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-elmer.data-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-elmer.data-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-elmer.data-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-elmer.data-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-elmer.data-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-elmer.data-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-elmer.data-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### gio-launch-desktop

```bash
$ singularity exec <container> /usr/local/bin/gio-launch-desktop
$ podman run --it --rm --entrypoint /usr/local/bin/gio-launch-desktop   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/gio-launch-desktop   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### c89

```bash
$ singularity exec <container> /usr/local/bin/c89
$ podman run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### c99

```bash
$ singularity exec <container> /usr/local/bin/c99
$ podman run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
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