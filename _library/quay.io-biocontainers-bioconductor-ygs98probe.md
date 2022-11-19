---
layout: container
name:  "quay.io/biocontainers/bioconductor-ygs98probe"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ygs98probe/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ygs98probe/container.yaml"
updated_at: "2022-11-19 02:35:32.725537"
latest: "2.18.0--r41hdfd78af_9"
container_url: "https://biocontainers.pro/tools/bioconductor-ygs98probe"
aliases:
 - ".bioconductor-ygs98probe-post-link.sh"
 - ".bioconductor-ygs98probe-pre-unlink.sh"
versions:
 - "2.18.0--r41hdfd78af_9"
description: "shpc-registry automated BioContainers addition for bioconductor-ygs98probe"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ygs98probe", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ygs98probe", "latest": {"2.18.0--r41hdfd78af_9": "sha256:5f3ff961c65028132dd68b363488197753e428356127d79ad7cd70a79538e991"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:5f3ff961c65028132dd68b363488197753e428356127d79ad7cd70a79538e991"}, "docker": "quay.io/biocontainers/bioconductor-ygs98probe", "aliases": {".bioconductor-ygs98probe-post-link.sh": "/usr/local/bin/.bioconductor-ygs98probe-post-link.sh", ".bioconductor-ygs98probe-pre-unlink.sh": "/usr/local/bin/.bioconductor-ygs98probe-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ygs98probe.
shpc-registry automated BioContainers addition for bioconductor-ygs98probe
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ygs98probe
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ygs98probe:2.18.0--r41hdfd78af_9
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ygs98probe/2.18.0--r41hdfd78af_9
$ module help quay.io/biocontainers/bioconductor-ygs98probe/2.18.0--r41hdfd78af_9
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ygs98probe-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ygs98probe-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ygs98probe-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ygs98probe-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ygs98probe-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ygs98probe-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-ygs98probe-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-ygs98probe-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-ygs98probe-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-ygs98probe-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-ygs98probe-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-ygs98probe-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-ygs98probe-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-ygs98probe-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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