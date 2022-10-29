---
layout: container
name:  "quay.io/biocontainers/bioconductor-curatedtcgadata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-curatedtcgadata/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-curatedtcgadata/container.yaml"
updated_at: "2022-10-29 18:26:42.647092"
latest: "1.8.0--r36_0"
container_url: "https://biocontainers.pro/tools/bioconductor-curatedtcgadata"
aliases:
 - ".bioconductor-curatedtcgadata-post-link.sh"
 - ".bioconductor-curatedtcgadata-pre-unlink.sh"
 - "gio-launch-desktop"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r36_0"
description: "shpc-registry automated BioContainers addition for bioconductor-curatedtcgadata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-curatedtcgadata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-curatedtcgadata", "latest": {"1.8.0--r36_0": "sha256:975d911f99fdae54b6b79d4fe5344d6a06d369f7c0745fbd72068f12f99274a6"}, "tags": {"1.8.0--r36_0": "sha256:975d911f99fdae54b6b79d4fe5344d6a06d369f7c0745fbd72068f12f99274a6"}, "docker": "quay.io/biocontainers/bioconductor-curatedtcgadata", "aliases": {".bioconductor-curatedtcgadata-post-link.sh": "/usr/local/bin/.bioconductor-curatedtcgadata-post-link.sh", ".bioconductor-curatedtcgadata-pre-unlink.sh": "/usr/local/bin/.bioconductor-curatedtcgadata-pre-unlink.sh", "gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-curatedtcgadata.
shpc-registry automated BioContainers addition for bioconductor-curatedtcgadata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-curatedtcgadata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-curatedtcgadata:1.8.0--r36_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-curatedtcgadata/1.8.0--r36_0
$ module help quay.io/biocontainers/bioconductor-curatedtcgadata/1.8.0--r36_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-curatedtcgadata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-curatedtcgadata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-curatedtcgadata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-curatedtcgadata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-curatedtcgadata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-curatedtcgadata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-curatedtcgadata-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-curatedtcgadata-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-curatedtcgadata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-curatedtcgadata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-curatedtcgadata-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-curatedtcgadata-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-curatedtcgadata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-curatedtcgadata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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